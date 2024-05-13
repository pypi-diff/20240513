# Comparing `tmp/codeflash-0.5.1.tar.gz` & `tmp/codeflash-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.5.1.tar", max compression
+gzip compressed data, was "codeflash-0.6.0.tar", max compression
```

## Comparing `codeflash-0.5.1.tar` & `codeflash-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,61 @@
--rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.5.1/README.md
--rw-r--r--   0        0        0     4405 2024-04-18 06:54:49.015842 codeflash-0.5.1/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.5.1/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.5.1/codeflash/api/__init__.py
--rw-r--r--   0        0        0     7886 2024-04-16 22:27:44.246474 codeflash-0.5.1/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4681 2024-04-18 03:01:28.772476 codeflash-0.5.1/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.5.1/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     7606 2024-04-18 19:11:45.874124 codeflash-0.5.1/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0    22865 2024-04-18 03:01:28.773022 codeflash-0.5.1/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      440 2024-04-16 22:27:44.247326 codeflash-0.5.1/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.5.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.5.1/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     7170 2024-04-16 22:27:44.247484 codeflash-0.5.1/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     9450 2024-04-16 22:27:44.247642 codeflash-0.5.1/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2572 2024-04-16 22:27:44.247908 codeflash-0.5.1/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-04-15 22:14:14.315668 codeflash-0.5.1/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.5.1/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3908 2024-04-18 03:01:28.775259 codeflash-0.5.1/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2880 2024-04-18 03:01:28.775549 codeflash-0.5.1/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     1979 2024-04-18 03:01:28.775777 codeflash-0.5.1/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3305 2024-04-18 03:01:28.775937 codeflash-0.5.1/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0    22720 2024-04-18 06:54:04.081262 codeflash-0.5.1/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0     3497 2024-04-18 03:01:28.776414 codeflash-0.5.1/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.5.1/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1860 2024-01-24 20:13:21.332617 codeflash-0.5.1/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.5.1/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    16173 2024-04-18 03:01:28.777556 codeflash-0.5.1/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    12401 2024-04-18 19:11:45.875161 codeflash-0.5.1/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1230 2024-04-18 03:01:28.780898 codeflash-0.5.1/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.5.1/codeflash/github/__init__.py
--rw-r--r--   0        0        0      725 2024-04-16 22:27:44.248364 codeflash-0.5.1/codeflash/main.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.5.1/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    11557 2024-04-16 22:27:44.248501 codeflash-0.5.1/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0    46035 2024-04-16 22:27:44.248849 codeflash-0.5.1/codeflash/optimization/optimizer.py
--rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.5.1/codeflash/result/__init__.py
--rw-r--r--   0        0        0     4625 2024-04-16 22:27:44.249419 codeflash-0.5.1/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1982 2024-02-01 23:15:04.024170 codeflash-0.5.1/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.5.1/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-18 03:01:28.781066 codeflash-0.5.1/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.5.1/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0        0 2024-04-18 19:11:45.875236 codeflash-0.5.1/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     4938 2024-04-18 19:11:45.876501 codeflash-0.5.1/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0     5160 2024-04-18 19:11:45.876985 codeflash-0.5.1/codeflash/tracing/tracer.py
--rw-r--r--   0        0        0     1905 2024-04-18 03:01:28.781529 codeflash-0.5.1/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.5.1/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4738 2024-04-18 03:01:28.781696 codeflash-0.5.1/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1139 2024-03-30 00:35:38.112124 codeflash-0.5.1/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14520 2024-04-18 06:54:04.082484 codeflash-0.5.1/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6581 2024-04-16 22:27:44.249777 codeflash-0.5.1/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1606 2024-04-18 03:01:28.782090 codeflash-0.5.1/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2327 2024-04-18 19:11:45.877370 codeflash-0.5.1/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4126 2024-04-18 03:01:28.782490 codeflash-0.5.1/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-04-18 19:13:22.432539 codeflash-0.5.1/codeflash/version.py
--rw-r--r--   0        0        0     2894 2024-04-18 19:13:22.431563 codeflash-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 codeflash-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 03:52:06.661399 codeflash-0.6.0/README.md
+-rw-r--r--   0        0        0     4405 2024-05-09 02:46:13.702044 codeflash-0.6.0/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-12 23:19:32.441827 codeflash-0.6.0/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.664022 codeflash-0.6.0/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     9084 2024-05-10 22:08:41.323160 codeflash-0.6.0/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4699 2024-05-09 01:04:19.208503 codeflash-0.6.0/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:20.903968 codeflash-0.6.0/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-13 20:50:08.613037 codeflash-0.6.0/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0    22865 2024-04-26 00:11:25.877653 codeflash-0.6.0/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      440 2024-04-13 01:39:38.777959 codeflash-0.6.0/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1827 2024-03-22 23:15:30.441796 codeflash-0.6.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.665124 codeflash-0.6.0/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     9536 2024-05-13 20:50:08.613395 codeflash-0.6.0/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     8556 2024-05-13 20:50:08.613897 codeflash-0.6.0/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2956 2024-05-13 20:50:08.614171 codeflash-0.6.0/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-03-09 01:29:18.207924 codeflash-0.6.0/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-12 23:19:32.443100 codeflash-0.6.0/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3908 2024-04-26 00:11:25.877810 codeflash-0.6.0/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2880 2024-04-26 00:11:25.877913 codeflash-0.6.0/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-13 20:50:08.614476 codeflash-0.6.0/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3329 2024-05-13 20:50:08.614854 codeflash-0.6.0/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0    23761 2024-05-13 20:50:08.615008 codeflash-0.6.0/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0      293 2024-05-09 02:00:12.294226 codeflash-0.6.0/codeflash/code_utils/main_calls_bubblesort.py
+-rw-r--r--   0        0        0     3497 2024-04-26 00:11:25.878498 codeflash-0.6.0/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0     1007 2024-01-05 03:52:06.666361 codeflash-0.6.0/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1898 2024-05-13 20:50:08.615426 codeflash-0.6.0/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.666515 codeflash-0.6.0/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    18567 2024-05-13 20:50:08.615782 codeflash-0.6.0/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    20447 2024-05-13 20:50:08.616245 codeflash-0.6.0/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1230 2024-04-26 00:11:25.879800 codeflash-0.6.0/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667045 codeflash-0.6.0/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-15 21:39:54.603831 codeflash-0.6.0/codeflash/main.py
+-rw-r--r--   0        0        0      133 2024-05-09 01:04:19.209290 codeflash-0.6.0/codeflash/models/ExperimentMetadata.py
+-rw-r--r--   0        0        0        0 2024-05-09 01:04:19.209321 codeflash-0.6.0/codeflash/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 03:52:06.667651 codeflash-0.6.0/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    11557 2024-05-06 23:55:18.537635 codeflash-0.6.0/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    53413 2024-05-13 20:50:08.616609 codeflash-0.6.0/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0    12288 2024-05-06 22:36:52.069428 codeflash-0.6.0/codeflash/output1.trace
+-rw-r--r--   0        0        0        0 2024-01-29 22:42:06.720542 codeflash-0.6.0/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4539 2024-05-13 20:50:08.617001 codeflash-0.6.0/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1992 2024-05-13 20:50:08.617647 codeflash-0.6.0/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 03:48:11.207605 codeflash-0.6.0/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-26 00:11:25.880328 codeflash-0.6.0/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-03-19 03:48:11.207884 codeflash-0.6.0/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0    20467 2024-05-13 20:50:08.617770 codeflash-0.6.0/codeflash/tracer.py
+-rw-r--r--   0        0        0        1 2024-05-13 20:50:08.617918 codeflash-0.6.0/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     2644 2024-05-13 20:50:08.618038 codeflash-0.6.0/codeflash/tracing/profile_stats.py
+-rw-r--r--   0        0        0     5942 2024-05-13 20:50:08.618326 codeflash-0.6.0/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0      210 2024-04-26 00:11:25.881219 codeflash-0.6.0/codeflash/tracing/tracing_utils.py
+-rw-r--r--   0        0        0     1905 2024-04-26 00:11:25.881455 codeflash-0.6.0/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-19 22:35:16.406336 codeflash-0.6.0/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4977 2024-05-09 01:04:19.210115 codeflash-0.6.0/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1139 2024-04-05 00:50:30.445955 codeflash-0.6.0/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14621 2024-05-13 20:50:08.618624 codeflash-0.6.0/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6776 2024-05-13 20:50:08.619311 codeflash-0.6.0/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1852 2024-05-13 20:50:08.619642 codeflash-0.6.0/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2338 2024-04-26 00:11:25.882465 codeflash-0.6.0/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4200 2024-05-10 22:08:41.328788 codeflash-0.6.0/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-05-13 21:06:20.912349 codeflash-0.6.0/codeflash/version.py
+-rw-r--r--   0        0        0     2910 2024-05-13 21:06:20.911383 codeflash-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 codeflash-0.6.0/PKG-INFO
```

### Comparing `codeflash-0.5.1/codeflash/LICENSE` & `codeflash-0.6.0/codeflash/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/api/aiservice.py` & `codeflash-0.6.0/codeflash/api/aiservice.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,213 +1,231 @@
+from __future__ import annotations
+
 import json
 import logging
 import os
 import platform
-from functools import lru_cache
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple
 
 import requests
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 
 from codeflash.code_utils.env_utils import get_codeflash_api_key
-from codeflash.discovery.functions_to_optimize import FunctionToOptimize
 from codeflash.telemetry.posthog import ph
 
-
-@lru_cache(maxsize=1)
-def get_aiservice_base_url() -> str:
-    if os.environ.get("AIS_SERVER", default="prod").lower() == "local":
-        logging.info("Using local AI Service at http://localhost:8000/")
-        return "http://localhost:8000/"
-    return "https://app.codeflash.ai"
-
-
-def make_ai_service_request(
-    endpoint: str,
-    method: str = "POST",
-    payload: Optional[Dict[str, Any]] = None,
-    timeout: float = None,
-) -> requests.Response:
-    """Make an API request to the given endpoint on the AI service.
-    :param endpoint: The endpoint to call, e.g., "/optimize".
-    :param method: The HTTP method to use ('GET' or 'POST').
-    :param payload: Optional JSON payload to include in the POST request body.
-    :param timeout: The timeout for the request.
-    :return: The response object from the API.
-    """
-    url = f"{get_aiservice_base_url()}/ai{endpoint}"
-    ai_service_headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
-    if method.upper() == "POST":
-        json_payload = json.dumps(payload, indent=None, default=pydantic_encoder)
-        ai_service_headers["Content-Type"] = "application/json"
-        response = requests.post(
-            url,
-            data=json_payload,
-            headers=ai_service_headers,
-            timeout=timeout,
-        )
-    else:
-        response = requests.get(url, headers=ai_service_headers, timeout=timeout)
-    # response.raise_for_status()  # Will raise an HTTPError if the HTTP request returned an unsuccessful status code
-    return response
+if TYPE_CHECKING:
+    from codeflash.discovery.functions_to_optimize import FunctionToOptimize
+    from codeflash.models.ExperimentMetadata import ExperimentMetadata
 
 
 @dataclass(frozen=True)
-class Optimization:
+class OptimizedCandidate:
     source_code: str
     explanation: str
     optimization_id: str
 
 
