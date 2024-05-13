# Comparing `tmp/mentabotix-0.1.3a2.tar.gz` & `tmp/mentabotix-0.1.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.3a2.tar", last modified: Sat May 11 09:40:05 2024, max compression
+gzip compressed data, was "mentabotix-0.1.3a3.tar", last modified: Mon May 13 04:47:39 2024, max compression
```

## Comparing `mentabotix-0.1.3a2.tar` & `mentabotix-0.1.3a3.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0    23777 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/README.md
--rw-r--r--   0        0        0      678 2024-05-11 09:40:05.521548 mentabotix-0.1.3a2/pyproject.toml
--rw-r--r--   0        0        0     1205 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    68552 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    19645 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     7826 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     5457 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/vision/camra.py
--rw-r--r--   0        0        0     8877 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/tests/__init__.py
--rw-r--r--   0        0        0    15471 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/tests/test_botix.py
--rw-r--r--   0        0        0     8569 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/tests/test_composer.py
--rw-r--r--   0        0        0     8042 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-11 09:39:40.373714 mentabotix-0.1.3a2/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24211 1970-01-01 00:00:00.000000 mentabotix-0.1.3a2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-11 10:49:56.434347 mentabotix-0.1.3a3/LICENSE
+-rw-r--r--   0        0        0    24490 2024-05-10 14:24:15.565070 mentabotix-0.1.3a3/README.md
+-rw-r--r--   0        0        0      678 2024-05-13 04:47:39.511660 mentabotix-0.1.3a3/pyproject.toml
+-rw-r--r--   0        0        0     1247 2024-05-11 09:34:46.781746 mentabotix-0.1.3a3/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    70023 2024-05-10 11:13:50.138660 mentabotix-0.1.3a3/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      243 2024-04-26 04:06:07.890426 mentabotix-0.1.3a3/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      607 2024-04-23 16:23:50.814617 mentabotix-0.1.3a3/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    20066 2024-04-23 16:16:48.574660 mentabotix-0.1.3a3/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     8042 2024-05-13 04:27:57.847730 mentabotix-0.1.3a3/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2374 2024-05-11 09:33:14.033099 mentabotix-0.1.3a3/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     5622 2024-05-04 13:49:32.402944 mentabotix-0.1.3a3/src/mentabotix/vision/camra.py
+-rw-r--r--   0        0        0     9183 2024-05-11 09:31:37.393645 mentabotix-0.1.3a3/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-04-21 15:01:09.781087 mentabotix-0.1.3a3/tests/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-13 04:31:00.807242 mentabotix-0.1.3a3/tests/composed.puml
+-rw-r--r--   0        0        0    10663 2024-05-13 04:31:01.398233 mentabotix-0.1.3a3/tests/long_chain.puml
+-rw-r--r--   0        0        0      729 2024-05-10 14:09:04.520348 mentabotix-0.1.3a3/tests/test.puml
+-rw-r--r--   0        0        0    15829 2024-05-10 11:11:09.668333 mentabotix-0.1.3a3/tests/test_botix.py
+-rw-r--r--   0        0        0     8777 2024-05-13 04:29:23.109111 mentabotix-0.1.3a3/tests/test_composer.py
+-rw-r--r--   0        0        0     8266 2024-04-24 04:50:22.570337 mentabotix-0.1.3a3/tests/test_menta.py
+-rw-r--r--   0        0        0     6645 2024-05-08 10:50:44.494471 mentabotix-0.1.3a3/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5707 2024-04-27 08:48:13.462320 mentabotix-0.1.3a3/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24211 1970-01-01 00:00:00.000000 mentabotix-0.1.3a3/PKG-INFO
```

### Comparing `mentabotix-0.1.3a2/README.md` & `mentabotix-0.1.3a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mentabotix
+Version: 0.1.3a3
+Summary: A Bot control lib
+Author-Email: Whth <88489697+Whth@users.noreply.github.com>
+License: MIT
+Requires-Python: >=3.11
+Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pyapriltags>=3.3.0.3
+Requires-Dist: terminaltables>=3.1.10
+Requires-Dist: bdmc>=0.1.5
+Requires-Dist: opencv-python-headless>=4.9.0.80
+Description-Content-Type: text/markdown
+
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
 
 ## Installation