-def optimize_python_code(source_code: str, trace_id: str, num_variants: int = 10) -> List[Optimization]:
-    """Optimize the given python code for performance by making a request to the Django endpoint.
-
-    Parameters
-    ----------
-    - source_code (str): The python code to optimize.
-    - num_variants (int): Number of optimization variants to generate. Default is 10.
-
-    Returns
-    -------
-    - List[Optimization]: A list of Optimization objects.
-
-    """
-    payload = {
-        "source_code": source_code,
-        "num_variants": num_variants,
-        "trace_id": trace_id,
-        "python_version": platform.python_version(),
-    }
-    logging.info("Generating optimized candidates ...")
-    try:
-        response = make_ai_service_request("/optimize", payload=payload, timeout=600)
-    except requests.exceptions.RequestException as e:
-        logging.exception(f"Error generating optimized candidates: {e}")
-        ph("cli-optimize-error-caught", {"error": str(e)})
-        return []
-
-    if response.status_code == 200:
-        optimizations_json = response.json()["optimizations"]
-        logging.info(f"Generated {len(optimizations_json)} candidates.")
-        return [
-            Optimization(
-                source_code=opt["source_code"],
-                explanation=opt["explanation"],
-                optimization_id=opt["optimization_id"],
+class AiServiceClient:
+    def __init__(self):
+        self.base_url = self.get_aiservice_base_url()
+        self.headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
+
+    def get_aiservice_base_url(self) -> str:
+        if os.environ.get("CODEFLASH_AIS_SERVER", default="prod").lower() == "local":
+            logging.info("Using local AI Service at http://localhost:8000/")
+            return "http://localhost:8000/"
+        return "https://app.codeflash.ai"
+
+    def make_ai_service_request(
+        self,
+        endpoint: str,
+        method: str = "POST",
+        payload: Optional[Dict[str, Any]] = None,
+        timeout: float = None,
+    ) -> requests.Response:
+        """Make an API request to the given endpoint on the AI service.
+
+        :param endpoint: The endpoint to call, e.g., "/optimize".
+        :param method: The HTTP method to use ('GET' or 'POST').
+        :param payload: Optional JSON payload to include in the POST request body.
+        :param timeout: The timeout for the request.
+        :return: The response object from the API.
+        """
+        url = f"{self.base_url}/ai{endpoint}"
+        if method.upper() == "POST":
+            json_payload = json.dumps(payload, indent=None, default=pydantic_encoder)
+            headers = {**self.headers, "Content-Type": "application/json"}
+            response = requests.post(url, data=json_payload, headers=headers, timeout=timeout)
+        else:
+            response = requests.get(url, headers=self.headers, timeout=timeout)
+        # response.raise_for_status()  # Will raise an HTTPError if the HTTP request returned an unsuccessful status code
+        return response
+
+    def optimize_python_code(
+        self,
+        source_code: str,
+        trace_id: str,
+        num_candidates: int = 10,
+        experiment_metadata: ExperimentMetadata | None = None,
+    ) -> list[OptimizedCandidate]:
+        """Optimize the given python code for performance by making a request to the Django endpoint.
+
+        Parameters
+        ----------
+        - source_code (str): The python code to optimize.
+        - num_variants (int): Number of optimization variants to generate. Default is 10.
+
+        Returns
+        -------
+        - List[Optimization]: A list of Optimization objects.
+
+        """
+        payload = {
+            "source_code": source_code,
+            "num_variants": num_candidates,
+            "trace_id": trace_id,
+            "python_version": platform.python_version(),
+            "experiment_metadata": experiment_metadata,
+        }
+        logging.info("Generating optimized candidates ...")
+        try:
+            response = self.make_ai_service_request(
+                "/optimize",
+                payload=payload,
+                timeout=600,
             )
-            for opt in optimizations_json
-        ]
-    try:
-        error = response.json()["error"]
-    except Exception:
-        error = response.text
-    logging.error(f"Error generating optimized candidates: {response.status_code} - {error}")
-    ph(
-        "cli-optimize-error-response",
-        {"response_status_code": response.status_code, "error": error},
-    )
-    return []
-
-
-def log_results(
-    function_trace_id: str,
-    speedup_ratio: Optional[Dict[str, float]],
-    original_runtime: Optional[float],
-    optimized_runtime: Optional[Dict[str, float]],
-    is_correct: Optional[Dict[str, bool]],
-) -> None:
-    """Log features to the database.
-
-    Parameters
-    ----------
-    - function_trace_id (str): The UUID.
-    - speedup_ratio (Optional[Dict[str, float]]): The speedup.
-    - original_runtime (Optional[Dict[str, float]]): The original runtime.
-    - optimized_runtime (Optional[Dict[str, float]]): The optimized runtime.
-    - is_correct (Optional[Dict[str, bool]]): Whether the optimized code is correct.
-
-    """
-    payload = {
-        "trace_id": function_trace_id,
-        "speedup_ratio": speedup_ratio,
-        "original_runtime": original_runtime,
-        "optimized_runtime": optimized_runtime,
-        "is_correct": is_correct,
-    }
-    try:
-        make_ai_service_request("/log_features", payload=payload, timeout=5)
-    except requests.exceptions.RequestException as e:
-        logging.exception(f"Error logging features: {e}")
-
-
-def generate_regression_tests(
-    source_code_being_tested: str,
-    function_to_optimize: FunctionToOptimize,
-    dependent_function_names: list[str],
-    module_path: str,
-    test_module_path: str,
-    test_framework: str,
-    test_timeout: int,
-    trace_id: str,
-) -> Optional[Tuple[str, str]]:
-    """Generate regression tests for the given function by making a request to the Django endpoint.
-
-    Parameters
-    ----------
-    - source_code_being_tested (str): The source code of the function being tested.
-    - function_to_optimize (FunctionToOptimize): The function to optimize.
-    - dependent_function_names (list[Source]): List of dependent function names.
-    - module_path (str): The module path where the function is located.
-    - test_module_path (str): The module path for the test code.
-    - test_framework (str): The test framework to use, e.g., "pytest".
-    - test_timeout (int): The timeout for each test in seconds.
-
-    Returns
-    -------
-    - Dict[str, str] | None: The generated regression tests and instrumented tests, or None if an error occurred.
-
-    """
-    assert test_framework in [
-        "pytest",
-        "unittest",
-    ], f"Invalid test framework, got {test_framework} but expected 'pytest' or 'unittest'"
-    payload = {
-        "source_code_being_tested": source_code_being_tested,
-        "function_to_optimize": function_to_optimize,
-        "dependent_function_names": dependent_function_names,
-        "module_path": module_path,
-        "test_module_path": test_module_path,
-        "test_framework": test_framework,
-        "test_timeout": test_timeout,
-        "trace_id": trace_id,
-        "python_version": platform.python_version(),
-    }
-    try:
-        response = make_ai_service_request("/testgen", payload=payload, timeout=600)
-    except requests.exceptions.RequestException as e:
-        logging.exception(f"Error generating tests: {e}")
-        ph("cli-testgen-error-caught", {"error": str(e)})
-        return None
-
-    # the timeout should be the same as the timeout for the AI service backend
-
-    if response.status_code == 200:
-        response_json = response.json()
-        logging.info(f"Generated tests for function {function_to_optimize.function_name}")
-        return response_json["generated_tests"], response_json["instrumented_tests"]
-    else:
+        except requests.exceptions.RequestException as e:
+            logging.exception(f"Error generating optimized candidates: {e}")
+            ph("cli-optimize-error-caught", {"error": str(e)})
+            return []
+
+        if response.status_code == 200:
+            optimizations_json = response.json()["optimizations"]
+            logging.info(f"Generated {len(optimizations_json)} candidates.")
+            return [
+                OptimizedCandidate(
+                    source_code=opt["source_code"],
+                    explanation=opt["explanation"],
+                    optimization_id=opt["optimization_id"],
+                )
+                for opt in optimizations_json
+            ]
         try:
             error = response.json()["error"]
-            logging.error(f"Error generating tests: {response.status_code} - {error}")
-            ph(
-                "cli-testgen-error-response",
-                {"response_status_code": response.status_code, "error": error},
-            )
-            return None
         except Exception:
-            logging.exception(f"Error generating tests: {response.status_code} - {response.text}")
-            ph(
-                "cli-testgen-error-response",
-                {"response_status_code": response.status_code, "error": response.text},
-            )
+            error = response.text
+        logging.error(f"Error generating optimized candidates: {response.status_code} - {error}")
+        ph(
+            "cli-optimize-error-response",
+            {"response_status_code": response.status_code, "error": error},
+        )
+        return []
+
+    def log_results(
+        self,
+        function_trace_id: str,
+        speedup_ratio: dict[str, float] | None,
+        original_runtime: float | None,
+        optimized_runtime: dict[str, float] | None,
+        is_correct: dict[str, bool] | None,
+    ) -> None:
+        """Log features to the database.
+
+        Parameters
+        ----------
+        - function_trace_id (str): The UUID.
+        - speedup_ratio (Optional[Dict[str, float]]): The speedup.
+        - original_runtime (Optional[Dict[str, float]]): The original runtime.
+        - optimized_runtime (Optional[Dict[str, float]]): The optimized runtime.
+        - is_correct (Optional[Dict[str, bool]]): Whether the optimized code is correct.
+
+        """
+        payload = {
+            "trace_id": function_trace_id,
+            "speedup_ratio": speedup_ratio,
+            "original_runtime": original_runtime,
+            "optimized_runtime": optimized_runtime,
+            "is_correct": is_correct,
+        }
+        try:
+            self.make_ai_service_request("/log_features", payload=payload, timeout=5)
+        except requests.exceptions.RequestException as e:
+            logging.exception(f"Error logging features: {e}")
+
+    def generate_regression_tests(
+        self,
+        source_code_being_tested: str,
+        function_to_optimize: FunctionToOptimize,
+        dependent_function_names: list[str],
+        module_path: str,
+        test_module_path: str,
+        test_framework: str,
+        test_timeout: int,
+        trace_id: str,
+    ) -> Optional[Tuple[str, str]]:
+        """Generate regression tests for the given function by making a request to the Django endpoint.
+
+        Parameters
+        ----------
+        - source_code_being_tested (str): The source code of the function being tested.
+        - function_to_optimize (FunctionToOptimize): The function to optimize.
+        - dependent_function_names (list[Source]): List of dependent function names.
+        - module_path (str): The module path where the function is located.
+        - test_module_path (str): The module path for the test code.
+        - test_framework (str): The test framework to use, e.g., "pytest".
+        - test_timeout (int): The timeout for each test in seconds.
+
+        Returns
+        -------
+        - Dict[str, str] | None: The generated regression tests and instrumented tests, or None if an error occurred.
+
+        """
+        assert test_framework in [
+            "pytest",
+            "unittest",
+        ], f"Invalid test framework, got {test_framework} but expected 'pytest' or 'unittest'"
+        payload = {
+            "source_code_being_tested": source_code_being_tested,
+            "function_to_optimize": function_to_optimize,
+            "dependent_function_names": dependent_function_names,
+            "module_path": module_path,
+            "test_module_path": test_module_path,
+            "test_framework": test_framework,
+            "test_timeout": test_timeout,
+            "trace_id": trace_id,
+            "python_version": platform.python_version(),
+        }
+        try:
+            response = self.make_ai_service_request("/testgen", payload=payload, timeout=600)
+        except requests.exceptions.RequestException as e:
+            logging.exception(f"Error generating tests: {e}")
+            ph("cli-testgen-error-caught", {"error": str(e)})
             return None
+
+        # the timeout should be the same as the timeout for the AI service backend
+
+        if response.status_code == 200:
+            response_json = response.json()
+            logging.info(f"Generated tests for function {function_to_optimize.function_name}")
+            return response_json["generated_tests"], response_json["instrumented_tests"]
+        else:
+            try:
+                error = response.json()["error"]
+                logging.error(f"Error generating tests: {response.status_code} - {error}")
+                ph(
+                    "cli-testgen-error-response",
+                    {"response_status_code": response.status_code, "error": error},
+                )
+                return None
+            except Exception:
+                logging.exception(f"Error generating tests: {response.status_code} - {response.text}")
+                ph(
+                    "cli-testgen-error-response",
+                    {"response_status_code": response.status_code, "error": response.text},
+                )
+                return None
+
+
+class LocalAiServiceClient(AiServiceClient):
+    def get_aiservice_base_url(self) -> str:
+        return "http://localhost:8000/"
```

### Comparing `codeflash-0.5.1/codeflash/api/cfapi.py` & `codeflash-0.6.0/codeflash/api/cfapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 import requests
 from pydantic.json import pydantic_encoder
 from requests import Response
 
 from codeflash.code_utils.env_utils import get_codeflash_api_key
 from codeflash.github.PrComment import FileDiffContent, PrComment
 
-if os.environ.get("CFAPI_SERVER", default="prod").lower() == "local":
+if os.environ.get("CODEFLASH_CFAPI_SERVER", default="prod").lower() == "local":
     CFAPI_BASE_URL = "http://localhost:3001"
     logging.info(f"Using local CF API at {CFAPI_BASE_URL}.")
 else:
     CFAPI_BASE_URL = "https://app.codeflash.ai"
 
 
 def make_cfapi_request(
-    endpoint: str, method: str, payload: Optional[Dict[str, Any]] = None,
+    endpoint: str,
+    method: str,
+    payload: Optional[Dict[str, Any]] = None,
 ) -> requests.Response:
     """Make an HTTP request using the specified method, URL, headers, and JSON payload.
     :param endpoint: The endpoint URL to send the request to.
     :param method: The HTTP method to use ('GET', 'POST', etc.).
     :param payload: Optional JSON payload to include in the POST request body.
     :return: The response object from the API.
     """
```

### Comparing `codeflash-0.5.1/codeflash/cli_cmds/cli.py` & `codeflash-0.6.0/codeflash/cli_cmds/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,24 @@
         help="Command that codeflash will use to run pytest. If not specified, codeflash will use 'pytest'",
     )
     parser.add_argument(
         "--use-cached-tests",
         action="store_true",
         help="Use cached tests from a specified file for debugging.",
     )
+    parser.add_argument(
+        "--replay-test",
+        type=str,
+        help="Path to replay test to optimize functions from",
+    )
+    parser.add_argument(
+        "--no-pr",
+        action="store_true",
+        help="Do not create a PR for the optimization, only update the code locally.",
+    )
     parser.add_argument("-v", "--verbose", action="store_true", help="Print verbose debug logs")
     parser.add_argument("--version", action="store_true", help="Print the version of codeflash")
     args: Namespace = parser.parse_args()
     return process_cmd_args(args)
 
 
 def process_cmd_args(args: Namespace) -> Namespace:
@@ -79,14 +89,18 @@
         exit()
     if args.function and not args.file:
         raise ValueError("If you specify a --function, you must specify the --file it is in")
     if args.file:
         if not os.path.exists(args.file):
             raise ValueError(f"File {args.file} does not exist")
         args.file = os.path.realpath(args.file)
+    if args.replay_test:
+        if not os.path.isfile(args.replay_test):
+            raise ValueError(f"Replay test file {args.replay_test} does not exist")
+        args.replay_test = os.path.realpath(args.replay_test)
 
     try:
         pyproject_config, pyproject_file_path = parse_config_file(args.config_file)
     except ValueError as e:
         logging.exception(e.args[0])
         exit(1)
     supported_keys = [
@@ -99,27 +113,25 @@
         "formatter_cmd",
         "disable_telemetry",
         "imports_sort_cmd",
     ]
     for key in supported_keys:
         if key in pyproject_config:
             if (
-                hasattr(args, key.replace("-", "_"))
-                and getattr(args, key.replace("-", "_")) is None
+                hasattr(args, key.replace("-", "_")) and getattr(args, key.replace("-", "_")) is None
             ) or not hasattr(args, key.replace("-", "_")):
                 setattr(args, key.replace("-", "_"), pyproject_config[key])
     assert args.module_root is not None and os.path.isdir(
         args.module_root,
     ), f"--module-root {args.module_root} must be a valid directory"
     assert args.tests_root is not None and os.path.isdir(
         args.tests_root,
     ), f"--tests-root {args.tests_root} must be a valid directory"
-    assert not (
-        env_utils.get_pr_number() is not None and not env_utils.ensure_codeflash_api_key()
-    ), (
+
+    assert not (env_utils.get_pr_number() is not None and not env_utils.ensure_codeflash_api_key()), (
         "Codeflash API key not found. When running in a Github Actions Context, provide the "
         "'CODEFLASH_API_KEY' environment variable as a secret.\n"
         "You can add a secret by going to your repository's settings page, then clicking 'Secrets' in the left sidebar.\n"
         "Then, click 'New repository secret' and add your api key with the variable name CODEFLASH_API_KEY.\n"
         f"Here's a direct link: {get_github_secrets_page_url()}\n"
         "Exiting..."
     )
@@ -131,48 +143,53 @@
             ), f"ignore-paths config must be a valid path. Path {path} does not exist"
             normalized_ignore_paths.append(os.path.realpath(path))
         args.ignore_paths = normalized_ignore_paths
     # Project root path is one level above the specified directory, because that's where the module can be imported from
     args.module_root = os.path.realpath(args.module_root)
     # If module-root is "." then all imports are relatives to it.
     # in this case, the ".." becomes outside project scope, causing issues with un-importable paths
-    if os.path.dirname(pyproject_file_path) == args.module_root:
-        args.project_root = args.module_root
-    else:
-        args.project_root = os.path.realpath(os.path.join(args.module_root, ".."))
+    args.project_root = project_root_from_module_root(args.module_root, pyproject_file_path)
     args.tests_root = os.path.realpath(args.tests_root)
     args = handle_optimize_all_arg_parsing(args)
     return args
 
 
+def project_root_from_module_root(module_root: str, pyproject_file_path: str) -> str:
+    if os.path.dirname(pyproject_file_path) == module_root:
+        return module_root
+    else:
+        return os.path.realpath(os.path.join(module_root, ".."))
+
+
 def handle_optimize_all_arg_parsing(args: Namespace) -> Namespace:
     if hasattr(args, "all"):
         # Ensure that the user can actually open PRs on the repo.
         try:
             git_repo = git.Repo(search_parent_directories=True)
         except git.exc.InvalidGitRepositoryError:
             logging.exception(
                 "I couldn't find a git repository in the current directory. "
                 "I need a git repository to run --all and open PRs for optimizations. Exiting...",
             )
             apologize_and_exit()
         owner, repo = get_repo_owner_and_name(git_repo)
-        try:
-            response = check_github_app_installed_on_repo(owner, repo)
-            if not response.ok or response.text != "true":
-                logging.error(f"Error: {response.text}")
-                raise Exception
-        except Exception:
-            logging.exception(
-                f"Could not find the Codeflash GitHub App installed on the repository {owner}/{repo} or the GitHub"
-                f" account linked to your CODEFLASH_API_KEY does not have access to the repository {owner}/{repo}.{LF}"
-                "Please install the Codeflash GitHub App on your repository to use --all. You can install it by going to "
-                f"https://github.com/settings/installations/{LF}",
-            )
-            apologize_and_exit()
+        if not args.no_pr:
+            try:
+                response = check_github_app_installed_on_repo(owner, repo)
+                if not response.ok or response.text != "true":
+                    logging.error(f"Error: {response.text}")
+                    raise Exception
+            except Exception:
+                logging.exception(
+                    f"Could not find the Codeflash GitHub App installed on the repository {owner}/{repo} or the GitHub"
+                    f" account linked to your CODEFLASH_API_KEY does not have access to the repository {owner}/{repo}.{LF}"
+                    "Please install the Codeflash GitHub App on your repository to use --all. You can install it by going to "
+                    f"https://github.com/settings/installations/{LF}",
+                )
+                apologize_and_exit()
     if not hasattr(args, "all"):
         args.all = None
     elif args.all == "":
         # The default behavior of --all is to optimize everything in args.module_root
         args.all = args.module_root
     else:
         args.all = os.path.realpath(args.all)
```

### Comparing `codeflash-0.5.1/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.6.0/codeflash/cli_cmds/cmd_init.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.6.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/code_utils/code_replacer.py` & `codeflash-0.6.0/codeflash/code_utils/code_replacer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from typing import IO
 
 import libcst as cst
 from libcst import FunctionDef
 
+from codeflash.code_utils.code_extractor import add_needed_imports_from_module
+
 
 class OptimFunctionCollector(cst.CSTVisitor):
     METADATA_DEPENDENCIES = (cst.metadata.ParentNodeProvider,)
 
     def __init__(
         self,
         function_name: str,
@@ -151,36 +153,14 @@
                     *node.body[class_index + 1 :],
                 ),
             )
         else:
             node = node.with_changes(body=(*self.optim_new_functions, *node.body))
         return node
 