```

### Comparing `mentabotix-0.1.3a2/pyproject.toml` & `mentabotix-0.1.3a3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.3a2"
+version = "0.1.3a3"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.3a2/src/mentabotix/__init__.py` & `mentabotix-0.1.3a3/src/mentabotix/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from .modules.botix import MovingState, MovingTransition, Botix
-from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
-from .modules.logger import set_log_level
-from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
-
-from .tools.composers import MovingChainComposer, straight_chain, snaking_chain, scanning_chain
-from .tools.generators import NameGenerator, Multipliers, make_multiplier_generator
-from .vision.camra import Camera
-from .vision.tagdetector import TagDetector
-
-__all__ = [
-    "set_log_level",
-    # botix
-    "MovingState",
-    "MovingTransition",
-    "Botix",
-    # menta
-    "Menta",
-    "SequenceSampler",
-    "IndexedSampler",
-    "DirectSampler",
-    "SamplerUsage",
-    "SamplerType",
-    "Sampler",
-    # vision
-    "Camera",
-    "TagDetector",
-    # exceptions
-    "BadSignatureError",
-    "RequirementError",
-    "SamplerTypeError",
-    "TokenizeError",
-    "StructuralError",
-    # tools/composers
-    "MovingChainComposer",
-    "straight_chain",
-    "snaking_chain",
-    "scanning_chain",
-    # tools/generators
-    "NameGenerator",
-    "Multipliers",
-]
+from .modules.botix import MovingState, MovingTransition, Botix
+from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
+from .modules.logger import set_log_level
+from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
+
+from .tools.composers import MovingChainComposer, straight_chain, snaking_chain, scanning_chain
+from .tools.generators import NameGenerator, Multipliers, make_multiplier_generator
+from .vision.camra import Camera
+from .vision.tagdetector import TagDetector
+
+__all__ = [
+    "set_log_level",
+    # botix
+    "MovingState",
+    "MovingTransition",
+    "Botix",
+    # menta
+    "Menta",
+    "SequenceSampler",
+    "IndexedSampler",
+    "DirectSampler",
+    "SamplerUsage",
+    "SamplerType",
+    "Sampler",
+    # vision
+    "Camera",
+    "TagDetector",
+    # exceptions
+    "BadSignatureError",
+    "RequirementError",
+    "SamplerTypeError",
+    "TokenizeError",
+    "StructuralError",
+    # tools/composers
+    "MovingChainComposer",
+    "straight_chain",
+    "snaking_chain",
+    "scanning_chain",
+    # tools/generators
+    "NameGenerator",
+    "Multipliers",
+]
```

### Comparing `mentabotix-0.1.3a2/src/mentabotix/modules/logger.py` & `mentabotix-0.1.3a3/src/mentabotix/modules/logger.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import logging
-
-import coloredlogs
-
-# 初始化logger
-_logger = logging.getLogger("mentabotix")
-coloredlogs.install(logger=_logger, level=logging.DEBUG)
-
-
-def set_log_level(level: int | str):
-    """
-    设置日志级别
-    :param level: 日志级别
-    :return:
-    """
-    _logger.setLevel(level)
-
-
-set_log_level(logging.INFO)
-
-if __name__ == "__main__":
-
-    _logger.debug("This is a debug log.")
-    _logger.info("This is a info log.")
-    _logger.warning("This is a warning log.")
-    _logger.error("This is a error log.")
-    _logger.critical("This is a critical log.")
+import logging
+
+import coloredlogs
+
+# 初始化logger
+_logger = logging.getLogger("mentabotix")
+coloredlogs.install(logger=_logger, level=logging.DEBUG)
+
+
+def set_log_level(level: int | str):
+    """
+    设置日志级别
+    :param level: 日志级别
+    :return:
+    """
+    _logger.setLevel(level)
+
+
+set_log_level(logging.INFO)
+
+if __name__ == "__main__":
+
+    _logger.debug("This is a debug log.")
+    _logger.info("This is a info log.")
+    _logger.warning("This is a warning log.")
+    _logger.error("This is a error log.")
+    _logger.critical("This is a critical log.")
```

### Comparing `mentabotix-0.1.3a2/src/mentabotix/modules/menta.py` & `mentabotix-0.1.3a3/src/mentabotix/modules/menta.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,421 +1,421 @@
-from enum import Enum
-from inspect import signature, Signature
-from typing import (
-    Callable,
-    TypeAlias,
-    List,
-    Optional,
-    Tuple,
-    Sequence,
-    NamedTuple,
-    Union,
-    Self,
-    SupportsInt,
-    SupportsFloat,
-    Dict,
-    Any,
-)
-
-from .exceptions import BadSignatureError, RequirementError
-from .logger import _logger
-
-SensorData: TypeAlias = float | int
-# basically, no restrictions, support py objects or ctypes._CData variants
-SensorDataSequence: TypeAlias = Sequence[SensorData]
-UpdaterClosure = Callable[[], SensorDataSequence] | Callable[[], SensorData]
-
-SequenceSampler: TypeAlias = Callable[[], SensorDataSequence]
-IndexedSampler: TypeAlias = Callable[[int], SensorData]
-DirectSampler: TypeAlias = Callable[[], SensorData]
-
-Sampler: TypeAlias = Union[SequenceSampler, IndexedSampler, DirectSampler]
-SourceCode: TypeAlias = str
-
-
-class SamplerType(Enum):
-    """
-    采样器类型
-    """
-
-    SEQ_SAMPLER: int = 1
-    IDX_SAMPLER: int = 2
-    DRC_SAMPLER: int = 3
-
-
-class SamplerUsage(NamedTuple):
-    used_sampler_index: int
-    required_data_indexes: Sequence[int]
-
-
-class Menta:
-    # reserved to check the return type of the sampler
-    __supported__ = (SupportsInt, SupportsFloat)
-
-    def __init__(
-        self,
-        samplers: Optional[List[Sampler]] = None,
-    ):
-        self.samplers: List[Sampler] = samplers or []
-        self.sampler_types: List[SamplerType] = []
-        self.update_sampler_types()
-
-    def update_sampler_types(self) -> Self:
-        """
-        更新采样器类型列表。遍历self.samplers中的每个采样器，根据其返回类型和参数数量将其分类为序列采样器（SEQ_SAMPLER）、
-        索引采样器（IDX_SAMPLER）或直接响应采样器（DRC_SAMPLER），并更新self.sampler_types列表。
-        如果采样器没有指定返回类型或指定的返回类型不被支持，则抛出异常。
-
-        返回值:
-            Self: 更新后的实例自身。
-        """
-
-        self.sampler_types.clear()  # 清空当前的采样器类型列表
-        for sampler in self.samplers:  # 遍历所有采样器
-            sig = signature(sampler)  # 获取采样器的签名
-
-            match sig.return_annotation:  # 根据采样器的返回类型进行匹配
-                case seq_sampler_ret if issubclass(seq_sampler_ret, Sequence) and len(sig.parameters) == 0:
-                    # 如果返回类型是序列且无参数，则认定为序列采样器
-                    self.sampler_types.append(SamplerType.SEQ_SAMPLER)
-                case idx_sampler_ret if len(sig.parameters) == 1 and isinstance(idx_sampler_ret, self.__supported__):
-                    # 如果返回类型是索引且只有一个参数，则认定为索引采样器
-                    self.sampler_types.append(SamplerType.IDX_SAMPLER)
-                case drc_sampler_ret if len(sig.parameters) == 0 and isinstance(drc_sampler_ret, self.__supported__):
-                    # 如果返回类型是直接响应且无参数，则认定为直接响应采样器
-                    self.sampler_types.append(SamplerType.DRC_SAMPLER)
-                case Signature.empty:
-                    # 如果采样器没有指定返回类型，则抛出异常
-                    raise BadSignatureError(
-                        f"Sampler {sampler} must have annotated return type!\nGot {sig.return_annotation}"
-                    )
-                case invalid_sampler_ret:
-                    # 如果采样器的返回类型注解无效，则抛出异常
-                    raise BadSignatureError(
-                        f"Sampler {sampler} has invalid return type annotation(s)!\n"
-                        f"Must be {SensorDataSequence} or {SensorData} but got {invalid_sampler_ret}"
-                    )
-        return self  # 返回更新后的实例自身
-
-    def construct_updater(self, usages: List[SamplerUsage]) -> Callable[[], Tuple] | Callable[[], SensorData]:
-        """
-        Constructs an updater function based on the given list of sampler usages.
-
-        Args:
-            usages (List[SamplerUsage]): A list of sampler usages.
-
-        Returns:
-            Callable[[], Tuple]: The constructed updater function.
-
-        Raises:
-            ValueError: If the number of sampler usages does not match the number of samplers.
-            RuntimeError: If an unsupported sampler type is encountered.
-        """
-        self.update_sampler_types()
-        if len(self.sampler_types) != len(self.samplers):
-            raise ValueError(
-                f"Number of sampler usages ({len(usages)}) does not match number of samplers ({len(self.samplers)}), have you used the update_sampler_types() method?"
-            )
-        if len(usages) == 0:
-            raise RequirementError("Can't resolve the empty Usage List")
-        update_funcs: List[UpdaterClosure] = []
-
-        for usage in usages:
-            _logger.debug(
-                f"Sampler_type: {self.sampler_types[usage.used_sampler_index]}|Required: {usage.required_data_indexes}"
-            )
-            sampler = self.samplers[usage.used_sampler_index]
-            sampler_type = self.sampler_types[usage.used_sampler_index]
-            match sampler_type:
-                case SamplerType.SEQ_SAMPLER:
-                    update_funcs.append(self.resolve_seq_sampler(sampler, usage.required_data_indexes))
-                case SamplerType.IDX_SAMPLER:
-                    update_funcs.append(self.resolve_idx_sampler(sampler, usage.required_data_indexes))
-                case SamplerType.DRC_SAMPLER:
-                    update_funcs.append(self.resolve_drc_sampler(sampler, usage.required_data_indexes))
-                case _:
-                    raise RuntimeError(f"Unsupported sampler type: {sampler_type}")
-
-        # TODO allow make flatten ret
-        if len(update_funcs) == 1:
-            return update_funcs[0]
-        eval_kwargs = {f"func_{i}": update_funcs[i] for i in range(len(update_funcs))}
-        func_call_strings = [f"{func}()" for func in eval_kwargs]
-        eval_string = "lambda:" + "(" + f",".join(func_call_strings) + ")"
-        eval_obj = eval(eval_string, eval_kwargs)
-        return eval_obj
-
-    def construct_judge_function(
-        self,
-        usages: List[SamplerUsage],
-        judging_source: List[SourceCode] | SourceCode,
-        extra_context: Dict[str, Any] = None,
-    ) -> Callable[[], bool]:
-        """
-        构造一个判断函数。该函数根据提供的采样器使用情况、判断源和额外的上下文信息，动态生成一个判断逻辑的函数。
-
-        参数:
-        - usages: 一个SamplerUsage对象的列表，描述了每个采样器是如何被使用的。
-        - judging_source: 判断源，可以是字符串或字符串列表。定义了判断逻辑的代码。
-        - extra_context: 可选的字典，提供了额外的上下文信息，这些信息在执行判断函数时会包含在执行环境中。
-
-        返回值:
-        - 一个无参数的布尔型函数，执行时根据判断逻辑返回True或False。
-        """
-
-        # 将judging_source统一处理为字符串格式
-        judging_source: str = judging_source if isinstance(judging_source, str) else "\n ".join(judging_source)
-
-        # 定义返回标识符，检查判断源中是否包含该标识符
-        RET_IDENTIFIER: str = "ret"
-        if RET_IDENTIFIER not in judging_source:
-            raise RequirementError(
-                f"Can't find {RET_IDENTIFIER} in judging source, you must define a variable named {RET_IDENTIFIER} in your judging source!\n"
-                f"Since it will be used as the return value of the judge function."
-            )
-
-        # 匹配使用情况与相应的采样器和采样器类型
-        _logger.debug("Match Usage with corresponding samplers and sampler_types")
-        used_samplers: Dict[str, Any] = {
-            f"func_{i}": self.samplers[usage.used_sampler_index] for i, usage in enumerate(usages)
-        }
-        _logger.debug(f"Matched samplers: {used_samplers}")
-        self.update_sampler_types()
-        used_sampler_types = [self.sampler_types[usage.used_sampler_index] for usage in usages]
-        _logger.debug(f"Matched sampler_types: {used_sampler_types}")
-
-        # 根据采样器类型，为采样器数据创建索引表达式
-        sampler_temp_var_names_mapping: Dict[str, str] = {}
-        indexed_expressions: List[str] = []
-        for usage, sampler_type, func_name in zip(usages, used_sampler_types, used_samplers):
-
-            match sampler_type:
-                case SamplerType.SEQ_SAMPLER:
-                    sampler_temp_var_names_mapping[temp_name := f"{func_name}_temp"] = func_name
-                    indexed_expressions.extend(self._index_for_seq_sampler_data(temp_name, usage.required_data_indexes))
-                case SamplerType.IDX_SAMPLER:
-                    indexed_expressions.extend(self._index_for_idx_sampler_data(func_name, usage.required_data_indexes))
-                case SamplerType.DRC_SAMPLER:
-                    sampler_temp_var_names_mapping[temp_name := f"{func_name}_temp"] = func_name
-                    indexed_expressions.extend(self._index_for_drc_sampler_data(temp_name, usage.required_data_indexes))
-                case _:
-                    raise RuntimeError(f"Unsupported sampler type: {sampler_type}")
-        _logger.debug(f"Created {len(indexed_expressions)} indexed expressions.")
-
-        # 创建占位变量并检查是否所有占位符都被包含在判断源中
-        placebo_var_names = [f"s{i}" for i in range(len(indexed_expressions))]
-        _logger.debug(f"Created {len(placebo_var_names)} placebo variables.")
-        _logger.debug("Checking that all placeholders are included in judging_source")
-        if not_included := [placebo for placebo in placebo_var_names if placebo not in judging_source]:
-            raise RequirementError(
-                f"Judging source must have all placeholders: {placebo_var_names} in judging_source\n"
-                f"Missing: {not_included}"
-            )
-
-        # 替换判断源中的占位符为索引表达式
-        for placebo, expr in zip(placebo_var_names, indexed_expressions):
-            _logger.debug(f'Replacing "{placebo}" with "{expr}".')
-            judging_source = judging_source.replace(placebo, expr)
-
-        # 创建临时变量的源代码，用于在执行环境中存储采样器的返回值
-        temp_var_source: str = (
-            ",".join(sampler_temp_var_names_mapping.keys())
-            + "="
-            + ",".join([f"{fname}()" for fname in sampler_temp_var_names_mapping.values()])
-        )
-        _logger.debug(f"Created temp_var_source: {temp_var_source}")
-
-        # 构建完整的函数源码并编译执行
-        func_source = f"def _func():\n" f" {temp_var_source}\n" f" {judging_source}\n" f" return {RET_IDENTIFIER}"
-        _logger.debug(f"Created func_source: {func_source}")
-        _logger.debug("Compiling func_source")
-
-        # 更新执行环境中的采样器和额外上下文信息
-        used_samplers.update(extra_context) if extra_context else None
-        exec(func_source, used_samplers)  # exec the source with the context
-        func_obj: Callable[[], bool] = used_samplers.get("_func")
-        _logger.debug(f"Succeed, compiled func_obj: {func_obj}")
-        return func_obj
-
-    @staticmethod
-    def _index_for_seq_sampler_data(data_var_name: str, required: List[int] | int) -> List[str]:
-        """
-        A function that generates a list of indexed expressions based on the given data variable name and a list of required indexes.
-
-        Args:
-            data_var_name (str): The name of the data variable.
-            required (List[int] | int): Either a single integer representing the required sequence length or a list of required data indexes.
-
-        Returns:
-            List[str]: A list of indexed expressions based on the data variable name and required indexes.
-        """
-        match required:
-            case int(required_seq_length):
-                final_required_data_indexes = range(required_seq_length)
-            case list(required_data_indexes):
-                final_required_data_indexes = required_data_indexes
-            case _:
-                raise RequirementError(
-                    f"Unknown Input, arg::required has to be either list[int] or int, got {required}"
-                )
-        return [f"{data_var_name}[{i}]" for i in final_required_data_indexes]
-
-    @staticmethod
-    def _index_for_drc_sampler_data(data_var_name: str, required: List[int] | int) -> List[str]:
-        """
-        A function that generates a list of indexed expressions based on the given data variable name and a list of required indexes.
-
-        Args:
-            data_var_name (str): The name of the data variable.
-            required (List[int] | int): Either a single integer representing the required sequence length or a list of required data indexes.
-
-        Returns:
-            List[str]: A list of indexed expressions based on the data variable name and required indexes.
-        """
-        match required:
-            case []:
-                raise RequirementError("Can't resolve the empty Usage List")
-            case int(required_seq_length):
-                final_required_data_indexes = range(required_seq_length)
-            case list(required_data_indexes):
-                final_required_data_indexes = required_data_indexes
-            case _:
-                raise RequirementError(
-                    f"Unknown Input, arg::required has to be either list[int] or int, got {required}"
-                )
-        return [f"(({data_var_name}>>{i})&1)" for i in final_required_data_indexes]
-
-    @staticmethod
-    def _index_for_idx_sampler_data(func_var_name: str, required: List[int]) -> List[str]:
-        """
-        Generate a list of indexed expressions based on the given function variable name and a list of required indexes.
-
-        Args:
-            func_var_name (str): The name of the function variable.
-            required (List[int]): A list of required indexes.
-
-        Returns:
-            List[str]: A list of indexed expressions based on the function variable name and required indexes.
-        """
-        return [f"{func_var_name}({i})" for i in required]
-
-    @staticmethod
-    def resolve_seq_sampler(sampler: SequenceSampler, required_data_indexes: Sequence[int]) -> UpdaterClosure:
-        """
-        Resolves the sampler based on the given sequence sampler and required data indexes.
-
-        Args:
-            sampler (SequenceSampler): The sequence sampler to resolve.
-            required_data_indexes (Sequence[int]): The required data indexes.
-
-        Returns:
-            UpdaterClosure: A callable that returns a tuple of SensorData objects
-            or a single SensorData object based on the number of required data indexes.
-
-        Raises:
-            None
-
-        Examples:
-            sampler = SequenceSampler()
-            required_data_indexes = []
-            resolved_sampler = resolve_seq_sampler(sampler, required_data_indexes)
-            data = resolved_sampler()  # Returns a tuple of all SensorData objects
-
-            sampler = SequenceSampler()
-            required_data_indexes = [0]
-            resolved_sampler = resolve_seq_sampler(sampler, required_data_indexes)
-            data = resolved_sampler()  # Returns the SensorData object at index 0
-
-            sampler = SequenceSampler()
-            required_data_indexes = [0, 1, 2]
-            resolved_sampler = resolve_seq_sampler(sampler, required_data_indexes)
-            data = resolved_sampler()  # Returns a tuple of SensorData objects at indexes 0, 1, and 2
-        """
-        match len(required_data_indexes):
-            case 0:
-                # 0 means require all data
-                return sampler  # Callable[[],SensorDataSequence]
-            case 1:
-                # 1 means require a specific data
-                unique_index = required_data_indexes[0]
-                return lambda: sampler()[unique_index]  # Callable[[], SensorData]
-            case _:
-                # >1 means require multiple data
-                required_indexes = required_data_indexes
-
-                def _fun() -> Tuple[SensorData, ...]:
-                    data = sampler()
-                    return tuple(data[i] for i in required_indexes)
-
-                return _fun  # Callable[[],SensorDataSequence]
-
-    @staticmethod
-    def resolve_idx_sampler(sampler: IndexedSampler, required_data_indexes: Sequence[int]) -> UpdaterClosure:
-        """
-        Resolves the indexed sampler based on the given sampler usage.
-
-        Args:
-            sampler (IndexedSampler): The indexed sampler to resolve.
-            required_data_indexes (Sequence[int]): The required data indexes.
-
-        Returns:
-            UpdaterClosure: A callable that returns a tuple of SensorData objects or a single SensorData object based on the number of required data indexes.
-
-        Raises:
-            RequirementError: If no required data indexes are specified.
-
-        Examples:
-            sampler = IndexedSampler()
-            required_data_indexes = []
-            resolved_sampler = resolve_idx_sampler(sampler, required_data_indexes)  # Raises RequirementError
-
-            sampler = IndexedSampler()
-            required_data_indexes = [0]
-            resolved_sampler = resolve_idx_sampler(sampler, required_data_indexes)
-            data = resolved_sampler()  # Returns the SensorData object at index 0
-
-            sampler = IndexedSampler()
-            required_data_indexes = [0, 1, 2]
-            resolved_sampler = resolve_idx_sampler(sampler, required_data_indexes)
-            data = resolved_sampler()  # Returns a tuple of the SensorData objects at indexes 0, 1, and 2
-        """
-
-        match len(required_data_indexes):
-            case 0:
-                raise RequirementError("Must specify at least one required data index")
-            case 1:
-                # 1 means require a specific data
-                unique_index = required_data_indexes[0]
-                return lambda: sampler(unique_index)  # Callable[[], SensorData]
-            case _:
-                # >1 means require multiple data
-                required_indexes = required_data_indexes
-                return lambda: tuple(sampler(ri) for ri in required_indexes)  # Callable[[], SensorDataSequence]
-
-    @staticmethod
-    def resolve_drc_sampler(sampler: DirectSampler, required_data_indexes: Sequence[int]) -> UpdaterClosure:
-        """
-        Resolves the direct sampler based on the given direct sampler and required data indexes.
-
-        Args:
-            sampler (DirectSampler): The direct sampler to resolve.
-            required_data_indexes (Sequence[int]): The required data indexes.
-
-        Returns:
-            UpdaterClosure: A callable that returns a tuple of SensorData objects or a single SensorData object based on the number of required data indexes.
-        """
-
-        match len(required_data_indexes):
-            case 0:
-                return sampler  # Callable[[], SensorData]
-            case 1:
-                # 1 means require a specific data
-                unique_index = required_data_indexes[0]
-                return lambda: (sampler() >> unique_index) & 1
-            case _:
-                # >1 means require multiple data
-
-                def _fun() -> SensorDataSequence:
-                    temp_seq = sampler()
-                    return tuple((temp_seq >> ri) & 1 for ri in required_data_indexes)
-
-                return _fun
+from enum import Enum
+from inspect import signature, Signature
+from typing import (
+    Callable,
+    TypeAlias,
+    List,
+    Optional,
+    Tuple,
+    Sequence,
+    NamedTuple,
+    Union,
+    Self,
+    SupportsInt,
+    SupportsFloat,
+    Dict,
+    Any,
+)
+
+from .exceptions import BadSignatureError, RequirementError
+from .logger import _logger
+
+SensorData: TypeAlias = float | int
+# basically, no restrictions, support py objects or ctypes._CData variants
+SensorDataSequence: TypeAlias = Sequence[SensorData]
+UpdaterClosure = Callable[[], SensorDataSequence] | Callable[[], SensorData]
+
+SequenceSampler: TypeAlias = Callable[[], SensorDataSequence]
+IndexedSampler: TypeAlias = Callable[[int], SensorData]
+DirectSampler: TypeAlias = Callable[[], SensorData]
+
+Sampler: TypeAlias = Union[SequenceSampler, IndexedSampler, DirectSampler]
+SourceCode: TypeAlias = str
+
+
+class SamplerType(Enum):
+    """
+    采样器类型
+    """
+
+    SEQ_SAMPLER: int = 1
+    IDX_SAMPLER: int = 2
+    DRC_SAMPLER: int = 3
+
+
+class SamplerUsage(NamedTuple):
+    used_sampler_index: int
+    required_data_indexes: Sequence[int]
+
+
+class Menta:
+    # reserved to check the return type of the sampler
+    __supported__ = (SupportsInt, SupportsFloat)
+
+    def __init__(
+        self,
+        samplers: Optional[List[Sampler]] = None,
+    ):
+        self.samplers: List[Sampler] = samplers or []
+        self.sampler_types: List[SamplerType] = []
+        self.update_sampler_types()
+
+    def update_sampler_types(self) -> Self:
+        """
+        更新采样器类型列表。遍历self.samplers中的每个采样器，根据其返回类型和参数数量将其分类为序列采样器（SEQ_SAMPLER）、
+        索引采样器（IDX_SAMPLER）或直接响应采样器（DRC_SAMPLER），并更新self.sampler_types列表。
+        如果采样器没有指定返回类型或指定的返回类型不被支持，则抛出异常。
+
+        返回值:
+            Self: 更新后的实例自身。
+        """
+
+        self.sampler_types.clear()  # 清空当前的采样器类型列表
+        for sampler in self.samplers:  # 遍历所有采样器
+            sig = signature(sampler)  # 获取采样器的签名
+
+            match sig.return_annotation:  # 根据采样器的返回类型进行匹配
+                case seq_sampler_ret if issubclass(seq_sampler_ret, Sequence) and len(sig.parameters) == 0:
+                    # 如果返回类型是序列且无参数，则认定为序列采样器
+                    self.sampler_types.append(SamplerType.SEQ_SAMPLER)
+                case idx_sampler_ret if len(sig.parameters) == 1 and isinstance(idx_sampler_ret, self.__supported__):
+                    # 如果返回类型是索引且只有一个参数，则认定为索引采样器
+                    self.sampler_types.append(SamplerType.IDX_SAMPLER)
+                case drc_sampler_ret if len(sig.parameters) == 0 and isinstance(drc_sampler_ret, self.__supported__):
+                    # 如果返回类型是直接响应且无参数，则认定为直接响应采样器
+                    self.sampler_types.append(SamplerType.DRC_SAMPLER)
+                case Signature.empty:
+                    # 如果采样器没有指定返回类型，则抛出异常
+                    raise BadSignatureError(
+                        f"Sampler {sampler} must have annotated return type!\nGot {sig.return_annotation}"
+                    )
+                case invalid_sampler_ret:
+                    # 如果采样器的返回类型注解无效，则抛出异常
+                    raise BadSignatureError(
+                        f"Sampler {sampler} has invalid return type annotation(s)!\n"
+                        f"Must be {SensorDataSequence} or {SensorData} but got {invalid_sampler_ret}"
+                    )
+        return self  # 返回更新后的实例自身
+
+    def construct_updater(self, usages: List[SamplerUsage]) -> Callable[[], Tuple] | Callable[[], SensorData]:
+        """
+        Constructs an updater function based on the given list of sampler usages.
+
+        Args:
+            usages (List[SamplerUsage]): A list of sampler usages.
+
+        Returns:
+            Callable[[], Tuple]: The constructed updater function.
+
+        Raises:
+            ValueError: If the number of sampler usages does not match the number of samplers.
+            RuntimeError: If an unsupported sampler type is encountered.
+        """
+        self.update_sampler_types()
+        if len(self.sampler_types) != len(self.samplers):
+            raise ValueError(
+                f"Number of sampler usages ({len(usages)}) does not match number of samplers ({len(self.samplers)}), have you used the update_sampler_types() method?"
+            )
+        if len(usages) == 0:
+            raise RequirementError("Can't resolve the empty Usage List")
+        update_funcs: List[UpdaterClosure] = []
+
+        for usage in usages:
+            _logger.debug(
+                f"Sampler_type: {self.sampler_types[usage.used_sampler_index]}|Required: {usage.required_data_indexes}"
+            )
+            sampler = self.samplers[usage.used_sampler_index]
+            sampler_type = self.sampler_types[usage.used_sampler_index]
+            match sampler_type:
+                case SamplerType.SEQ_SAMPLER:
+                    update_funcs.append(self.resolve_seq_sampler(sampler, usage.required_data_indexes))
+                case SamplerType.IDX_SAMPLER:
+                    update_funcs.append(self.resolve_idx_sampler(sampler, usage.required_data_indexes))
+                case SamplerType.DRC_SAMPLER:
+                    update_funcs.append(self.resolve_drc_sampler(sampler, usage.required_data_indexes))
+                case _:
+                    raise RuntimeError(f"Unsupported sampler type: {sampler_type}")
+
+        # TODO allow make flatten ret
+        if len(update_funcs) == 1:
+            return update_funcs[0]
+        eval_kwargs = {f"func_{i}": update_funcs[i] for i in range(len(update_funcs))}
+        func_call_strings = [f"{func}()" for func in eval_kwargs]
+        eval_string = "lambda:" + "(" + f",".join(func_call_strings) + ")"
+        eval_obj = eval(eval_string, eval_kwargs)
+        return eval_obj
+
+    def construct_judge_function(
+        self,
+        usages: List[SamplerUsage],
+        judging_source: List[SourceCode] | SourceCode,
+        extra_context: Dict[str, Any] = None,
+    ) -> Callable[[], bool]:
+        """
+        构造一个判断函数。该函数根据提供的采样器使用情况、判断源和额外的上下文信息，动态生成一个判断逻辑的函数。
+
+        参数:
+        - usages: 一个SamplerUsage对象的列表，描述了每个采样器是如何被使用的。
+        - judging_source: 判断源，可以是字符串或字符串列表。定义了判断逻辑的代码。
+        - extra_context: 可选的字典，提供了额外的上下文信息，这些信息在执行判断函数时会包含在执行环境中。
+
+        返回值:
+        - 一个无参数的布尔型函数，执行时根据判断逻辑返回True或False。
+        """
+
+        # 将judging_source统一处理为字符串格式
+        judging_source: str = judging_source if isinstance(judging_source, str) else "\n ".join(judging_source)
+
+        # 定义返回标识符，检查判断源中是否包含该标识符
+        RET_IDENTIFIER: str = "ret"
+        if RET_IDENTIFIER not in judging_source:
+            raise RequirementError(
+                f"Can't find {RET_IDENTIFIER} in judging source, you must define a variable named {RET_IDENTIFIER} in your judging source!\n"
+                f"Since it will be used as the return value of the judge function."
+            )
+
+        # 匹配使用情况与相应的采样器和采样器类型
+        _logger.debug("Match Usage with corresponding samplers and sampler_types")
+        used_samplers: Dict[str, Any] = {
+            f"func_{i}": self.samplers[usage.used_sampler_index] for i, usage in enumerate(usages)
+        }
+        _logger.debug(f"Matched samplers: {used_samplers}")
+        self.update_sampler_types()
+        used_sampler_types = [self.sampler_types[usage.used_sampler_index] for usage in usages]
+        _logger.debug(f"Matched sampler_types: {used_sampler_types}")
+
+        # 根据采样器类型，为采样器数据创建索引表达式
+        sampler_temp_var_names_mapping: Dict[str, str] = {}
+        indexed_expressions: List[str] = []
+        for usage, sampler_type, func_name in zip(usages, used_sampler_types, used_samplers):
+
+            match sampler_type:
+                case SamplerType.SEQ_SAMPLER:
+                    sampler_temp_var_names_mapping[temp_name := f"{func_name}_temp"] = func_name
+                    indexed_expressions.extend(self._index_for_seq_sampler_data(temp_name, usage.required_data_indexes))
+                case SamplerType.IDX_SAMPLER:
+                    indexed_expressions.extend(self._index_for_idx_sampler_data(func_name, usage.required_data_indexes))
+                case SamplerType.DRC_SAMPLER:
+                    sampler_temp_var_names_mapping[temp_name := f"{func_name}_temp"] = func_name
+                    indexed_expressions.extend(self._index_for_drc_sampler_data(temp_name, usage.required_data_indexes))
+                case _:
+                    raise RuntimeError(f"Unsupported sampler type: {sampler_type}")
+        _logger.debug(f"Created {len(indexed_expressions)} indexed expressions.")
+
+        # 创建占位变量并检查是否所有占位符都被包含在判断源中
+        placebo_var_names = [f"s{i}" for i in range(len(indexed_expressions))]
+        _logger.debug(f"Created {len(placebo_var_names)} placebo variables.")
+        _logger.debug("Checking that all placeholders are included in judging_source")
+        if not_included := [placebo for placebo in placebo_var_names if placebo not in judging_source]:
+            raise RequirementError(
+                f"Judging source must have all placeholders: {placebo_var_names} in judging_source\n"
+                f"Missing: {not_included}"
+            )
+
+        # 替换判断源中的占位符为索引表达式
+        for placebo, expr in zip(placebo_var_names, indexed_expressions):
+            _logger.debug(f'Replacing "{placebo}" with "{expr}".')
+            judging_source = judging_source.replace(placebo, expr)
+
+        # 创建临时变量的源代码，用于在执行环境中存储采样器的返回值
+        temp_var_source: str = (
+            ",".join(sampler_temp_var_names_mapping.keys())
+            + "="
+            + ",".join([f"{fname}()" for fname in sampler_temp_var_names_mapping.values()])
+        )
+        _logger.debug(f"Created temp_var_source: {temp_var_source}")
+
+        # 构建完整的函数源码并编译执行
+        func_source = f"def _func():\n" f" {temp_var_source}\n" f" {judging_source}\n" f" return {RET_IDENTIFIER}"
+        _logger.debug(f"Created func_source: {func_source}")
+        _logger.debug("Compiling func_source")
+
+        # 更新执行环境中的采样器和额外上下文信息
+        used_samplers.update(extra_context) if extra_context else None
+        exec(func_source, used_samplers)  # exec the source with the context
+        func_obj: Callable[[], bool] = used_samplers.get("_func")
+        _logger.debug(f"Succeed, compiled func_obj: {func_obj}")
+        return func_obj
+
+    @staticmethod
+    def _index_for_seq_sampler_data(data_var_name: str, required: List[int] | int) -> List[str]:
+        """
+        A function that generates a list of indexed expressions based on the given data variable name and a list of required indexes.
+
+        Args:
+            data_var_name (str): The name of the data variable.
+            required (List[int] | int): Either a single integer representing the required sequence length or a list of required data indexes.
+
+        Returns:
+            List[str]: A list of indexed expressions based on the data variable name and required indexes.
+        """
+        match required:
+            case int(required_seq_length):
+                final_required_data_indexes = range(required_seq_length)
+            case list(required_data_indexes):
+                final_required_data_indexes = required_data_indexes
+            case _:
+                raise RequirementError(
+                    f"Unknown Input, arg::required has to be either list[int] or int, got {required}"
+                )
+        return [f"{data_var_name}[{i}]" for i in final_required_data_indexes]
+
+    @staticmethod
+    def _index_for_drc_sampler_data(data_var_name: str, required: List[int] | int) -> List[str]:
+        """
+        A function that generates a list of indexed expressions based on the given data variable name and a list of required indexes.
+
+        Args:
+            data_var_name (str): The name of the data variable.
+            required (List[int] | int): Either a single integer representing the required sequence length or a list of required data indexes.
+
+        Returns:
+            List[str]: A list of indexed expressions based on the data variable name and required indexes.
+        """
+        match required:
+            case []:
+                raise RequirementError("Can't resolve the empty Usage List")
+            case int(required_seq_length):
+                final_required_data_indexes = range(required_seq_length)
+            case list(required_data_indexes):
+                final_required_data_indexes = required_data_indexes
+            case _:
+                raise RequirementError(
+                    f"Unknown Input, arg::required has to be either list[int] or int, got {required}"
+                )
+        return [f"(({data_var_name}>>{i})&1)" for i in final_required_data_indexes]
+
+    @staticmethod
+    def _index_for_idx_sampler_data(func_var_name: str, required: List[int]) -> List[str]:
+        """
+        Generate a list of indexed expressions based on the given function variable name and a list of required indexes.
+
+        Args:
+            func_var_name (str): The name of the function variable.
+            required (List[int]): A list of required indexes.
+
+        Returns:
+            List[str]: A list of indexed expressions based on the function variable name and required indexes.
+        """
+        return [f"{func_var_name}({i})" for i in required]
+
+    @staticmethod
+    def resolve_seq_sampler(sampler: SequenceSampler, required_data_indexes: Sequence[int]) -> UpdaterClosure:
+        """
+        Resolves the sampler based on the given sequence sampler and required data indexes.
+
+        Args:
+            sampler (SequenceSampler): The sequence sampler to resolve.
+            required_data_indexes (Sequence[int]): The required data indexes.
+
+        Returns:
+            UpdaterClosure: A callable that returns a tuple of SensorData objects
+            or a single SensorData object based on the number of required data indexes.
+
+        Raises:
+            None
+
+        Examples:
+            sampler = SequenceSampler()
+            required_data_indexes = []
+            resolved_sampler = resolve_seq_sampler(sampler, required_data_indexes)
+            data = resolved_sampler()  # Returns a tuple of all SensorData objects
+
+            sampler = SequenceSampler()
+            required_data_indexes = [0]
+            resolved_sampler = resolve_seq_sampler(sampler, required_data_indexes)
+            data = resolved_sampler()  # Returns the SensorData object at index 0
+
+            sampler = SequenceSampler()
+            required_data_indexes = [0, 1, 2]
+            resolved_sampler = resolve_seq_sampler(sampler, required_data_indexes)
+            data = resolved_sampler()  # Returns a tuple of SensorData objects at indexes 0, 1, and 2
+        """
+        match len(required_data_indexes):
+            case 0:
+                # 0 means require all data
+                return sampler  # Callable[[],SensorDataSequence]
+            case 1:
+                # 1 means require a specific data
+                unique_index = required_data_indexes[0]
+                return lambda: sampler()[unique_index]  # Callable[[], SensorData]
+            case _:
+                # >1 means require multiple data
+                required_indexes = required_data_indexes
+
+                def _fun() -> Tuple[SensorData, ...]:
+                    data = sampler()
+                    return tuple(data[i] for i in required_indexes)
+
+                return _fun  # Callable[[],SensorDataSequence]
+
+    @staticmethod
+    def resolve_idx_sampler(sampler: IndexedSampler, required_data_indexes: Sequence[int]) -> UpdaterClosure:
+        """
+        Resolves the indexed sampler based on the given sampler usage.
+
+        Args:
+            sampler (IndexedSampler): The indexed sampler to resolve.
+            required_data_indexes (Sequence[int]): The required data indexes.
+
+        Returns:
+            UpdaterClosure: A callable that returns a tuple of SensorData objects or a single SensorData object based on the number of required data indexes.
+
+        Raises:
+            RequirementError: If no required data indexes are specified.
+
+        Examples:
+            sampler = IndexedSampler()
+            required_data_indexes = []
+            resolved_sampler = resolve_idx_sampler(sampler, required_data_indexes)  # Raises RequirementError
+
+            sampler = IndexedSampler()
+            required_data_indexes = [0]
+            resolved_sampler = resolve_idx_sampler(sampler, required_data_indexes)
+            data = resolved_sampler()  # Returns the SensorData object at index 0
+
+            sampler = IndexedSampler()
+            required_data_indexes = [0, 1, 2]
+            resolved_sampler = resolve_idx_sampler(sampler, required_data_indexes)
+            data = resolved_sampler()  # Returns a tuple of the SensorData objects at indexes 0, 1, and 2
+        """
+
+        match len(required_data_indexes):
+            case 0:
+                raise RequirementError("Must specify at least one required data index")
+            case 1:
+                # 1 means require a specific data
+                unique_index = required_data_indexes[0]
+                return lambda: sampler(unique_index)  # Callable[[], SensorData]
+            case _:
+                # >1 means require multiple data
+                required_indexes = required_data_indexes
+                return lambda: tuple(sampler(ri) for ri in required_indexes)  # Callable[[], SensorDataSequence]
+
+    @staticmethod
+    def resolve_drc_sampler(sampler: DirectSampler, required_data_indexes: Sequence[int]) -> UpdaterClosure:
+        """
+        Resolves the direct sampler based on the given direct sampler and required data indexes.
+
+        Args:
+            sampler (DirectSampler): The direct sampler to resolve.
+            required_data_indexes (Sequence[int]): The required data indexes.
+
+        Returns:
+            UpdaterClosure: A callable that returns a tuple of SensorData objects or a single SensorData object based on the number of required data indexes.
+        """
+
+        match len(required_data_indexes):
+            case 0:
+                return sampler  # Callable[[], SensorData]
+            case 1:
+                # 1 means require a specific data
+                unique_index = required_data_indexes[0]
+                return lambda: (sampler() >> unique_index) & 1
+            case _:
+                # >1 means require multiple data
+
+                def _fun() -> SensorDataSequence:
+                    temp_seq = sampler()
+                    return tuple((temp_seq >> ri) & 1 for ri in required_data_indexes)
+
+                return _fun
```

### Comparing `mentabotix-0.1.3a2/src/mentabotix/tools/composers.py` & `mentabotix-0.1.3a3/src/mentabotix/tools/composers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,200 +1,201 @@
-from typing import List, Tuple, Callable, Optional, Self, Type, TypeVar, Dict
-
-from numpy import arange
-
-from ..modules.botix import MovingState, MovingTransition, __PLACE_HOLDER__
-
-StateTransitionPack = Tuple[List[MovingState], List[MovingTransition]]
-
-UnitType = TypeVar("UnitType", Type[MovingState], Type[MovingTransition])
-
-
-class MovingChainComposer:
-    """
-    A class that manages the composition of moving states and transitions.
-
-    Properties:
-    - last_state (MovingState): The last state object in the chain container.
-    - last_transition (MovingTransition): The last transition object in the chain container if it exists, otherwise None.
-    - next_need (UnitType): The next unit type to be added to the chain container.
-    """
-
-    @property
-    def last_state(self) -> MovingState:
-        """
-        Returns the last state object in the chain container.
-
-        Returns:
-            MovingState: The last state object in the chain container, or None if the container is empty.
-        """
-        container = self._chain_container[MovingState]
-        return container[-1] if container else None
-
-    @property
-    def last_transition(self) -> MovingTransition:
-        """
-        Returns the last transition object in the chain container.
-
-        Returns:
-            MovingTransition: The last transition object in the chain container if it exists, otherwise None.
-        """
-        container = self._chain_container[MovingTransition]
-        return container[-1] if container else None
-
-    @property
-    def next_need(self) -> UnitType:
-        return self._type_container[0]
-
-    def __init__(self) -> None:
-        self._type_container: List[UnitType] = [MovingState, MovingTransition]
-
-        self._chain_container: Dict[Type, List] = {MovingState: [], MovingTransition: []}
-
-    def _flip(self):
-        self._type_container.reverse()
-
-    def init_container(self) -> None:
-        """
-        Initializes the chain container by clearing all the lists in the `_chain_container` dictionary.
-        If the `next_need` is not `MovingState`, the `_type_container` list is reversed.
-
-        Parameters:
-            self (MovingChainComposer): The instance of the class.
-
-        Returns:
-            None: This function does not return anything.
-        """
-        if self.next_need != MovingState:
-            self._flip()
-        for cont in self._chain_container.values():
-            cont.clear()
-
-    def export_structure(self) -> StateTransitionPack:
-        """
-        Exports the structure of the chain container.
-
-        Returns:
-            StateTransitionPack: A tuple containing two lists, the first list contains all the MovingState objects in the chain container, and the second list contains all the MovingTransition objects in the chain container.
-
-        Side Effects:
-            - Initializes the chain container by calling the `init_container` method.
-        """
-        ret_pack = list(self._chain_container.get(MovingState)), list(self._chain_container.get(MovingTransition))
-        self.init_container()
-        return ret_pack
-
-    def add(self, unit: MovingState | MovingTransition) -> Self:
-        """
-        Adds a `MovingState` or `MovingTransition` object to the chain container.
-
-        Args:
-            unit (MovingState | MovingTransition): The unit to be added to the chain container.
-
-        Returns:
-            Self: The current instance of the class.
-
-        Raises:
-            ValueError: If the type of the unit does not match the next need.
-            RuntimeError: If the type of the unit is neither `MovingState` nor `MovingTransition`.
-        """
-        unit_type = type(unit)
-        if unit_type != self.next_need:
-            raise ValueError(f"Need {self.next_need}, got {unit}!")
-        elif unit_type == MovingState:
-            self._chain_container[MovingState].append(unit)
-            if self.last_transition:
-                self.last_transition.to_states[__PLACE_HOLDER__] = unit
-        elif unit_type == MovingTransition:
-            unit.from_states.append(self.last_state)
-            self._chain_container[MovingTransition].append(unit)
-        else:
-            raise RuntimeError("Should never reach here!")
-        self._flip()
-        return self
-
-
-def straight_chain(
-    start_speed: int,
-    end_speed: int,
-    duration: float,
-    power_exponent: float = 1.0,
-    interval: float = 0.07,
-    breaker: Optional[Callable[[], bool]] = None,
-    state_on_break: Optional[MovingState] = MovingState(0),
-) -> StateTransitionPack:
-    """
-    A function that calculates the states and transitions for a straight chain based on the input parameters.
-
-    Args:
-        start_speed (int): The initial speed of the chain.
-        end_speed (int): The final speed of the chain.
-        duration (float): The total duration of the chain movement.
-        power_exponent (float, optional): The power exponent used in the calculation. Defaults to 1.0.
-        interval (float, optional): The interval used in the calculation. Defaults to 0.07.
-        breaker (Optional[Callable[[], bool]], optional): A function to determine if the transition should be broken. Defaults to None.
-        state_on_break (Optional[MovingState], optional): The state to transition to if the chain is broken. Defaults to MovingState(0).
-
-    Returns:
-        StateTransitionPack: A tuple containing the list of states and transitions for the straight chain.
-    """
-    # Initialize the list of states with the starting state
-    states: List[MovingState] = [MovingState(start_speed)]
-    # Initialize an empty list for transitions
-    transitions: List[MovingTransition] = []
-
-    # Calculate the deviation in speed for uniform distribution across the duration
-    deviation = end_speed - start_speed
-    # Generate a sequence of speeds based on the given parameters
-    speed_seq = [
-        start_speed + round(deviation * x**power_exponent) for x in arange(0, 1.0, interval / (duration - interval))
-    ]
-
-    # Handle different scenarios based on whether a breaker function is provided
-    match breaker:
-        case None:
-            # If no breaker function, create transitions without breaking condition
-            for cur_speed in speed_seq:
-                last_state = states[-1]
-                cur_state = MovingState(cur_speed)
-                cur_transition = MovingTransition(from_states=last_state, to_states=cur_state, duration=interval)
-                states.append(cur_state)
-                transitions.append(cur_transition)
-            return states, transitions
-
-        case break_function if callable(break_function):
-            # If a breaker function is provided, create transitions that can be broken
-            for cur_speed in speed_seq:
-                last_state = states[-1]
-                cur_state = MovingState(cur_speed)
-                cur_transition = MovingTransition(
-                    from_states=last_state,
-                    to_states={False: cur_state, True: state_on_break},
-                    duration=interval,
-                    breaker=break_function,
-                )
-                states.append(cur_state)
-                transitions.append(cur_transition)
-            # Append the break state to the states list
-            states.append(state_on_break)
-            return states, transitions
-        case _:
-            # If breaker is neither None nor callable, raise an error
-            raise ValueError("breaker must be callable or None")
-
-
-def scanning_chain():
-    """
-    A function that calculates the states and transitions for a scanning chain.
-    Returns:
-
-    """
-    raise NotImplementedError
-
-
-def snaking_chain():
-    """
-    A function that calculates the states and transitions for a snaking chain.
-    Returns:
-
-    """
-    raise NotImplementedError
+from typing import List, Tuple, Callable, Optional, Self, Type, TypeVar, Dict
+
+from numpy import arange
+
+from ..modules.botix import MovingState, MovingTransition, __PLACE_HOLDER__
+
+StateTransitionPack = Tuple[List[MovingState], List[MovingTransition]]
+
+UnitType = TypeVar("UnitType", Type[MovingState], Type[MovingTransition])
+
+
+class MovingChainComposer:
+    """
+    A class that manages the composition of moving states and transitions.
+
+    Properties:
+    - last_state (MovingState): The last state object in the chain container.
+    - last_transition (MovingTransition): The last transition object in the chain container if it exists, otherwise None.
+    - next_need (UnitType): The next unit type to be added to the chain container.
+    """
+
+    @property
+    def last_state(self) -> MovingState:
+        """
+        Returns the last state object in the chain container.
+
+        Returns:
+            MovingState: The last state object in the chain container, or None if the container is empty.
+        """
+        container = self._chain_container[MovingState]
+        return container[-1] if container else None
+
+    @property
+    def last_transition(self) -> MovingTransition:
+        """
+        Returns the last transition object in the chain container.
+
+        Returns:
+            MovingTransition: The last transition object in the chain container if it exists, otherwise None.
+        """
+        container = self._chain_container[MovingTransition]
+        return container[-1] if container else None
+
+    @property
+    def next_need(self) -> UnitType:
+        return self._type_container[0]
+
+    def __init__(self) -> None:
+        self._type_container: List[UnitType] = [MovingState, MovingTransition]
+
+        self._chain_container: Dict[Type, List] = {MovingState: [], MovingTransition: []}
+
+    def _flip(self):
+        self._type_container.reverse()
+
+    def init_container(self) -> Self:
+        """
+        Initializes the chain container by clearing all the lists in the `_chain_container` dictionary.
+        If the `next_need` is not `MovingState`, the `_type_container` list is reversed.
+
+        Parameters:
+            self (MovingChainComposer): The instance of the class.
+
+        Returns:
+            Self: The current instance of the class.
+        """
+        if self.next_need != MovingState:
+            self._flip()
+        for cont in self._chain_container.values():
+            cont.clear()
+        return self
+
+    def export_structure(self) -> StateTransitionPack:
+        """
+        Exports the structure of the chain container.
+
+        Returns:
+            StateTransitionPack: A tuple containing two lists, the first list contains all the MovingState objects in the chain container, and the second list contains all the MovingTransition objects in the chain container.
+
+        Side Effects:
+            - Initializes the chain container by calling the `init_container` method.
+        """
+        ret_pack = list(self._chain_container.get(MovingState)), list(self._chain_container.get(MovingTransition))
+        self.init_container()
+        return ret_pack
+
+    def add(self, unit: MovingState | MovingTransition) -> Self:
+        """
+        Adds a `MovingState` or `MovingTransition` object to the chain container.
+
+        Args:
+            unit (MovingState | MovingTransition): The unit to be added to the chain container.
+
+        Returns:
+            Self: The current instance of the class.
+
+        Raises:
+            ValueError: If the type of the unit does not match the next need.
+            RuntimeError: If the type of the unit is neither `MovingState` nor `MovingTransition`.
+        """
+        unit_type = type(unit)
+        if unit_type != self.next_need:
+            raise ValueError(f"Need {self.next_need}, got {unit}!")
+        elif unit_type == MovingState:
+            self._chain_container[MovingState].append(unit)
+            if self.last_transition:
+                self.last_transition.to_states[__PLACE_HOLDER__] = unit
+        elif unit_type == MovingTransition:
+            unit.from_states.append(self.last_state)
+            self._chain_container[MovingTransition].append(unit)
+        else:
+            raise RuntimeError("Should never reach here!")
+        self._flip()
+        return self
+
+
+def straight_chain(
+    start_speed: int,
+    end_speed: int,
+    duration: float,
+    power_exponent: float = 1.0,
+    interval: float = 0.07,
+    breaker: Optional[Callable[[], bool]] = None,
+    state_on_break: Optional[MovingState] = MovingState(0),
+) -> StateTransitionPack:
+    """
+    A function that calculates the states and transitions for a straight chain based on the input parameters.
+
+    Args:
+        start_speed (int): The initial speed of the chain.
+        end_speed (int): The final speed of the chain.
+        duration (float): The total duration of the chain movement.
+        power_exponent (float, optional): The power exponent used in the calculation. Defaults to 1.0.
+        interval (float, optional): The interval used in the calculation. Defaults to 0.07.
+        breaker (Optional[Callable[[], bool]], optional): A function to determine if the transition should be broken. Defaults to None.
+        state_on_break (Optional[MovingState], optional): The state to transition to if the chain is broken. Defaults to MovingState(0).
+
+    Returns:
+        StateTransitionPack: A tuple containing the list of states and transitions for the straight chain.
+    """
+    # Initialize the list of states with the starting state
+    states: List[MovingState] = [MovingState(start_speed)]
+    # Initialize an empty list for transitions
+    transitions: List[MovingTransition] = []
+
+    # Calculate the deviation in speed for uniform distribution across the duration
+    deviation = end_speed - start_speed
+    # Generate a sequence of speeds based on the given parameters
+    speed_seq = [
+        start_speed + round(deviation * x**power_exponent) for x in arange(0, 1.0, interval / (duration - interval))
+    ]
+
+    # Handle different scenarios based on whether a breaker function is provided
+    match breaker:
+        case None:
+            # If no breaker function, create transitions without breaking condition
+            for cur_speed in speed_seq:
+                last_state = states[-1]
+                cur_state = MovingState(cur_speed)
+                cur_transition = MovingTransition(from_states=last_state, to_states=cur_state, duration=interval)
+                states.append(cur_state)
+                transitions.append(cur_transition)
+            return states, transitions
+
+        case break_function if callable(break_function):
+            # If a breaker function is provided, create transitions that can be broken
+            for cur_speed in speed_seq:
+                last_state = states[-1]
+                cur_state = MovingState(cur_speed)
+                cur_transition = MovingTransition(
+                    from_states=last_state,
+                    to_states={False: cur_state, True: state_on_break},
+                    duration=interval,
+                    breaker=break_function,
+                )
+                states.append(cur_state)
+                transitions.append(cur_transition)
+            # Append the break state to the states list
+            states.append(state_on_break)
+            return states, transitions
+        case _:
+            # If breaker is neither None nor callable, raise an error
+            raise ValueError("breaker must be callable or None")
+
+
+def scanning_chain():
+    """
+    A function that calculates the states and transitions for a scanning chain.
+    Returns:
+
+    """
+    raise NotImplementedError
+
+
+def snaking_chain():
+    """
+    A function that calculates the states and transitions for a snaking chain.
+    Returns:
+
+    """
+    raise NotImplementedError
```

### Comparing `mentabotix-0.1.3a2/src/mentabotix/tools/generators.py` & `mentabotix-0.1.3a3/src/mentabotix/tools/generators.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from enum import Enum
-from typing import Callable
-
-from numpy.random import choice
-
-
-class NameGenerator:
-    """
-    Class for generating unique names.
-
-    Attributes:
-        basename: the base name
-        counter: the counter
-    """
-
-    @property
-    def basename(self) -> str:
-        return self._basename
-
-    @property
-    def counter(self) -> int:
-        return self._counter
-
-    def __init__(self, basename: str):
-        self._basename = basename
-        self._counter = 0
-
-    def __call__(self) -> str:
-        self._counter += 1
-        return f"{self._basename}{self._counter}"
-
-
-class Multipliers(Enum):
-    """
-    Enum class for different multipliers.
-    Notes:
-        FLT: for float
-        SRK: for shrink
-        ENLG: for enlarge
-    Attributes:
-        FLT_UPPER: float around 1.0 but slightly higher
-        FLT_MIDDLE: float exactly around 1.0
-        FLT_LOWER: float around 1.0 but slightly lower
-
-        SRK_L: slightly shrink
-        SRK_LL: moderate shrink
-        SRK_LLL: significantly shrink
-
-        ENLG_L: slightly enlarge
-        ENLG_LL: moderate enlarge
-        ENLG_LLL: significantly enlarge
-    """
-
-    FLT_UPPER = (0.9, 0.925, 0.95, 1.0, 1.05, 1.08, 1.1, 1.17, 1.25)
-    FLT_MIDDLE = (0.8, 0.85, 0.9, 0.95, 1.0, 1.05, 1.1, 1.17, 1.25)
-    FLT_LOWER = (0.8, 0.825, 0.85, 0.875, 0.9, 0.925, 0.95, 1.0, 1.05, 1.08, 1.1)
-
-    SRK_L = (0.65, 0.7, 0.725, 0.7375, 0.75, 0.7625, 0.775, 0.7875, 0.8)
-    SRK_LL = (0.55, 0.6, 0.625, 0.65, 0.6625, 0.675, 0.6875, 0.7)
-    SRK_LLL = (0.40, 0.5, 0.525, 0.55, 0.5625, 0.575, 0.5875, 0.6)
-
-    ENLG_L = (1.25, 1.275, 1.3, 1.325, 1.35, 1.375, 1.4, 1.45, 1.5)
-    ENLG_LL = (1.5, 1.525, 1.55, 1.575, 1.6, 1.625, 1.65, 1.7, 1.75)
-    ENLG_LLL = (1.75, 1.775, 1.8, 1.825, 1.85, 1.875, 1.9, 1.95, 2.0, 2.1, 2.2, 2.4)
-
-
-def make_multiplier_generator(mult: "Multipliers") -> Callable[[], float]:
-    """
-    Generates a function that returns a random float value from the given multiplier sequence.
-
-    Parameters:
-        mult (Multipliers): The multiplier enum value.
-
-    Returns:
-        Callable[[], float]: A function that returns a random float value from the multiplier sequence.
-    """
-    seq = mult.value
-
-    def _make_multiplier() -> float:
-        return choice(seq)
-
-    return _make_multiplier
+from enum import Enum
+from typing import Callable
+
+from numpy.random import choice
+
+
+class NameGenerator:
+    """
+    Class for generating unique names.
+
+    Attributes:
+        basename: the base name
+        counter: the counter
+    """
+
+    @property
+    def basename(self) -> str:
+        return self._basename
+
+    @property
+    def counter(self) -> int:
+        return self._counter
+
+    def __init__(self, basename: str):
+        self._basename = basename
+        self._counter = 0
+
+    def __call__(self) -> str:
+        self._counter += 1
+        return f"{self._basename}{self._counter}"
+
+
+class Multipliers(Enum):
+    """
+    Enum class for different multipliers.
+    Notes:
+        FLT: for float
+        SRK: for shrink
+        ENLG: for enlarge
+    Attributes:
+        FLT_UPPER: float around 1.0 but slightly higher
+        FLT_MIDDLE: float exactly around 1.0
+        FLT_LOWER: float around 1.0 but slightly lower
+
+        SRK_L: slightly shrink
+        SRK_LL: moderate shrink
+        SRK_LLL: significantly shrink
+
+        ENLG_L: slightly enlarge
+        ENLG_LL: moderate enlarge
+        ENLG_LLL: significantly enlarge
+    """
+
+    FLT_UPPER = (0.9, 0.925, 0.95, 1.0, 1.05, 1.08, 1.1, 1.17, 1.25)
+    FLT_MIDDLE = (0.8, 0.85, 0.9, 0.95, 1.0, 1.05, 1.1, 1.17, 1.25)
+    FLT_LOWER = (0.8, 0.825, 0.85, 0.875, 0.9, 0.925, 0.95, 1.0, 1.05, 1.08, 1.1)
+
+    SRK_L = (0.65, 0.7, 0.725, 0.7375, 0.75, 0.7625, 0.775, 0.7875, 0.8)
+    SRK_LL = (0.55, 0.6, 0.625, 0.65, 0.6625, 0.675, 0.6875, 0.7)
+    SRK_LLL = (0.40, 0.5, 0.525, 0.55, 0.5625, 0.575, 0.5875, 0.6)
+
+    ENLG_L = (1.25, 1.275, 1.3, 1.325, 1.35, 1.375, 1.4, 1.45, 1.5)
+    ENLG_LL = (1.5, 1.525, 1.55, 1.575, 1.6, 1.625, 1.65, 1.7, 1.75)
+    ENLG_LLL = (1.75, 1.775, 1.8, 1.825, 1.85, 1.875, 1.9, 1.95, 2.0, 2.1, 2.2, 2.4)
+
+
+def make_multiplier_generator(mult: "Multipliers") -> Callable[[], float]:
+    """
+    Generates a function that returns a random float value from the given multiplier sequence.
+
+    Parameters:
+        mult (Multipliers): The multiplier enum value.
+
+    Returns:
+        Callable[[], float]: A function that returns a random float value from the multiplier sequence.
+    """
+    seq = mult.value
+
+    def _make_multiplier() -> float:
+        return choice(seq)
+
+    return _make_multiplier
```

### Comparing `mentabotix-0.1.3a2/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.3a3/src/mentabotix/vision/tagdetector.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,306 +1,306 @@
-"""
-apriltag detecting app
-"""
-
-import warnings
-from copy import deepcopy
-from threading import Thread
-from time import sleep
-from typing import Tuple, List, Dict, Optional, Literal, Union
-
-import cv2
-from cv2 import Mat, cvtColor, COLOR_RGB2GRAY
-from numpy import ndarray, array
-from numpy.linalg import linalg
-from pyapriltags import Detector, Detection
-
-DetectResult = Union[Detection, None]
-
-DEFAULT_TAG_TABLE: Dict[int, Tuple[DetectResult, float]] = {2: (None, 0.0), 1: (None, 0.0), 0: (None, 0.0)}
-
-DEFAULT_TAG_ID = -1
-
-NULL_TAG = -999
-
-TABLE_INIT_VALUE = (None, 0.0)
-
-CAMERA_RESOLUTION_MULTIPLIER = 0.4
-
-BLUE_TEAM = "blue"
-YELLOW_TEAM = "yellow"
-
-
-def get_center_tag(frame_center: ndarray, tags: List[Detection]):
-    """
-    get the tag in which is the nearest to the frame center
-    Args:
-        frame_center:
-        tags:
-
-    Returns:
-
-    """
-    # 获取离图像中心最近的 AprilTag
-    closest_tag = None
-    closest_dist = float("inf")
-    for tag in tags:
-        # 计算当前 AprilTag 中心点与图像中心的距离
-        # Convert tuples to NumPy arrays if necessary
-        point_1 = array(tag.center)
-        point_2 = array(frame_center)
-        # Calculate Euclidean distance using NumPy's vectorized operations
-        dist = linalg.norm(tag.center - frame_center)
-        if dist < closest_dist:
-            closest_dist = dist
-            closest_tag = tag
-    return closest_tag
-
-
-class TagDetector:
-    """
-    use cam to detect apriltags
-    """
-
-    detector = Detector(
-        families="tag36h11",
-        nthreads=2,
-        quad_decimate=1.0,
-        refine_edges=False,
-        debug=False,
-    )
-    __tag_detect = detector.detect
-
-    def __init__(
-        self,
-        cam_id: int,
-        team_color: Literal["blue", "yellow"],
-        start_detect_tag: bool = True,
-        single_tag_mode: bool = True,
-        minimal_resolution: bool = True,
-    ):
-        """
-
-        Args:
-
-            team_color:
-            start_detect_tag:
-            single_tag_mode:if check only a single tag one time
-        """
-
-        self._camera: cv2.VideoCapture = cv2.VideoCapture(cam_id)
-        if minimal_resolution:
-            self._camera.set(cv2.CAP_PROP_FRAME_WIDTH, 1)
-            self._camera.set(cv2.CAP_PROP_FRAME_HEIGHT, 1)
-        self._frame_center: Tuple[float, float] = (
-            self._camera.get(cv2.CAP_PROP_FRAME_WIDTH) / 2,
-            self._camera.get(cv2.CAP_PROP_FRAME_HEIGHT) / 2,
-        )
-        self._tags_table: Dict[int, Tuple[Optional[Detection], int | float]] = {}
-
-        self._tag_id: int = DEFAULT_TAG_ID
-        self._tag_monitor_switch: bool = True
-        self._enemy_tag_id: int = NULL_TAG
-        self._ally_tag_id: int = NULL_TAG
-        self._neutral_tag_id: int = NULL_TAG
-
-        self.team_color = team_color
-        self._init_tags_table()
-        self._single_tag_mode: bool = single_tag_mode
-        self._apriltag_detect: Optional[Thread] = None
-        self._detect_should_continue: bool = True
-
-        self.apriltag_detect_start() if start_detect_tag else None
-
-    def _init_tags_table(self):
-        """
-        the tag table stores the tag obj and the distance to the camera center
-        :return:
-        """
-        self._tags_table[self._enemy_tag_id] = TABLE_INIT_VALUE
-        self._tags_table[self._ally_tag_id] = TABLE_INIT_VALUE
-        self._tags_table[self._neutral_tag_id] = TABLE_INIT_VALUE
-
-    @property
-    def team_color(self) -> str:
-        """
-
-        Returns: team color
-
-        """
-
-        return self._team_color
-
-    @team_color.setter
-    def team_color(self, team_color: Literal["blue", "yellow"] = BLUE_TEAM):
-        """
-        set the ally/enemy tag according the team color
-        yellow: ally: 2 | enemy: 1|neutral: 0
-        blue: ally: 1 | enemy: 2 | neutral: 0
-
-        :param team_color: blue or yellow
-        :return:
-        """
-        self._team_color = team_color
-        self._neutral_tag_id = 0
-        if team_color == BLUE_TEAM:
-            self._enemy_tag_id = 2
-            self._ally_tag_id = 1
-        elif team_color == YELLOW_TEAM:
-            self._enemy_tag_id = 1
-            self._ally_tag_id = 2
-
-    @property
-    def detect_should_continue(self) -> bool:
-        """
-
-        Returns: the alive-status of the detection process
-
-        """
-        return self._detect_should_continue
-
-    @detect_should_continue.setter
-    def detect_should_continue(self, should: bool):
-
-        self._detect_should_continue = should
-
-    def apriltag_detect_start(self):
-        """
-        start the tag-detection thread and set it to daemon
-        :return:
-        """
-        warnings.warn("AprilTag detect Activating")
-        self._detect_should_continue: bool = True
-        apriltag_detect = Thread(target=self._apriltag_detect_loop, name="apriltag_detect_Process")
-        apriltag_detect.daemon = True
-        apriltag_detect.start()
-
-        self._apriltag_detect = apriltag_detect
-
-    def _apriltag_detect_loop(self):
-        """
-        这是一个线程函数，它从摄像头捕获视频帧，处理帧以检测 AprilTags，
-        :return:
-        """
-        frame_updater = self._camera.read
-
-        warnings.warn("Detection Activated")
-        while self._detect_should_continue:
-            if self._tag_monitor_switch:  # 台上开启 台下关闭 节约性能
-                success, frame = frame_updater()  # extract frame from the cam
-                if success:
-                    self._update_tags(frame)  # extract tags in the detection
-                    # extract the correct tag in the detection,
-                    # for example, the tag in the center of the frame
-                    self._update_tag_id()
-                else:
-                    break
-            else:
-                sleep(0.4)
-        warnings.warn("\n##########CAMERA CLOSED###########\n" "###ENTERING NO CAMERA MODE###")
-        self._tag_id = DEFAULT_TAG_ID
-
-    def _update_tags(self, frame: Mat):
-        """
-        update tags from the newly sampled frame
-        :return:
-        """
-        # 将帧转换为灰度并存储在 gray 变量中。
-        # 使用 AprilTag 检测器对象（self.tag_detector）在灰度帧中检测 AprilTags。检测到的标记存储在 self._tags 变量中。
-        # override old tags
-        temp_dict = deepcopy(DEFAULT_TAG_TABLE)
-        for tag in self.__tag_detect(cvtColor(frame, COLOR_RGB2GRAY)):
-            # Convert tuples to NumPy arrays if necessary
-            start = array(tag.center)
-            target = array(self._frame_center)
-            # Calculate Manhattan distance using absolute differences and summing them up
-            temp_dict[tag.tag_id] = (tag, sum(abs(tag.center - self._frame_center)))
-        self._tags_table = temp_dict
-
-    def _update_tag_id(self):
-        """
-        update the tag id from the self._tags_table
-        :return:
-        """
-
-        def _single_mode():
-
-            self._tag_id = DEFAULT_TAG_ID
-            for tag_data in self._tags_table.values():
-                if tag_data[0]:
-                    self._tag_id = tag_data[0].tag_id
-                    break
-
-        def _nearest_mode():
-            closest_dist = float("inf")
-            closest_tag = None
-            for tag_data in self._tags_table.values():
-                # check the tag obj is valid and compare with the closest tag
-                if tag_data[0] and tag_data[1] < closest_dist:
-                    closest_dist = tag_data[1]
-                    closest_tag = tag_data[0]
-            self._tag_id = closest_tag.tag_id if closest_tag else DEFAULT_TAG_ID
-
-        _single_mode() if self._single_tag_mode else _nearest_mode()
-
-    @property
-    def tag_table(self):
-        """
-
-        Returns: the tag table that contains all the results
-
-        """
-        return self._tags_table
-
-    @property
-    def tag_id(self):
-        """
-        :return:  current tag id
-        """
-        return self._tag_id
-
-    @property
-    def tag_detection_switch(self):
-        """
-
-        Returns: the detector status
-
-        """
-        return self._tag_monitor_switch
-
-    @tag_detection_switch.setter
-    def tag_detection_switch(self, switch: bool):
-        """
-        setter for the switch
-        :param switch:
-        :return:
-        """
-        if switch != self._tag_monitor_switch:
-            self._tag_monitor_switch = switch
-            self._tag_id = DEFAULT_TAG_ID
-
-    @property
-    def ally_tag_id(self) -> int:
-        """
-
-        Returns: the tag id of ally
-
-        """
-        return self._ally_tag_id
-
-    @property
-    def enemy_tag_id(self) -> int:
-        """
-
-        Returns: the tag id of the enemy
-
-        """
-        return self._enemy_tag_id
-
-    @property
-    def neutral_tag_id(self) -> int:
-        """
-
-        Returns: the tag id of the neutral
-
-        """
-        return self._neutral_tag_id
+"""
+apriltag detecting app
+"""
+
+import warnings
+from copy import deepcopy
+from threading import Thread
+from time import sleep
+from typing import Tuple, List, Dict, Optional, Literal, Union
+
+import cv2
+from cv2 import Mat, cvtColor, COLOR_RGB2GRAY
+from numpy import ndarray, array
+from numpy.linalg import linalg
+from pyapriltags import Detector, Detection
+
+DetectResult = Union[Detection, None]
+
+DEFAULT_TAG_TABLE: Dict[int, Tuple[DetectResult, float]] = {2: (None, 0.0), 1: (None, 0.0), 0: (None, 0.0)}
+
+DEFAULT_TAG_ID = -1
+
+NULL_TAG = -999
+
+TABLE_INIT_VALUE = (None, 0.0)
+
+CAMERA_RESOLUTION_MULTIPLIER = 0.4
+
+BLUE_TEAM = "blue"
+YELLOW_TEAM = "yellow"
+
+
+def get_center_tag(frame_center: ndarray, tags: List[Detection]):
+    """
+    get the tag in which is the nearest to the frame center
+    Args:
+        frame_center:
+        tags:
+
+    Returns:
+
+    """
+    # 获取离图像中心最近的 AprilTag
+    closest_tag = None
+    closest_dist = float("inf")
+    for tag in tags:
+        # 计算当前 AprilTag 中心点与图像中心的距离
+        # Convert tuples to NumPy arrays if necessary
+        point_1 = array(tag.center)
+        point_2 = array(frame_center)
+        # Calculate Euclidean distance using NumPy's vectorized operations
+        dist = linalg.norm(tag.center - frame_center)
+        if dist < closest_dist:
+            closest_dist = dist
+            closest_tag = tag
+    return closest_tag
+
+
+class TagDetector:
+    """
+    use cam to detect apriltags
+    """
+
+    detector = Detector(
+        families="tag36h11",
+        nthreads=2,
+        quad_decimate=1.0,
+        refine_edges=False,
+        debug=False,
+    )
+    __tag_detect = detector.detect
+
+    def __init__(
+        self,
+        cam_id: int,
+        team_color: Literal["blue", "yellow"],
+        start_detect_tag: bool = True,
+        single_tag_mode: bool = True,
+        minimal_resolution: bool = True,
+    ):
+        """
+
+        Args:
+
+            team_color:
+            start_detect_tag:
+            single_tag_mode:if check only a single tag one time
+        """
+
+        self._camera: cv2.VideoCapture = cv2.VideoCapture(cam_id)
+        if minimal_resolution:
+            self._camera.set(cv2.CAP_PROP_FRAME_WIDTH, 1)
+            self._camera.set(cv2.CAP_PROP_FRAME_HEIGHT, 1)
+        self._frame_center: Tuple[float, float] = (
+            self._camera.get(cv2.CAP_PROP_FRAME_WIDTH) / 2,
+            self._camera.get(cv2.CAP_PROP_FRAME_HEIGHT) / 2,
+        )
+        self._tags_table: Dict[int, Tuple[Optional[Detection], int | float]] = {}
+
+        self._tag_id: int = DEFAULT_TAG_ID
+        self._tag_monitor_switch: bool = True
+        self._enemy_tag_id: int = NULL_TAG
+        self._ally_tag_id: int = NULL_TAG
+        self._neutral_tag_id: int = NULL_TAG
+
+        self.team_color = team_color
+        self._init_tags_table()
+        self._single_tag_mode: bool = single_tag_mode
+        self._apriltag_detect: Optional[Thread] = None
+        self._detect_should_continue: bool = True
+
+        self.apriltag_detect_start() if start_detect_tag else None
+
+    def _init_tags_table(self):
+        """
+        the tag table stores the tag obj and the distance to the camera center
+        :return:
+        """
+        self._tags_table[self._enemy_tag_id] = TABLE_INIT_VALUE
+        self._tags_table[self._ally_tag_id] = TABLE_INIT_VALUE
+        self._tags_table[self._neutral_tag_id] = TABLE_INIT_VALUE
+
+    @property
+    def team_color(self) -> str:
+        """
+
+        Returns: team color
+
+        """
+
+        return self._team_color
+
+    @team_color.setter
+    def team_color(self, team_color: Literal["blue", "yellow"] = BLUE_TEAM):
+        """
+        set the ally/enemy tag according the team color
+        yellow: ally: 2 | enemy: 1|neutral: 0
+        blue: ally: 1 | enemy: 2 | neutral: 0
+
+        :param team_color: blue or yellow
+        :return:
+        """
+        self._team_color = team_color
+        self._neutral_tag_id = 0
+        if team_color == BLUE_TEAM:
+            self._enemy_tag_id = 2
+            self._ally_tag_id = 1
+        elif team_color == YELLOW_TEAM:
+            self._enemy_tag_id = 1
+            self._ally_tag_id = 2
+
+    @property
+    def detect_should_continue(self) -> bool:
+        """
+
+        Returns: the alive-status of the detection process
+
+        """
+        return self._detect_should_continue
+
+    @detect_should_continue.setter
+    def detect_should_continue(self, should: bool):
+
+        self._detect_should_continue = should
+
+    def apriltag_detect_start(self):
+        """
+        start the tag-detection thread and set it to daemon
+        :return:
+        """
+        warnings.warn("AprilTag detect Activating")
+        self._detect_should_continue: bool = True
+        apriltag_detect = Thread(target=self._apriltag_detect_loop, name="apriltag_detect_Process")
+        apriltag_detect.daemon = True
+        apriltag_detect.start()
+
+        self._apriltag_detect = apriltag_detect
+
+    def _apriltag_detect_loop(self):
+        """
+        这是一个线程函数，它从摄像头捕获视频帧，处理帧以检测 AprilTags，
+        :return:
+        """
+        frame_updater = self._camera.read
+
+        warnings.warn("Detection Activated")
+        while self._detect_should_continue:
+            if self._tag_monitor_switch:  # 台上开启 台下关闭 节约性能
+                success, frame = frame_updater()  # extract frame from the cam
+                if success:
+                    self._update_tags(frame)  # extract tags in the detection
+                    # extract the correct tag in the detection,
+                    # for example, the tag in the center of the frame
+                    self._update_tag_id()
+                else:
+                    break
+            else:
+                sleep(0.4)
+        warnings.warn("\n##########CAMERA CLOSED###########\n" "###ENTERING NO CAMERA MODE###")
+        self._tag_id = DEFAULT_TAG_ID
+
+    def _update_tags(self, frame: Mat):
+        """
+        update tags from the newly sampled frame
+        :return:
+        """
+        # 将帧转换为灰度并存储在 gray 变量中。
+        # 使用 AprilTag 检测器对象（self.tag_detector）在灰度帧中检测 AprilTags。检测到的标记存储在 self._tags 变量中。
+        # override old tags
+        temp_dict = deepcopy(DEFAULT_TAG_TABLE)
+        for tag in self.__tag_detect(cvtColor(frame, COLOR_RGB2GRAY)):
+            # Convert tuples to NumPy arrays if necessary
+            start = array(tag.center)
+            target = array(self._frame_center)
+            # Calculate Manhattan distance using absolute differences and summing them up
+            temp_dict[tag.tag_id] = (tag, sum(abs(tag.center - self._frame_center)))
+        self._tags_table = temp_dict
+
+    def _update_tag_id(self):
+        """
+        update the tag id from the self._tags_table
+        :return:
+        """
+
+        def _single_mode():
+
+            self._tag_id = DEFAULT_TAG_ID
+            for tag_data in self._tags_table.values():
+                if tag_data[0]:
+                    self._tag_id = tag_data[0].tag_id
+                    break
+
+        def _nearest_mode():
+            closest_dist = float("inf")
+            closest_tag = None
+            for tag_data in self._tags_table.values():
+                # check the tag obj is valid and compare with the closest tag
+                if tag_data[0] and tag_data[1] < closest_dist:
+                    closest_dist = tag_data[1]
+                    closest_tag = tag_data[0]
+            self._tag_id = closest_tag.tag_id if closest_tag else DEFAULT_TAG_ID
+
+        _single_mode() if self._single_tag_mode else _nearest_mode()
+
+    @property
+    def tag_table(self):
+        """
+
+        Returns: the tag table that contains all the results
+
+        """
+        return self._tags_table
+
+    @property
+    def tag_id(self):
+        """
+        :return:  current tag id
+        """
+        return self._tag_id
+
+    @property
+    def tag_detection_switch(self):
+        """
+
+        Returns: the detector status
+
+        """
+        return self._tag_monitor_switch
+
+    @tag_detection_switch.setter
+    def tag_detection_switch(self, switch: bool):
+        """
+        setter for the switch
+        :param switch:
+        :return:
+        """
+        if switch != self._tag_monitor_switch:
+            self._tag_monitor_switch = switch
+            self._tag_id = DEFAULT_TAG_ID
+
+    @property
+    def ally_tag_id(self) -> int:
+        """
+
+        Returns: the tag id of ally
+
+        """
+        return self._ally_tag_id
+
+    @property
+    def enemy_tag_id(self) -> int:
+        """
+
+        Returns: the tag id of the enemy
+
+        """
+        return self._enemy_tag_id
+
+    @property
+    def neutral_tag_id(self) -> int:
+        """
+
+        Returns: the tag id of the neutral
+
+        """
+        return self._neutral_tag_id
```

### Comparing `mentabotix-0.1.3a2/tests/test_composer.py` & `mentabotix-0.1.3a3/tests/test_composer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,244 +1,243 @@
-import random
-import unittest
-
-from bdmc import CloseLoopController, MotorInfo
-
-from mentabotix import MovingChainComposer, MovingState, MovingTransition, straight_chain, Botix
-
-
-# Assuming MovingState, MovingTransition, UnitType, StateTransitionPack are defined elsewhere
-# You'll need to replace these with the actual classes and types
-
-
-class TestComposer(unittest.TestCase):
-    def setUp(self):
-        self.moving_chain_composer = MovingChainComposer()
-
-    def test_last_state(self):
-        # Test when there are no states
-        self.assertIsNone(self.moving_chain_composer.last_state)
-
-        # Test with one state
-        state1 = MovingState(10)
-        self.moving_chain_composer.add(state1)
-        self.assertEqual(self.moving_chain_composer.last_state, state1)
-
-        # Test with multiple states
-        state2 = MovingState(100)
-        with self.assertRaises(ValueError):
-            self.moving_chain_composer.add(state2)
-
-        tran1 = MovingTransition(1)
-        tran2 = MovingTransition(2)
-        self.moving_chain_composer.add(tran1)
-        with self.assertRaises(ValueError):
-            self.moving_chain_composer.add(tran2)
-        # Test with one state
-        state3 = MovingState(1052)
-        self.moving_chain_composer.add(state3)
-        self.assertEqual(self.moving_chain_composer.last_state, state3)
-
-    def test_last_transition(self):
-        # Test when there are no transitions
-        self.assertIsNone(self.moving_chain_composer.last_transition)
-        self.moving_chain_composer.add(MovingState(0))
-        # Test with one transition
-        tran1 = MovingTransition(10)
-        self.moving_chain_composer.add(tran1)
-        self.assertEqual(self.moving_chain_composer.last_transition, tran1)
-
-        # Test with multiple transitions
-        tran2 = MovingTransition(100)
-        with self.assertRaises(ValueError):
-            self.moving_chain_composer.add(tran2)
-
-        state1 = MovingState(1)
-        state2 = MovingState(2)
-        self.moving_chain_composer.add(state1)
-        with self.assertRaises(ValueError):
-            self.moving_chain_composer.add(state2)
-        # Test with one transition
-        tran3 = MovingTransition(1052)
-        self.moving_chain_composer.add(tran3)
-        self.assertEqual(self.moving_chain_composer.last_transition, tran3)
-
-    def test_next_need(self):
-        # Test initial next need
-        self.assertEqual(self.moving_chain_composer.next_need, MovingState)
-
-        # Test after adding a MovingState
-        self.moving_chain_composer.add(MovingState(0))
-        self.assertEqual(self.moving_chain_composer.next_need, MovingTransition)
-
-    def test_init_container(self):
-        self.moving_chain_composer.add(MovingState(0))
-        self.moving_chain_composer.init_container()
-        self.moving_chain_composer.add(MovingState(0))
-
-    def test_export_structure(self):
-        # Test with no units
-        self.assertEqual(self.moving_chain_composer.export_structure(), ([], []))
-
-        # Test with states and transitions
-        state1, state2 = MovingState(1), MovingState(2)
-        transition1, transition2 = MovingTransition(1), MovingTransition(2)
-        (self.moving_chain_composer.add(state1).add(transition1).add(state2).add(transition2))
-
-        expected_structure = ([state1, state2], [transition1, transition2])
-        self.assertEqual(self.moving_chain_composer.export_structure(), expected_structure)
-
-    def test_add(self):
-        # Test adding correct unit types
-        state = MovingState(1)
-        transition = MovingTransition(1)
-        self.moving_chain_composer.add(state)
-        self.moving_chain_composer.add(transition)
-
-        # Test adding incorrect unit type
-        with self.assertRaises(ValueError):
-            self.moving_chain_composer.add(14)
-
-    # 测试没有breaker的情况
-    def test_straight_chain_without_breaker(self):
-        start_speed = 50
-        end_speed = 100
-        duration = 5.0
-        power_exponent = 1.0
-        interval = 0.07
-
-        # 调用待测试函数
-        states, transitions = straight_chain(
-            start_speed=start_speed,
-            end_speed=end_speed,
-            duration=duration,
-            power_exponent=power_exponent,
-            interval=interval,
-        )
-
-        # 断言判断结果是否符合预期
-        self.assertEqual(len(states), int(duration / interval) + 1)
-        self.assertEqual(states[0].unwrap()[0], start_speed)
-        self.assertEqual(states[-1].unwrap()[0], end_speed)
-        for i in range(len(transitions) - 1):
-            self.assertIsInstance(transitions[i], MovingTransition)
-            self.assertEqual(transitions[i].duration, interval)
-
-    # 测试有breaker函数的情况
-    def test_straight_chain_with_breaker(self):
-        start_speed = 50
-        end_speed = 100
-        duration = 5.0
-        power_exponent = 1.0
-        interval = 0.1
-
-        def break_function() -> bool:
-            return random.random() < 0.1
-
-        # 调用待测试函数
-        states, transitions = straight_chain(
-            start_speed=start_speed,
-            end_speed=end_speed,
-            duration=duration,
-            power_exponent=power_exponent,
-            interval=interval,
-            breaker=break_function,
-        )
-
-        # 断言判断结果是否符合预期
-        self.assertTrue(any(isinstance(t, MovingTransition) and t.breaker for t in transitions))
-        self.assertEqual(int(duration / interval), len(transitions))
-        self.assertAlmostEqual(duration, sum(t.duration for t in transitions))
-        self.assertEqual(int(duration / interval) + 1 + 1, len(states))  # 包含了break状态
-        self.assertIn(MovingState(0), states)  # 确认state_on_break被加入到states列表中
-
-    def test_exp(self):
-        start_speed = 50
-        end_speed = 100
-        duration = 5.0
-        power_exponent = 2.0
-        interval = 0.1
-
-        def break_function() -> bool:
-            return random.random() < 0.1
-
-        # 调用待测试函数
-        states, transitions = straight_chain(
-            start_speed=start_speed,
-            end_speed=end_speed,
-            duration=duration,
-            power_exponent=power_exponent,
-            interval=interval,
-            breaker=break_function,
-        )
-
-    def test_structure(self):
-        start_speed = 50
-        end_speed = 100
-        duration = 5.0
-        power_exponent = 2.0
-        interval = 0.1
-
-        def break_function() -> bool:
-            return random.random() < 0.1
-
-        # 调用待测试函数
-        states, transitions = straight_chain(
-            start_speed=start_speed,
-            end_speed=end_speed,
-            duration=duration,
-            power_exponent=power_exponent,
-            interval=interval,
-            breaker=break_function,
-        )
-
-        botix = Botix(controller=CloseLoopController([MotorInfo(i) for i in range(4)]), token_pool=transitions)
-        botix.export_structure("long_chain.puml")
-
-    # 测试breaker不是None且不是callable的情况
-    def test_straight_chain_with_invalid_breaker(self):
-        start_speed = 50
-        end_speed = 100
-        duration = 5.0
-        power_exponent = 1.0
-        interval = 0.07
-
-        # 使用错误的breaker参数
-        with self.assertRaises(ValueError):
-            straight_chain(
-                start_speed=start_speed,
-                end_speed=end_speed,
-                duration=duration,
-                power_exponent=power_exponent,
-                interval=interval,
-                breaker="not a callable",
-            )
-
-    def test_mk(self):
-        from mentabotix import MovingChainComposer, MovingState, MovingTransition
-
-        # init the state-transition composer
-        comp = MovingChainComposer()
-
-        # add some states and transitions one by one to the composer, the composer will auto-connect the states and transitions
-        (
-            comp.add(MovingState(0))
-            .add(MovingTransition(0.2))
-            .add(MovingState(1000))
-            .add(MovingTransition(0.3))
-            .add(MovingState(2000))
-        )
-
-        # export the structure
-        states, transitions = comp.export_structure()
-
-        # let's use botix to make the visualization!
-        # first make the botix object
-        con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
-        botix = Botix(controller=con, token_pool=transitions)
-
-        # make the visualization
-        botix.export_structure("composed.puml")
-
-
-if __name__ == "__main__":
-    unittest.main()
+import random
+import unittest
+
+from bdmc import CloseLoopController, MotorInfo
+
+from mentabotix import MovingChainComposer, MovingState, MovingTransition, straight_chain, Botix
+
+
+# Assuming MovingState, MovingTransition, UnitType, StateTransitionPack are defined elsewhere
+# You'll need to replace these with the actual classes and types
+
+
+class TestComposer(unittest.TestCase):
+    def setUp(self):
+        self.moving_chain_composer = MovingChainComposer()
+
+    def test_last_state(self):
+        # Test when there are no states
+        self.assertIsNone(self.moving_chain_composer.last_state)
+
+        # Test with one state
+        state1 = MovingState(10)
+        self.moving_chain_composer.add(state1)
+        self.assertEqual(self.moving_chain_composer.last_state, state1)
+
+        # Test with multiple states
+        state2 = MovingState(100)
+        with self.assertRaises(ValueError):
+            self.moving_chain_composer.add(state2)
+
+        tran1 = MovingTransition(1)
+        tran2 = MovingTransition(2)
+        self.moving_chain_composer.add(tran1)
+        with self.assertRaises(ValueError):
+            self.moving_chain_composer.add(tran2)
+        # Test with one state
+        state3 = MovingState(1052)
+        self.moving_chain_composer.add(state3)
+        self.assertEqual(self.moving_chain_composer.last_state, state3)
+
+    def test_last_transition(self):
+        # Test when there are no transitions
+        self.assertIsNone(self.moving_chain_composer.last_transition)
+        self.moving_chain_composer.add(MovingState(0))
+        # Test with one transition
+        tran1 = MovingTransition(10)
+        self.moving_chain_composer.add(tran1)
+        self.assertEqual(self.moving_chain_composer.last_transition, tran1)
+
+        # Test with multiple transitions
+        tran2 = MovingTransition(100)
+        with self.assertRaises(ValueError):
+            self.moving_chain_composer.add(tran2)
+
+        state1 = MovingState(1)
+        state2 = MovingState(2)
+        self.moving_chain_composer.add(state1)
+        with self.assertRaises(ValueError):
+            self.moving_chain_composer.add(state2)
+        # Test with one transition
+        tran3 = MovingTransition(1052)
+        self.moving_chain_composer.add(tran3)
+        self.assertEqual(self.moving_chain_composer.last_transition, tran3)
+
+    def test_next_need(self):
+        # Test initial next need
+        self.assertEqual(self.moving_chain_composer.next_need, MovingState)
+
+        # Test after adding a MovingState
+        self.moving_chain_composer.add(MovingState(0))
+        self.assertEqual(self.moving_chain_composer.next_need, MovingTransition)
+
+    def test_init_container(self):
+        self.moving_chain_composer.add(MovingState(0))
+        self.moving_chain_composer.init_container().add(MovingState(0))
+
+    def test_export_structure(self):
+        # Test with no units
+        self.assertEqual(self.moving_chain_composer.export_structure(), ([], []))
+
+        # Test with states and transitions
+        state1, state2 = MovingState(1), MovingState(2)
+        transition1, transition2 = MovingTransition(1), MovingTransition(2)
+        (self.moving_chain_composer.add(state1).add(transition1).add(state2).add(transition2))
+
+        expected_structure = ([state1, state2], [transition1, transition2])
+        self.assertEqual(self.moving_chain_composer.export_structure(), expected_structure)
+
+    def test_add(self):
+        # Test adding correct unit types
+        state = MovingState(1)
+        transition = MovingTransition(1)
+        self.moving_chain_composer.add(state)
+        self.moving_chain_composer.add(transition)
+
+        # Test adding incorrect unit type
+        with self.assertRaises(ValueError):
+            self.moving_chain_composer.add(14)
+
+    # 测试没有breaker的情况
+    def test_straight_chain_without_breaker(self):
+        start_speed = 50
+        end_speed = 100
+        duration = 5.0
+        power_exponent = 1.0
+        interval = 0.07
+
+        # 调用待测试函数
+        states, transitions = straight_chain(
+            start_speed=start_speed,
+            end_speed=end_speed,
+            duration=duration,
+            power_exponent=power_exponent,
+            interval=interval,
+        )
+
+        # 断言判断结果是否符合预期
+        self.assertEqual(len(states), int(duration / interval) + 1)
+        self.assertEqual(states[0].unwrap()[0], start_speed)
+        self.assertEqual(states[-1].unwrap()[0], end_speed)
+        for i in range(len(transitions) - 1):
+            self.assertIsInstance(transitions[i], MovingTransition)
+            self.assertEqual(transitions[i].duration, interval)
+
+    # 测试有breaker函数的情况
+    def test_straight_chain_with_breaker(self):
+        start_speed = 50
+        end_speed = 100
+        duration = 5.0
+        power_exponent = 1.0
+        interval = 0.1
+
+        def break_function() -> bool:
+            return random.random() < 0.1
+
+        # 调用待测试函数
+        states, transitions = straight_chain(
+            start_speed=start_speed,
+            end_speed=end_speed,
+            duration=duration,
+            power_exponent=power_exponent,
+            interval=interval,
+            breaker=break_function,
+        )
+
+        # 断言判断结果是否符合预期
+        self.assertTrue(any(isinstance(t, MovingTransition) and t.breaker for t in transitions))
+        self.assertEqual(int(duration / interval), len(transitions))
+        self.assertAlmostEqual(duration, sum(t.duration for t in transitions))
+        self.assertEqual(int(duration / interval) + 1 + 1, len(states))  # 包含了break状态
+        self.assertIn(MovingState(0), states)  # 确认state_on_break被加入到states列表中
+
+    def test_exp(self):
+        start_speed = 50
+        end_speed = 100
+        duration = 5.0
+        power_exponent = 2.0
+        interval = 0.1
+
+        def break_function() -> bool:
+            return random.random() < 0.1
+
+        # 调用待测试函数
+        states, transitions = straight_chain(
+            start_speed=start_speed,
+            end_speed=end_speed,
+            duration=duration,
+            power_exponent=power_exponent,
+            interval=interval,
+            breaker=break_function,
+        )
+
+    def test_structure(self):
+        start_speed = 50
+        end_speed = 100
+        duration = 5.0
+        power_exponent = 2.0
+        interval = 0.1
+
+        def break_function() -> bool:
+            return random.random() < 0.1
+
+        # 调用待测试函数
+        states, transitions = straight_chain(
+            start_speed=start_speed,
+            end_speed=end_speed,
+            duration=duration,
+            power_exponent=power_exponent,
+            interval=interval,
+            breaker=break_function,
+        )
+
+        botix = Botix(controller=CloseLoopController([MotorInfo(i) for i in range(4)]), token_pool=transitions)
+        botix.export_structure("long_chain.puml")
+
+    # 测试breaker不是None且不是callable的情况
+    def test_straight_chain_with_invalid_breaker(self):
+        start_speed = 50
+        end_speed = 100
+        duration = 5.0
+        power_exponent = 1.0
+        interval = 0.07
+
+        # 使用错误的breaker参数
+        with self.assertRaises(ValueError):
+            straight_chain(
+                start_speed=start_speed,
+                end_speed=end_speed,
+                duration=duration,
+                power_exponent=power_exponent,
+                interval=interval,
+                breaker="not a callable",
+            )
+
+    def test_mk(self):
+        from mentabotix import MovingChainComposer, MovingState, MovingTransition
+
+        # init the state-transition composer
+        comp = MovingChainComposer()
+
+        # add some states and transitions one by one to the composer, the composer will auto-connect the states and transitions
+        (
+            comp.add(MovingState(0))
+            .add(MovingTransition(0.2))
+            .add(MovingState(1000))
+            .add(MovingTransition(0.3))
+            .add(MovingState(2000))
+        )
+
+        # export the structure
+        states, transitions = comp.export_structure()
+
+        # let's use botix to make the visualization!
+        # first make the botix object
+        con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
+        botix = Botix(controller=con, token_pool=transitions)
+
+        # make the visualization
+        botix.export_structure("composed.puml")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mentabotix-0.1.3a2/tests/test_menta.py` & `mentabotix-0.1.3a3/tests/test_menta.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-import unittest
-from typing import List, Callable
-
-from mentabotix import set_log_level
-from mentabotix.modules.menta import (
-    Menta,
-    SamplerType,
-    SamplerUsage,
-)
-
-
-# 示例采样器实现
-def mock_sequence_sampler() -> List:
-    return [1.2, 32, 1.3]
-
-
-def mock_indexed_sampler(index: int) -> int:
-    return 10 * index
-
-
-def mock_direct_sampler() -> int:
-    return 42
-
-
-class TestMenta(unittest.TestCase):
-
-    def setUp(self):
-        set_log_level(10)
-        self.menta = Menta(
-            [
-                mock_sequence_sampler,
-                mock_indexed_sampler,
-                mock_direct_sampler,
-            ]
-        )
-
-    def test_init(self):
-        self.assertIsInstance(self.menta.samplers, List)
-        self.assertEqual(len(self.menta.samplers), 3)
-        self.assertIsNotNone(self.menta.sampler_types)
-
-    def test_update_sampler_types(self):
-        self.menta.update_sampler_types()
-        self.assertEqual(
-            self.menta.sampler_types,
-            [
-                SamplerType.SEQ_SAMPLER,
-                SamplerType.IDX_SAMPLER,
-                SamplerType.DRC_SAMPLER,
-            ],
-        )
-
-    def test_construct_updater_single_seq_sampler(self):
-        usage = SamplerUsage(used_sampler_index=0, required_data_indexes=[])
-        updater = self.menta.construct_updater([usage])
-        result = updater()
-        self.assertIsInstance(result, List)
-        self.assertEqual(len(result), 3)
-        for data in result:
-            self.assertIsInstance(data, int | float)
-
-    def test_construct_updater_single_idx_sampler(self):
-        usage = SamplerUsage(used_sampler_index=1, required_data_indexes=[0])
-        updater = self.menta.construct_updater([usage])
-        result = updater()
-        self.assertIsInstance(result, int)
-        self.assertEqual(result, 0)
-
-    def test_construct_updater_single_drc_sampler(self):
-        usage = SamplerUsage(used_sampler_index=2, required_data_indexes=[])
-        updater = self.menta.construct_updater([usage])
-        result = updater()
-        self.assertIsInstance(result, int)
-        self.assertEqual(result, 42)
-
-    def test_construct_updater_multiple_samplers(self):
-        usages = [
-            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
-            SamplerUsage(used_sampler_index=2, required_data_indexes=[]),
-        ]
-        updater = self.menta.construct_updater(usages)
-        results = updater()
-        print(results)
-        self.assertIsInstance(results, tuple)
-        self.assertEqual(len(results), 3)
-        self.assertEqual(results[0], (1.2, 1.3))
-        self.assertEqual(results[1], 50)
-        self.assertEqual(results[2], 42)
-
-    def test_resolve_drc_sampler(self):
-        usage = SamplerUsage(used_sampler_index=2, required_data_indexes=[])
-        updater = self.menta.resolve_drc_sampler(
-            sampler=self.menta.samplers[usage.used_sampler_index], required_data_indexes=usage.required_data_indexes
-        )
-        result = updater()
-        self.assertIsInstance(result, int)
-        self.assertEqual(result, 42)
-
-        """
-        f'{42:08b}' => '00101010'
-        # make this 8-bits to list should get [0,1,0,1,0,1,0,0], it is reversed
-        """
-        usage = SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2])
-        updater = self.menta.resolve_drc_sampler(
-            sampler=self.menta.samplers[usage.used_sampler_index], required_data_indexes=usage.required_data_indexes
-        )
-        result = updater()
-        print(result)
-        self.assertIsInstance(result, tuple)
-        self.assertEqual(0, result[0])
-        self.assertEqual(1, result[1])
-        self.assertEqual(0, result[2])
-
-    def test_construct_judge(self):
-        # Test with multiple usages
-        sages = [
-            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
-            SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
-        ]
-        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0 or s1 or s2 or s3 or s4 or s5")
-        self.assertIsInstance(func, Callable)
-        self.assertEqual(func(), 1.2)
-        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
-        self.assertIsInstance(func, Callable)
-        self.assertEqual(func(), 53.5)
-
-        # Test with 1 usage
-        func = self.menta.construct_judge_function(
-            usages=[
-                SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-            ],
-            judging_source="ret=s0 + s1",
-        )
-        self.assertIsInstance(func, Callable)
-        self.assertEqual(func(), 2.5)
-
-        # Test with  multiline judging source
-        func = self.menta.construct_judge_function(
-            usages=sages,
-            judging_source=["a=s0+s1", "print(f'this is {a}')", "b=s3+s4+s5", "print(f'this is {b}')", "ret=s2"],
-        )
-        self.assertIsInstance(func, Callable)
-        self.assertEqual(func(), 50)
-
-    def test_indexer_seq(self):
-        varname = "hel"
-        req = [0, 1, 2, 3]
-        data_1 = self.menta._index_for_seq_sampler_data(varname, req)
-        print(data_1)
-        self.assertEqual(["hel[0]", "hel[1]", "hel[2]", "hel[3]"], data_1)
-
-        data_2 = self.menta._index_for_seq_sampler_data(varname, len(req))
-        self.assertEqual(["hel[0]", "hel[1]", "hel[2]", "hel[3]"], data_2)
-
-    def test_indexer_drc(self):
-        varname = "hel"
-        req = [0, 1, 2]
-
-        data_3 = self.menta._index_for_drc_sampler_data(varname, req)
-        self.assertEqual(["((hel>>0)&1)", "((hel>>1)&1)", "((hel>>2)&1)"], data_3)
-
-        data_4 = self.menta._index_for_drc_sampler_data(varname, len(req))
-        self.assertEqual(["((hel>>0)&1)", "((hel>>1)&1)", "((hel>>2)&1)"], data_4)
-
-    def test_indexer_idx(self):
-        varname = "hel"
-        req = [0, 1, 2]
-        data_1 = self.menta._index_for_idx_sampler_data(varname, req)
-        print(data_1)
-        self.assertEqual(["hel(0)", "hel(1)", "hel(2)"], data_1)
-
-    def test_constructed_judge_function_performance(self):
-        sages = [
-            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
-            SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
-        ]
-        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
-
-        def _manual_seq_func():
-            seq_temp = mock_sequence_sampler()
-
-            return seq_temp[0], seq_temp[2]
-
-        def _manual_drc_func():
-            drc_temp = mock_direct_sampler()
-            return tuple((drc_temp >> ri) & 1 for ri in [0, 1, 2])
-
-        def _manual_asm_func():
-            return *_manual_seq_func(), mock_indexed_sampler(5), *_manual_drc_func()
-
-        def _manual_judge_func():
-            return sum(_manual_asm_func())
-
-        self.assertEqual(func(), _manual_judge_func())
-
-        import timeit
-
-        # 假设这两个函数已经在你的代码中定义好了
-
-        # 设置测试次数（例如：1000次）
-        number_of_runs = 1000
-
-        # 对func()进行计时测试
-        func_time = timeit.timeit(lambda: func(), number=number_of_runs)
-
-        print(f"func() execution time for {number_of_runs} runs: {func_time:.6f} seconds")
-
-        # 对_manual_judge_func()进行计时测试
-        manual_judge_func_time = timeit.timeit(lambda: _manual_judge_func(), number=number_of_runs)
-
-        print(f"_manual_judge_func() execution time for {number_of_runs} runs: {manual_judge_func_time:.6f} seconds")
-
-        print(f"func() is {manual_judge_func_time / func_time:.2f} times faster than _manual_judge_func()")
-
-    def tearDown(self):
-        # 清理可能的副作用
-        pass
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from typing import List, Callable
+
+from mentabotix import set_log_level
+from mentabotix.modules.menta import (
+    Menta,
+    SamplerType,
+    SamplerUsage,
+)
+
+
+# 示例采样器实现
+def mock_sequence_sampler() -> List:
+    return [1.2, 32, 1.3]
+
+
+def mock_indexed_sampler(index: int) -> int:
+    return 10 * index
+
+
+def mock_direct_sampler() -> int:
+    return 42
+
+
+class TestMenta(unittest.TestCase):
+
+    def setUp(self):
+        set_log_level(10)
+        self.menta = Menta(
+            [
+                mock_sequence_sampler,
+                mock_indexed_sampler,
+                mock_direct_sampler,
+            ]
+        )
+
+    def test_init(self):
+        self.assertIsInstance(self.menta.samplers, List)
+        self.assertEqual(len(self.menta.samplers), 3)
+        self.assertIsNotNone(self.menta.sampler_types)
+
+    def test_update_sampler_types(self):
+        self.menta.update_sampler_types()
+        self.assertEqual(
+            self.menta.sampler_types,
+            [
+                SamplerType.SEQ_SAMPLER,
+                SamplerType.IDX_SAMPLER,
+                SamplerType.DRC_SAMPLER,
+            ],
+        )
+
+    def test_construct_updater_single_seq_sampler(self):
+        usage = SamplerUsage(used_sampler_index=0, required_data_indexes=[])
+        updater = self.menta.construct_updater([usage])
+        result = updater()
+        self.assertIsInstance(result, List)
+        self.assertEqual(len(result), 3)
+        for data in result:
+            self.assertIsInstance(data, int | float)
+
+    def test_construct_updater_single_idx_sampler(self):
+        usage = SamplerUsage(used_sampler_index=1, required_data_indexes=[0])
+        updater = self.menta.construct_updater([usage])
+        result = updater()
+        self.assertIsInstance(result, int)
+        self.assertEqual(result, 0)
+
+    def test_construct_updater_single_drc_sampler(self):
+        usage = SamplerUsage(used_sampler_index=2, required_data_indexes=[])
+        updater = self.menta.construct_updater([usage])
+        result = updater()
+        self.assertIsInstance(result, int)
+        self.assertEqual(result, 42)
+
+    def test_construct_updater_multiple_samplers(self):
+        usages = [
+            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
+            SamplerUsage(used_sampler_index=2, required_data_indexes=[]),
+        ]
+        updater = self.menta.construct_updater(usages)
+        results = updater()
+        print(results)
+        self.assertIsInstance(results, tuple)
+        self.assertEqual(len(results), 3)
+        self.assertEqual(results[0], (1.2, 1.3))
+        self.assertEqual(results[1], 50)
+        self.assertEqual(results[2], 42)
+
+    def test_resolve_drc_sampler(self):
+        usage = SamplerUsage(used_sampler_index=2, required_data_indexes=[])
+        updater = self.menta.resolve_drc_sampler(
+            sampler=self.menta.samplers[usage.used_sampler_index], required_data_indexes=usage.required_data_indexes
+        )
+        result = updater()
+        self.assertIsInstance(result, int)
+        self.assertEqual(result, 42)
+
+        """
+        f'{42:08b}' => '00101010'
+        # make this 8-bits to list should get [0,1,0,1,0,1,0,0], it is reversed
+        """
+        usage = SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2])
+        updater = self.menta.resolve_drc_sampler(
+            sampler=self.menta.samplers[usage.used_sampler_index], required_data_indexes=usage.required_data_indexes
+        )
+        result = updater()
+        print(result)
+        self.assertIsInstance(result, tuple)
+        self.assertEqual(0, result[0])
+        self.assertEqual(1, result[1])
+        self.assertEqual(0, result[2])
+
+    def test_construct_judge(self):
+        # Test with multiple usages
+        sages = [
+            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
+            SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
+        ]
+        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0 or s1 or s2 or s3 or s4 or s5")
+        self.assertIsInstance(func, Callable)
+        self.assertEqual(func(), 1.2)
+        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
+        self.assertIsInstance(func, Callable)
+        self.assertEqual(func(), 53.5)
+
+        # Test with 1 usage
+        func = self.menta.construct_judge_function(
+            usages=[
+                SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+            ],
+            judging_source="ret=s0 + s1",
+        )
+        self.assertIsInstance(func, Callable)
+        self.assertEqual(func(), 2.5)
+
+        # Test with  multiline judging source
+        func = self.menta.construct_judge_function(
+            usages=sages,
+            judging_source=["a=s0+s1", "print(f'this is {a}')", "b=s3+s4+s5", "print(f'this is {b}')", "ret=s2"],
+        )
+        self.assertIsInstance(func, Callable)
+        self.assertEqual(func(), 50)
+
+    def test_indexer_seq(self):
+        varname = "hel"
+        req = [0, 1, 2, 3]
+        data_1 = self.menta._index_for_seq_sampler_data(varname, req)
+        print(data_1)
+        self.assertEqual(["hel[0]", "hel[1]", "hel[2]", "hel[3]"], data_1)
+
+        data_2 = self.menta._index_for_seq_sampler_data(varname, len(req))
+        self.assertEqual(["hel[0]", "hel[1]", "hel[2]", "hel[3]"], data_2)
+
+    def test_indexer_drc(self):
+        varname = "hel"
+        req = [0, 1, 2]
+
+        data_3 = self.menta._index_for_drc_sampler_data(varname, req)
+        self.assertEqual(["((hel>>0)&1)", "((hel>>1)&1)", "((hel>>2)&1)"], data_3)
+
+        data_4 = self.menta._index_for_drc_sampler_data(varname, len(req))
+        self.assertEqual(["((hel>>0)&1)", "((hel>>1)&1)", "((hel>>2)&1)"], data_4)
+
+    def test_indexer_idx(self):
+        varname = "hel"
+        req = [0, 1, 2]
+        data_1 = self.menta._index_for_idx_sampler_data(varname, req)
+        print(data_1)
+        self.assertEqual(["hel(0)", "hel(1)", "hel(2)"], data_1)
+
+    def test_constructed_judge_function_performance(self):
+        sages = [
+            SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+            SamplerUsage(used_sampler_index=1, required_data_indexes=[5]),
+            SamplerUsage(used_sampler_index=2, required_data_indexes=[0, 1, 2]),
+        ]
+        func = self.menta.construct_judge_function(usages=sages, judging_source="ret=s0+s1+s2+s3+s4+s5")
+
+        def _manual_seq_func():
+            seq_temp = mock_sequence_sampler()
+
+            return seq_temp[0], seq_temp[2]
+
+        def _manual_drc_func():
+            drc_temp = mock_direct_sampler()
+            return tuple((drc_temp >> ri) & 1 for ri in [0, 1, 2])
+
+        def _manual_asm_func():
+            return *_manual_seq_func(), mock_indexed_sampler(5), *_manual_drc_func()
+
+        def _manual_judge_func():
+            return sum(_manual_asm_func())
+
+        self.assertEqual(func(), _manual_judge_func())
+
+        import timeit
+
+        # 假设这两个函数已经在你的代码中定义好了
+
+        # 设置测试次数（例如：1000次）
+        number_of_runs = 1000
+
+        # 对func()进行计时测试
+        func_time = timeit.timeit(lambda: func(), number=number_of_runs)
+
+        print(f"func() execution time for {number_of_runs} runs: {func_time:.6f} seconds")
+
+        # 对_manual_judge_func()进行计时测试
+        manual_judge_func_time = timeit.timeit(lambda: _manual_judge_func(), number=number_of_runs)
+
+        print(f"_manual_judge_func() execution time for {number_of_runs} runs: {manual_judge_func_time:.6f} seconds")
+
+        print(f"func() is {manual_judge_func_time / func_time:.2f} times faster than _manual_judge_func()")
+
+    def tearDown(self):
+        # 清理可能的副作用
+        pass
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mentabotix-0.1.3a2/tests/test_moving_state.py` & `mentabotix-0.1.3a3/tests/test_moving_state.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import unittest
-from unittest.mock import Mock
-
-from bdmc.modules.controller import CloseLoopController, MotorInfo
-
-from mentabotix import MovingState
-
-
-class TestMovingState(unittest.TestCase):
-
-    def setUp(self):
-        MovingState.__state_id_counter__ = 0
-
-    def test_init_speeds(self):
-        # Test FullPattern
-        state_full = MovingState(50)
-        self.assertEqual(state_full.unwrap(), (50, 50, 50, 50))
-
-        # Test LRPattern
-        state_lr = MovingState(30, 60)
-        self.assertEqual(state_lr.unwrap(), (30, 30, 60, 60))
-
-        # Test IndividualPattern
-        state_individual = MovingState(10, 20, 30, 40)
-        self.assertEqual(state_individual.unwrap(), (10, 20, 30, 40))
-
-    def test_init_speed_expressions(self):
-        used_context_variables = ["var1", "var2"]
-
-        # Test FullExpressionPattern
-        state_full_expr = MovingState(speed_expressions="var1+var2", used_context_variables=used_context_variables)
-        self.assertEqual(state_full_expr.speed_expressions, ("var1+var2", "var1+var2", "var1+var2", "var1+var2"))
-
-        # Test LRExpressionPattern
-        state_lr_expr = MovingState(speed_expressions=("var1", "var2"), used_context_variables=used_context_variables)
-        self.assertEqual(state_lr_expr.speed_expressions, ("var1", "var1", "var2", "var2"))
-
-        # Test IndividualExpressionPattern
-        state_indiv_expr = MovingState(
-            speed_expressions=("var1", "var2", "var1+var2", "2*var1-var2"),
-            used_context_variables=used_context_variables,
-        )
-        self.assertEqual(state_indiv_expr.speed_expressions, ("var1", "var2", "var1+var2", "2*var1-var2"))
-
-    def test_init_invalid_arguments(self):
-        with self.assertRaises(ValueError):
-            MovingState()
-
-        with self.assertRaises(ValueError):
-            MovingState(1, 2, 3, 5, speed_expressions=("expr1", "expr2"))
-
-        with self.assertRaises(ValueError):
-            MovingState(speed_expressions=("expr1", "expr2"), used_context_variables=["var1", "var2"])
-
-    def test_class_methods(self):
-        # Test halt
-        state_halt = MovingState.halt()
-        self.assertEqual(state_halt.unwrap(), (0, 0, 0, 0))
-
-        # Test straight
-        state_straight_fwd = MovingState.straight(80)
-        self.assertEqual(state_straight_fwd.unwrap(), (80, 80, 80, 80))
-        state_straight_bwd = MovingState.straight(-80)
-        self.assertEqual(state_straight_bwd.unwrap(), (-80, -80, -80, -80))
-
-        # Test differential
-        state_diff_l = MovingState.differential("l", radius=20, outer_speed=70)
-        self.assertEqual(state_diff_l.unwrap(), (11, 11, 70, 70))
-        state_diff_r = MovingState.differential("r", radius=20, outer_speed=70)
-        self.assertEqual(state_diff_r.unwrap(), (70, 70, 11, 11))
-
-        # Test turn
-        state_turn_l = MovingState.turn("l", 90)
-        self.assertEqual(state_turn_l.unwrap(), (-90, -90, 90, 90))
-        state_turn_r = MovingState.turn("r", 90)
-        self.assertEqual(state_turn_r.unwrap(), (90, 90, -90, -90))
-
-        # Test drift
-        state_drift_fl = MovingState.drift("fl", 50)
-        self.assertEqual(state_drift_fl.unwrap(), (0, 50, int(76.5), 50))
-        state_drift_rl = MovingState.drift("rl", 50)
-        self.assertEqual(state_drift_rl.unwrap(), (50, 0, 50, int(76.5)))
-        state_drift_rr = MovingState.drift("rr", 50)
-        self.assertEqual(state_drift_rr.unwrap(), (int(76.5), 50, 0, 50))
-        state_drift_fr = MovingState.drift("fr", 50)
-        self.assertEqual(state_drift_fr.unwrap(), (50, int(76.5), 50, 0))
-
-    def test_apply(self):
-        state = MovingState(20, 30, 40, 50)
-        state_applied = state.apply(1.5)
-
-        self.assertEqual(state_applied.unwrap(), (30, 45, 60, 75))
-
-    def test_clone(self):
-        original_state = MovingState(10, 20, 30, 40)
-        cloned_state = original_state.clone()
-
-        self.assertEqual(cloned_state.unwrap(), (10, 20, 30, 40))
-        self.assertIsNot(cloned_state, original_state)  # Ensure a new instance is returned
-
-    def test_tokenize(self):
-
-        con_mock = Mock(
-            spec=CloseLoopController(
-                [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM4", context={"var1": 10, "var2": 20}
-            )
-        )
-
-        state_with_speeds = MovingState(10, 20, 30, 40)
-        tokens, context = state_with_speeds.tokenize(con_mock)
-        self.assertEqual(tokens, [".set_motors_speed((10, 20, 30, 40))"])
-        self.assertEqual(context, {})  # No context needed for states with speeds
-
-        state_with_expressions = MovingState(
-            speed_expressions=("var1", "var2", "var1+var2", "2*var1-var2"),
-            used_context_variables=["var1", "var2"],
-        )
-        tokens, context = state_with_expressions.tokenize(con_mock)
-        self.assertCountEqual(
-            [
-                ".set_motors_speed(((state1_context_getter_temp_2:=state1_context_getter_2()), "
-                "(state1_context_getter_temp_1:=state1_context_getter_1()), "
-                "state1_context_getter_temp_2+state1_context_getter_temp_1, "
-                "2*state1_context_getter_temp_2-state1_context_getter_temp_1))"
-            ][0],
-            tokens[0],
-        )
-
-        self.assertIn("state1_context_getter_1", context)
-        self.assertIn("state1_context_getter_2", context)
-
-        print(f"Tokens: {tokens}, Context: {context}")
-        # Tokens and context assertions depend on the NameGenerator implementation, which is not provided
-        # You can add appropriate assertions here once you have the actual generated tokens and context
-
-    def test_hash_and_eq(self):
-        state1 = MovingState(10, 20, 30, 40)
-        print(f"State1: {state1}")
-        state2 = MovingState(10, 20, 30, 40)
-        print(f"State2: {state2}")
-        state3 = MovingState(11, 20, 30, 40)
-        print(f"State3: {state3}")
-        self.assertEqual(hash(state1), hash(state2) - 1)
-        self.assertNotEqual(hash(state1), hash(state3))
-
-        self.assertEqual(state1, state2)
-        self.assertNotEqual(state1, state3)
-
-    def test_str(self):
-        state = MovingState(10, 20, 30, 40)
-        self.assertEqual(str(state), f"{state.state_id}-MovingState(10, 20, 30, 40)")
-        state = MovingState(speed_expressions="var1", used_context_variables=["var1"])
-        self.assertEqual(str(state), f"{state.state_id}-MovingState('var1', 'var1', 'var1', 'var1')")
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from unittest.mock import Mock
+
+from bdmc.modules.controller import CloseLoopController, MotorInfo
+
+from mentabotix import MovingState
+
+
+class TestMovingState(unittest.TestCase):
+
+    def setUp(self):
+        MovingState.__state_id_counter__ = 0
+
+    def test_init_speeds(self):
+        # Test FullPattern
+        state_full = MovingState(50)
+        self.assertEqual(state_full.unwrap(), (50, 50, 50, 50))
+
+        # Test LRPattern
+        state_lr = MovingState(30, 60)
+        self.assertEqual(state_lr.unwrap(), (30, 30, 60, 60))
+
+        # Test IndividualPattern
+        state_individual = MovingState(10, 20, 30, 40)
+        self.assertEqual(state_individual.unwrap(), (10, 20, 30, 40))
+
+    def test_init_speed_expressions(self):
+        used_context_variables = ["var1", "var2"]
+
+        # Test FullExpressionPattern
+        state_full_expr = MovingState(speed_expressions="var1+var2", used_context_variables=used_context_variables)
+        self.assertEqual(state_full_expr.speed_expressions, ("var1+var2", "var1+var2", "var1+var2", "var1+var2"))
+
+        # Test LRExpressionPattern
+        state_lr_expr = MovingState(speed_expressions=("var1", "var2"), used_context_variables=used_context_variables)
+        self.assertEqual(state_lr_expr.speed_expressions, ("var1", "var1", "var2", "var2"))
+
+        # Test IndividualExpressionPattern
+        state_indiv_expr = MovingState(
+            speed_expressions=("var1", "var2", "var1+var2", "2*var1-var2"),
+            used_context_variables=used_context_variables,
+        )
+        self.assertEqual(state_indiv_expr.speed_expressions, ("var1", "var2", "var1+var2", "2*var1-var2"))
+
+    def test_init_invalid_arguments(self):
+        with self.assertRaises(ValueError):
+            MovingState()
+
+        with self.assertRaises(ValueError):
+            MovingState(1, 2, 3, 5, speed_expressions=("expr1", "expr2"))
+
+        with self.assertRaises(ValueError):
+            MovingState(speed_expressions=("expr1", "expr2"), used_context_variables=["var1", "var2"])
+
+    def test_class_methods(self):
+        # Test halt
+        state_halt = MovingState.halt()
+        self.assertEqual(state_halt.unwrap(), (0, 0, 0, 0))
+
+        # Test straight
+        state_straight_fwd = MovingState.straight(80)
+        self.assertEqual(state_straight_fwd.unwrap(), (80, 80, 80, 80))
+        state_straight_bwd = MovingState.straight(-80)
+        self.assertEqual(state_straight_bwd.unwrap(), (-80, -80, -80, -80))
+
+        # Test differential
+        state_diff_l = MovingState.differential("l", radius=20, outer_speed=70)
+        self.assertEqual(state_diff_l.unwrap(), (11, 11, 70, 70))
+        state_diff_r = MovingState.differential("r", radius=20, outer_speed=70)
+        self.assertEqual(state_diff_r.unwrap(), (70, 70, 11, 11))
+
+        # Test turn
+        state_turn_l = MovingState.turn("l", 90)
+        self.assertEqual(state_turn_l.unwrap(), (-90, -90, 90, 90))
+        state_turn_r = MovingState.turn("r", 90)
+        self.assertEqual(state_turn_r.unwrap(), (90, 90, -90, -90))
+
+        # Test drift
+        state_drift_fl = MovingState.drift("fl", 50)
+        self.assertEqual(state_drift_fl.unwrap(), (0, 50, int(76.5), 50))
+        state_drift_rl = MovingState.drift("rl", 50)
+        self.assertEqual(state_drift_rl.unwrap(), (50, 0, 50, int(76.5)))
+        state_drift_rr = MovingState.drift("rr", 50)
+        self.assertEqual(state_drift_rr.unwrap(), (int(76.5), 50, 0, 50))
+        state_drift_fr = MovingState.drift("fr", 50)
+        self.assertEqual(state_drift_fr.unwrap(), (50, int(76.5), 50, 0))
+
+    def test_apply(self):
+        state = MovingState(20, 30, 40, 50)
+        state_applied = state.apply(1.5)
+
+        self.assertEqual(state_applied.unwrap(), (30, 45, 60, 75))
+
+    def test_clone(self):
+        original_state = MovingState(10, 20, 30, 40)
+        cloned_state = original_state.clone()
+
+        self.assertEqual(cloned_state.unwrap(), (10, 20, 30, 40))
+        self.assertIsNot(cloned_state, original_state)  # Ensure a new instance is returned
+
+    def test_tokenize(self):
+
+        con_mock = Mock(
+            spec=CloseLoopController(
+                [MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4)], port="COM4", context={"var1": 10, "var2": 20}
+            )
+        )
+
+        state_with_speeds = MovingState(10, 20, 30, 40)
+        tokens, context = state_with_speeds.tokenize(con_mock)
+        self.assertEqual(tokens, [".set_motors_speed((10, 20, 30, 40))"])
+        self.assertEqual(context, {})  # No context needed for states with speeds
+
+        state_with_expressions = MovingState(
+            speed_expressions=("var1", "var2", "var1+var2", "2*var1-var2"),
+            used_context_variables=["var1", "var2"],
+        )
+        tokens, context = state_with_expressions.tokenize(con_mock)
+        self.assertCountEqual(
+            [
+                ".set_motors_speed(((state1_context_getter_temp_2:=state1_context_getter_2()), "
+                "(state1_context_getter_temp_1:=state1_context_getter_1()), "
+                "state1_context_getter_temp_2+state1_context_getter_temp_1, "
+                "2*state1_context_getter_temp_2-state1_context_getter_temp_1))"
+            ][0],
+            tokens[0],
+        )
+
+        self.assertIn("state1_context_getter_1", context)
+        self.assertIn("state1_context_getter_2", context)
+
+        print(f"Tokens: {tokens}, Context: {context}")
+        # Tokens and context assertions depend on the NameGenerator implementation, which is not provided
+        # You can add appropriate assertions here once you have the actual generated tokens and context
+
+    def test_hash_and_eq(self):
+        state1 = MovingState(10, 20, 30, 40)
+        print(f"State1: {state1}")
+        state2 = MovingState(10, 20, 30, 40)
+        print(f"State2: {state2}")
+        state3 = MovingState(11, 20, 30, 40)
+        print(f"State3: {state3}")
+        self.assertEqual(hash(state1), hash(state2) - 1)
+        self.assertNotEqual(hash(state1), hash(state3))
+
+        self.assertEqual(state1, state2)
+        self.assertNotEqual(state1, state3)
+
+    def test_str(self):
+        state = MovingState(10, 20, 30, 40)
+        self.assertEqual(str(state), f"{state.state_id}-MovingState(10, 20, 30, 40)")
+        state = MovingState(speed_expressions="var1", used_context_variables=["var1"])
+        self.assertEqual(str(state), f"{state.state_id}-MovingState('var1', 'var1', 'var1', 'var1')")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mentabotix-0.1.3a2/tests/test_moving_transition.py` & `mentabotix-0.1.3a3/tests/test_moving_transition.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import unittest
-from itertools import zip_longest
-from unittest.mock import patch
-
-from terminaltables import SingleTable
-
-from mentabotix.modules.botix import MovingTransition, MovingState
-
-
-# Define a mock MovingState class for testing purposes
-
-
-class TestMovingTransition(unittest.TestCase):
-
-    def setUp(self):
-        self.default_duration = 1.5
-
-        def breker() -> bool:
-            return True
-
-        self.default_breaker = breker
-        self.default_check_interval = 0.2
-        self.default_from_state = MovingState(0)
-        self.default_to_state = MovingState(0)
-
-    def test_init_valid_input(self):
-        # Test valid input with all parameters provided
-        transition = MovingTransition(
-            self.default_duration,
-            self.default_breaker,
-            self.default_check_interval,
-            self.default_from_state,
-            self.default_to_state,
-        )
-        self.assertEqual(transition.duration, self.default_duration)
-        self.assertEqual(transition.breaker, self.default_breaker)
-        self.assertEqual(transition.check_interval, self.default_check_interval)
-        self.assertIsInstance(transition.from_states, list)
-        self.assertIsInstance(transition.to_states, dict)
-
-    def test_init_duration_not_positive(self):
-        with self.assertRaises(ValueError):
-            MovingTransition(-1, None, None, None, None)
-
-    def test_init_breaker_no_return_type_annotation(self):
-        def invalid_breaker():
-            pass
-
-        with self.assertRaises(ValueError):
-            MovingTransition(self.default_duration, invalid_breaker, None, None, None)
-
-    def test_init_from_states_valid_types(self):
-        # Test valid from_states types
-        transition = MovingTransition(self.default_duration, None, None, self.default_from_state, None)
-        self.assertEqual(len(transition.from_states), 1)
-        self.assertEqual(transition.from_states[0], self.default_from_state)
-
-        from_states_iterable = [MovingState(0), MovingState(0)]
-        transition = MovingTransition(self.default_duration, None, None, from_states_iterable, None)
-        self.assertEqual(len(transition.from_states), len(from_states_iterable))
-        self.assertEqual(transition.from_states, list(from_states_iterable))
-
-    def test_init_from_states_invalid_type(self):
-        with self.assertRaises(ValueError):
-            MovingTransition(self.default_duration, None, None, "invalid", None)
-
-    def test_init_to_states_valid_types(self):
-        # Test valid to_states types
-        transition = MovingTransition(self.default_duration, None, None, None, self.default_to_state)
-        self.assertEqual(len(transition.to_states), 1)
-        self.assertEqual(list(transition.to_states.values())[0], self.default_to_state)
-
-        to_states_dict = {1: MovingState(0), 2: MovingState(1)}
-        transition = MovingTransition(self.default_duration, None, None, None, to_states_dict)
-        self.assertEqual(len(transition.to_states), len(to_states_dict))
-        self.assertEqual(transition.to_states, to_states_dict)
-
-    def test_init_to_states_invalid_type(self):
-        with self.assertRaises(ValueError):
-            MovingTransition(self.default_duration, None, None, None, "invalid")
-
-    def test_add_from_state(self):
-        transition = MovingTransition(self.default_duration, None, None, None, None)
-        transition.add_from_state(self.default_from_state)
-        self.assertEqual(len(transition.from_states), 1)
-        self.assertEqual(transition.from_states[0], self.default_from_state)
-
-    def test_add_to_state(self):
-        transition = MovingTransition(self.default_duration, None, None, None, None)
-        key = 1
-        transition.add_to_state(key, self.default_to_state)
-        self.assertEqual(len(transition.to_states), 1)
-        self.assertEqual(transition.to_states[key], self.default_to_state)
-
-    @patch("mentabotix.MovingTransition.tokenize")
-    def test_tokenize_called(self, mock_tokenize):
-        transition = MovingTransition(self.default_duration, None, None, None, None)
-        transition.tokenize()
-        mock_tokenize.assert_called_once_with()
-
-    @patch("mentabotix.MovingTransition.clone")
-    def test_clone_called(self, mock_clone):
-        transition = MovingTransition(self.default_duration, None, None, None, None)
-        transition.clone()
-        mock_clone.assert_called_once_with()
-
-    def test_identifier(self):
-        transition1 = MovingTransition(self.default_duration, None, None, None, None)
-        transition2 = MovingTransition(self.default_duration, None, None, None, None)
-        self.assertNotEqual(transition1.identifier, transition2.identifier)
-
-    def test_str(self):
-        from_states = [MovingState(100), MovingState(0)]
-        to_states = {1: MovingState(4100), 2: MovingState(2000), 3: MovingState(0)}
-        transition = MovingTransition(self.default_duration, None, None, from_states, to_states)
-        temp = [["From", "To"]]
-        for from_state, to_state in zip_longest(transition.from_states, transition.to_states.values()):
-            temp.append([str(from_state) if from_state else "", str(to_state) if to_state else ""])
-
-        self.assertEqual(str(transition), SingleTable(temp).table)
-
-    def test_hash(self):
-        transition1 = MovingTransition(self.default_duration, None, None, None, None)
-        transition2 = MovingTransition(self.default_duration, None, None, None, None)
-        self.assertNotEqual(hash(transition1), hash(transition2))
-
-
-if __name__ == "__main__":
-    unittest.main()
+import unittest
+from itertools import zip_longest
+from unittest.mock import patch
+
+from terminaltables import SingleTable
+
+from mentabotix.modules.botix import MovingTransition, MovingState
+
+
+# Define a mock MovingState class for testing purposes
+
+
+class TestMovingTransition(unittest.TestCase):
+
+    def setUp(self):
+        self.default_duration = 1.5
+
+        def breker() -> bool:
+            return True
+
+        self.default_breaker = breker
+        self.default_check_interval = 0.2
+        self.default_from_state = MovingState(0)
+        self.default_to_state = MovingState(0)
+
+    def test_init_valid_input(self):
+        # Test valid input with all parameters provided
+        transition = MovingTransition(
+            self.default_duration,
+            self.default_breaker,
+            self.default_check_interval,
+            self.default_from_state,
+            self.default_to_state,
+        )
+        self.assertEqual(transition.duration, self.default_duration)
+        self.assertEqual(transition.breaker, self.default_breaker)
+        self.assertEqual(transition.check_interval, self.default_check_interval)
+        self.assertIsInstance(transition.from_states, list)
+        self.assertIsInstance(transition.to_states, dict)
+
+    def test_init_duration_not_positive(self):
+        with self.assertRaises(ValueError):
+            MovingTransition(-1, None, None, None, None)
+
+    def test_init_breaker_no_return_type_annotation(self):
+        def invalid_breaker():
+            pass
+
+        with self.assertRaises(ValueError):
+            MovingTransition(self.default_duration, invalid_breaker, None, None, None)
+
+    def test_init_from_states_valid_types(self):
+        # Test valid from_states types
+        transition = MovingTransition(self.default_duration, None, None, self.default_from_state, None)
+        self.assertEqual(len(transition.from_states), 1)
+        self.assertEqual(transition.from_states[0], self.default_from_state)
+
+        from_states_iterable = [MovingState(0), MovingState(0)]
+        transition = MovingTransition(self.default_duration, None, None, from_states_iterable, None)
+        self.assertEqual(len(transition.from_states), len(from_states_iterable))
+        self.assertEqual(transition.from_states, list(from_states_iterable))
+
+    def test_init_from_states_invalid_type(self):
+        with self.assertRaises(ValueError):
+            MovingTransition(self.default_duration, None, None, "invalid", None)
+
+    def test_init_to_states_valid_types(self):
+        # Test valid to_states types
+        transition = MovingTransition(self.default_duration, None, None, None, self.default_to_state)
+        self.assertEqual(len(transition.to_states), 1)
+        self.assertEqual(list(transition.to_states.values())[0], self.default_to_state)
+
+        to_states_dict = {1: MovingState(0), 2: MovingState(1)}
+        transition = MovingTransition(self.default_duration, None, None, None, to_states_dict)
+        self.assertEqual(len(transition.to_states), len(to_states_dict))
+        self.assertEqual(transition.to_states, to_states_dict)
+
+    def test_init_to_states_invalid_type(self):
+        with self.assertRaises(ValueError):
+            MovingTransition(self.default_duration, None, None, None, "invalid")
+
+    def test_add_from_state(self):
+        transition = MovingTransition(self.default_duration, None, None, None, None)
+        transition.add_from_state(self.default_from_state)
+        self.assertEqual(len(transition.from_states), 1)
+        self.assertEqual(transition.from_states[0], self.default_from_state)
+
+    def test_add_to_state(self):
+        transition = MovingTransition(self.default_duration, None, None, None, None)
+        key = 1
+        transition.add_to_state(key, self.default_to_state)
+        self.assertEqual(len(transition.to_states), 1)
+        self.assertEqual(transition.to_states[key], self.default_to_state)
+
+    @patch("mentabotix.MovingTransition.tokenize")
+    def test_tokenize_called(self, mock_tokenize):
+        transition = MovingTransition(self.default_duration, None, None, None, None)
+        transition.tokenize()
+        mock_tokenize.assert_called_once_with()
+
+    @patch("mentabotix.MovingTransition.clone")
+    def test_clone_called(self, mock_clone):
+        transition = MovingTransition(self.default_duration, None, None, None, None)
+        transition.clone()
+        mock_clone.assert_called_once_with()
+
+    def test_identifier(self):
+        transition1 = MovingTransition(self.default_duration, None, None, None, None)
+        transition2 = MovingTransition(self.default_duration, None, None, None, None)
+        self.assertNotEqual(transition1.identifier, transition2.identifier)
+
+    def test_str(self):
+        from_states = [MovingState(100), MovingState(0)]
+        to_states = {1: MovingState(4100), 2: MovingState(2000), 3: MovingState(0)}
+        transition = MovingTransition(self.default_duration, None, None, from_states, to_states)
+        temp = [["From", "To"]]
+        for from_state, to_state in zip_longest(transition.from_states, transition.to_states.values()):
+            temp.append([str(from_state) if from_state else "", str(to_state) if to_state else ""])
+
+        self.assertEqual(str(transition), SingleTable(temp).table)
+
+    def test_hash(self):
+        transition1 = MovingTransition(self.default_duration, None, None, None, None)
+        transition2 = MovingTransition(self.default_duration, None, None, None, None)
+        self.assertNotEqual(hash(transition1), hash(transition2))
+
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `mentabotix-0.1.3a2/PKG-INFO` & `mentabotix-0.1.3a3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,728 +1,713 @@
-Metadata-Version: 2.1
-Name: mentabotix
-Version: 0.1.3a2
-Summary: A Bot control lib
-Author-Email: Whth <88489697+Whth@users.noreply.github.com>
-License: MIT
-Requires-Python: >=3.11
-Requires-Dist: coloredlogs>=15.0.1
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyapriltags>=3.3.0.3
-Requires-Dist: terminaltables>=3.1.10
-Requires-Dist: bdmc>=0.1.5
-Requires-Dist: opencv-python-headless>=4.9.0.80
-Description-Content-Type: text/markdown
-
-# mentabotix
-
-> A dedicated lib to control 4-fixed-wheels robot
----
-
-## Installation
-
-Use `pdm` to install mentabotix
-
-```shell
-# install pdm
-python -m pip install pdm
-
-# config pdm
-pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
-
-# for stable release
-pdm add mentabotix
-
-# for unstable release
-pdm add mentabotix --pre
-
-```
-
-## Usage
-
-### Menta
-
-You can use `Menta` to create the judge function closure of the robot, using the sensor data as the input.
-
-#### Step 1: Define Sampler Functions
-
-Firstly, you need to define sampler functions that adhere to the specifications outlined by the `Menta` class. These
-could include sequence samplers that return a series of data points, index samplers that provide data at a specific
-index, and direct response samplers that give an immediate value.
-
-|               Sampler                |                 Description                  |                    Type                    |
-|:------------------------------------:|:--------------------------------------------:|:------------------------------------------:|
-| `mentabotix.SamplerType.SEQ_SAMPLER` | The sensor data is returned in a `Sequence`. | `Callable[[], Sequence[Union[float,int]]]` |
-| `mentabotix.SamplerType.IDX_SAMPLER` |         Use a index to get the data.         |    `Callable[[int], Union[float,int]]`     |
-| `mentabotix.SamplerType.DRC_SAMPLER` |  Direct read sensor data without any args.   |      `Callable[[], Union[float,int]]`      |
-
-> Do remember to add return type annotations to your sampler functions, which will be used to classify the samplers into
-> their respective types in the `Menta` class.
-
-```python
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-```
-
-#### Step 2: Initialize Menta Instance and Add Samplers
-
-After defining the sampler functions, initialize the `Menta` instance and add these samplers to it.
-
-```python
-from mentabotix import Menta  # Ensure to import the correct Menta class
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
-```
-
-#### Step 3: Update Sampler Types
-
-Invoke the `update_sampler_types` method to automatically classify the samplers into their respective types.
-
-```python
-from mentabotix import Menta  # Ensure to import the correct Menta class
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
-menta_instance.update_sampler_types()
-```
-
-#### Step 4: Construct Judge Function
-
-To use the samplers in a meaningful way, you can construct an updater function that encapsulates a condition based on
-which system updates might occur. For example:
-
-```python
-from mentabotix import SamplerUsage, Menta
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
-menta_instance.update_sampler_types()
-
-# Define how samplers will be used
-usages = [
-
-    # Use sequence sampler for first and third temp data
-    SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-    # Use index sampler for the first humidity value
-    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),
-]
-
-# Note: the judge source has some built-in syntaxes.Currently, sensor data indexes flattening and extra data context insertion
-# s0 stands for the data at index 0 of the first sampler
-# s1 stands for the data at index 2 of the first sampler
-# s3 stands for the data at index 1 of the second sampler
-
-judging_source = "(s0 > 25 and s1 < 50) or s3>baseline"
-
-# Extra context for the judge function, here only contains the "baseline"
-extra_context = {"baseline": 47}
-
-from typing import Callable
-
-# Construct the judge function object
-updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
-                                                                               extra_context=extra_context)
-
-# Use the judge function to update the system
-updater_function()
-
-
-# Below is the equivalent implementation of the judge function, but is defined manually. 
-# It acts exactly the same as the `updater_function` above.
-def manual_judge_function() -> bool:
-    """Manually construct the judge function."""
-    seq_temp = temperature_sequence_sampler()
-    return (seq_temp[0] > 25 and seq_temp[2] < 50) or humidity_index_sampler(0) > 47
-```
-
-In this case, a judge function closure is created using `exec()` method.Normally the built should have a better
-performance since the all the calls and variables are inlined and stored in the closure.
----
-
-## Botix
-
-Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
-walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
-schemas into executable closures using the Botix framework.
-
-### Understanding State-Transition Control Schema
-
-Let's start with the fundamental schema rules:
-> - A `MovingState` **MUST** connect exactly **ONE** `MovingTransition` as its input state.
->- A `MovingTransition` **MUST** have at least **ONE** `MovingState` as either input or output.
->- A State-Transition Control Schema **MUST** have **EXACTLY ONE** `MovingState` as its initial state and **AT LEAST ONE
-   ** `MovingState` as its final state.
->- A State-Transition Control Schema **MUST NOT** have any loop, a correct control schema should always be a tree graph.
-
-Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
-robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
-these states are triggered by events or conditions, forming a **control schema**.
-
-#### States
-
-- In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
-  motor speeds or changing direction.
-- A state describe the robot's **moving behavior**, 4 motor speeds in this case
-
-#### Transitions
-
-- Transitions between states are handled by the `MovingTransition` class. They define how and when the robot moves from
-  one state to another, possibly based on sensor inputs or internal conditions.
-- Transitions describe how the robot **moves** from one state to another
-
-### Building Your Control Schema
-
-#### Step 1: Define States
-
-For each distinct behavior, create a `MovingState` instance. Include the actions or configurations that should occur in
-that state. For instance, creating a state for moving forward might look like this:
-
-```python
-from mentabotix import MovingState
-
-# the most basic syntax to control the robot advance in a straight line with speed of 10
-# speed of all motors is 10
-moving_forward = MovingState(10)
-# Speeds for left and right motors are 10
-moving_forward = MovingState(10, 10)
-# Speeds for, in order, front_left, rear_left, rear_right, front_right motors are 10
-moving_forward = MovingState(10, 10, 10, 10)
-
-# Use assistant method to create the state instance
-moving_forward = MovingState.straight(10)
-moving_backward = MovingState.straight(-10)
-
-turn_left = MovingState.turn("l", 10)
-turn_right = MovingState.turn("r", 10)
-
-diff_move_left = MovingState.differential("l", radius=20, outer_speed=70)
-diff_move_right = MovingState.differential("r", radius=20, outer_speed=70)
-
-drift_fl = MovingState.drift("fl", 50)
-drift_rl = MovingState.drift("rl", 50)
-drift_rr = MovingState.drift("rr", 50)
-drift_fr = MovingState.drift("fr", 50)
-
-stopped_state = MovingState.halt()
-
-
-
-
-```
-
-#### Step 2: Define Transitions
-
-Transitions are created with `MovingTransition`. Specify the duration, any conditions under which the transition should
-occur (using a breaker function), and the source and destination states.
-
-```python
-from mentabotix import MovingTransition, MovingState
-from random import random
-
-sensor_reading = lambda: random()  # Example sensor reading function
-threshold = 0.6
-
-
-def stop_condition() -> bool:  # the return type must be annotated, since an exception will be raised otherwise
-    return sensor_reading() < threshold
-
-
-moving_forward = MovingState(10)
-stopped_state = MovingState(0)
-
-transition_forward_to_stop = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=stop_condition,  # When to break the transition
-    from_states=moving_forward,
-    to_states=stopped_state,
-)
-# Such transition indicate the bot will move forward for 2 seconds OR stop when the sensor reading is below 25.0 
-
-```
-
-But some time you might want to create a transition that branches out to other states. For example, if the robot needs
-to move forward and then turn left. This can be done by creating a `MovingTransition` like this:
-
-```python
-from mentabotix import MovingTransition, MovingState
-from random import choice
-
-
-def stop_condition() -> int:  # return type must be annotated
-    return choice([0, 1, 2])
-
-
-moving_left = MovingState.turn("l", 10)
-moving_right = MovingState.turn("r", 10)
-moving_dash = MovingState.straight(100)
-stopped_state = MovingState(0)
-
-transition_forward_to_stop = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=stop_condition,  # When to break the transition
-    from_states=stopped_state,
-    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
-)
-
-# Such transition indicate the bot will stop for 2 seconds and then dash forward if nothing happens. ( means the top_condition never return a Non-Zero value)
-
-# If the stop_condition do return a Non-Zero value, 
-# the 2-seconds stop will be broken and the bot will either turn left or right according to the value returned by the stop_condition. (means if the value is 1, it will turn left, if the value is 2, it will turn right)
-
-```
-
-#### Step 3: Connect States with Transitions
-
-Create a collection of your states and transitions, ensuring each transition correctly references its source and target
-states.
-
-A legal control schema should have a start state and at least one end state.
-And each state can **ONLY** connect to **ONE** transition as its input state
-
-```python
-from mentabotix import MovingState, MovingTransition
-import random
-
-moving_left = MovingState.turn("l", 10)
-moving_right = MovingState.turn("r", 10)
-moving_dash = MovingState.straight(100)
-stopped_state = MovingState(0)
-
-start_state = MovingState(100)
-
-
-def _breaker_1() -> int:
-    return random.choice([0, 1, 2])
-
-
-def _breaker_2() -> int:
-    return random.choice([0, 1])
-
-
-transition_1 = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=_breaker_1,  # When to break the transition
-    from_states=stopped_state,
-    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
-)
-
-transition_2 = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=_breaker_2,  # When to break the transition
-    from_states=stopped_state,
-    to_states={0: moving_dash, 1: stopped_state},
-)
-
-
-```
-
-As the above example, `transition_1` and `transition_2` both have the `stopped_state` as the input state,which means
-the `stopped_state` connects more than **ONE** transition. Definition as such is illegal and will not pass the compile
-stage.
-
-Normally, you can ensure that the structure is valid by using `ensure_structure_validity`. to eliminate this problem.
-
-```python
-from mentabotix import Botix
-
-# A StructuralError will be raised if the structure is not valid
-Botix.ensure_structure_validity([transition_1, transition_2])
-```
-
-### Compiling to Closures with Botix
-
-Once your control schema is defined, Botix can help you compile this structure into executable code, often referred to
-as closures, which can directly control the robot's behavior.
-
-#### Step 4: Compile the Schema
-
-Botix provides methods to compile your states and transitions into a Match-Case-Structured Closure.
-
-```python
-from mentabotix import MovingState, MovingTransition, Botix
-from bdmc import CloseLoopController, MotorInfo
-
-con: CloseLoopController = CloseLoopController(motor_infos=[MotorInfo(code_sign=3, direction=1),
-                                                            MotorInfo(code_sign=1, direction=1),
-                                                            MotorInfo(code_sign=2, direction=-1),
-                                                            MotorInfo(code_sign=4, direction=-1)], port="COM3")
-
-start_state = MovingState(-1)
-state_a = MovingState(0)
-state_b = MovingState(1)
-state_c = MovingState(2)
-# 创建一些假的MovingTransition对象用于测试
-transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
-transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
-transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
-
-botix = Botix(controller=con)
-botix.token_pool.append(transition_start_a)
-botix.token_pool.append(transition_ab)
-botix.token_pool.append(transition_bc)
-
-# not compile the code into closure, just return the code lines and context, which is human readable.
-compiled_code_lines, variables_context = botix.compile(return_median=True)
-
-print(compiled_code_lines)
-
-
-```
-
-By printing out the `compiled_code_lines` list, you can see the code lines that are generated by Botix.
-
-```python
-[
-    "def _func():",
-    "    con.set_motors_speed((-1, -1, -1, -1)).delay(0.1).set_motors_speed((0, 0, 0, 0)).delay(1).set_motors_speed((1, 1, 1, 1)).delay(2).set_motors_speed((2, 2, 2, 2))",
-]
-
-```
-
-But usually, you want to compile the code into a closure that can be used to control the robot with higher performance
-and less human error.
-
-```python
-from mentabotix import MovingState, MovingTransition, Botix
-from bdmc import CloseLoopController, MotorInfo
-from typing import Callable
-
-con: CloseLoopController = CloseLoopController(motor_infos=[MotorInfo(code_sign=3, direction=1),
-                                                            MotorInfo(code_sign=1, direction=1),
-                                                            MotorInfo(code_sign=2, direction=-1),
-                                                            MotorInfo(code_sign=4, direction=-1)], port="COM3")
-
-start_state = MovingState(-1)
-state_a = MovingState(0)
-state_b = MovingState(1)
-state_c = MovingState(2)
-# create some transitions
-transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
-transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
-transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
-
-botix = Botix(controller=con)
-botix.token_pool.append(transition_start_a)
-botix.token_pool.append(transition_ab)
-botix.token_pool.append(transition_bc)
-
-# not compile the code into closure, just return the code lines and context, which is human-readable.
-function_closure: Callable[[], None] = botix.compile(return_median=False)
-
-print(function_closure)
-```
-
-By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
-
-```
-< function _func at 0x0000020D40EAECA0 >
-```
-
-Usage is as follows
-
-```python
-# call the closure, which will execute the compiled code
-function_closure()
-```
-
-Of course, you can also build a closure with branching logic in it.
-
-```python
-from mentabotix import MovingState, MovingTransition, Botix
-from bdmc import CloseLoopController, MotorInfo
-import random
-from typing import List, Tuple, Dict, Any, Callable
-
-controller: CloseLoopController = CloseLoopController(
-    motor_infos=[MotorInfo(code_sign=3, direction=1),
-                 MotorInfo(code_sign=1, direction=1),
-                 MotorInfo(code_sign=2, direction=-1),
-                 MotorInfo(code_sign=4, direction=-1)], port="COM3"
-)
-
-botix = Botix(controller=controller)
-state_a = MovingState(100)
-state_b = MovingState(200)
-state_c = MovingState(300)
-state_d = MovingState(400)
-state_e = MovingState(500)
-state_f = MovingState(600)
-
-
-def transition_breaker_fac(lst: List[int]):  # a simple tool function to create the breaker
-    def _inner() -> int:
-        return random.choice(lst)
-
-    return _inner
-
-
-transition_a_bcd = MovingTransition(
-    duration=1,
-    from_states=state_a,
-    to_states={0: state_b, 1: state_c, 2: state_d},
-    breaker=transition_breaker_fac([0, 1, 2]),
-)
-transition_d_ef = MovingTransition(
-    duration=1,
-    from_states=state_d,
-    to_states={2: state_e, 1: state_f},
-    breaker=transition_breaker_fac([0, 1]),
-)
-
-botix.token_pool.extend([transition_a_bcd, transition_d_ef])
-
-compiled: Tuple[List[str], Dict[str, Any]] = botix.compile(
-    return_median=True)  # not compile the code into closure, just return the code lines and context, which is human readable.
-assert (
-    [
-        "def _func():",
-        "    match con.set_motors_speed((100, 100, 100, 100)).delay_b_match(1,transition0_breaker_1,0.01):",
-        "        case 0:",
-        "            con.set_motors_speed((200, 200, 200, 200))",
-        "        case 1:",
-        "            con.set_motors_speed((300, 300, 300, 300))",
-        "        case 2:",
-        "            match con.set_motors_speed((400, 400, 400, 400)).delay_b_match(1,transition1_breaker_1,0.01):",
-        "                case 0:",
-        "                    con.set_motors_speed((500, 500, 500, 500))",
-        "                case 1:",
-        "                    con.set_motors_speed((600, 600, 600, 600))",
-    ] == compiled[0],
-)
-
-# compile to closure
-compiled_closure: Callable[[], None] = botix.compile(return_median=False)
-
-# call the closure, which will execute the compiled code
-compiled_closure()
-
-
-
-```
-
-### Schema Visualization
-
-Botix support schema visualization with `export_structure` method, which write Puml source code to a file.
-
-```python
-from mentabotix import MovingState, MovingTransition, Botix
-from bdmc import CloseLoopController, MotorInfo
-from typing import List
-import random
-
-# init the state-transition schema
-state_a = MovingState(100)
-state_b = MovingState(200)
-state_c = MovingState(300)
-state_d = MovingState(400)
-state_e = MovingState(500)
-state_f = MovingState(600)
-
-
-def transition_breaker_fac(lst: List[int]):
-    def _inner() -> int:
-        return random.choice(lst)
-
-    return _inner
-
-
-transition_a_bcd = MovingTransition(
-    duration=1,
-    from_states=state_a,
-    to_states={1: state_b, 2: state_c, 3: state_d},
-    breaker=transition_breaker_fac([1, 2, 3]),
-)
-transition_d_ef = MovingTransition(
-    duration=1,
-    from_states=state_d,
-    to_states={1: state_e, 2: state_f},
-    breaker=transition_breaker_fac([1, 2]),
-)
-
-# make the botix object
-botix = Botix(controller=CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)], port="COM3"))
-
-# add the transition
-botix.token_pool.extend([transition_a_bcd, transition_d_ef])
-
-# export the structure
-botix.export_structure("schema.puml")
-```
-
-The result will be written to `schema.puml` and below is the expected Puml source code.
-
-```plantuml
-@startuml
-state "5-MovingState(600, 600, 600, 600)" as state_6
-state "4-MovingState(500, 500, 500, 500)" as state_5
-state break_2 <<choice>>
-note right of break_2: _inner() -> int
-state "3-MovingState(400, 400, 400, 400)" as state_4
-state "2-MovingState(300, 300, 300, 300)" as state_3
-state "1-MovingState(200, 200, 200, 200)" as state_2
-state break_1 <<choice>>
-note right of break_1: _inner() -> int
-state "0-MovingState(100, 100, 100, 100)" as state_1
-state_1 --> break_1
-break_1 --> state_2: 1
-break_1 --> state_3: 2
-break_1 --> state_4: 3
-state_4 --> break_2
-break_2 --> state_5: 1
-break_2 --> state_6: 2
-
-[*] --> state_1
-
-state_2 --> [*]
-state_3 --> [*]
-state_5 --> [*]
-state_6 --> [*]
-
-@enduml
-
-```
-
-Below is the expected render result:
-
-![image](docs/assets/state.png)
-
-### Use State-Transition Composer
-
-State-Transition Composer is a tool that helps you to design and compile state-transition control schema.
-
-```python
-from mentabotix import MovingChainComposer, MovingState, MovingTransition, Botix
-from bdmc import CloseLoopController, MotorInfo
-
-# init the state-transition composer
-comp = MovingChainComposer()
-
-# add some states and transitions one by one to the composer, the composer will auto-connect the states and transitions
-(comp
- .add(MovingState(0))
- .add(MovingTransition(0.2))
- .add(MovingState(1000))
- .add(MovingTransition(0.3))
- .add(MovingState(2000)))
-
-# export the structure
-states, transitions = comp.export_structure()
-
-# let's use botix to make the visualization!
-# first make the botix object
-con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
-botix = Botix(controller=con)
-
-# make the visualization
-botix.export_structure("composed.puml", transitions=transitions)
-```
-
-The exported structure will be written to `composed.puml`, and below is the expected Puml source code.
-
-```plantuml
-@startuml
-state "3-MovingState(2000, 2000, 2000, 2000)" as state_3
-state "2-MovingState(1000, 1000, 1000, 1000)" as state_2
-state "1-MovingState(0, 0, 0, 0)" as state_1
-state_1 --> state_2
-state_2 --> state_3
-
-[*] --> state_1
-
-state_3 --> [*]
-
-@enduml
-```
-
-The render result is shown below:
-
-![image](docs/assets/composed.png)
-
-## Logging
-
-use `set_log_level` to silent the console to improve the performance in high pressure conditions
-
-```python
-from mentabotix import set_log_level
-
-"""
-Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
-Logging INFO - Information message, used to inform the general program running status, with a value of 20.
-Logging WARN - A warning message indicating that there may be a problem but the program is still running, with a value of 30.
-Logging Error - Error message indicating an issue preventing the program from executing properly, with a value of 40.
-Logging CRITICAL - Fatal error message indicating a serious system failure with a value of 50.
-"""
-
-set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
-
-from logging import CRITICAL
-
-set_log_level(CRITICAL)  # this has the same effect as above
-```
+# mentabotix
+
+> A dedicated lib to control 4-fixed-wheels robot
+---
+
+## Installation
+
+Use `pdm` to install mentabotix
+
+```shell
+# install pdm
+python -m pip install pdm
+
+# config pdm
+pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
+
+# for stable release
+pdm add mentabotix
+
+# for unstable release
+pdm add mentabotix --pre
+
+```
+
+## Usage
+
+### Menta
+
+You can use `Menta` to create the judge function closure of the robot, using the sensor data as the input.
+
+#### Step 1: Define Sampler Functions
+
+Firstly, you need to define sampler functions that adhere to the specifications outlined by the `Menta` class. These
+could include sequence samplers that return a series of data points, index samplers that provide data at a specific
+index, and direct response samplers that give an immediate value.
+
+|               Sampler                |                 Description                  |                    Type                    |
+|:------------------------------------:|:--------------------------------------------:|:------------------------------------------:|
+| `mentabotix.SamplerType.SEQ_SAMPLER` | The sensor data is returned in a `Sequence`. | `Callable[[], Sequence[Union[float,int]]]` |
+| `mentabotix.SamplerType.IDX_SAMPLER` |         Use a index to get the data.         |    `Callable[[int], Union[float,int]]`     |
+| `mentabotix.SamplerType.DRC_SAMPLER` |  Direct read sensor data without any args.   |      `Callable[[], Union[float,int]]`      |
+
+> Do remember to add return type annotations to your sampler functions, which will be used to classify the samplers into
+> their respective types in the `Menta` class.
+
+```python
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+```
+
+#### Step 2: Initialize Menta Instance and Add Samplers
+
+After defining the sampler functions, initialize the `Menta` instance and add these samplers to it.
+
+```python
+from mentabotix import Menta  # Ensure to import the correct Menta class
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+```
+
+#### Step 3: Update Sampler Types
+
+Invoke the `update_sampler_types` method to automatically classify the samplers into their respective types.
+
+```python
+from mentabotix import Menta  # Ensure to import the correct Menta class
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+menta_instance.update_sampler_types()
+```
+
+#### Step 4: Construct Judge Function
+
+To use the samplers in a meaningful way, you can construct an updater function that encapsulates a condition based on
+which system updates might occur. For example:
+
+```python
+from mentabotix import SamplerUsage, Menta
+
+
+def temperature_sequence_sampler() -> list[float]:
+    """Simulates a sequence of temperature readings."""
+    return [25.5, 26.0, 25.8]
+
+
+def humidity_index_sampler(index: int) -> float:
+    """Returns simulated humidity data at a given index."""
+    humidity_values = [45.0, 50.0, 55.0]
+    return humidity_values[index]
+
+
+def light_direct_sampler() -> float:
+    """Provides the current light intensity reading."""
+    return 750.0
+
+
+menta_instance = Menta()
+menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+
+menta_instance.update_sampler_types()
+
+# Define how samplers will be used
+usages = [
+
+    # Use sequence sampler for first and third temp data
+    SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
+    # Use index sampler for the first humidity value
+    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),
+]
+
+# Note: the judge source has some built-in syntaxes.Currently, sensor data indexes flattening and extra data context insertion
+# s0 stands for the data at index 0 of the first sampler
+# s1 stands for the data at index 2 of the first sampler
+# s3 stands for the data at index 1 of the second sampler
+
+judging_source = "(s0 > 25 and s1 < 50) or s3>baseline"
+
+# Extra context for the judge function, here only contains the "baseline"
+extra_context = {"baseline": 47}
+
+from typing import Callable
+
+# Construct the judge function object
+updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
+                                                                               extra_context=extra_context)
+
+# Use the judge function to update the system
+updater_function()
+
+
+# Below is the equivalent implementation of the judge function, but is defined manually. 
+# It acts exactly the same as the `updater_function` above.
+def manual_judge_function() -> bool:
+    """Manually construct the judge function."""
+    seq_temp = temperature_sequence_sampler()
+    return (seq_temp[0] > 25 and seq_temp[2] < 50) or humidity_index_sampler(0) > 47
+```
+
+In this case, a judge function closure is created using `exec()` method.Normally the built should have a better
+performance since the all the calls and variables are inlined and stored in the closure.
+---
+
+## Botix
+
+Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
+walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
+schemas into executable closures using the Botix framework.
+
+### Understanding State-Transition Control Schema
+
+Let's start with the fundamental schema rules:
+> - A `MovingState` **MUST** connect exactly **ONE** `MovingTransition` as its input state.
+>- A `MovingTransition` **MUST** have at least **ONE** `MovingState` as either input or output.
+>- A State-Transition Control Schema **MUST** have **EXACTLY ONE** `MovingState` as its initial state and **AT LEAST ONE
+   ** `MovingState` as its final state.
+>- A State-Transition Control Schema **MUST NOT** have any loop, a correct control schema should always be a tree graph.
+
+Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
+robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
+these states are triggered by events or conditions, forming a **control schema**.
+
+#### States
+
+- In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
+  motor speeds or changing direction.
+- A state describe the robot's **moving behavior**, 4 motor speeds in this case
+
+#### Transitions
+
+- Transitions between states are handled by the `MovingTransition` class. They define how and when the robot moves from
+  one state to another, possibly based on sensor inputs or internal conditions.
+- Transitions describe how the robot **moves** from one state to another
+
+### Building Your Control Schema
+
+#### Step 1: Define States
+
+For each distinct behavior, create a `MovingState` instance. Include the actions or configurations that should occur in
+that state. For instance, creating a state for moving forward might look like this:
+
+```python
+from mentabotix import MovingState
+
+# the most basic syntax to control the robot advance in a straight line with speed of 10
+# speed of all motors is 10
+moving_forward = MovingState(10)
+# Speeds for left and right motors are 10
+moving_forward = MovingState(10, 10)
+# Speeds for, in order, front_left, rear_left, rear_right, front_right motors are 10
+moving_forward = MovingState(10, 10, 10, 10)
+
+# Use assistant method to create the state instance
+moving_forward = MovingState.straight(10)
+moving_backward = MovingState.straight(-10)
+
+turn_left = MovingState.turn("l", 10)
+turn_right = MovingState.turn("r", 10)
+
+diff_move_left = MovingState.differential("l", radius=20, outer_speed=70)
+diff_move_right = MovingState.differential("r", radius=20, outer_speed=70)
+
+drift_fl = MovingState.drift("fl", 50)
+drift_rl = MovingState.drift("rl", 50)
+drift_rr = MovingState.drift("rr", 50)
+drift_fr = MovingState.drift("fr", 50)
+
+stopped_state = MovingState.halt()
+
+
+
+
+```
+
+#### Step 2: Define Transitions
+
+Transitions are created with `MovingTransition`. Specify the duration, any conditions under which the transition should
+occur (using a breaker function), and the source and destination states.
+
+```python
+from mentabotix import MovingTransition, MovingState
+from random import random
+
+sensor_reading = lambda: random()  # Example sensor reading function
+threshold = 0.6
+
+
+def stop_condition() -> bool:  # the return type must be annotated, since an exception will be raised otherwise
+    return sensor_reading() < threshold
+
+
+moving_forward = MovingState(10)
+stopped_state = MovingState(0)
+
+transition_forward_to_stop = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=stop_condition,  # When to break the transition
+    from_states=moving_forward,
+    to_states=stopped_state,
+)
+# Such transition indicate the bot will move forward for 2 seconds OR stop when the sensor reading is below 25.0 
+
+```
+
+But some time you might want to create a transition that branches out to other states. For example, if the robot needs
+to move forward and then turn left. This can be done by creating a `MovingTransition` like this:
+
+```python
+from mentabotix import MovingTransition, MovingState
+from random import choice
+
+
+def stop_condition() -> int:  # return type must be annotated
+    return choice([0, 1, 2])
+
+
+moving_left = MovingState.turn("l", 10)
+moving_right = MovingState.turn("r", 10)
+moving_dash = MovingState.straight(100)
+stopped_state = MovingState(0)
+
+transition_forward_to_stop = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=stop_condition,  # When to break the transition
+    from_states=stopped_state,
+    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
+)
+
+# Such transition indicate the bot will stop for 2 seconds and then dash forward if nothing happens. ( means the top_condition never return a Non-Zero value)
+
+# If the stop_condition do return a Non-Zero value, 
+# the 2-seconds stop will be broken and the bot will either turn left or right according to the value returned by the stop_condition. (means if the value is 1, it will turn left, if the value is 2, it will turn right)
+
+```
+
+#### Step 3: Connect States with Transitions
+
+Create a collection of your states and transitions, ensuring each transition correctly references its source and target
+states.
+
+A legal control schema should have a start state and at least one end state.
+And each state can **ONLY** connect to **ONE** transition as its input state
+
+```python
+from mentabotix import MovingState, MovingTransition
+import random
+
+moving_left = MovingState.turn("l", 10)
+moving_right = MovingState.turn("r", 10)
+moving_dash = MovingState.straight(100)
+stopped_state = MovingState(0)
+
+start_state = MovingState(100)
+
+
+def _breaker_1() -> int:
+    return random.choice([0, 1, 2])
+
+
+def _breaker_2() -> int:
+    return random.choice([0, 1])
+
+
+transition_1 = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=_breaker_1,  # When to break the transition
+    from_states=stopped_state,
+    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
+)
+
+transition_2 = MovingTransition(
+    duration=2,  # Duration to transition
+    breaker=_breaker_2,  # When to break the transition
+    from_states=stopped_state,
+    to_states={0: moving_dash, 1: stopped_state},
+)
+
+
+```
+
+As the above example, `transition_1` and `transition_2` both have the `stopped_state` as the input state,which means
+the `stopped_state` connects more than **ONE** transition. Definition as such is illegal and will not pass the compile
+stage.
+
+Normally, you can ensure that the structure is valid by using `ensure_structure_validity`. to eliminate this problem.
+
+```python
+from mentabotix import Botix
+
+# A StructuralError will be raised if the structure is not valid
+Botix.ensure_structure_validity([transition_1, transition_2])
+```
+
+### Compiling to Closures with Botix
+
+Once your control schema is defined, Botix can help you compile this structure into executable code, often referred to
+as closures, which can directly control the robot's behavior.
+
+#### Step 4: Compile the Schema
+
+Botix provides methods to compile your states and transitions into a Match-Case-Structured Closure.
+
+```python
+from mentabotix import MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+
+con: CloseLoopController = CloseLoopController(motor_infos=[MotorInfo(code_sign=3, direction=1),
+                                                            MotorInfo(code_sign=1, direction=1),
+                                                            MotorInfo(code_sign=2, direction=-1),
+                                                            MotorInfo(code_sign=4, direction=-1)], port="COM3")
+
+start_state = MovingState(-1)
+state_a = MovingState(0)
+state_b = MovingState(1)
+state_c = MovingState(2)
+# 创建一些假的MovingTransition对象用于测试
+transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
+transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
+transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
+
+botix = Botix(controller=con)
+botix.token_pool.append(transition_start_a)
+botix.token_pool.append(transition_ab)
+botix.token_pool.append(transition_bc)
+
+# not compile the code into closure, just return the code lines and context, which is human readable.
+compiled_code_lines, variables_context = botix.compile(return_median=True)
+
+print(compiled_code_lines)
+
+
+```
+
+By printing out the `compiled_code_lines` list, you can see the code lines that are generated by Botix.
+
+```python
+[
+    "def _func():",
+    "    con.set_motors_speed((-1, -1, -1, -1)).delay(0.1).set_motors_speed((0, 0, 0, 0)).delay(1).set_motors_speed((1, 1, 1, 1)).delay(2).set_motors_speed((2, 2, 2, 2))",
+]
+
+```
+
+But usually, you want to compile the code into a closure that can be used to control the robot with higher performance
+and less human error.
+
+```python
+from mentabotix import MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+from typing import Callable
+
+con: CloseLoopController = CloseLoopController(motor_infos=[MotorInfo(code_sign=3, direction=1),
+                                                            MotorInfo(code_sign=1, direction=1),
+                                                            MotorInfo(code_sign=2, direction=-1),
+                                                            MotorInfo(code_sign=4, direction=-1)], port="COM3")
+
+start_state = MovingState(-1)
+state_a = MovingState(0)
+state_b = MovingState(1)
+state_c = MovingState(2)
+# create some transitions
+transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
+transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
+transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
+
+botix = Botix(controller=con)
+botix.token_pool.append(transition_start_a)
+botix.token_pool.append(transition_ab)
+botix.token_pool.append(transition_bc)
+
+# not compile the code into closure, just return the code lines and context, which is human-readable.
+function_closure: Callable[[], None] = botix.compile(return_median=False)
+
+print(function_closure)
+```
+
+By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
+
+```
+< function _func at 0x0000020D40EAECA0 >
+```
+
+Usage is as follows
+
+```python
+# call the closure, which will execute the compiled code
+function_closure()
+```
+
+Of course, you can also build a closure with branching logic in it.
+
+```python
+from mentabotix import MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+import random
+from typing import List, Tuple, Dict, Any, Callable
+
+controller: CloseLoopController = CloseLoopController(
+    motor_infos=[MotorInfo(code_sign=3, direction=1),
+                 MotorInfo(code_sign=1, direction=1),
+                 MotorInfo(code_sign=2, direction=-1),
+                 MotorInfo(code_sign=4, direction=-1)], port="COM3"
+)
+
+botix = Botix(controller=controller)
+state_a = MovingState(100)
+state_b = MovingState(200)
+state_c = MovingState(300)
+state_d = MovingState(400)
+state_e = MovingState(500)
+state_f = MovingState(600)
+
+
+def transition_breaker_fac(lst: List[int]):  # a simple tool function to create the breaker
+    def _inner() -> int:
+        return random.choice(lst)
+
+    return _inner
+
+
+transition_a_bcd = MovingTransition(
+    duration=1,
+    from_states=state_a,
+    to_states={0: state_b, 1: state_c, 2: state_d},
+    breaker=transition_breaker_fac([0, 1, 2]),
+)
+transition_d_ef = MovingTransition(
+    duration=1,
+    from_states=state_d,
+    to_states={2: state_e, 1: state_f},
+    breaker=transition_breaker_fac([0, 1]),
+)
+
+botix.token_pool.extend([transition_a_bcd, transition_d_ef])
+
+compiled: Tuple[List[str], Dict[str, Any]] = botix.compile(
+    return_median=True)  # not compile the code into closure, just return the code lines and context, which is human readable.
+assert (
+    [
+        "def _func():",
+        "    match con.set_motors_speed((100, 100, 100, 100)).delay_b_match(1,transition0_breaker_1,0.01):",
+        "        case 0:",
+        "            con.set_motors_speed((200, 200, 200, 200))",
+        "        case 1:",
+        "            con.set_motors_speed((300, 300, 300, 300))",
+        "        case 2:",
+        "            match con.set_motors_speed((400, 400, 400, 400)).delay_b_match(1,transition1_breaker_1,0.01):",
+        "                case 0:",
+        "                    con.set_motors_speed((500, 500, 500, 500))",
+        "                case 1:",
+        "                    con.set_motors_speed((600, 600, 600, 600))",
+    ] == compiled[0],
+)
+
+# compile to closure
+compiled_closure: Callable[[], None] = botix.compile(return_median=False)
+
+# call the closure, which will execute the compiled code
+compiled_closure()
+
+
+
+```
+
+### Schema Visualization
+
+Botix support schema visualization with `export_structure` method, which write Puml source code to a file.
+
+```python
+from mentabotix import MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+from typing import List
+import random
+
+# init the state-transition schema
+state_a = MovingState(100)
+state_b = MovingState(200)
+state_c = MovingState(300)
+state_d = MovingState(400)
+state_e = MovingState(500)
+state_f = MovingState(600)
+
+
+def transition_breaker_fac(lst: List[int]):
+    def _inner() -> int:
+        return random.choice(lst)
+
+    return _inner
+
+
+transition_a_bcd = MovingTransition(
+    duration=1,
+    from_states=state_a,
+    to_states={1: state_b, 2: state_c, 3: state_d},
+    breaker=transition_breaker_fac([1, 2, 3]),
+)
+transition_d_ef = MovingTransition(
+    duration=1,
+    from_states=state_d,
+    to_states={1: state_e, 2: state_f},
+    breaker=transition_breaker_fac([1, 2]),
+)
+
+# make the botix object
+botix = Botix(controller=CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)], port="COM3"))
+
+# add the transition
+botix.token_pool.extend([transition_a_bcd, transition_d_ef])
+
+# export the structure
+botix.export_structure("schema.puml")
+```
+
+The result will be written to `schema.puml` and below is the expected Puml source code.
+
+```plantuml
+@startuml
+state "5-MovingState(600, 600, 600, 600)" as state_6
+state "4-MovingState(500, 500, 500, 500)" as state_5
+state break_2 <<choice>>
+note right of break_2: _inner() -> int
+state "3-MovingState(400, 400, 400, 400)" as state_4
+state "2-MovingState(300, 300, 300, 300)" as state_3
+state "1-MovingState(200, 200, 200, 200)" as state_2
+state break_1 <<choice>>
+note right of break_1: _inner() -> int
+state "0-MovingState(100, 100, 100, 100)" as state_1
+state_1 --> break_1
+break_1 --> state_2: 1
+break_1 --> state_3: 2
+break_1 --> state_4: 3
+state_4 --> break_2
+break_2 --> state_5: 1
+break_2 --> state_6: 2
+
+[*] --> state_1
+
+state_2 --> [*]
+state_3 --> [*]
+state_5 --> [*]
+state_6 --> [*]
+
+@enduml
+
+```
+
+Below is the expected render result:
+
+![image](docs/assets/state.png)
+
+### Use State-Transition Composer
+
+State-Transition Composer is a tool that helps you to design and compile state-transition control schema.
+
+```python
+from mentabotix import MovingChainComposer, MovingState, MovingTransition, Botix
+from bdmc import CloseLoopController, MotorInfo
+
+# init the state-transition composer
+comp = MovingChainComposer()
+
+# add some states and transitions one by one to the composer, the composer will auto-connect the states and transitions
+(comp
+ .add(MovingState(0))
+ .add(MovingTransition(0.2))
+ .add(MovingState(1000))
+ .add(MovingTransition(0.3))
+ .add(MovingState(2000)))
+
+# export the structure
+states, transitions = comp.export_structure()
+
+# let's use botix to make the visualization!
+# first make the botix object
+con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
+botix = Botix(controller=con)
+
+# make the visualization
+botix.export_structure("composed.puml", transitions=transitions)
+```
+
+The exported structure will be written to `composed.puml`, and below is the expected Puml source code.
+
+```plantuml
+@startuml
+state "3-MovingState(2000, 2000, 2000, 2000)" as state_3
+state "2-MovingState(1000, 1000, 1000, 1000)" as state_2
+state "1-MovingState(0, 0, 0, 0)" as state_1
+state_1 --> state_2
+state_2 --> state_3
+
+[*] --> state_1
+
+state_3 --> [*]
+
+@enduml
+```
+
+The render result is shown below:
+
+![image](docs/assets/composed.png)
+
+## Logging
+
+use `set_log_level` to silent the console to improve the performance in high pressure conditions
+
+```python
+from mentabotix import set_log_level
+
+"""
+Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
+Logging INFO - Information message, used to inform the general program running status, with a value of 20.
+Logging WARN - A warning message indicating that there may be a problem but the program is still running, with a value of 30.
+Logging Error - Error message indicating an issue preventing the program from executing properly, with a value of 40.
+Logging CRITICAL - Fatal error message indicating a serious system failure with a value of 50.
+"""
+
+set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
+
+from logging import CRITICAL
+
+set_log_level(CRITICAL)  # this has the same effect as above
+```
```