-    # TODO: Implement the logic to not duplicate imports. This is supported by libcst, figure out how to use it.
-    # def leave_Module(self, original_node: "Module", updated_node: "Module") -> "Module":
-    #     print(self.context)
-    #     for import_node in self.optim_new_imports:
-    #         # updated_node = updated_node.with_changes(
-    #         #     body=(*updated_node.body, import_node)
-    #         # )
-    #         if isinstance(import_node, cst.Import):
-    #             #print(import_node.names)
-    #             for name in import_node.names:
-    #                 print(name)
-    #                 print(name.asname.name.value)
-    #                 asname = name.asname.name.value if name.asname else None
-    #                 AddImportsVisitor.add_needed_import(self.context, name.name.value, asname=asname)
-    #         if isinstance(import_node, cst.ImportFrom):
-    #             print(import_node)
-    #             for name in import_node.names:
-    #                 asname = name.asname.name.value if name.asname else None
-    #                 AddImportsVisitor.add_needed_import(
-    #                 self.context, module =import_node.module.value,  obj=name.name.value, asname=asname)
-    #     #print(updated_node)
-
 
 def replace_functions_in_file(
     source_code: str,
     original_function_names: list[str],
     optimized_code: str,
     preexisting_functions: list[str],
     contextual_functions: set[tuple[str, str]],
@@ -226,23 +206,31 @@
 
     return source_code
 
 
 def replace_function_definitions_in_module(
     function_names: list[str],
     optimized_code: str,
+    file_path_of_module_with_function_to_optimize: str,
     module_abspath: str,
     preexisting_functions: list[str],
     contextual_functions: set[tuple[str, str]],
+    project_root_path: str,
 ) -> None:
     file: IO[str]
     with open(module_abspath, encoding="utf8") as file:
         source_code: str = file.read()
-    new_code: str = replace_functions_in_file(
-        source_code,
-        function_names,
+    new_code: str = add_needed_imports_from_module(
         optimized_code,
-        preexisting_functions,
-        contextual_functions,
+        replace_functions_in_file(
+            source_code,
+            function_names,
+            optimized_code,
+            preexisting_functions,
+            contextual_functions,
+        ),
+        file_path_of_module_with_function_to_optimize,
+        module_abspath,
+        project_root_path,
     )
     with open(module_abspath, "w", encoding="utf8") as file:
         file.write(new_code)
```

### Comparing `codeflash-0.5.1/codeflash/code_utils/code_utils.py` & `codeflash-0.6.0/codeflash/code_utils/code_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import logging
 import os
 import site
 from tempfile import TemporaryDirectory
 from typing import List, Optional, Tuple, Union
 
 
-def module_name_from_file_path(file_path: str, project_root: str) -> str:
-    relative_path = os.path.relpath(file_path, project_root)
+def module_name_from_file_path(file_path: str, project_root_path: str) -> str:
+    relative_path = os.path.relpath(file_path, project_root_path)
     module_path = relative_path.replace(os.sep, ".")
     if module_path.lower().endswith(".py"):
         module_path = module_path[:-3]
     return module_path
 
 
-def file_path_from_module_name(module_name: str, project_root: str) -> str:
+def file_path_from_module_name(module_name: str, project_root_path: str) -> str:
     """Get file path from module path"""
-    return os.path.join(project_root, module_name.replace(".", os.sep) + ".py")
+    return os.path.join(project_root_path, module_name.replace(".", os.sep) + ".py")
 
 
 def ellipsis_in_ast(module: ast.AST) -> bool:
     for node in ast.walk(module):
         if isinstance(node, ast.Constant) and node.value == ...:
             return True
     return False
@@ -67,10 +67,24 @@
 def get_run_tmp_file(file_path: str) -> str:
     if not hasattr(get_run_tmp_file, "tmpdir"):
         get_run_tmp_file.tmpdir = TemporaryDirectory(prefix="codeflash_")
     return os.path.join(get_run_tmp_file.tmpdir.name, file_path)
 
 
 def path_belongs_to_site_packages(file_path: str) -> bool:
-    return any(  # The definition is not part of a site-package Python library
-        [file_path.startswith(site_package_path + os.sep) for site_package_path in site.getsitepackages()],
-    )
+    site_packages = site.getsitepackages()
+    for site_package_path in site_packages:
+        if file_path.startswith(site_package_path + os.sep):
+            return True
+    return False
+
+
+def is_class_defined_in_file(class_name: str, file_path: str) -> bool:
+    if not os.path.exists(file_path):
+        return False
+    with open(file_path) as file:
+        source = file.read()
+    tree = ast.parse(source)
+    for node in ast.walk(tree):
+        if isinstance(node, ast.ClassDef) and node.name == class_name:
+            return True
+    return False
```

### Comparing `codeflash-0.5.1/codeflash/code_utils/config_parser.py` & `codeflash-0.6.0/codeflash/code_utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/code_utils/env_utils.py` & `codeflash-0.6.0/codeflash/code_utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/code_utils/formatter.py` & `codeflash-0.6.0/codeflash/code_utils/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,40 @@
 import os.path
 import subprocess
 
 import isort
 
 
 def format_code(
-    formatter_cmd: str, imports_sort_cmd: str, should_sort_imports: bool, path: str,
+    formatter_cmd: str,
+    imports_sort_cmd: str,
+    should_sort_imports: bool,
+    path: str,
 ) -> str:
     # TODO: Only allow a particular whitelist of formatters here to prevent arbitrary code execution
     if formatter_cmd.lower() == "disabled":
         if should_sort_imports:
             return sort_imports(imports_sort_cmd, should_sort_imports, path)
 
         with open(path, encoding="utf8") as f:
             new_code = f.read()
         return new_code
 
     formatter_cmd_list = [chunk for chunk in formatter_cmd.split(" ") if chunk != ""]
     logging.info(f"Formatting code with {formatter_cmd} ...")
     # black currently does not have a stable public API, so we are using the CLI
     # the main problem is custom config parsing https://github.com/psf/black/issues/779
-    assert os.path.exists(path), f"File {path} does not exist. Cannot format the file. Exiting..."
+    assert os.path.exists(
+        path
+    ), f"File {path} does not exist. Cannot format the file. Exiting..."
     result = subprocess.run(
-        formatter_cmd_list + [path], stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False,
+        formatter_cmd_list + [path],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        check=False,
     )
     if result.returncode == 0:
         logging.info("OK")
     else:
         logging.error(f"Failed to format code with {formatter_cmd}")
 
     if should_sort_imports:
@@ -36,24 +44,21 @@
     with open(path, encoding="utf8") as f:
         new_code = f.read()
 
     return new_code
 
 
 def sort_imports(imports_sort_cmd: str, should_sort_imports: bool, path: str) -> str:
-    if imports_sort_cmd.lower() == "disabled":
+    try:
         with open(path, encoding="utf8") as f:
             code = f.read()
-        return code
 
-    if should_sort_imports:
-        # Deduplicate and sort imports
-        isort.file(path)
+        if imports_sort_cmd.lower() == "disabled" or not should_sort_imports:
+            return code
 
-        with open(path, encoding="utf8") as f:
-            new_code = f.read()
-        return new_code
-    else:
-        # Return original code
-        with open(path, encoding="utf8") as f:
-            code = f.read()
-        return code
+        # Deduplicate and sort imports, modify the code in memory, not on disk
+        sorted_code = isort.code(code)
+    except Exception as e:
+        logging.exception(f"Failed to sort imports with isort for {path}: {e}")
+        return code  # Fall back to original code if isort fails
+
+    return sorted_code
```

### Comparing `codeflash-0.5.1/codeflash/code_utils/git_utils.py` & `codeflash-0.6.0/codeflash/code_utils/git_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 
 import git
 from git import Repo
 from unidiff import PatchSet
 
 
 def get_git_diff(
-    repo_directory: str = os.getcwd(), uncommitted_changes: bool = False,
+    repo_directory: str = os.getcwd(),
+    uncommitted_changes: bool = False,
 ) -> dict[str, list[int]]:
     repository = git.Repo(repo_directory, search_parent_directories=True)
     commit = repository.head.commit
     if uncommitted_changes:
         uni_diff_text = repository.git.diff(
-            None, "HEAD", ignore_blank_lines=True, ignore_space_at_eol=True,
+            None,
+            "HEAD",
+            ignore_blank_lines=True,
+            ignore_space_at_eol=True,
         )
     else:
         uni_diff_text = repository.git.diff(
             commit.hexsha + "^1",
             commit.hexsha,
             ignore_blank_lines=True,
             ignore_space_at_eol=True,
@@ -71,17 +75,15 @@
 
 def get_repo_owner_and_name(repo: Optional[Repo] = None) -> tuple[str, str]:
     remote_url = get_remote_url(repo)  # call only once
     remote_url = remote_url.rstrip(".git") if remote_url.endswith(".git") else remote_url
     split_url = remote_url.split("/")
     repo_owner_with_github, repo_name = split_url[-2], split_url[-1]
     repo_owner = (
-        repo_owner_with_github.split(":")[1]
-        if ":" in repo_owner_with_github
-        else repo_owner_with_github
+        repo_owner_with_github.split(":")[1] if ":" in repo_owner_with_github else repo_owner_with_github
     )
     return repo_owner, repo_name
 
 
 def get_github_secrets_page_url(repo: Optional[Repo] = None) -> str:
     owner, repo_name = get_repo_owner_and_name(repo)
     return f"https://github.com/{owner}/{repo_name}/settings/secrets/actions"
```

### Comparing `codeflash-0.5.1/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.6.0/codeflash/code_utils/instrument_existing_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,27 @@
 
 class ReplaceCallNodeWithName(ast.NodeTransformer):
     def __init__(self, only_function_name, new_variable_name="codeflash_return_value"):
         self.only_function_name = only_function_name
         self.new_variable_name = new_variable_name
 
     def visit_Call(self, node: ast.Call):
-        if isinstance(node, ast.Call) and (
-            (hasattr(node.func, "id") and node.func.id == self.only_function_name)
-            or (hasattr(node.func, "attr") and node.func.attr == self.only_function_name)
-        ):
-            return ast.Name(id=self.new_variable_name, ctx=ast.Load())
+        if isinstance(node, ast.Call):
+            if hasattr(node.func, "id"):
+                function_name = node.func.id
+
+            if hasattr(node.func, "attr"):
+                function_name = node.func.attr
+
+            if hasattr(node.func, "value") and hasattr(node.func.value, "id"):
+                function_name = node.func.value.id + "." + function_name
+
+            if function_name == self.only_function_name:
+                return ast.Name(id=self.new_variable_name, ctx=ast.Load())
+
         self.generic_visit(node)
         return node
 
 
 class InjectPerfOnly(ast.NodeTransformer):
     def __init__(self, function_name, module_path):
         self.only_function_name = function_name
@@ -29,35 +37,44 @@
         self,
         test_node,
         node_name,
         index: str,
         test_class_name: Optional[str] = None,
     ):
         call_node = None
+        function_name = ""
         for node in ast.walk(test_node):
-            if isinstance(node, ast.Call) and (
-                (hasattr(node.func, "id") and node.func.id == self.only_function_name)
-                or (hasattr(node.func, "attr") and node.func.attr == self.only_function_name)
-            ):
-                call_node = node
+            if isinstance(node, ast.Call):
+                if hasattr(node.func, "id"):
+                    function_name = node.func.id
+
+                if hasattr(node.func, "attr"):
+                    function_name = node.func.attr
+
+                if hasattr(node.func, "value") and hasattr(node.func.value, "id"):
+                    function_name = node.func.value.id + "." + function_name
+
+                if function_name == self.only_function_name:
+                    call_node = node
+
         if call_node is None:
             return [test_node]
 
         if hasattr(call_node.func, "id"):
             function_id = call_node.func.id
         else:
             function_id = call_node.func.attr
 
         updated_nodes = [
             ast.Assign(
                 targets=[ast.Name(id="codeflash_return_value", ctx=ast.Store())],
                 value=ast.Call(
                     func=ast.Name(id="codeflash_wrap", ctx=ast.Load()),
                     args=[
-                        ast.Name(id=function_id, ctx=ast.Load()),
+                        ast.Name(id=function_name, ctx=ast.Load()),
                         ast.Constant(value=self.module_path),
                         ast.Constant(value=test_class_name or None),
                         ast.Constant(value=node_name),
                         ast.Constant(value=self.only_function_name),
                         ast.Constant(value=index),
                         ast.Name(id="codeflash_cur", ctx=ast.Load()),
                         ast.Name(id="codeflash_con", ctx=ast.Load()),
@@ -77,19 +94,27 @@
         #  in a more robust way.
 
         updated_nodes.append(subbed_node)
         return updated_nodes
 
     def is_target_function_line(self, line_node):
         for node in ast.walk(line_node):
-            if isinstance(node, ast.Call) and (
-                (hasattr(node.func, "id") and node.func.id == self.only_function_name)
-                or (hasattr(node.func, "attr") and node.func.attr == self.only_function_name)
-            ):
-                return True
+            if isinstance(node, ast.Call):
+                if hasattr(node.func, "id"):
+                    function_name = node.func.id
+
+                if hasattr(node.func, "attr"):
+                    function_name = node.func.attr
+
+                if hasattr(node.func, "value") and hasattr(node.func.value, "id"):
+                    function_name = node.func.value.id + "." + function_name
+
+                if function_name == self.only_function_name:
+                    return True
+
         return False
 
     def visit_ClassDef(self, node: ClassDef) -> Any:
         # TODO: Ensure that this class inherits from unittest.TestCase. Don't modify non unittest.TestCase classes
         for inner_node in ast.walk(node):
             if isinstance(inner_node, (ast.FunctionDef, ast.AsyncFunctionDef)):
                 inner_node = self.visit_FunctionDef(inner_node, node.name)
@@ -225,39 +250,48 @@
 
 class FunctionImportedAsVisitor(ast.NodeVisitor):
     """This checks if a function has been imported as an alias. We only care about the alias then.
     from numpy import array as np_array
     np_array is what we want
     """
 
-    def __init__(self, original_function_name):
-        self.original_function_name = original_function_name
-        self.imported_as_function_name = original_function_name
+    def __init__(self, qualified_name: str):
+        self.split_qualified_name = qualified_name.split(".")
+        assert len(self.split_qualified_name) <= 2, "Only support functions in the format module.function"
+        self.imported_as = qualified_name
+        self.to_match = self.split_qualified_name[0]
+        try:
+            self.optional_method_name = self.split_qualified_name[1]
+        except IndexError:
+            self.optional_method_name = None
 
     # TODO: Validate if the function imported is actually from the right module
     def visit_ImportFrom(self, node: ast.ImportFrom):
         for alias in node.names:
-            if alias.name == self.original_function_name:
+            if alias.name == self.to_match:
                 if hasattr(alias, "asname") and alias.asname is not None:
-                    self.imported_as_function_name = alias.asname
+                    self.imported_as = alias.asname + (
+                        "." + self.optional_method_name if self.optional_method_name else ""
+                    )
 
 
 def inject_profiling_into_existing_test(test_path, function_name, root_path) -> Tuple[bool, str]:
     with open(test_path, encoding="utf8") as f:
         test_code = f.read()
     try:
         tree = ast.parse(test_code)
     except SyntaxError as e:
         print(f"Syntax error in code: {e}")
         return False, None
     # TODO: Pass the full name of function here, otherwise we can run into namespace clashes
+    module_path = module_name_from_file_path(test_path, root_path)
     import_visitor = FunctionImportedAsVisitor(function_name)
     import_visitor.visit(tree)
-    function_name = import_visitor.imported_as_function_name
-    module_path = module_name_from_file_path(test_path, root_path)
+    function_name = import_visitor.imported_as
+
     tree = InjectPerfOnly(function_name, module_path).visit(tree)
     new_imports = [
         ast.Import(names=[ast.alias(name="time")]),
         ast.Import(names=[ast.alias(name="gc")]),
         ast.Import(names=[ast.alias(name="os")]),
         ast.Import(names=[ast.alias(name="sqlite3")]),
         ast.Import(names=[ast.alias(name="dill", asname="pickle")]),
```

### Comparing `codeflash-0.5.1/codeflash/code_utils/shell_utils.py` & `codeflash-0.6.0/codeflash/code_utils/shell_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.6.0/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.6.0/codeflash/discovery/discover_unit_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,93 +7,104 @@
 from collections import defaultdict
 from enum import Enum
 from typing import Dict, List, Optional
 
 import jedi
 from pydantic.dataclasses import dataclass
 
+from codeflash.code_utils.code_utils import module_name_from_file_path
+from codeflash.verification.test_results import TestType
 from codeflash.verification.verification_utils import TestConfig
 
 
 class ParseType(Enum):
     CO = "co"
     Q = "q"
 
 
 @dataclass(frozen=True)
 class TestsInFile:
     test_file: str
-    test_class: Optional[str]
+    test_class: Optional[str]  # This might be unused...
     test_function: str
     test_suite: Optional[str]
+    test_type: TestType
 
     @classmethod
     def from_pytest_stdout_line_co(cls, module: str, function: str, directory: str):
-        absolute_test_path = os.path.join(directory, module)
+        absolute_test_path = os.path.normpath(os.path.join(directory, module))
+        if "__replay_test" in absolute_test_path:
+            test_type = TestType.REPLAY_TEST
+        else:
+            test_type = TestType.EXISTING_UNIT_TEST
         assert os.path.exists(
             absolute_test_path,
         ), f"Test discovery failed - Test file does not exist {absolute_test_path}"
         return cls(
             test_file=absolute_test_path,
             test_class=None,
             test_function=function,
             test_suite=None,
+            test_type=test_type,
         )
 
     @classmethod
     def from_pytest_stdout_line_q(cls, line: str, pytest_rootdir: str):
         parts = line.split("::")
-        absolute_test_path = os.path.join(pytest_rootdir, parts[0])
+        absolute_test_path = os.path.normpath(os.path.join(pytest_rootdir, parts[0]))
+        if "__replay_test" in absolute_test_path:
+            test_type = TestType.REPLAY_TEST
+        else:
+            test_type = TestType.EXISTING_UNIT_TEST
         assert os.path.exists(
             absolute_test_path,
         ), f"Test discovery failed - Test file does not exist {absolute_test_path}"
         if len(parts) == 3:
             return cls(
                 test_file=absolute_test_path,
                 test_class=parts[1],
                 test_function=parts[2],
                 test_suite=None,
+                test_type=test_type,
             )
         elif len(parts) == 2:
             return cls(
                 test_file=absolute_test_path,
                 test_class=None,
                 test_function=parts[1],
                 test_suite=None,
+                test_type=test_type,
             )
         else:
             raise ValueError(f"Unexpected pytest result format: {line}")
 
 
 @dataclass(frozen=True)
 class TestFunction:
     function_name: str
     test_suite_name: Optional[str]
     parameters: Optional[str]
+    test_type: TestType
 
 
-@dataclass(frozen=True)
-class TestDetails:
-    test_function: str
-    test_module_path: str
-    test_suite_name: str
-
-
-def discover_unit_tests(cfg: TestConfig) -> Dict[str, List[TestsInFile]]:
+def discover_unit_tests(
+    cfg: TestConfig,
+    discover_only_these_tests: Optional[List[str]] = None,
+) -> Dict[str, List[TestsInFile]]:
     test_frameworks = {
         "pytest": discover_tests_pytest,
         "unittest": discover_tests_unittest,
     }
     discover_tests = test_frameworks.get(cfg.test_framework)
     if discover_tests is None:
         raise ValueError(f"Unsupported test framework: {cfg.test_framework}")
-    return discover_tests(cfg)
+    return discover_tests(cfg, discover_only_these_tests)
 
 
-def get_pytest_rootdir_only(pytest_cmd_list, tests_root, project_root) -> str:
+def get_pytest_rootdir_only(pytest_cmd_list: List[str], tests_root: str, project_root: str) -> str:
     # Ref - https://docs.pytest.org/en/stable/reference/customize.html#initialization-determining-rootdir-and-configfile
     # A very hacky solution that only runs the --co mode until we see the rootdir print and then it just kills the
     # pytest to save time. We should find better ways to just get the rootdir, one way is to not use the -q flag and
     # parse the --co output, but that could be more work.
     process = subprocess.Popen(
         pytest_cmd_list + [tests_root, "--co"],
         stdout=subprocess.PIPE,
@@ -110,109 +121,128 @@
         if output:
             if rootdir_re.search(output):
                 process.kill()
                 return rootdir_re.search(output).group(1)
     raise ValueError(f"Could not find rootdir in pytest output for {tests_root}")
 
 
-def discover_tests_pytest(cfg: TestConfig) -> Dict[str, List[TestsInFile]]:
+def discover_tests_pytest(
+    cfg: TestConfig,
+    discover_only_these_tests: Optional[List[str]] = None,
+) -> Dict[str, List[TestsInFile]]:
     tests_root = cfg.tests_root
     project_root = cfg.project_root_path
     pytest_cmd_list = [chunk for chunk in cfg.pytest_cmd.split(" ") if chunk != ""]
     pytest_result = subprocess.run(
         pytest_cmd_list + [f"{tests_root}", "--co", "-q", "-m", "not skip"],
         stdout=subprocess.PIPE,
-        cwd=project_root, check=False,
+        cwd=project_root,
+        check=False,
     )
 
     pytest_stdout = pytest_result.stdout.decode("utf-8")
 
     parse_type = ParseType.Q
     if "rootdir: " not in pytest_stdout:
-        pytest_rootdir = get_pytest_rootdir_only(pytest_cmd_list, tests_root, project_root)
+        pytest_rootdir = get_pytest_rootdir_only(
+            pytest_cmd_list,
+            tests_root,
+            project_root,
+        )
     else:
         rootdir_re = re.compile(r"^rootdir:\s?(\S*)", re.MULTILINE)
         pytest_rootdir_match = rootdir_re.search(pytest_stdout)
         if not pytest_rootdir_match:
-            raise ValueError(f"Could not find rootdir in pytest output for {tests_root}")
+            raise ValueError(
+                f"Could not find rootdir in pytest output for {tests_root}",
+            )
         pytest_rootdir = pytest_rootdir_match.group(1)
         parse_type = ParseType.CO
 
     tests = parse_pytest_stdout(pytest_stdout, pytest_rootdir, tests_root, parse_type)
     file_to_test_map = defaultdict(list)
 
     for test in tests:
-        file_to_test_map[test.test_file].append({"test_function": test.test_function})
+        if discover_only_these_tests and test.test_file not in discover_only_these_tests:
+            continue
+        file_to_test_map[test.test_file].append(test)
     # Within these test files, find the project functions they are referring to and return their names/locations
     return process_test_files(file_to_test_map, cfg)
 
 
-def discover_tests_unittest(cfg: TestConfig) -> Dict[str, List[TestsInFile]]:
+def discover_tests_unittest(
+    cfg: TestConfig,
+    discover_only_these_tests: Optional[List[str]] = None,
+) -> Dict[str, List[TestsInFile]]:
     tests_root = cfg.tests_root
-    project_root_path = cfg.project_root_path
     loader = unittest.TestLoader()
     tests = loader.discover(str(tests_root))
     file_to_test_map = defaultdict(list)
 
-    def get_test_details(_test) -> Optional[TestDetails]:
+    def get_test_details(_test) -> Optional[TestsInFile]:
         _test_function, _test_module, _test_suite_name = (
             _test._testMethodName,
             _test.__class__.__module__,
             _test.__class__.__qualname__,
         )
 
         _test_module_path = _test_module.replace(".", os.sep)
-        _test_module_path = os.path.join(str(tests_root), _test_module_path) + ".py"
-        if not os.path.exists(_test_module_path):
+        _test_module_path = os.path.normpath(os.path.join(str(tests_root), _test_module_path) + ".py")
+        if not os.path.exists(_test_module_path) or (
+            discover_only_these_tests and _test_module_path not in discover_only_these_tests
+        ):
             return None
-        return TestDetails(_test_function, _test_module_path, _test_suite_name)
+        if "__replay_test" in _test_module_path:
+            test_type = TestType.REPLAY_TEST
+        else:
+            test_type = TestType.EXISTING_UNIT_TEST
+        return TestsInFile(
+            test_file=_test_module_path,
+            test_suite=_test_suite_name,
+            test_function=_test_function,
+            test_type=test_type,
+            test_class=None,  # TODO: Validate if it is correct to set test_class to None
+        )
 
     for _test_suite in tests._tests:
         for test_suite_2 in _test_suite._tests:
             if not hasattr(test_suite_2, "_tests"):
                 logging.warning(f"Didn't find tests for {test_suite_2}")
                 continue
 
             for test in test_suite_2._tests:
                 # some test suites are nested, so we need to go deeper
                 if not hasattr(test, "_testMethodName") and hasattr(test, "_tests"):
                     for test_2 in test._tests:
                         if not hasattr(test_2, "_testMethodName"):
-                            logging.warning(f"Didn't find tests for {test_2}")  # it goes deeper?
+                            logging.warning(
+                                f"Didn't find tests for {test_2}",
+                            )  # it goes deeper?
                             continue
                         details = get_test_details(test_2)
                         if details is not None:
-                            file_to_test_map[details.test_module_path].append(
-                                {
-                                    "test_function": details.test_function,
-                                    "test_suite_name": details.test_suite_name,
-                                },
-                            )
+                            file_to_test_map[details.test_file].append(details)
                 else:
                     details = get_test_details(test)
                     if details is not None:
-                        file_to_test_map[details.test_module_path].append(
-                            {
-                                "test_function": details.test_function,
-                                "test_suite_name": details.test_suite_name,
-                            },
-                        )
+                        file_to_test_map[details.test_file].append(details)
     return process_test_files(file_to_test_map, cfg)
 
 
 def discover_parameters_unittest(function_name: str):
     function_name = function_name.split("_")
     if len(function_name) > 1 and function_name[-1].isdigit():
         return True, "_".join(function_name[:-1]), function_name[-1]
 
     return False, function_name, None
 
 
 def process_test_files(
-    file_to_test_map: Dict[str, List[Dict[str, str]]], cfg: TestConfig,
+    file_to_test_map: Dict[str, List[TestsInFile]],
+    cfg: TestConfig,
 ) -> Dict[str, List[TestsInFile]]:
     project_root_path = cfg.project_root_path
     test_framework = cfg.test_framework
     function_to_test_map = defaultdict(list)
     jedi_project = jedi.Project(path=project_root_path)
 
     for test_file, functions in file_to_test_map.items():
@@ -220,27 +250,30 @@
         test_functions = set()
         top_level_names = script.get_names()
         all_names = script.get_names(all_scopes=True, references=True)
         all_defs = script.get_names(all_scopes=True, definitions=True)
 
         for name in top_level_names:
             if test_framework == "pytest":
-                functions_to_search = [elem["test_function"] for elem in functions]
-                for function in functions_to_search:
+                functions_to_search = [elem.test_function for elem in functions]
+                for i, function in enumerate(functions_to_search):
                     if "[" in function:
                         function_name = re.split(r"\[|\]", function)[0]
                         parameters = re.split(r"\[|\]", function)[1]
                         if name.name == function_name and name.type == "function":
-                            test_functions.add(TestFunction(name.name, None, parameters))
+                            test_functions.add(
+                                TestFunction(name.name, None, parameters, functions[i].test_type),
+                            )
                     elif name.name == function and name.type == "function":
-                        test_functions.add(TestFunction(name.name, None, None))
+                        test_functions.add(TestFunction(name.name, None, None, functions[i].test_type))
                         break
             if test_framework == "unittest":
-                functions_to_search = [elem["test_function"] for elem in functions]
-                test_suites = [elem["test_suite_name"] for elem in functions]
+                functions_to_search = [elem.test_function for elem in functions]
+                test_suites = [elem.test_suite for elem in functions]
+
                 if name.name in test_suites and name.type == "class":
                     for def_name in all_defs:
                         if (
                             def_name.type == "function"
                             and def_name.full_name is not None
                             and f".{name.name}." in def_name.full_name
                         ):
@@ -249,18 +282,25 @@
                                     is_parameterized,
                                     new_function,
                                     parameters,
                                 ) = discover_parameters_unittest(function)
 
                                 if is_parameterized and new_function == def_name.name:
                                     test_functions.add(
-                                        TestFunction(def_name.name, name.name, parameters),
+                                        TestFunction(
+                                            def_name.name,
+                                            name.name,
+                                            parameters,
+                                            functions[0].test_type,
+                                        ),  # A test file must not have more than one test type
                                     )
                                 elif function == def_name.name:
-                                    test_functions.add(TestFunction(def_name.name, name.name, None))
+                                    test_functions.add(
+                                        TestFunction(def_name.name, name.name, None, functions[0].test_type),
+                                    )
 
         test_functions_list = list(test_functions)
         test_functions_raw = [elem.function_name for elem in test_functions_list]
 
         for name in all_names:
             if name.full_name is None:
                 continue
@@ -269,14 +309,15 @@
                 continue
             scope = m.group(1)
             indices = [i for i, x in enumerate(test_functions_raw) if x == scope]
             for index in indices:
                 scope_test_function = test_functions_list[index].function_name
                 scope_test_suite = test_functions_list[index].test_suite_name
                 scope_parameters = test_functions_list[index].parameters
+                test_type = test_functions_list[index].test_type
                 try:
                     definition = script.goto(
                         line=name.line,
                         column=name.column,
                         follow_imports=True,
                         follow_builtin_imports=False,
                     )
@@ -291,34 +332,51 @@
                         and definition[0].module_name != name.module_name
                     ):
                         if scope_parameters is not None:
                             if test_framework == "pytest":
                                 scope_test_function += "[" + scope_parameters + "]"
                             if test_framework == "unittest":
                                 scope_test_function += "_" + scope_parameters
-
-                        function_to_test_map[definition[0].full_name].append(
-                            TestsInFile(test_file, None, scope_test_function, scope_test_suite),
+                        full_name_without_module_prefix = definition[0].full_name.replace(
+                            definition[0].module_name + ".",
+                            "",
+                            1,
+                        )
+                        qualified_name_with_modules_from_root = f"{module_name_from_file_path(definition[0].module_path, project_root_path)}.{full_name_without_module_prefix}"
+                        function_to_test_map[qualified_name_with_modules_from_root].append(
+                            TestsInFile(
+                                test_file=test_file,
+                                test_class=None,
+                                test_function=scope_test_function,
+                                test_suite=scope_test_suite,
+                                test_type=test_type,
+                            ),
                         )
     deduped_function_to_test_map = {}
     for function, tests in function_to_test_map.items():
         deduped_function_to_test_map[function] = list(set(tests))
     return deduped_function_to_test_map
 
 
 def parse_pytest_stdout(
-    pytest_stdout: str, pytest_rootdir: str, tests_root: str, parse_type: ParseType,
+    pytest_stdout: str,
+    pytest_rootdir: str,
+    tests_root: str,
+    parse_type: ParseType,
 ) -> List[TestsInFile]:
     test_results = []
     if parse_type == ParseType.Q:
         for line in pytest_stdout.splitlines():
             if line.startswith("==") or line.startswith("\n") or line == "":
                 break
             try:
-                test_result = TestsInFile.from_pytest_stdout_line_q(line, pytest_rootdir)
+                test_result = TestsInFile.from_pytest_stdout_line_q(
+                    line,
+                    pytest_rootdir,
+                )
                 test_results.append(test_result)
             except ValueError as e:
                 logging.warning(str(e))
                 continue
         return test_results
 
     directory = tests_root
@@ -367,26 +425,30 @@
 
                 while len(module_list) > 1:
                     directory = os.path.join(directory, module_list[0])
                     module_list = module_list[1:]
 
                 module = module_list[0]
 
-            while len(directory) > 0 and not os.path.exists(os.path.join(directory, module)):
+            while len(directory) > 0 and not os.path.exists(
+                os.path.join(directory, module),
+            ):
                 directory = os.path.dirname(directory)
 
             if len(directory) == 0:
                 return test_results
 
         elif "<Function " in line and module is not None:
             function = re.match(r"\s*<Function (.+)>", line)
             if function:
                 function = function.group(1)
                 try:
                     test_result = TestsInFile.from_pytest_stdout_line_co(
-                        module, function, directory,
+                        module,
+                        function,
+                        directory,
                     )
                     test_results.append(test_result)
                 except ValueError as e:
                     logging.warning(str(e))
 
     return test_results
```

### Comparing `codeflash-0.5.1/codeflash/github/PrComment.py` & `codeflash-0.6.0/codeflash/github/PrComment.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/main.py` & `codeflash-0.6.0/codeflash/main.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/optimization/function_context.py` & `codeflash-0.6.0/codeflash/optimization/function_context.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/optimization/optimizer.py` & `codeflash-0.6.0/codeflash/optimization/optimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,61 @@
+from __future__ import annotations
+
 import concurrent.futures
 import logging
 import os
 import pathlib
+import sys
 import uuid
 from argparse import Namespace
 from collections import defaultdict
-from typing import IO, Dict, List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
+import isort
 import libcst as cst
 from pydantic import BaseModel
 from returns.pipeline import is_successful
 from returns.result import Failure, Result, Success
 
-from codeflash.api.aiservice import Optimization, log_results, optimize_python_code
+from codeflash.api.aiservice import (
+    AiServiceClient,
+    LocalAiServiceClient,
+    OptimizedCandidate,
+)
 from codeflash.code_utils import env_utils
-from codeflash.code_utils.code_extractor import extract_code
+from codeflash.code_utils.code_extractor import add_needed_imports_from_module, extract_code
 from codeflash.code_utils.code_replacer import replace_function_definitions_in_module
 from codeflash.code_utils.code_utils import (
     get_all_function_names,
     get_run_tmp_file,
     module_name_from_file_path,
 )
 from codeflash.code_utils.config_consts import (
     INDIVIDUAL_TEST_TIMEOUT,
     MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS,
     MAX_FUNCTION_TEST_SECONDS,
     MAX_TEST_FUNCTION_RUNS,
     MAX_TEST_RUN_ITERATIONS,
     N_CANDIDATES,
 )
-from codeflash.code_utils.formatter import format_code, sort_imports
-from codeflash.code_utils.instrument_existing_tests import inject_profiling_into_existing_test
+from codeflash.code_utils.formatter import format_code
+from codeflash.code_utils.instrument_existing_tests import (
+    inject_profiling_into_existing_test,
+)
 from codeflash.code_utils.time_utils import humanize_runtime
-from codeflash.discovery.discover_unit_tests import TestsInFile, discover_unit_tests
+from codeflash.discovery.discover_unit_tests import (
+    TestsInFile,
+    discover_unit_tests,
+)
 from codeflash.discovery.functions_to_optimize import (
     FunctionParent,
     FunctionToOptimize,
-    get_functions_to_optimize_by_file,
+    get_functions_to_optimize,
 )
+from codeflash.models.ExperimentMetadata import ExperimentMetadata
 from codeflash.optimization.function_context import (
     Source,
     get_constrained_function_context_and_dependent_functions,
 )
 from codeflash.result.create_pr import check_create_pr, existing_tests_source_for
 from codeflash.result.explanation import Explanation
 from codeflash.telemetry import posthog
@@ -51,415 +65,531 @@
 from codeflash.verification.parse_test_output import parse_test_results
 from codeflash.verification.test_results import TestResults, TestType
 from codeflash.verification.test_runner import run_tests
 from codeflash.verification.verification_utils import TestConfig, get_test_file_path
 from codeflash.verification.verifier import generate_tests
 
 
+class OptimizationSet(BaseModel):
+    control: list[OptimizedCandidate]
+    experiment: list[OptimizedCandidate] | None
+
+
 class OptimizedCandidateResult(BaseModel):
     times_run: int
     best_test_runtime: int
     best_test_results: TestResults
 
 
 class OriginalCodeBaseline(BaseModel):
     generated_test_results: TestResults
-    overall_test_results: Optional[TestResults]
+    existing_test_results: TestResults
+    overall_test_results: TestResults | None
     runtime: int
 
 
-class TestsAndOptimizationsResult(BaseModel):
+class GeneratedTests(BaseModel):
     generated_original_test_source: str
     instrumented_test_source: str
-    optimizations: List[Optimization]
 
 
 class BestOptimization(BaseModel):
-    source_code: str
-    explanation: str
-    dependent_functions: list[Tuple[Source, str, str]]
+    candidate: OptimizedCandidate
+    dependent_functions: list[tuple[Source, str, str]]
+    runtime: int
+    winning_test_results: TestResults
 
 
 class CodeOptimizationContext(BaseModel):
     code_to_optimize_with_dependents: str
     contextual_dunder_methods: set[tuple[str, str]]
-    dependent_functions: List[Tuple[Source, str, str]]
-    preexisting_functions: List[str]
+    dependent_functions: list[tuple[Source, str, str]]
+    preexisting_functions: list[str]
 
 
 class Optimizer:
-    def __init__(self, args: Namespace):
+    def __init__(self, args: Namespace) -> None:
         self.args = args
         init_sentry(not args.disable_telemetry)
         posthog.initialize_posthog(not args.disable_telemetry)
 
         self.test_cfg = TestConfig(
             tests_root=args.tests_root,
             project_root_path=args.project_root,
             test_framework=args.test_framework,
             pytest_cmd=args.pytest_cmd,
         )
 
+        self.aiservice_client = AiServiceClient()
+        self.experiment_id = os.getenv("CODEFLASH_EXPERIMENT_ID", None)
+        self.local_aiservice_client = LocalAiServiceClient() if self.experiment_id else None
+
+        self.test_files_created: set[str] = set()
+        self.instrumented_unittests_created: set[str] = set()
+
     def run(self) -> None:
         ph("cli-optimize-run-start")
         logging.info("Running optimizer.")
         if not env_utils.ensure_codeflash_api_key():
             return
         if not env_utils.ensure_git_repo(module_root=self.args.module_root):
             logging.error("No git repository detected and user aborted run. Exiting...")
-            exit(1)
+            sys.exit(1)
 
         file_to_funcs_to_optimize: dict[str, list[FunctionToOptimize]]
         num_optimizable_functions: int
+
         (
             file_to_funcs_to_optimize,
             num_optimizable_functions,
-        ) = get_functions_to_optimize_by_file(
+        ) = get_functions_to_optimize(
             optimize_all=self.args.all,
+            replay_test=self.args.replay_test,
             file=self.args.file,
-            function=self.args.function,
+            only_get_this_function=self.args.function,
             test_cfg=self.test_cfg,
             ignore_paths=self.args.ignore_paths,
             project_root=self.args.project_root,
             module_root=self.args.module_root,
         )
 
-        test_files_created: set[str] = set()
-        instrumented_unittests_created: set[str] = set()
         optimizations_found: int = 0
 
         function_iterator_count: int = 0
+
         try:
-            ph("cli-optimize-functions-to-optimize", {"num_functions": num_optimizable_functions})
+            ph(
+                "cli-optimize-functions-to-optimize",
+                {"num_functions": num_optimizable_functions},
+            )
             if num_optimizable_functions == 0:
                 logging.info("No functions found to optimize. Exiting...")
                 return
-            logging.info(f"Discovering existing unit tests in {self.test_cfg.tests_root} ...")
-            function_to_tests: dict[str, list[TestsInFile]] = discover_unit_tests(self.test_cfg)
-            num_discovered_tests: int = sum([len(value) for value in function_to_tests.values()])
+            logging.info(
+                f"Discovering existing unit tests in {self.test_cfg.tests_root} ...",
+            )
+            function_to_tests: dict[str, list[TestsInFile]] = discover_unit_tests(
+                self.test_cfg,
+            )
+            num_discovered_tests: int = sum(
+                [len(value) for value in function_to_tests.values()],
+            )
             logging.info(
                 f"Discovered {num_discovered_tests} existing unit tests in {self.test_cfg.tests_root}",
             )
             ph("cli-optimize-discovered-tests", {"num_tests": num_discovered_tests})
-            path: str
             for path in file_to_funcs_to_optimize:
                 logging.info(f"Examining file {path} ...")
-                # TODO: Sequence the functions one goes through intelligently. If we are optimizing f(g(x)),
-                #  then we might want to first optimize f rather than g because optimizing f would already
-                #  optimize g as it is a dependency
-                f: IO[str]
-                with open(path, encoding="utf8") as f:
+                # TODO @afik.cohen: Sequence the functions one goes through intelligently. If we are
+                #  optimizing f(g(x)), then we might want to first optimize f rather than g because optimizing
+                #  f would already optimize g as it is a dependency.
+                with pathlib.Path(path).open(encoding="utf8") as f:
                     original_code: str = f.read()
 
-                function_to_optimize: FunctionToOptimize
                 for function_to_optimize in file_to_funcs_to_optimize[path]:
-                    function_trace_id: str = str(uuid.uuid4())
-                    ph("cli-optimize-function-start", {"function_trace_id": function_trace_id})
                     function_iterator_count += 1
                     logging.info(
                         f"Optimizing function {function_iterator_count} of {num_optimizable_functions} - {function_to_optimize.qualified_name}",
                     )
-                    winning_test_results = None
-                    self.cleanup_leftover_test_return_values()
-                    ctx_result = self.get_code_optimization_context(function_to_optimize)
-                    if not is_successful(ctx_result):
-                        logging.error(ctx_result.failure())
-                        continue
-                    code_context: CodeOptimizationContext = ctx_result.unwrap()
-                    dependent_functions_by_module_abspath = defaultdict(set)
-                    for _, module_abspath, qualified_name in code_context.dependent_functions:
-                        dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
-                    original_dependent_code = {}
-                    for module_abspath in dependent_functions_by_module_abspath.keys():
-                        with open(module_abspath, encoding="utf8") as f:
-                            dependent_code = f.read()
-                            original_dependent_code[module_abspath] = dependent_code
-                    logging.info(f"Code to be optimized:\n{code_context.code_to_optimize_with_dependents}")
-                    module_path = module_name_from_file_path(path, self.args.project_root)
-
-                    instrumented_unittests_created_for_function = self.instrument_existing_tests(
-                        function_name=function_to_optimize.qualified_name,
-                        module_path=module_path,
-                        function_to_tests=function_to_tests,
-                    )
-                    instrumented_unittests_created.update(
-                        instrumented_unittests_created_for_function,
-                    )
-
-                    tests_result = self.generate_tests_and_optimizations(
-                        code_context.code_to_optimize_with_dependents,
+                    best_optimization = self.optimize_function(
                         function_to_optimize,
-                        code_context.dependent_functions,
-                        module_path,
-                        function_trace_id,
+                        function_to_tests,
+                        original_code,
                     )
-                    if not is_successful(tests_result):
-                        logging.error(tests_result.failure())
+                    if is_successful(best_optimization):
+                        optimizations_found += 1
+                    else:
+                        logging.error(best_optimization.failure())
                         continue
-                    tests_and_optimizations: TestsAndOptimizationsResult = tests_result.unwrap()
+            ph("cli-optimize-run-finished", {"optimizations_found": optimizations_found})
+            if optimizations_found == 0:
+                logging.info("❌ No optimizations found.")
+            elif self.args.all:
+                logging.info("✨ All functions have been optimized! ✨")
+        finally:
+            # TODO @afik.cohen: Also revert the file/function being optimized if the process did not succeed
+            for test_file in self.instrumented_unittests_created:
+                pathlib.Path(test_file).unlink(missing_ok=True)
+            for test_file in self.test_files_created:
+                pathlib.Path(test_file).unlink(missing_ok=True)
+            if hasattr(get_run_tmp_file, "tmpdir"):
+                get_run_tmp_file.tmpdir.cleanup()
 
-                    generated_tests_path = get_test_file_path(
-                        self.args.tests_root,
-                        function_to_optimize.function_name,
-                        0,
-                    )
-                    with open(generated_tests_path, "w", encoding="utf8") as file:
-                        file.write(tests_and_optimizations.instrumented_test_source)
+    def optimize_function(
+        self,
+        function_to_optimize: FunctionToOptimize,
+        function_to_tests: dict[str, list[TestsInFile]],
+        original_code: str,
+    ) -> Result[BestOptimization, str]:
+        should_run_experiment = self.experiment_id is not None
+        function_trace_id: str = str(uuid.uuid4())
+        ph("cli-optimize-function-start", {"function_trace_id": function_trace_id})
+        self.cleanup_leftover_test_return_values()
+        ctx_result = self.get_code_optimization_context(
+            function_to_optimize,
+            self.args.project_root,
+            original_code,
+        )
+        if not is_successful(ctx_result):
+            return Failure(ctx_result.failure())
+        code_context: CodeOptimizationContext = ctx_result.unwrap()
+        dependent_functions_by_module_abspath = defaultdict(set)
+        for _, module_abspath, qualified_name in code_context.dependent_functions:
+            dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
+        original_dependent_code = {}
+        for module_abspath in dependent_functions_by_module_abspath:
+            with pathlib.Path(module_abspath).open(encoding="utf8") as f:
+                dependent_code = f.read()
+                original_dependent_code[module_abspath] = dependent_code
+        logging.info(f"Code to be optimized:\n{code_context.code_to_optimize_with_dependents}")
+        module_path = module_name_from_file_path(function_to_optimize.file_path, self.args.project_root)
+
+        for module_abspath in original_dependent_code:
+            code_context.code_to_optimize_with_dependents = add_needed_imports_from_module(
+                original_dependent_code[module_abspath],
+                code_context.code_to_optimize_with_dependents,
+                module_abspath,
+                function_to_optimize.file_path,
+                self.args.project_root,
+            )
 
-                    test_files_created.add(generated_tests_path)
-                    baseline_result = self.establish_original_code_baseline(
-                        function_to_optimize.qualified_name,
-                        instrumented_unittests_created_for_function,
-                        generated_tests_path,
-                    )
-                    if not is_successful(baseline_result):
-                        logging.error(baseline_result.failure())
-                        continue
-                    original_code_baseline: OriginalCodeBaseline = baseline_result.unwrap()
-                    best_runtime = original_code_baseline.runtime  # The fastest code runtime until now
-                    logging.info("Optimizing code ...")
-                    # TODO: Postprocess the optimized function to include the original docstring and such
-
-                    best_optimization: Optional[BestOptimization] = None
-                    speedup_ratios: Dict[str, float | None] = dict()
-                    optimized_runtimes = dict()
-                    is_correct = dict()
-
-                    for i, optimization in enumerate(tests_and_optimizations.optimizations):
-                        j = i + 1
-                        if optimization.source_code is None:
-                            continue
-                        # remove left overs from previous run
-                        pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
-                            missing_ok=True,
-                        )
-                        pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
-                            missing_ok=True,
-                        )
-                        logging.info("Optimized candidate:")
-                        logging.info(optimization.source_code)
-                        try:
-                            replace_function_definitions_in_module(
-                                [function_to_optimize.qualified_name],
-                                optimization.source_code,
-                                path,
-                                code_context.preexisting_functions,
-                                code_context.contextual_dunder_methods,
-                            )
-                            for (
-                                module_abspath,
-                                qualified_names,
-                            ) in dependent_functions_by_module_abspath.items():
-                                replace_function_definitions_in_module(
-                                    list(qualified_names),
-                                    optimization.source_code,
-                                    module_abspath,
-                                    [],
-                                    code_context.contextual_dunder_methods,
-                                )
-                        except (
-                            ValueError,
-                            SyntaxError,
-                            cst.ParserSyntaxError,
-                            AttributeError,
-                        ) as e:
-                            logging.exception(e)
-                            self.write_code_and_dependents(
-                                original_code,
-                                original_dependent_code,
-                                path,
-                                dependent_functions_by_module_abspath,
-                            )
-                            continue
+        instrumented_unittests_created_for_function = self.instrument_existing_tests(
+            function_to_optimize=function_to_optimize,
+            function_to_tests=function_to_tests,
+        )
+        self.instrumented_unittests_created.update(instrumented_unittests_created_for_function)
 
-                        run_results = self.run_optimized_candidate(
-                            optimization_index=j,
-                            instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
-                            overall_original_test_results=original_code_baseline.overall_test_results,
-                            original_gen_results=original_code_baseline.generated_test_results,
-                            generated_tests_path=generated_tests_path,
-                            best_runtime_until_now=best_runtime,
-                        )
-                        if not is_successful(run_results):
-                            optimized_runtimes[optimization.optimization_id] = None
-                            is_correct[optimization.optimization_id] = False
-                            speedup_ratios[optimization.optimization_id] = None
-                        else:
-                            candidate_result: OptimizedCandidateResult = run_results.unwrap()
-                            best_test_runtime = candidate_result.best_test_runtime
-                            optimized_runtimes[optimization.optimization_id] = best_test_runtime
-                            is_correct[optimization.optimization_id] = True
-                            speedup_ratios[optimization.optimization_id] = (
-                                original_code_baseline.runtime - best_test_runtime
-                            ) / best_test_runtime
+        generated_results = self.generate_tests_and_optimizations(
+            code_context.code_to_optimize_with_dependents,
+            function_to_optimize,
+            code_context.dependent_functions,
+            module_path,
+            function_trace_id,
+            run_experiment=should_run_experiment,
+        )
+        if not is_successful(generated_results):
+            return Failure(generated_results.failure())
+        tests_and_opts: tuple[GeneratedTests, OptimizationSet] = generated_results.unwrap()
+        generated_tests, optimizations_set = tests_and_opts
+        generated_tests_path = get_test_file_path(
+            self.args.tests_root,
+            function_to_optimize.function_name,
+            0,
+        )
+        with pathlib.Path(generated_tests_path).open("w", encoding="utf8") as file:
+            file.write(generated_tests.instrumented_test_source)
+        self.test_files_created.add(generated_tests_path)
+        baseline_result = self.establish_original_code_baseline(
+            function_to_optimize.qualified_name,
+            instrumented_unittests_created_for_function,
+            generated_tests_path,
+            function_to_tests.get(module_path + "." + function_to_optimize.qualified_name, []),
+        )
+        if not is_successful(baseline_result):
+            pathlib.Path(generated_tests_path).unlink(missing_ok=True)
+            for instrumented_path in instrumented_unittests_created_for_function:
+                pathlib.Path(instrumented_path).unlink(missing_ok=True)
+            return Failure(baseline_result.failure())
+        original_code_baseline: OriginalCodeBaseline = baseline_result.unwrap()
+        logging.info("Optimizing code ...")
+        # TODO: Postprocess the optimized function to include the original docstring and such
 
-                            logging.info(
-                                f"Candidate runtime measured over {candidate_result.times_run} run{'s' if candidate_result.times_run > 1 else ''}: "
-                                f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
-                                f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime):.3f}",
-                            )
-                            if (
-                                ((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)
-                                > self.args.minimum_performance_gain
-                            ) and best_test_runtime < best_runtime:
-                                logging.info(
-                                    "This candidate is better than the previous best candidate.",
-                                )
-
-                                logging.info(
-                                    f"Original runtime: {humanize_runtime(original_code_baseline.runtime)} Best test runtime: "
-                                    f"{humanize_runtime(best_test_runtime)}, ratio = "
-                                    f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)}",
-                                )
-                                best_optimization = BestOptimization(
-                                    source_code=optimization.source_code,
-                                    explanation=optimization.explanation,
-                                    dependent_functions=code_context.dependent_functions,
-                                )
-                                best_runtime = best_test_runtime
-                                winning_test_results = candidate_result.best_test_results
-                        self.write_code_and_dependents(
-                            original_code,
-                            original_dependent_code,
-                            path,
-                            dependent_functions_by_module_abspath,
-                        )
-                        logging.info("----------------")
-                    log_results(
-                        function_trace_id=function_trace_id,
-                        speedup_ratio=speedup_ratios,
-                        original_runtime=original_code_baseline.runtime,
-                        optimized_runtime=optimized_runtimes,
-                        is_correct=is_correct,
-                    )
-                    ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
+        for u, candidates in enumerate(
+            [optimizations_set.control, optimizations_set.experiment],
+        ):
+            if candidates is None:
+                continue
 
-                    if best_optimization:
-                        optimizations_found += 1
-                        logging.info(
-                            f"Best candidate:\n{best_optimization.source_code}, {best_optimization.explanation}",
-                        )
+            tests_in_file: list[TestsInFile] = function_to_tests.get(
+                function_to_optimize.qualified_name_with_modules_from_root(self.args.project_root),
+                [],
+            )
 
-                        optimized_code = best_optimization.source_code
-                        explanation = Explanation(
-                            raw_explanation_message=best_optimization.explanation,
-                            winning_test_results=winning_test_results,
-                            original_runtime_ns=original_code_baseline.runtime,
-                            best_runtime_ns=best_runtime,
-                            function_name=function_to_optimize.qualified_name,
-                            path=path,
-                        )
+            best_optimization = self.determine_best_candidate(
+                candidates,
+                code_context,
+                dependent_functions_by_module_abspath,
+                function_to_optimize,
+                generated_tests_path,
+                instrumented_unittests_created_for_function,
+                original_code,
+                original_code_baseline,
+                original_dependent_code,
+                function_trace_id[:-4] + f"EXP{u}" if should_run_experiment else function_trace_id,
+                tests_in_file,
+            )
+            ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
 
-                        logging.info(
-                            f"⚡️ Optimization successful! 📄 {function_to_optimize.qualified_name} in {explanation.path}",
-                        )
-                        logging.info(f"📈 {explanation.perf_improvement_line}")
-                        logging.info(f"Explanation: \n{explanation.to_console_string()}")
-                        logging.info(
-                            f"Optimization was validated for correctness by running the following tests - "
-                            f"\n{tests_and_optimizations.generated_original_test_source}",
-                        )
+            if best_optimization:
+                logging.info(
+                    f"Best candidate:\n{best_optimization.candidate.source_code}, {best_optimization.candidate.explanation}",
+                )
 
-                        ph(
-                            "cli-optimize-success",
-                            {
-                                "function_trace_id": function_trace_id,
-                                "speedup_x": explanation.speedup_x,
-                                "speedup_pct": explanation.speedup_pct,
-                                "best_runtime": explanation.best_runtime_ns,
-                                "original_runtime": explanation.original_runtime_ns,
-                                "winning_test_results": {
-                                    tt.to_name(): v
-                                    for tt, v in explanation.winning_test_results.get_test_pass_fail_report_by_type().items()
-                                },
-                            },
-                        )
+                explanation = Explanation(
+                    raw_explanation_message=best_optimization.candidate.explanation,
+                    winning_test_results=best_optimization.winning_test_results,
+                    original_runtime_ns=original_code_baseline.runtime,
+                    best_runtime_ns=best_optimization.runtime,
+                    function_name=function_to_optimize.qualified_name,
+                    file_path=function_to_optimize.file_path,
+                )
 
-                        existing_tests = existing_tests_source_for(
-                            function_to_optimize.qualified_name,
-                            module_path,
-                            function_to_tests,
-                        )
+                self.log_successful_optimization(
+                    explanation,
+                    function_to_optimize,
+                    function_trace_id,
+                    generated_tests,
+                )
 
-                        self.replace_function_and_dependents_with_optimized_code(
-                            code_context,
-                            dependent_functions_by_module_abspath,
-                            explanation,
-                            optimized_code,
-                            function_to_optimize.qualified_name,
-                        )
+                self.replace_function_and_dependents_with_optimized_code(
+                    code_context,
+                    dependent_functions_by_module_abspath,
+                    explanation,
+                    best_optimization.candidate.source_code,
+                    function_to_optimize.qualified_name,
+                )
 
-                        new_code, new_dependent_code = self.reformat_code_and_dependents(
-                            dependent_functions_by_module_abspath,
-                            explanation.path,
+                new_code, new_dependent_code = self.reformat_code_and_dependents(
+                    dependent_functions_by_module_abspath,
+                    explanation.file_path,
+                    original_code,
+                )
+
+                existing_tests = existing_tests_source_for(
+                    function_to_optimize.qualified_name_with_modules_from_root(self.args.project_root),
+                    function_to_tests,
+                    tests_root=self.test_cfg.tests_root,
+                )
+
+                original_code_combined = original_dependent_code.copy()
+                original_code_combined[explanation.file_path] = original_code
+                new_code_combined = new_dependent_code.copy()
+                new_code_combined[explanation.file_path] = new_code
+                if not self.args.no_pr:
+                    check_create_pr(
+                        original_code=original_code_combined,
+                        new_code=new_code_combined,
+                        explanation=explanation,
+                        existing_tests_source=existing_tests,
+                        generated_original_test_source=generated_tests.generated_original_test_source,
+                    )
+                    if self.args.all or env_utils.get_pr_number():
+                        # Reverting to original code, because optimizing functions in a sequence can lead to
+                        #  a) Error propagation, where error in one function can cause the next optimization to fail
+                        #  b) Performance estimates become unstable, as the runtime of an optimization might be
+                        #     dependent on the runtime of the previous optimization
+                        self.write_code_and_dependents(
                             original_code,
+                            original_dependent_code,
+                            function_to_optimize.file_path,
+                            dependent_functions_by_module_abspath,
                         )
+        # Delete all the generated tests to not cause any clutter.
+        pathlib.Path(generated_tests_path).unlink(missing_ok=True)
+        for test_paths in instrumented_unittests_created_for_function:
+            pathlib.Path(test_paths).unlink(missing_ok=True)
+        return Success(best_optimization)
 
-                        original_code_combined = original_dependent_code.copy()
-                        original_code_combined[explanation.path] = original_code
-                        new_code_combined = new_dependent_code.copy()
-                        new_code_combined[explanation.path] = new_code
-                        check_create_pr(
-                            optimize_all=self.args.all,
-                            original_code=original_code_combined,
-                            new_code=new_code_combined,
-                            explanation=explanation,
-                            existing_tests_source=existing_tests,
-                            generated_original_test_source=tests_and_optimizations.generated_original_test_source,
-                        )
-                        if self.args.all or env_utils.get_pr_number():
-                            # Reverting to original code, because optimizing functions in a sequence can lead to
-                            #  a) Error propagation, where error in one function can cause the next optimization to fail
-                            #  b) Performance estimates become unstable, as the runtime of an optimization might be
-                            #     dependent on the runtime of the previous optimization
-                            self.write_code_and_dependents(
-                                original_code,
-                                original_dependent_code,
-                                path,
-                                dependent_functions_by_module_abspath,
-                            )
-                    # Delete all the generated tests to not cause any clutter.
-                    pathlib.Path(generated_tests_path).unlink(missing_ok=True)
-                    for test_paths in instrumented_unittests_created_for_function:
-                        pathlib.Path(test_paths).unlink(missing_ok=True)
-            ph("cli-optimize-run-finished", {"optimizations_found": optimizations_found})
-            if optimizations_found == 0:
-                logging.info("❌ No optimizations found.")
-            elif self.args.all:
-                logging.info("✨ All functions have been optimized! ✨")
-        finally:
-            # TODO: Also revert the file/function being optimized if the process did not succeed
-            for test_file in instrumented_unittests_created:
-                pathlib.Path(test_file).unlink(missing_ok=True)
-            for test_file in test_files_created:
-                pathlib.Path(test_file).unlink(missing_ok=True)
-            if hasattr(get_run_tmp_file, "tmpdir"):
-                get_run_tmp_file.tmpdir.cleanup()
+    def determine_best_candidate(
+        self,
+        candidates: list[OptimizedCandidate],
+        code_context: CodeOptimizationContext,
+        dependent_functions_by_module_abspath: dict[str, set[str]],
+        function_to_optimize: FunctionToOptimize,
+        generated_tests_path: str,
+        instrumented_unittests_created_for_function: set[str],
+        original_code: str,
+        original_code_baseline: OriginalCodeBaseline,
+        original_dependent_code: dict[str, str],
+        function_trace_id: str,
+        only_run_this_test_function: list[TestsInFile] | None = None,
+    ) -> BestOptimization | None:
+        best_optimization: BestOptimization | None = None
+        best_runtime_until_now = original_code_baseline.runtime  # The fastest code runtime until now
+
+        speedup_ratios: dict[str, float | None] = {}
+        optimized_runtimes = {}
+        is_correct = {}
+
+        for i, candidate in enumerate(candidates):
+            j = i + 1
+            if candidate.source_code is None:
+                continue
+            # remove left overs from previous run
+            pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
+                missing_ok=True,
+            )
+            pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
+                missing_ok=True,
+            )
+            logging.info("Optimized candidate:")
+            logging.info(candidate.source_code)
+            try:
+                replace_function_definitions_in_module(
+                    function_names=[function_to_optimize.qualified_name],
+                    optimized_code=candidate.source_code,
+                    file_path_of_module_with_function_to_optimize=function_to_optimize.file_path,
+                    module_abspath=function_to_optimize.file_path,
+                    preexisting_functions=code_context.preexisting_functions,
+                    contextual_functions=code_context.contextual_dunder_methods,
+                    project_root_path=self.args.project_root,
+                )
+                for (
+                    module_abspath,
+                    qualified_names,
+                ) in dependent_functions_by_module_abspath.items():
+                    replace_function_definitions_in_module(
+                        function_names=list(qualified_names),
+                        optimized_code=candidate.source_code,
+                        file_path_of_module_with_function_to_optimize=function_to_optimize.file_path,
+                        module_abspath=module_abspath,
+                        preexisting_functions=[],
+                        contextual_functions=code_context.contextual_dunder_methods,
+                        project_root_path=self.args.project_root,
+                    )
+            except (
+                ValueError,
+                SyntaxError,
+                cst.ParserSyntaxError,
+                AttributeError,
+            ) as e:
+                logging.exception(e)
+                self.write_code_and_dependents(
+                    original_code,
+                    original_dependent_code,
+                    function_to_optimize.file_path,
+                    dependent_functions_by_module_abspath,
+                )
+                continue
+
+            # Run generated tests if at least one of them passed
+            run_generated_tests = False
+            if original_code_baseline.generated_test_results:
+                for test_result in original_code_baseline.generated_test_results.test_results:
+                    if test_result.did_pass:
+                        run_generated_tests = True
+                        break
+
+            run_results = self.run_optimized_candidate(
+                optimization_index=j,
+                instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
+                overall_original_test_results=original_code_baseline.overall_test_results,
+                existing_test_results=original_code_baseline.existing_test_results,
+                original_gen_results=original_code_baseline.generated_test_results,
+                generated_tests_path=generated_tests_path,
+                best_runtime_until_now=best_runtime_until_now,
+                tests_in_file=only_run_this_test_function,
+                run_generated_tests=run_generated_tests,
+            )
+            if not is_successful(run_results):
+                optimized_runtimes[candidate.optimization_id] = None
+                is_correct[candidate.optimization_id] = False
+                speedup_ratios[candidate.optimization_id] = None
+            else:
+                candidate_result: OptimizedCandidateResult = run_results.unwrap()
+                best_test_runtime = candidate_result.best_test_runtime
+                optimized_runtimes[candidate.optimization_id] = best_test_runtime
+                is_correct[candidate.optimization_id] = True
+                speedup_ratios[candidate.optimization_id] = (
+                    original_code_baseline.runtime - best_test_runtime
+                ) / best_test_runtime
+
+                logging.info(
+                    f"Candidate runtime measured over {candidate_result.times_run} run{'s' if candidate_result.times_run > 1 else ''}: "
+                    f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
+                    f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime):.3f}",
+                )
+                if (
+                    ((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)
+                    > self.args.minimum_performance_gain
+                ) and best_test_runtime < best_runtime_until_now:
+                    logging.info(
+                        "This candidate is better than the previous best candidate.",
+                    )
+
+                    logging.info(
+                        f"Original runtime: {humanize_runtime(original_code_baseline.runtime)} Best test runtime: "
+                        f"{humanize_runtime(best_test_runtime)}, ratio = "
+                        f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)}",
+                    )
+                    best_optimization = BestOptimization(
+                        candidate=candidate,
+                        dependent_functions=code_context.dependent_functions,
+                        runtime=best_test_runtime,
+                        winning_test_results=candidate_result.best_test_results,
+                    )
+                    best_runtime_until_now = best_test_runtime
+            self.write_code_and_dependents(
+                original_code,
+                original_dependent_code,
+                function_to_optimize.file_path,
+                dependent_functions_by_module_abspath,
+            )
+            logging.info("----------------")
+        self.aiservice_client.log_results(
+            function_trace_id=function_trace_id,
+            speedup_ratio=speedup_ratios,
+            original_runtime=original_code_baseline.runtime,
+            optimized_runtime=optimized_runtimes,
+            is_correct=is_correct,
+        )
+        return best_optimization
+
+    def log_successful_optimization(
+        self,
+        explanation: Explanation,
+        function_to_optimize: FunctionToOptimize,
+        function_trace_id: str,
+        generated_tests: GeneratedTests,
+    ) -> None:
+        logging.info(
+            f"⚡️ Optimization successful! 📄 {function_to_optimize.qualified_name} in {explanation.file_path}",
+        )
+        logging.info(f"📈 {explanation.perf_improvement_line}")
+        logging.info(f"Explanation: \n{explanation.to_console_string()}")
+        logging.info(
+            f"Optimization was validated for correctness by running the following tests - "
+            f"\n{generated_tests.generated_original_test_source}",
+        )
+        ph(
+            "cli-optimize-success",
+            {
+                "function_trace_id": function_trace_id,
+                "speedup_x": explanation.speedup_x,
+                "speedup_pct": explanation.speedup_pct,
+                "best_runtime": explanation.best_runtime_ns,
+                "original_runtime": explanation.original_runtime_ns,
+                "winning_test_results": {
+                    tt.to_name(): v
+                    for tt, v in explanation.winning_test_results.get_test_pass_fail_report_by_type().items()
+                },
+            },
+        )
 
     def write_code_and_dependents(
         self,
         original_code: str,
-        original_dependent_code: Dict[str, str],
+        original_dependent_code: dict[str, str],
         path: str,
-        dependent_functions_by_module_abspath: Dict[str, set[str]],
+        dependent_functions_by_module_abspath: dict[str, set[str]],
     ) -> None:
-        with open(path, "w", encoding="utf8") as f:
+        with pathlib.Path(path).open("w", encoding="utf8") as f:
             f.write(original_code)
         for module_abspath in dependent_functions_by_module_abspath:
-            with open(module_abspath, "w", encoding="utf8") as f:
+            with pathlib.Path(module_abspath).open("w", encoding="utf8") as f:
                 f.write(original_dependent_code[module_abspath])
 
     def reformat_code_and_dependents(
         self,
-        dependent_functions_by_module_abspath: Dict[str, set[str]],
+        dependent_functions_by_module_abspath: dict[str, set[str]],
         path: str,
         original_code: str,
-    ) -> Tuple[str, Dict[str, str]]:
+    ) -> tuple[str, dict[str, str]]:
         should_sort_imports = True
-        if sort_imports(self.args.imports_sort_cmd, should_sort_imports, path) != original_code:
+        if isort.code(original_code) != original_code:
             should_sort_imports = False
 
         new_code = format_code(
             self.args.formatter_cmd,
             self.args.imports_sort_cmd,
             should_sort_imports,
             path,
@@ -474,51 +604,60 @@
             for module_abspath in dependent_functions_by_module_abspath
         }
         return new_code, new_dependent_code
 
     def replace_function_and_dependents_with_optimized_code(
         self,
         code_context: CodeOptimizationContext,
-        dependent_functions_by_module_abspath: Dict[str, set[str]],
+        dependent_functions_by_module_abspath: dict[str, set[str]],
         explanation: Explanation,
         optimized_code: str,
         qualified_function_name: str,
     ) -> None:
         replace_function_definitions_in_module(
-            [qualified_function_name],
-            optimized_code,
-            explanation.path,
-            code_context.preexisting_functions,
-            code_context.contextual_dunder_methods,
+            function_names=[qualified_function_name],
+            optimized_code=optimized_code,
+            file_path_of_module_with_function_to_optimize=explanation.file_path,
+            module_abspath=explanation.file_path,
+            preexisting_functions=code_context.preexisting_functions,
+            contextual_functions=code_context.contextual_dunder_methods,
+            project_root_path=self.args.project_root,
         )
         for (
             module_abspath,
             qualified_names,
         ) in dependent_functions_by_module_abspath.items():
             replace_function_definitions_in_module(
-                list(qualified_names),
-                optimized_code,
-                module_abspath,
-                [],
-                code_context.contextual_dunder_methods,
+                function_names=list(qualified_names),
+                optimized_code=optimized_code,
+                file_path_of_module_with_function_to_optimize=explanation.file_path,
+                module_abspath=module_abspath,
+                preexisting_functions=[],
+                contextual_functions=code_context.contextual_dunder_methods,
+                project_root_path=self.args.project_root,
             )
 
     def get_code_optimization_context(
         self,
         function_to_optimize: FunctionToOptimize,
+        project_root: str,
+        original_source_code: str,
     ) -> Result[CodeOptimizationContext, str]:
         code_to_optimize, contextual_dunder_methods = extract_code(
             [function_to_optimize],
         )
         if code_to_optimize is None:
             return Failure("Could not find function to optimize.")
         success, preexisting_functions = get_all_function_names(code_to_optimize)
         if not success:
             return Failure("Error in parsing the code, skipping optimization.")
-        dependent_code, dependent_functions = get_constrained_function_context_and_dependent_functions(
+        (
+            dependent_code,
+            dependent_functions,
+        ) = get_constrained_function_context_and_dependent_functions(
             function_to_optimize,
             self.args.project_root,
             code_to_optimize,
         )
         if function_to_optimize.parents:
             function_class = function_to_optimize.parents[0].name
             dependent_methods = [
@@ -539,129 +678,153 @@
             if len(optimizable_methods) > 1:
                 code_to_optimize, contextual_dunder_methods = extract_code(
                     optimizable_methods,
                 )
                 if code_to_optimize is None:
                     return Failure("Could not find function to optimize.")
         code_to_optimize_with_dependents = dependent_code + "\n" + code_to_optimize
+
+        code_to_optimize_with_dependents_and_imports = add_needed_imports_from_module(
+            original_source_code,
+            code_to_optimize_with_dependents,
+            function_to_optimize.file_path,
+            function_to_optimize.file_path,
+            project_root,
+        )
         preexisting_functions.extend(
             [fn[0].full_name.split(".")[-1] for fn in dependent_functions],
         )
         return Success(
             CodeOptimizationContext(
-                code_to_optimize_with_dependents=code_to_optimize_with_dependents,
+                code_to_optimize_with_dependents=code_to_optimize_with_dependents_and_imports,
                 contextual_dunder_methods=contextual_dunder_methods,
                 dependent_functions=dependent_functions,
                 preexisting_functions=preexisting_functions,
             ),
         )
 
-    def cleanup_leftover_test_return_values(self):
+    def cleanup_leftover_test_return_values(self) -> None:
         # remove leftovers from previous run
         pathlib.Path(get_run_tmp_file("test_return_values_0.bin")).unlink(
             missing_ok=True,
         )
         pathlib.Path(get_run_tmp_file("test_return_values_0.sqlite")).unlink(
             missing_ok=True,
         )
 
     def instrument_existing_tests(
         self,
-        function_name: str,
-        module_path: str,
+        function_to_optimize: FunctionToOptimize,
         function_to_tests: dict[str, list[TestsInFile]],
-    ):
+    ) -> set[str]:
         relevant_test_files_count = 0
         unique_original_test_files = set()
         unique_instrumented_test_files = set()
 
-        full_module_function_path = module_path + "." + function_name
-        if full_module_function_path not in function_to_tests:
+        func_qualname = function_to_optimize.qualified_name_with_modules_from_root(
+            self.args.project_root,
+        )
+        if func_qualname not in function_to_tests:
             logging.info(
-                "Did not find any pre-existing tests for '%s', will only use generated tests.",
-                full_module_function_path,
+                f"Did not find any pre-existing tests for '{func_qualname}', will only use generated tests.",
             )
         else:
-            for tests_in_file in function_to_tests.get(full_module_function_path):
+            for tests_in_file in function_to_tests.get(func_qualname):
                 if tests_in_file.test_file in unique_original_test_files:
                     continue
                 relevant_test_files_count += 1
                 success, injected_test = inject_profiling_into_existing_test(
                     tests_in_file.test_file,
-                    function_name,
+                    function_to_optimize.function_name,
                     self.args.project_root,
                 )
                 if not success:
                     continue
-                new_test_path = (
-                    os.path.splitext(tests_in_file.test_file)[0]
-                    + "__perfinstrumented"
-                    + os.path.splitext(tests_in_file.test_file)[1]
-                )
-                with open(new_test_path, "w", encoding="utf8") as f:
+                new_test_path = f"{os.path.splitext(tests_in_file.test_file)[0]}__perfinstrumented{os.path.splitext(tests_in_file.test_file)[1]}"
+                with pathlib.Path(new_test_path).open("w", encoding="utf8") as f:
                     f.write(injected_test)
                 unique_instrumented_test_files.add(new_test_path)
                 unique_original_test_files.add(tests_in_file.test_file)
             logging.info(
                 f"Discovered {relevant_test_files_count} existing unit test file"
-                f"{'s' if relevant_test_files_count != 1 else ''} for {full_module_function_path}",
+                f"{'s' if relevant_test_files_count != 1 else ''} for {func_qualname}",
             )
         return unique_instrumented_test_files
 
     def generate_tests_and_optimizations(
         self,
         code_to_optimize_with_dependents: str,
         function_to_optimize: FunctionToOptimize,
-        dependent_functions: list[Tuple[Source, str, str]],
+        dependent_functions: list[tuple[Source, str, str]],
         module_path: str,
         function_trace_id: str,
-    ) -> Result[TestsAndOptimizationsResult, str]:
+        run_experiment: bool = False,
+    ) -> Result[tuple[GeneratedTests, OptimizationSet], str]:
         generated_original_test_source = None
         instrumented_test_source = None
-        with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
+        max_workers = 2 if not run_experiment else 3
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_tests = executor.submit(
                 self.generate_and_instrument_tests,
                 code_to_optimize_with_dependents,
                 function_to_optimize,
                 [definition[0].full_name for definition in dependent_functions],
                 module_path,
-                function_trace_id,
+                function_trace_id[:-4] + "EXP0" if run_experiment else function_trace_id,
             )
-            future_optimization = executor.submit(
-                optimize_python_code,
+            future_optimization_candidates = executor.submit(
+                self.aiservice_client.optimize_python_code,
                 code_to_optimize_with_dependents,
-                function_trace_id,
+                function_trace_id[:-4] + "EXP0" if run_experiment else function_trace_id,
                 N_CANDIDATES,
+                ExperimentMetadata(id=self.experiment_id, group="control") if run_experiment else None,
             )
+            if run_experiment:
+                future_candidates_exp = executor.submit(
+                    self.local_aiservice_client.optimize_python_code,
+                    code_to_optimize_with_dependents,
+                    function_trace_id[:-4] + "EXP1",
+                    N_CANDIDATES,
+                    ExperimentMetadata(id=self.experiment_id, group="experiment"),
+                )
 
             future_tests_result = future_tests.result()
-            optimizations: List[Optimization] = future_optimization.result()
+            candidates: list[OptimizedCandidate] = future_optimization_candidates.result()
+
+            candidates_experiment = future_candidates_exp.result() if run_experiment else None
+
         if future_tests_result and isinstance(future_tests_result, tuple) and len(future_tests_result) == 2:
             (
                 generated_original_test_source,
                 instrumented_test_source,
             ) = future_tests_result
 
         else:
             return Failure(f"/!\\ NO TESTS GENERATED for {function_to_optimize.function_name}")
-        if not optimizations:
+        if not candidates:
             return Failure(f"/!\\ NO OPTIMIZATIONS GENERATED for {function_to_optimize.function_name}")
         return Success(
-            TestsAndOptimizationsResult(
-                generated_original_test_source=generated_original_test_source,
-                instrumented_test_source=instrumented_test_source,
-                optimizations=optimizations,
+            (
+                GeneratedTests(
+                    generated_original_test_source=generated_original_test_source,
+                    instrumented_test_source=instrumented_test_source,
+                ),
+                OptimizationSet(
+                    control=candidates,
+                    experiment=candidates_experiment,
+                ),
             ),
         )
 
     def establish_original_code_baseline(
         self,
         function_name: str,
         instrumented_unittests_created_for_function: set[str],
         generated_tests_path: str,
+        tests_in_file: List[TestsInFile],
     ) -> Result[OriginalCodeBaseline, str]:
         original_runtime = None
         best_runtime = None
         original_gen_results = None
         overall_original_test_results = None
         times_run = 0
         success = True
@@ -669,14 +832,15 @@
         generated_tests_elapsed_time = 0.0
 
         # For the original function - run the tests and get the runtime
         # TODO: Compare the function return values over the multiple runs and check if they are any different,
         #  if they are different, then we can't optimize this function because it is a non-deterministic function
         test_env = os.environ.copy()
         test_env["CODEFLASH_TEST_ITERATION"] = str(0)
+        test_env["CODEFLASH_TRACER_DISABLE"] = "1"
         if "PYTHONPATH" not in test_env:
             test_env["PYTHONPATH"] = self.args.project_root
         else:
             test_env["PYTHONPATH"] += os.pathsep + self.args.project_root
         cumulative_test_runtime = 0
         cumulative_test_runs = 0
         first_run = True
@@ -687,24 +851,38 @@
         ):
             for i in range(MAX_TEST_RUN_ITERATIONS):
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
                     do_break = True
                     break
                 instrumented_existing_test_timing = []
                 original_test_results_iter = TestResults()
+                existing_test_results = TestResults()
                 for test_file in instrumented_unittests_created_for_function:
+                    relevant_tests_in_file = [
+                        test_in_file
+                        for test_in_file in tests_in_file
+                        if test_in_file.test_file == test_file.replace("__perfinstrumented", "")
+                    ]
+                    is_replay_test = relevant_tests_in_file[0].test_type == TestType.REPLAY_TEST
+                    if is_replay_test and len(relevant_tests_in_file) > 1:
+                        logging.warning(
+                            f"Multiple tests found for the replay test {test_file}. Should not happen",
+                        )
+
                     unittest_results = self.run_and_parse_tests(
                         test_env,
                         test_file,
-                        TestType.EXISTING_UNIT_TEST,
+                        relevant_tests_in_file[0].test_type,
                         0,
+                        relevant_tests_in_file[0].test_function if is_replay_test else None,
                     )
 
                     timing = unittest_results.total_passed_runtime()
                     original_test_results_iter.merge(unittest_results)
+                    existing_test_results.merge(unittest_results)
                     instrumented_existing_test_timing.append(timing)
                 if i == 0 and first_run:
                     logging.info(
                         f"original code, existing unit test results -> {original_test_results_iter.get_test_pass_fail_report()}",
                     )
 
                 original_gen_results = self.run_and_parse_tests(
@@ -729,17 +907,21 @@
                 #  the execution to not reach the runtime measurement part. We are currently ignoring such tests, because the performance
                 #  for such a execution that raises an exception should not matter.
                 if i == 0 and first_run:
                     logging.info(
                         f"original generated tests results -> {original_gen_results.get_test_pass_fail_report()}",
                     )
 
-                original_total_runtime_iter = original_gen_results.total_passed_runtime() + sum(
-                    instrumented_existing_test_timing,
-                )
+                if not original_gen_results:
+                    original_total_runtime_iter = sum(instrumented_existing_test_timing)
+                else:
+                    original_total_runtime_iter = original_gen_results.total_passed_runtime() + sum(
+                        instrumented_existing_test_timing,
+                    )
+
                 if original_total_runtime_iter == 0:
                     logging.warning(
                         "The overall test runtime of the original function is 0, couldn't run tests.",
                     )
                     logging.warning(original_gen_results.test_results)
                     do_break = True
                     break
@@ -755,50 +937,55 @@
                 cumulative_test_runtime += original_total_runtime_iter
                 times_run += 1
             if first_run:
                 first_run = False
             if do_break:
                 break
 
-        if times_run == 0:
+        if times_run == 0 and original_runtime is None:
             logging.warning(
                 "Failed to run the tests for the original function, skipping optimization",
             )
             success = False
         if not success:
             return Failure("Failed to establish a baseline for the original code.")
         logging.info(
             f"Original code runtime measured over {times_run} run{'s' if times_run > 1 else ''}: {humanize_runtime(original_runtime)}",
         )
         return Success(
             OriginalCodeBaseline(
                 generated_test_results=original_gen_results,
+                existing_test_results=existing_test_results,
                 overall_test_results=overall_original_test_results,
                 runtime=best_runtime,
             ),
         )
 
     def run_optimized_candidate(
         self,
         optimization_index: int,
         instrumented_unittests_created_for_function: set[str],
         overall_original_test_results: TestResults,
+        existing_test_results: TestResults,
         original_gen_results: TestResults,
         generated_tests_path: str,
         best_runtime_until_now: int,
+        tests_in_file: Optional[List[TestsInFile]],
+        run_generated_tests: bool,
     ) -> Result[OptimizedCandidateResult, str]:
         success = True
         best_test_runtime = None
         best_test_results = None
         equal_results = True
         generated_tests_elapsed_time = 0.0
 
         times_run = 0
         test_env = os.environ.copy()
         test_env["CODEFLASH_TEST_ITERATION"] = str(optimization_index)
+        test_env["CODEFLASH_TRACER_DISABLE"] = "1"
         if "PYTHONPATH" not in test_env:
             test_env["PYTHONPATH"] = self.args.project_root
         else:
             test_env["PYTHONPATH"] += os.pathsep + self.args.project_root
         cumulative_test_runtime = 0
         cumulative_test_runs = 0
         first_run = True
@@ -817,77 +1004,100 @@
                 if generated_tests_elapsed_time > MAX_FUNCTION_TEST_SECONDS:
                     do_break = True
                     break
 
                 optimized_test_results_iter = TestResults()
                 instrumented_test_timing = []
                 for instrumented_test_file in instrumented_unittests_created_for_function:
+                    relevant_tests_in_file = [
+                        test_in_file
+                        for test_in_file in tests_in_file
+                        if test_in_file.test_file == instrumented_test_file.replace("__perfinstrumented", "")
+                    ]
+                    is_replay_test = relevant_tests_in_file[0].test_type == TestType.REPLAY_TEST
+                    if is_replay_test and len(relevant_tests_in_file) > 1:
+                        logging.warning(
+                            f"Multiple tests found for the replay test {instrumented_test_file}. Should not happen",
+                        )
                     unittest_results_optimized = self.run_and_parse_tests(
                         test_env,
                         instrumented_test_file,
-                        TestType.EXISTING_UNIT_TEST,
+                        relevant_tests_in_file[0].test_type,
                         optimization_index,
+                        relevant_tests_in_file[0].test_function if is_replay_test else None,
                     )
                     timing = unittest_results_optimized.total_passed_runtime()
                     optimized_test_results_iter.merge(unittest_results_optimized)
                     instrumented_test_timing.append(timing)
                 if first_run and test_index == 0:
                     equal_results = True
                     logging.info(
                         f"optimized existing unit tests result -> {optimized_test_results_iter.get_test_pass_fail_report()}",
                     )
+                    equal_return_values = compare_results(
+                        existing_test_results,
+                        optimized_test_results_iter,
+                    )
                     for test_invocation in optimized_test_results_iter:
                         if (
                             overall_original_test_results.get_by_id(test_invocation.id) is None
                             or test_invocation.did_pass
-                            != overall_original_test_results.get_by_id(test_invocation.id).did_pass
+                            != overall_original_test_results.get_by_id(
+                                test_invocation.id,
+                            ).did_pass
+                            or not equal_return_values
                         ):
                             logging.info("Results did not match.")
                             logging.info(
                                 f"Test {test_invocation.id} failed on the optimized code. Skipping this optimization",
                             )
                             equal_results = False
                             do_break = True
                             break
                     if not equal_results:
                         do_break = True
                         break
 
-                test_results = self.run_and_parse_tests(
-                    test_env,
-                    generated_tests_path,
-                    TestType.GENERATED_REGRESSION,
-                    optimization_index,
-                )
+                test_results = None
+                if run_generated_tests:
+                    test_results = self.run_and_parse_tests(
+                        test_env,
+                        generated_tests_path,
+                        TestType.GENERATED_REGRESSION,
+                        optimization_index,
+                    )
 
-                if first_run and test_index == 0:
+                if test_results and first_run and test_index == 0:
                     logging.info(
                         f"generated test_results optimized -> {test_results.get_test_pass_fail_report()}",
                     )
-                    if test_results:
-                        if compare_results(original_gen_results, test_results):
-                            equal_results = True
-                            logging.info("Results matched!")
-                        else:
-                            logging.info("Results did not match.")
-                            equal_results = False
+                    if compare_results(original_gen_results, test_results):
+                        equal_results = True
+                        logging.info("Results matched!")
+                    else:
+                        logging.info("Results did not match.")
+                        equal_results = False
                 if not equal_results:
                     do_break = True
                     break
 
-                test_runtime = test_results.total_passed_runtime() + sum(instrumented_test_timing)
+                if not test_results:
+                    test_runtime = sum(instrumented_test_timing)
+                else:
+                    test_runtime = test_results.total_passed_runtime() + sum(instrumented_test_timing)
 
                 if test_runtime == 0:
                     logging.warning(
                         "The overall test runtime of the optimized function is 0, couldn't run tests.",
                     )
                     do_break = True
                     break
                 if best_test_runtime is None or test_runtime < best_test_runtime:
-                    optimized_test_results_iter.merge(test_results)
+                    if test_results:
+                        optimized_test_results_iter.merge(test_results)
                     best_test_runtime = test_runtime
                     best_test_results = optimized_test_results_iter
                 cumulative_test_runs += 1
                 cumulative_test_runtime += test_runtime
                 times_run += 1
             if first_run:
                 first_run = False
@@ -920,23 +1130,25 @@
 
     def run_and_parse_tests(
         self,
         test_env: dict[str, str],
         test_file: str,
         test_type: TestType,
         optimization_iteration: int,
+        test_function: Optional[str] = None,
     ) -> TestResults:
         result_file_path, run_result = run_tests(
             test_file,
             test_framework=self.args.test_framework,
             cwd=self.args.project_root,
             pytest_timeout=INDIVIDUAL_TEST_TIMEOUT,
             pytest_cmd=self.test_cfg.pytest_cmd,
             verbose=True,
             test_env=test_env,
+            only_run_this_test_function=test_function,
         )
         if run_result.returncode != 0:
             logging.debug(
                 f"Nonzero return code {run_result.returncode} when running tests in {test_file}.\n"
                 f"stdout: {run_result.stdout}\n"
                 f"stderr: {run_result.stderr}\n",
             )
@@ -955,14 +1167,15 @@
         source_code_being_tested: str,
         function_to_optimize: FunctionToOptimize,
         dependent_function_names: list[str],
         module_path: str,
         function_trace_id: str,
     ) -> Union[Tuple[str, str], None]:
         tests = generate_tests(
+            self.aiservice_client,
             source_code_being_tested=source_code_being_tested,
             function_to_optimize=function_to_optimize,
             dependent_function_names=dependent_function_names,
             module_path=module_path,
             test_cfg=self.test_cfg,
             test_timeout=INDIVIDUAL_TEST_TIMEOUT,
             use_cached_tests=self.args.use_cached_tests,
```

### Comparing `codeflash-0.5.1/codeflash/result/create_pr.py` & `codeflash-0.6.0/codeflash/result/create_pr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,52 @@
+from __future__ import annotations
+
 import logging
 import os.path
 import pathlib
-from typing import Dict, List, Optional
+from typing import Dict, Optional
 
 from codeflash.api import cfapi
 from codeflash.code_utils import env_utils
 from codeflash.code_utils.git_utils import (
     get_current_branch,
     get_repo_owner_and_name,
     git_root_dir,
 )
 from codeflash.discovery.discover_unit_tests import TestsInFile
 from codeflash.github.PrComment import FileDiffContent, PrComment
 from codeflash.result.explanation import Explanation
 
 
 def existing_tests_source_for(
-    qualified_function_name: str,
-    module_path: str,
-    function_to_tests: Dict[str, List[TestsInFile]],
+    function_qualified_name_with_modules_from_root: str,
+    function_to_tests: Dict[str, list[TestsInFile]],
+    tests_root: str,
 ) -> str:
-    test_files = function_to_tests.get(module_path + "." + qualified_function_name)
+    test_files = function_to_tests.get(function_qualified_name_with_modules_from_root)
     existing_tests = ""
     if test_files:
         for test_file in test_files:
-            with open(test_file.test_file, encoding="utf8") as f:
-                new_test = "".join(f.readlines())
-                if new_test not in existing_tests:
-                    existing_tests += new_test
+            existing_tests += "- " + os.path.relpath(test_file.test_file, tests_root) + "\n"
     return existing_tests
 
 
 def check_create_pr(
-    optimize_all: bool,
     original_code: dict[str, str],
     new_code: dict[str, str],
     explanation: Explanation,
     existing_tests_source: str,
     generated_original_test_source: str,
-):
+) -> None:
     pr_number: Optional[int] = env_utils.get_pr_number()
 
     if pr_number is not None:
         logging.info(f"Suggesting changes to PR #{pr_number} ...")
         owner, repo = get_repo_owner_and_name()
-        relative_path = str(pathlib.Path(os.path.relpath(explanation.path, git_root_dir())).as_posix())
+        relative_path = str(pathlib.Path(os.path.relpath(explanation.file_path, git_root_dir())).as_posix())
         response = cfapi.suggest_changes(
             owner=owner,
             repo=repo,
             pr_number=pr_number,
             file_changes={
                 str(pathlib.Path(os.path.relpath(p, git_root_dir())).as_posix()): FileDiffContent(
                     oldContent=original_code[p],
@@ -72,20 +70,19 @@
         if response.ok:
             logging.info(f"Suggestions were successfully made to PR #{pr_number}")
         else:
             logging.error(
                 f"Optimization was successful, but I failed to suggest changes to PR #{pr_number}."
                 f" Response from server was: {response.text}",
             )
-
-    elif optimize_all:
+    else:
         logging.info("Creating a new PR with the optimized code...")
         owner, repo = get_repo_owner_and_name()
 
-        relative_path = str(pathlib.Path(os.path.relpath(explanation.path, git_root_dir())).as_posix())
+        relative_path = str(pathlib.Path(os.path.relpath(explanation.file_path, git_root_dir())).as_posix())
         base_branch = get_current_branch()
         response = cfapi.create_pr(
             owner=owner,
             repo=repo,
             base_branch=base_branch,
             file_changes={
                 str(pathlib.Path(os.path.relpath(p, git_root_dir())).as_posix()): FileDiffContent(
```

### Comparing `codeflash-0.5.1/codeflash/result/explanation.py` & `codeflash-0.6.0/codeflash/result/explanation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @dataclass(frozen=True, config={"arbitrary_types_allowed": True})
 class Explanation:
     raw_explanation_message: str
     winning_test_results: TestResults
     original_runtime_ns: int
     best_runtime_ns: int
     function_name: str
-    path: str
+    file_path: str
 
     @property
     def perf_improvement_line(self) -> str:
         return f"{self.speedup_pct} improvement ({self.speedup_x} faster)."
 
     @property
     def speedup(self) -> float:
@@ -32,15 +32,15 @@
     def to_console_string(self) -> str:
         # TODO: After doing the best optimization, remove the test cases that errored on the new code, because they might be failing because of syntax errors and such.
         # TODO: Sometimes the explanation says something similar to "This is the code that was optimized", remove such parts
         original_runtime_human = humanize_runtime(self.original_runtime_ns)
         best_runtime_human = humanize_runtime(self.best_runtime_ns)
 
         explanation = (
-            f"Optimized {self.function_name} in {self.path}\n"
+            f"Optimized {self.function_name} in {self.file_path}\n"
             f"{self.perf_improvement_line}\n"
             f"Runtime went down from {original_runtime_human} to {best_runtime_human} \n\n"
             + "Explanation:\n"
             + self.raw_explanation_message
             + " \n\n"
             + "The new optimized code was tested for correctness. The results are listed below.\n"
             + f"{TestResults.report_to_string(self.winning_test_results.get_test_pass_fail_report_by_type())}\n"
```

### Comparing `codeflash-0.5.1/codeflash/telemetry/posthog.py` & `codeflash-0.6.0/codeflash/telemetry/posthog.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/telemetry/sentry.py` & `codeflash-0.6.0/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/update_license_version.py` & `codeflash-0.6.0/codeflash/update_license_version.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/verification/comparator.py` & `codeflash-0.6.0/codeflash/verification/comparator.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,16 @@
                 pandas.Categorical,
                 pandas.arrays.SparseArray,
             ),
         ):
             return orig.equals(new)
 
         if HAS_PANDAS and isinstance(
-            orig, (pandas.CategoricalDtype, pandas.Interval, pandas.Period),
+            orig,
+            (pandas.CategoricalDtype, pandas.Interval, pandas.Period),
         ):
             return orig == new
 
         # This should be at the end of all numpy checking
         try:
             if HAS_NUMPY and np.isnan(orig):
                 return np.isnan(new)
@@ -130,21 +131,27 @@
         except Exception:
             pass
 
         if isinstance(orig, (datetime.datetime, datetime.date, datetime.timedelta)):
             return orig == new
 
         # If the object passed has a user defined __eq__ method, use that
-        # This could fail if the user defined __eq__ is defined with cython
+        # This could fail if the user defined __eq__ is defined with C-extensions
         try:
             if hasattr(orig, "__eq__") and str(type(orig.__eq__)) == "<class 'method'>":
                 return orig == new
         except Exception:
             pass
 
+        # For class objects
+        if hasattr(orig, "__dict__") and hasattr(new, "__dict__"):
+            orig_keys = orig.__dict__
+            new_keys = new.__dict__
+            return comparator(orig_keys, new_keys)
+
         # TODO : Add other types here
         logging.warning(f"Unknown comparator input type: {type(orig)}")
         return True
     except RecursionError as e:
         logging.exception(f"RecursionError while comparing objects: {e}")
         sentry_sdk.capture_exception(e)
         return False
```

### Comparing `codeflash-0.5.1/codeflash/verification/equivalence.py` & `codeflash-0.6.0/codeflash/verification/equivalence.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.1/codeflash/verification/parse_test_output.py` & `codeflash-0.6.0/codeflash/verification/parse_test_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,23 @@
     test_type: TestType,
     test_config: TestConfig,
 ):
     test_results = TestResults()
     if not os.path.exists(sqlite_file_path):
         logging.warning(f"No test results for {sqlite_file_path} found.")
         return test_results
-    db = sqlite3.connect(sqlite_file_path)
-    cur = db.cursor()
-    data = cur.execute(
-        "SELECT test_module_path , test_class_name , test_function_name , "
-        "function_getting_tested , iteration_id , runtime  FROM test_results",
-    ).fetchall()
+    try:
+        db = sqlite3.connect(sqlite_file_path)
+        cur = db.cursor()
+        data = cur.execute(
+            "SELECT test_module_path , test_class_name , test_function_name , "
+            "function_getting_tested , iteration_id , runtime, return_value  FROM test_results",
+        ).fetchall()
+    finally:
+        db.close()
     for val in data:
         test_results.add(
             FunctionTestInvocation(
                 id=InvocationId(
                     test_module_path=val[0],
                     test_class_name=val[1],
                     test_function_name=val[2],
@@ -102,15 +105,15 @@
                     iteration_id=val[4],
                 ),
                 file_name=test_py_file_path,
                 did_pass=True,
                 runtime=val[5],
                 test_framework=test_config.test_framework,
                 test_type=test_type,
-                return_value=None,
+                return_value=pickle.loads(val[6]),
             ),
         )
         # return_value is only None temporarily as this is only being used for the existing tests. This should generalize
         # to read the return_value from the sqlite file as well.
         # Hardcoding the test result to True because the test did execute and we are only interested in the return values,
         # the did_pass comes from the xml results file
     return test_results
@@ -321,20 +324,20 @@
             )
         except AttributeError as e:
             logging.exception(e)
             test_results_bin_file = TestResults()
             pathlib.Path(
                 get_run_tmp_file(f"test_return_values_{optimization_iteration}.bin"),
             ).unlink(missing_ok=True)
-    elif test_type == TestType.EXISTING_UNIT_TEST:
+    elif test_type in [TestType.EXISTING_UNIT_TEST, TestType.REPLAY_TEST]:
         try:
             test_results_bin_file = parse_sqlite_test_results(
                 get_run_tmp_file(f"test_return_values_{optimization_iteration}.sqlite"),
                 test_py_file_path=test_py_path,
-                test_type=TestType.EXISTING_UNIT_TEST,
+                test_type=test_type,
                 test_config=test_config,
             )
         except AttributeError as e:
             logging.exception(e)
             test_results_bin_file = TestResults()
     else:
         raise ValueError(f"Invalid test type: {test_type}")
```

### Comparing `codeflash-0.5.1/codeflash/verification/test_results.py` & `codeflash-0.6.0/codeflash/verification/test_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from codeflash.verification.comparator import comparator
 
 
 class TestType(Enum):
     EXISTING_UNIT_TEST = 1
     INSPIRED_REGRESSION = 2
     GENERATED_REGRESSION = 3
+    REPLAY_TEST = 4
 
     def to_name(self) -> str:
         names = {
             TestType.EXISTING_UNIT_TEST: "⚙️ Existing Unit Tests",
             TestType.INSPIRED_REGRESSION: "🎨 Inspired Regression Tests",
             TestType.GENERATED_REGRESSION: "🌀 Generated Regression Tests",
+            TestType.REPLAY_TEST: "⏪ Replay Tests",
         }
         return names[self]
 
 
 @dataclass(frozen=True)
 class InvocationId:
     test_module_path: str  # The fully qualified name of the test module
@@ -73,15 +75,18 @@
 
     def add(self, function_test_invocation: FunctionTestInvocation) -> None:
         self.test_results.append(function_test_invocation)
 
     def merge(self, other: TestResults) -> None:
         self.test_results.extend(other.test_results)
 
-    def get_by_id(self, invocation_id: InvocationId) -> Optional[FunctionTestInvocation]:
+    def get_by_id(
+        self,
+        invocation_id: InvocationId,
+    ) -> Optional[FunctionTestInvocation]:
         return next((r for r in self.test_results if r.id == invocation_id), None)
 
     def get_all_ids(self) -> List[InvocationId]:
         return [test_result.id for test_result in self.test_results]
 
     def get_test_pass_fail_report(self) -> str:
         passed = 0
@@ -112,15 +117,17 @@
                 for test_type in TestType
             ],
         )
 
     def total_passed_runtime(self) -> int:
         for result in self.test_results:
             if result.did_pass and result.runtime is None:
-                logging.debug(f"Ignoring test case that passed but had no runtime -> {result.id}")
+                logging.debug(
+                    f"Ignoring test case that passed but had no runtime -> {result.id}",
+                )
         timing = sum(
             [
                 result.runtime
                 for result in self.test_results
                 if (result.did_pass and result.runtime is not None)
             ],
         )
@@ -163,13 +170,16 @@
                 sys.setrecursionlimit(5000)
             if (
                 test_result.file_name != other_test_result.file_name
                 or test_result.did_pass != other_test_result.did_pass
                 or test_result.runtime != other_test_result.runtime
                 or test_result.test_framework != other_test_result.test_framework
                 or test_result.test_type != other_test_result.test_type
-                or not comparator(test_result.return_value, other_test_result.return_value)
+                or not comparator(
+                    test_result.return_value,
+                    other_test_result.return_value,
+                )
             ):
                 sys.setrecursionlimit(original_recursion_limit)
                 return False
         sys.setrecursionlimit(original_recursion_limit)
         return True
```

### Comparing `codeflash-0.5.1/codeflash/verification/test_runner.py` & `codeflash-0.6.0/codeflash/verification/test_runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 import subprocess
 from typing import Optional, Tuple
 
 from codeflash.code_utils.code_utils import get_run_tmp_file
 
 
 def run_tests(
-    test_path,
+    test_path: str,
     test_framework: str,
     cwd: Optional[str] = None,
     test_env: Optional[dict[str, str]] = None,
     pytest_timeout: Optional[int] = None,
     pytest_cmd: str = "pytest",
     verbose: bool = False,
+    only_run_this_test_function: Optional[str] = None,
 ) -> Tuple[str, subprocess.CompletedProcess]:
     assert test_framework in ["pytest", "unittest"]
+    if only_run_this_test_function and "__replay_test" in test_path:
+        test_path = test_path + "::" + only_run_this_test_function
+
     if test_framework == "pytest":
         result_file_path = get_run_tmp_file("pytest_results.xml")
         pytest_cmd_list = [chunk for chunk in pytest_cmd.split(" ") if chunk != ""]
         results = subprocess.run(
             pytest_cmd_list
             + [
                 test_path,
                 "-q",
                 f"--timeout={pytest_timeout}",
                 f"--junitxml={result_file_path}",
             ],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
-            env=test_env, check=False,
+            env=test_env,
+            check=False,
+            timeout=600,
         )
     elif test_framework == "unittest":
         result_file_path = get_run_tmp_file("unittest_results.xml")
         results = subprocess.run(
             ["python", "-m", "xmlrunner"]
             + (["-v"] if verbose else [])
             + [test_path]
             + ["--output-file", result_file_path],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
-            env=test_env, check=False,
+            env=test_env,
+            check=False,
         )
     else:
         raise ValueError("Invalid test framework -- I only support Pytest and Unittest currently.")
     return result_file_path, results
```

### Comparing `codeflash-0.5.1/codeflash/verification/verification_utils.py` & `codeflash-0.6.0/codeflash/verification/verification_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_test_file_path(
     test_dir: str, function_name: str, iteration: int = 0, test_type: str = "unit",
 ) -> str:
     assert test_type in ["unit", "inspired", "replay"]
     function_name = function_name.replace(".", "_")
     path = os.path.join(test_dir, f"test_{function_name}__{test_type}_test_{iteration}.py")
     if os.path.exists(path):
-        return get_test_file_path(test_dir, function_name, iteration + 1)
+        return get_test_file_path(test_dir, function_name, iteration + 1, test_type)
     return path
 
 
 def delete_multiple_if_name_main(test_ast: ast.Module) -> ast.Module:
     if_indexes = []
     for index, node in enumerate(test_ast.body):
         if isinstance(node, ast.If):
```

### Comparing `codeflash-0.5.1/codeflash/verification/verifier.py` & `codeflash-0.6.0/codeflash/verification/verifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import ast
 import logging
 from typing import Optional, Tuple
 
-from codeflash.api.aiservice import generate_regression_tests
+from codeflash.api.aiservice import AiServiceClient
 from codeflash.code_utils.code_utils import get_run_tmp_file, module_name_from_file_path
 from codeflash.discovery.functions_to_optimize import FunctionToOptimize
 from codeflash.verification.verification_utils import (
     ModifyInspiredTests,
     TestConfig,
     delete_multiple_if_name_main,
     get_test_file_path,
 )
 
 
 def generate_tests(
+    aiservice_client: AiServiceClient,
     source_code_being_tested: str,
     function_to_optimize: FunctionToOptimize,
     dependent_function_names: list[str],
     module_path: str,
     test_cfg: TestConfig,
     test_timeout: int,
     use_cached_tests: bool,
@@ -30,37 +31,39 @@
         import importlib
 
         module = importlib.import_module(module_path)
         generated_test_source = module.CACHED_TESTS
         instrumented_test_source = module.CACHED_INSTRUMENTED_TESTS
         path = get_run_tmp_file("").replace("\\", "\\\\")  # Escape backslash for windows paths
         instrumented_test_source = instrumented_test_source.replace(
-            "{codeflash_run_tmp_dir_client_side}", path,
+            "{codeflash_run_tmp_dir_client_side}",
+            path,
         )
         logging.info(f"Using cached tests from {module_path}.CACHED_TESTS")
     else:
         test_module_path = module_name_from_file_path(
             get_test_file_path(test_cfg.tests_root, function_to_optimize.function_name, 0),
             test_cfg.project_root_path,
         )
-        response = generate_regression_tests(
+        response = aiservice_client.generate_regression_tests(
             source_code_being_tested=source_code_being_tested,
             function_to_optimize=function_to_optimize,
             dependent_function_names=dependent_function_names,
             module_path=module_path,
             test_module_path=test_module_path,
             test_framework=test_cfg.test_framework,
             test_timeout=test_timeout,
             trace_id=function_trace_id,
         )
         if response and isinstance(response, tuple) and len(response) == 2:
             generated_test_source, instrumented_test_source = response
             path = get_run_tmp_file("").replace("\\", "\\\\")  # Escape backslash for windows paths
             instrumented_test_source = instrumented_test_source.replace(
-                "{codeflash_run_tmp_dir_client_side}", path,
+                "{codeflash_run_tmp_dir_client_side}",
+                path,
             )
         else:
             logging.error(f"Failed to generate and instrument tests for {function_to_optimize.function_name}")
             return None
 
     # TODO: Add support for inspired tests
     # inspired_unit_tests = ""
```

### Comparing `codeflash-0.5.1/pyproject.toml` & `codeflash-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.5.1" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.6.0" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
@@ -14,40 +14,40 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 unidiff = ">=0.7.4"
 pytest = ">=7.0.0"
 gitpython = ">=3.1.31"
 libcst = ">=1.0.1"
-jedi = ">=0.19.0"
+jedi = ">=0.19.1"
 tiktoken = ">=0.3.2"
 timeout-decorator = ">=0.5.0"
 pytest-timeout = ">=2.1.0"
 tomlkit = ">=0.11.7"
 unittest-xml-reporting = ">=3.2.0"
 junitparser = ">=3.1.0"
 pydantic = ">=1.10.1"
 black = ">=22.3.0"
 humanize = ">=4.0.0"
 posthog = ">=3.0.0"
 click = ">=8.1.0"
 inquirer = ">=3.0.0"
-sentry-sdk = "^1.40.6"
+sentry-sdk = ">=1.40.6,<3.0.0"
 parameterized = ">=0.9.0"
 returns = "^0.22.0"
 isort = ">=5.11.0"
 dill = "^0.3.8"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.12.0"
 mypy = "^1.9.0"
-ruff = "^0.3.5"
+ruff = ">=0.3.5,<0.5.0"
 ruff-lsp = "^0.0.53"
 
 
 [tool.poetry.build]
 script = "codeflash/update_license_version.py"
 
 [tool.poetry.scripts]
```

### Comparing `codeflash-0.5.1/PKG-INFO` & `codeflash-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.5.1
+Version: 0.6.0
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=22.3.0)
 Requires-Dist: click (>=8.1.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: gitpython (>=3.1.31)
 Requires-Dist: humanize (>=4.0.0)
 Requires-Dist: inquirer (>=3.0.0)
 Requires-Dist: isort (>=5.11.0)
-Requires-Dist: jedi (>=0.19.0)
+Requires-Dist: jedi (>=0.19.1)
 Requires-Dist: junitparser (>=3.1.0)
 Requires-Dist: libcst (>=1.0.1)
 Requires-Dist: parameterized (>=0.9.0)
 Requires-Dist: posthog (>=3.0.0)
 Requires-Dist: pydantic (>=1.10.1)
 Requires-Dist: pytest (>=7.0.0)
 Requires-Dist: pytest-timeout (>=2.1.0)
 Requires-Dist: returns (>=0.22.0,<0.23.0)
-Requires-Dist: sentry-sdk (>=1.40.6,<2.0.0)
+Requires-Dist: sentry-sdk (>=1.40.6,<3.0.0)
 Requires-Dist: tiktoken (>=0.3.2)
 Requires-Dist: timeout-decorator (>=0.5.0)
 Requires-Dist: tomlkit (>=0.11.7)
 Requires-Dist: unidiff (>=0.7.4)
 Requires-Dist: unittest-xml-reporting (>=3.2.0)
 Description-Content-Type: text/markdown
```

