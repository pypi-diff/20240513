# Comparing `tmp/bdmc-0.1.5.tar.gz` & `tmp/bdmc-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.tar", last modified: Fri May 10 15:17:59 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.1.tar", last modified: Mon May 13 08:37:14 2024, max compression
```

## Comparing `bdmc-0.1.5.tar` & `bdmc-0.1.5.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     5615 2024-05-02 00:54:03.168793 bdmc-0.1.5/README.md
--rw-r--r--   0        0        0      545 2024-05-10 15:17:59.850642 bdmc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      575 2024-05-10 13:50:47.522562 bdmc-0.1.5/src/bdmc/__init__.py
--rw-r--r--   0        0        0      436 2024-05-03 08:30:16.300622 bdmc-0.1.5/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    17567 2024-05-10 15:03:44.336123 bdmc-0.1.5/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2339 2024-04-19 15:02:17.856714 bdmc-0.1.5/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      601 2024-04-18 07:29:21.037654 bdmc-0.1.5/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1398 2024-04-17 15:25:57.810945 bdmc-0.1.5/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7622 2024-04-18 07:22:00.698698 bdmc-0.1.5/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      707 2024-04-24 15:25:32.371252 bdmc-0.1.5/tests/find_tests.py
--rw-r--r--   0        0        0     4479 2024-05-10 14:58:28.040552 bdmc-0.1.5/tests/test_context.py
--rw-r--r--   0        0        0     2045 2024-05-10 14:58:04.544953 bdmc-0.1.5/tests/test_controller.py
--rw-r--r--   0        0        0   631171 2024-05-10 15:03:08.468920 bdmc-0.1.5/tests/viz_output/test_send.json
--rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 bdmc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/README.md
+-rw-r--r--   0        0        0      547 2024-05-13 08:37:14.022550 bdmc-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    17112 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-13 08:36:54.362503 bdmc-0.1.5.1/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-13 08:36:54.366503 bdmc-0.1.5.1/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.1/PKG-INFO
```

### Comparing `bdmc-0.1.5/README.md` & `bdmc-0.1.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,149 +1,160 @@
-# bdmc
----
-> This lib is especially designed to control the BDMC drivers, which is under the sales of TechStar.
-
-## TODO
-
-- [x] Basic motor serial controller.
-- [x] Basic Transmitting channel builder.
-- [ ] Fully integrate the standard serial cmds into this lib.
-- [ ] More capable controller implementations that support more complicated control strategies.
-
-## Install
-
-Install use pdm
-
-```shell
-
-# install pdm
-python -m pip install pdm
-
-# config pdm
-pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
-
-# for stable version
-pdm add bdmc 
-
-# for unstable version
-pdm add bdmc -pre
-```
-
-## QuickStart
-
-The minimal example is as below.
-
-```python
-from bdmc import CloseLoopController, MotorInfo, CMD
-
-# Create a MotorInfo Sequence, with 4 motors defined here.
-motor_seq = (MotorInfo(code_sign=1, direction=1),
-             # code_sign is used as unique identifier, while the direction are used as motor rotate direction adjuster
-             MotorInfo(3, 1),
-             MotorInfo(4, -1),
-             MotorInfo(2, -1))
-
-# Define the name of the serial device that will be used to control the motor
-port = "tty0"
-# port="COM3"  on windows, device name differ from that in  the linux
-
-# Create the controller obj, with starting the msg sending thread and send a broadcast RESET cmd to init the motors being controlled
-con = (CloseLoopController(motor_infos=motor_seq, port=port)
-       .start_msg_sending()
-       .send_cmd(CMD.RESET))
-
-# Use the set_motors_speed method, to set all 4 motors speed.
-# In this case,motor_1 receives 100*direction, motor_3 receive 200*direction,and so on. 
-# NOTE1: the speed used here will multiply the motor's direction accordingly.
-# NOTE2: the speed sequence MUST have the same length as the motor_seq, a ValueException will be raised otherwise.
-con.set_motors_speed([100, 200, 300, 400])
-
-# Supports chain calls
-# In this case, these 3 cmds will be sent to the motors at almost the same time, only the [0]*4 will take effect as a result
-(con
- .set_motors_speed([100, 200, 300, 400])
- .set_motors_speed([1000] * 4)  # move all 4 motors with the speed of 1000
- .set_motors_speed([0] * 4))
-
-# Chain call with delay
-# In this case, these 3 cmds will be sent to motors with the specified interval
-(con
- .set_motors_speed([100, 200, 300, 400])
- .delay(1.2)  # delay 1.2 sec
- .set_motors_speed([1000] * 4)
- .delay(3)  # delay 3.0 sec
- .set_motors_speed([0] * 4))
-
-# Chain call with delay_b
-# In this case, these 3 cmds will be sent to motors with specified interval,but with a break checker
-# NOTE1: you can't set check_interval bigger than delay_sec
-from random import random
-
-(con
- .set_motors_speed([100, 200, 300, 400])
- .delay_b(delay_sec=1.2, breaker=lambda: random() > 0.8,
-          check_interval=0.01)  # delay 1.2 sec, will skip the 1.2 sec on the breaker returns True, execute the checker every 0.01 sec
- .set_motors_speed([1000] * 4)
- .delay_b(3, breaker=lambda: random() > 0.5,
-          check_interval=0.02)  # delay 3.0 sec, will skip the 1.2 sec on the breaker returns True, execute the checker every 0.02 sec
- .set_motors_speed([0] * 4))
-
-# Branched chain call with delay_b_match
-# In this case, a switch-case branch has been enforced.
-# Once the breaker returns a True during the 1.2 sec delay, a FULL_STOP cmd will be sent.
-# if the breaker never return a True, then the 1.2sec delay will be fully waited and the [500]*4 cmd will be sent.
-
-# NOTE1: delay_b_match has same delay logic as delay_b, the only difference is the return value:
-# delay_b       returns Self
-# delay_b_match returns breaker()
-
-
-match (con
-       .set_motors_speed([100] * 4)
-       .delay_b_match(1.2, breaker=lambda: random() > 0.8)):
-    case True:
-        con.send_cmd(CMD.FULL_STOP)
-    case False:
-        con.set_motors_speed([500] * 4)
-    case _:
-        raise ValueError("should never be here")
-
-# A more complex usage of delay_b_match
-# Note
-from random import choice
-
-match (con
-       .set_motors_speed([100] * 4)
-       .delay_b_match(1.2, breaker=lambda: choice([0, 0, 1, 2, 3]), check_interval=0.1)):
-    case 1:
-        con.send_cmd(CMD.FULL_STOP)  # Switch to this case once the breaker returns 1
-    case 2:
-        con.set_motors_speed([666] * 4)  # Switch to this case once the breaker returns 2
-    case 3:
-        con.set_motors_speed([777] * 4)  # Switch to this case once the breaker returns 3
-    case 0:
-        con.set_motors_speed([555] * 4)  # Switch to this case if the breaker has never returned a non-zero value
-    case _:
-        raise ValueError("should never be here")
-
-
-```
-
-use `set_log_level` to silent the console to improve the performance in high pressure conditions
-
-```python
-from bdmc import set_log_level
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
+Metadata-Version: 2.1
+Name: bdmc
+Version: 0.1.5.1
+Summary: An api wrapper lib designed for the uptech BDMC divers
+Author-Email: Whth <88489697+Whth@users.noreply.github.com>
+License: MIT
+Requires-Python: >=3.11
+Requires-Dist: pyserial>=3.5
+Requires-Dist: coloredlogs>=15.0.1
+Description-Content-Type: text/markdown
+
+# bdmc
+---
+> This lib is especially designed to control the BDMC drivers, which is under the sales of TechStar.
+
+## TODO
+
+- [x] Basic motor serial controller.
+- [x] Basic Transmitting channel builder.
+- [ ] Fully integrate the standard serial cmds into this lib.
+- [ ] More capable controller implementations that support more complicated control strategies.
+
+## Install
+
+Install use pdm
+
+```shell
+
+# install pdm
+python -m pip install pdm
+
+# config pdm
+pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
+
+# for stable version
+pdm add bdmc 
+
+# for unstable version
+pdm add bdmc -pre
+```
+
+## QuickStart
+
+The minimal example is as below.
+
+```python
+from bdmc import CloseLoopController, MotorInfo, CMD
+
+# Create a MotorInfo Sequence, with 4 motors defined here.
+motor_seq = (MotorInfo(code_sign=1, direction=1),
+             # code_sign is used as unique identifier, while the direction are used as motor rotate direction adjuster
+             MotorInfo(3, 1),
+             MotorInfo(4, -1),
+             MotorInfo(2, -1))
+
+# Define the name of the serial device that will be used to control the motor
+port = "tty0"
+# port="COM3"  on windows, device name differ from that in  the linux
+
+# Create the controller obj, with starting the msg sending thread and send a broadcast RESET cmd to init the motors being controlled
+con = (CloseLoopController(motor_infos=motor_seq, port=port)
+       .start_msg_sending()
+       .send_cmd(CMD.RESET))
+
+# Use the set_motors_speed method, to set all 4 motors speed.
+# In this case,motor_1 receives 100*direction, motor_3 receive 200*direction,and so on. 
+# NOTE1: the speed used here will multiply the motor's direction accordingly.
+# NOTE2: the speed sequence MUST have the same length as the motor_seq, a ValueException will be raised otherwise.
+con.set_motors_speed([100, 200, 300, 400])
+
+# Supports chain calls
+# In this case, these 3 cmds will be sent to the motors at almost the same time, only the [0]*4 will take effect as a result
+(con
+ .set_motors_speed([100, 200, 300, 400])
+ .set_motors_speed([1000] * 4)  # move all 4 motors with the speed of 1000
+ .set_motors_speed([0] * 4))
+
+# Chain call with delay
+# In this case, these 3 cmds will be sent to motors with the specified interval
+(con
+ .set_motors_speed([100, 200, 300, 400])
+ .delay(1.2)  # delay 1.2 sec
+ .set_motors_speed([1000] * 4)
+ .delay(3)  # delay 3.0 sec
+ .set_motors_speed([0] * 4))
+
+# Chain call with delay_b
+# In this case, these 3 cmds will be sent to motors with specified interval,but with a break checker
+# NOTE1: you can't set check_interval bigger than delay_sec
+from random import random
+
+(con
+ .set_motors_speed([100, 200, 300, 400])
+ .delay_b(delay_sec=1.2, breaker=lambda: random() > 0.8,
+          check_interval=0.01)  # delay 1.2 sec, will skip the 1.2 sec on the breaker returns True, execute the checker every 0.01 sec
+ .set_motors_speed([1000] * 4)
+ .delay_b(3, breaker=lambda: random() > 0.5,
+          check_interval=0.02)  # delay 3.0 sec, will skip the 1.2 sec on the breaker returns True, execute the checker every 0.02 sec
+ .set_motors_speed([0] * 4))
+
+# Branched chain call with delay_b_match
+# In this case, a switch-case branch has been enforced.
+# Once the breaker returns a True during the 1.2 sec delay, a FULL_STOP cmd will be sent.
+# if the breaker never return a True, then the 1.2sec delay will be fully waited and the [500]*4 cmd will be sent.
+
+# NOTE1: delay_b_match has same delay logic as delay_b, the only difference is the return value:
+# delay_b       returns Self
+# delay_b_match returns breaker()
+
+
+match (con
+       .set_motors_speed([100] * 4)
+       .delay_b_match(1.2, breaker=lambda: random() > 0.8)):
+    case True:
+        con.send_cmd(CMD.FULL_STOP)
+    case False:
+        con.set_motors_speed([500] * 4)
+    case _:
+        raise ValueError("should never be here")
+
+# A more complex usage of delay_b_match
+# Note
+from random import choice
+
+match (con
+       .set_motors_speed([100] * 4)
+       .delay_b_match(1.2, breaker=lambda: choice([0, 0, 1, 2, 3]), check_interval=0.1)):
+    case 1:
+        con.send_cmd(CMD.FULL_STOP)  # Switch to this case once the breaker returns 1
+    case 2:
+        con.set_motors_speed([666] * 4)  # Switch to this case once the breaker returns 2
+    case 3:
+        con.set_motors_speed([777] * 4)  # Switch to this case once the breaker returns 3
+    case 0:
+        con.set_motors_speed([555] * 4)  # Switch to this case if the breaker has never returned a non-zero value
+    case _:
+        raise ValueError("should never be here")
+
+
+```
+
+use `set_log_level` to silent the console to improve the performance in high pressure conditions
+
+```python
+from bdmc import set_log_level
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

### Comparing `bdmc-0.1.5/pyproject.toml` & `bdmc-0.1.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5"
+version = "0.1.5.1"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5/src/bdmc/modules/controller.py` & `bdmc-0.1.5.1/src/bdmc/modules/controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,431 +1,430 @@
-from queue import Queue
-from threading import Thread
-from time import sleep, time
-from typing import (
-    List,
-    Optional,
-    ByteString,
-    Literal,
-    TypeAlias,
-    Sequence,
-    Self,
-    Callable,
-    Any,
-    TypeVar,
-    Hashable,
-    Dict,
-    Tuple,
-)
-
-from bdmc.modules.cmd import CMD
-from bdmc.modules.logger import _logger
-from bdmc.modules.seriald import SerialClient
-
-DIRECTION: TypeAlias = Literal[1, -1]
-GT = TypeVar("GT", bound=Hashable)
-
-
-class MotorInfo:
-    """
-    A class representing a motor's ID and direction.
-    """
-
-    def __init__(self, code_sign: int, direction: DIRECTION = 1):
-        self.code_sign = code_sign
-        self.direction = direction
-
-    def __eq__(self, other) -> bool:
-        return self.code_sign == other.code_sign
-
-    def __hash__(self) -> int:
-        return hash(self.code_sign)
-
-
-ClassicMIs: Tuple[MotorInfo, MotorInfo, MotorInfo, MotorInfo] = (MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4))
-
-
-class CloseLoopController:
-    """
-    CloseLoopController is a class designed to manage and control a system involving multiple motors with closed-loop feedback.
-    It provides methods for setting motor speeds, sending commands, introducing delays with breakers, and updating a shared context.
-    The controller maintains a connection to a serial client for communication with the hardware, manages a command queue,
-    and runs a dedicated thread for message sending. It also allows registering context updaters and getters to facilitate data flow within the application.
-
-    Key features and functionality include:
-
-    1. **Initialization**:
-       - Accepts a list of `MotorInfo` objects, specifying motor IDs and directions, and an optional serial port for communication.
-       - Initializes a `SerialClient` for interfacing with the hardware, a command queue, and a flag for controlling the message sending thread.
-
-    2. **Context Management**:
-       - Maintains a dictionary (`_context`) to store shared data across the application.
-       - Provides methods `register_context_updater` and `register_context_getter` to register functions that update or retrieve specific context variables.
-
-    3. **Motor Control**:
-       - `set_motors_speed`: Sets the speed of each motor based on a provided list of speeds, ensuring consistency with the provided `MotorInfo`.
-       - `send_cmd`: Adds a command to the command queue for transmission to the hardware.
-
-    4. **Message Sending**:
-       - Manages a background thread (`_msg_send_thread`) responsible for continuously retrieving messages from the command queue and writing them to the serial channel.
-       - Offers `start_msg_sending` and `stop_msg_sending` methods to control the message sending thread's lifecycle.
-
-    5. **Delay Functions**:
-       - `delay`: Introduces a simple delay for a specified duration in seconds.
-       - `delay_b`: Delays execution for a given time, periodically checking a breaker function that can abort the delay if it returns True.
-       - `delay_b_match`: Similar to `delay_b`, but returns the result of the breaker function once the delay has completed or the breaker condition is met.
-
-    6. **Utility Methods**:
-       - `wait_exec`: Executes a given function and returns the instance of the class itself.
-       - Properties `context`, `motor_ids`, `motor_dirs`, `cmd_queue`, and `serial_client` provide convenient access to internal attributes.
-
-    Overall, the CloseLoopController serves as a central hub for coordinating motor operations, handling communication with the hardware, managing shared data, and introducing controlled delays with breakers in a closed-loop motor control system.
-    """
-
-    def __init__(
-        self,
-        motor_infos: Sequence[MotorInfo] = ClassicMIs,
-        port: Optional[str] = None,
-        context: Optional[Dict[str, Any]] = None,
-    ) -> None:
-        """
-        :param motor_infos: A list of MotorInfo objects containing motor ID and direction.
-        """
-        if len(motor_infos) != len(set(motor_infos)):
-            raise ValueError("Motor infos must be unique.")
-
-        self._serial: SerialClient = SerialClient(port=port)
-        self._motor_infos: Sequence[MotorInfo] = motor_infos
-        self._cmd_queue: Queue[ByteString] = Queue()
-        self._msg_send_thread: Optional[Thread] = None
-        self._msg_send_thread_should_run: bool = True
-        self._context: Dict[str, Any] = context or {}
-
-    def register_context_updater(
-        self, function: Callable[..., Any], input_keys: List[str], output_keys: List[str], freeze_inputs: bool = False
-    ) -> Callable[[], None]:
-        """
-        Registers a context updater function that updates the context with the specified input and output keys.
-
-        Args:
-            function (Callable[..., Any]): The function to register as a context updater.
-            input_keys (List[str]): The list of input keys to use for the context updater.
-            output_keys (List[str]): The list of output keys to update in the context.
-            freeze_inputs (bool, optional): Whether to freeze the input data. Defaults to False.
-
-        Returns:
-            Callable[[], None]: The registered context updater function.
-
-        Raises:
-            ValueError: If either input_keys or output_keys is empty.
-            ValueError: If any input variable is not found in the context.
-            ValueError: If invalid arguments are provided.
-        """
-        if input_keys == [] and output_keys == []:
-            raise ValueError("Either input_keys or output_keys must be non-empty.")
-        # 确保输入和输出变量存在于上下文中
-        if not_included := [var for var in input_keys if var not in self._context]:
-            raise ValueError(f"Input variables {not_included} not found in context.")
-
-        context = self._context
-        input_keys = tuple(input_keys)
-        output_keys = tuple(output_keys)
-        frozen_input_data = tuple(context.get(key) for key in input_keys)
-
-        match freeze_inputs, input_keys, output_keys:
-            case _, (), (output_key,):
-
-                def _updater() -> None:
-                    context[output_key] = function()
-
-            case _, (), all_output_keys:
-
-                def _updater() -> None:
-                    for key, val in zip(all_output_keys, function()):
-                        context[key] = val
-
-            case False, (input_key,), ():
-
-                def _updater() -> None:
-                    function(context.get(input_key))
-
-            case True, (input_key,), ():
-                input_data = context.get(input_key)
-
-                def _updater() -> None:
-                    function(input_data)
-
-            case False, all_input_keys, ():
-
-                def _updater() -> None:
-                    function(*(tuple(context.get(key) for key in all_input_keys)))
-
-            case True, all_input_keys, ():
-
-                def _updater() -> None:
-                    function(*frozen_input_data)
-
-            case False, (input_key,), (output_key,):
-
-                def _updater() -> None:
-                    context[output_key] = function(context.get(input_key))
-
-            case True, (input_key,), (output_key,):
-                input_data = context.get(input_key)
-
-                def _updater() -> None:
-                    context[output_key] = function(input_data)
-
-            case False, all_input_keys, all_output_keys:
-
-                def _updater() -> None:
-                    frozen_input_data = tuple(context.get(key) for key in all_input_keys)
-                    for key, output_data in zip(all_output_keys, function(*frozen_input_data)):
-                        context[key] = output_data
-
-            case True, all_input_keys, all_output_keys:
-
-                def _updater() -> None:
-                    for key, output_data in zip(all_output_keys, function(*frozen_input_data)):
-                        context[key] = output_data
-
-            case _:
-                raise ValueError(
-                    f"Invalid arguments for register_context_updater function. got {input_keys} and {output_keys} and {freeze_inputs}"
-                )
-        return _updater
-
-    def register_context_getter(self, var_key: str) -> Callable[[], Any]:
-        """
-        Register a context getter function for a given variable key.
-
-        Args:
-            var_key (str): The key of the variable.
-
-        Returns:
-            Callable[[], Any]: A function that returns the value of the variable.
-        """
-        context = self._context
-        return lambda: context.get(var_key)
-
-    def wait_exec(self, function: Callable[[], None]) -> Self:
-        """
-        Executes the given function and returns the instance of the class itself.
-
-        Parameters:
-            function (Callable[[], None]): The function to be executed.
-
-        Returns:
-            Self: The instance of the class itself.
-        """
-        function()
-        return self
-
-    @property
-    def context(self) -> Dict[str, Any]:
-        """
-        Returns the context dictionary of the object.
-
-        :return: A dictionary containing the context of the object.
-        :rtype: Dict[str, Any]
-        """
-        return self._context
-
-    @property
-    def motor_ids(self) -> List[int]:
-        """
-        A property that returns a list of motor ids from the motor infos.
-        """
-        return [motor_info.code_sign for motor_info in self._motor_infos]
-
-    @property
-    def motor_dirs(self) -> List[DIRECTION]:
-        """
-        Return the list of directions for each motor in the motor_infos.
-        """
-        return [motor_info.direction for motor_info in self._motor_infos]
-
-    @property
-    def cmd_queue(self) -> Queue[ByteString]:
-        """
-        Return the message queue.
-        """
-        return self._cmd_queue
-
-    @property
-    def serial_client(self) -> SerialClient:
-        """
-        A property that returns the serial client.
-        """
-        return self._serial
-
-    def stop_msg_sending(self) -> Self:
-        """
-        Stop the message sending by setting the _msg_send_thread_should_run flag to False and joining the message send thread.
-        """
-        self._msg_send_thread_should_run = False
-        self._msg_send_thread.join()
-        self._msg_send_thread = None
-        return self
-
-    def start_msg_sending(self) -> Self:
-        """
-        A description of the entire function, its parameters, and its return types.
-        """
-
-        _logger.info("MSG sending thread starting")
-        self._msg_send_thread_should_run = True
-        _logger.info(f"MSG sending thread started")
-        self._msg_send_thread = Thread(name="msg_send_thread", target=self._msg_sending_loop)
-        self._msg_send_thread.daemon = True
-        self._msg_send_thread.start()
-        _logger.info("MSG sending thread stopped")
-        return self
-
-    def _msg_sending_loop(self) -> None:
-        """
-        A function that handles the sending of messages in a loop.
-        It continuously retrieves messages from a queue and writes them to a channel until the thread should stop running.
-        Returns None.
-        """
-
-        while self._msg_send_thread_should_run:
-            temp = self._cmd_queue.get()
-            _logger.debug(f"Writing {temp} to channel,remaining {self._cmd_queue.qsize()}")
-            self._serial.write(temp)
-
-    def set_motors_speed(self, speeds: Sequence[int | float]) -> Self:
-        """
-        Set the speed for each motor based on the provided speed_list.
-
-        Parameters:
-            speeds (Sequence[int|float]): A list of speeds for each motor.
-
-        Returns:
-            None
-        """
-
-        if len(speeds) != len(self._motor_infos):
-            raise ValueError("Length of speed_list must be equal to the number of motors")
-        self._cmd_queue.put(
-            (
-                "".join(
-                    f"{motor_info.code_sign}v{int(speed * motor_info.direction)}\r"
-                    for motor_info, speed in zip(self._motor_infos, speeds)
-                )
-            ).encode("ascii")
-        )
-        return self
-
-    def send_cmd(self, cmd: CMD) -> Self:
-        """
-        Add a command to the command queue.
-
-        Args:
-            cmd (CMD): The command to be added to the queue.
-
-        Returns:
-            Self: Returns the instance of the class.
-        """
-        self._cmd_queue.put(cmd.value)
-        return self
-
-    def delay_b(
-        self,
-        delay_sec: float,
-        breaker: Callable[[], Any],
-        check_interval: float = 0.01,
-    ) -> Self:
-        """
-        Delays the execution of the function by a specified amount of time, while checking a breaker function periodically.
-
-        Parameters:
-            delay_sec (float): The amount of time to delay the execution in seconds.
-            breaker (Callable[[], Any]): A function that returns a boolean value indicating whether the delay should be aborted.
-            check_interval (float, optional): The interval in seconds between each check of the breaker function. Defaults to 0.01.
-
-        Returns:
-            Self: The instance of the class itself.
-
-        Raises:
-            ValueError: If the check_interval is not at least twice as large as the delay_sec.
-
-        Notes:
-            - The delay_sec parameter specifies the total amount of time to delay the execution,
-             including the initial delay and the time spent checking the breaker function.
-            - The check_interval parameter specifies the interval in seconds between each check of the breaker function.
-             It should be at least twice as large as the delay_sec parameter to ensure accurate timing.
-            - The breaker function is called periodically to check if the delay should be aborted.
-            If the breaker function returns True, the delay is aborted and the function returns immediately.
-            - If the breaker function returns False, the function continues to check the breaker function until either
-            the delay is completed or the breaker function returns True.
-            - If the delay is completed before the breaker function returns True, the function returns immediately.
-        """
-        if not (delay_sec > check_interval * 2):
-            raise ValueError(
-                f"check_interval must be 2 times greater than delay_sec, while 2 x {check_interval} > {delay_sec}"
-            )
-
-        ed_time = time() + delay_sec - check_interval
-        # this is to add the first time check, since the timer waits before the check
-        if alarm := breaker():
-            return self
-        while not alarm and time() < ed_time:
-            alarm = breaker()
-            sleep(check_interval)
-        return self
-
-    @staticmethod
-    def delay_b_match(
-        delay_sec: float,
-        breaker: Callable[[], GT],
-        check_interval: float = 0.01,
-    ) -> GT:
-        """
-        Delays the execution of a function until a condition is met.
-
-        Args:
-            delay_sec (float): The number of seconds to delay the execution.
-            breaker (Callable[[], GT]): The function to be executed after the delay.
-            check_interval (float, optional): The interval between each check. Defaults to 0.01.
-
-        Returns:
-            GT: The result of the `breaker` function after the delay.
-
-        Raises:
-            ValueError: If `check_interval` is not 2 times greater than `delay_sec`.
-
-        Note:
-            - The `delay_sec` parameter specifies the total amount of time to delay the execution,
-            including the initial delay and the time spent checking the `breaker` function.
-            - The `check_interval` parameter specifies the interval in seconds between each check.
-            It should be at least twice as large as the `delay_sec` parameter to ensure accurate timing.
-            - The `breaker` function is called periodically to check if the delay should be aborted.
-            If the `breaker` function returns True, the delay is aborted and the function returns immediately.
-            - If the `breaker` function returns False, the function continues to check the `breaker` function until
-            either the delay is completed or the `breaker` function returns True.
-        """
-        if not (delay_sec > check_interval * 2):
-            raise ValueError(
-                f"check_interval must be 2 times greater than delay_sec, while 2 x {check_interval} > {delay_sec}"
-            )
-        ed_time = time() + delay_sec - check_interval
-        # this is to add the first time check, since the timer waits before the check
-        if alarm := breaker():
-            return alarm
-        while not alarm and time() < ed_time:
-            alarm = breaker()
-            sleep(check_interval)
-        return alarm
-
-    def delay(self, delay_sec: float) -> Self:
-        """
-        A function to introduce a delay of a specified time.
-
-        Parameters:
-            delay_sec (float): The time in seconds to delay.
-
-        Returns:
-            Self
-        """
-        sleep(delay_sec)
-        return self
+from queue import Queue
+from threading import Thread
+from time import sleep, time
+from typing import (
+    List,
+    Optional,
+    ByteString,
+    Literal,
+    TypeAlias,
+    Sequence,
+    Self,
+    Callable,
+    Any,
+    TypeVar,
+    Hashable,
+    Dict,
+    Tuple,
+)
+
+from bdmc.modules.cmd import CMD
+from bdmc.modules.logger import _logger
+from bdmc.modules.seriald import SerialClient
+
+DIRECTION: TypeAlias = Literal[1, -1]
+GT = TypeVar("GT", bound=Hashable)
+
+
+class MotorInfo:
+    """
+    A class representing a motor's ID and direction.
+    """
+
+    def __init__(self, code_sign: int, direction: DIRECTION = 1):
+        self.code_sign = code_sign
+        self.direction = direction
+
+    def __eq__(self, other) -> bool:
+        return self.code_sign == other.code_sign
+
+    def __hash__(self) -> int:
+        return hash(self.code_sign)
+
+
+ClassicMIs: Tuple[MotorInfo, MotorInfo, MotorInfo, MotorInfo] = (MotorInfo(1), MotorInfo(2), MotorInfo(3), MotorInfo(4))
+
+
+class CloseLoopController:
+    """
+    CloseLoopController is a class designed to manage and control a system involving multiple motors with closed-loop feedback.
+    It provides methods for setting motor speeds, sending commands, introducing delays with breakers, and updating a shared context.
+    The controller maintains a connection to a serial client for communication with the hardware, manages a command queue,
+    and runs a dedicated thread for message sending. It also allows registering context updaters and getters to facilitate data flow within the application.
+
+    Key features and functionality include:
+
+    1. **Initialization**:
+       - Accepts a list of `MotorInfo` objects, specifying motor IDs and directions, and an optional serial port for communication.
+       - Initializes a `SerialClient` for interfacing with the hardware, a command queue, and a flag for controlling the message sending thread.
+
+    2. **Context Management**:
+       - Maintains a dictionary (`_context`) to store shared data across the application.
+       - Provides methods `register_context_updater` and `register_context_getter` to register functions that update or retrieve specific context variables.
+
+    3. **Motor Control**:
+       - `set_motors_speed`: Sets the speed of each motor based on a provided list of speeds, ensuring consistency with the provided `MotorInfo`.
+       - `send_cmd`: Adds a command to the command queue for transmission to the hardware.
+
+    4. **Message Sending**:
+       - Manages a background thread (`_msg_send_thread`) responsible for continuously retrieving messages from the command queue and writing them to the serial channel.
+       - Offers `start_msg_sending` and `stop_msg_sending` methods to control the message sending thread's lifecycle.
+
+    5. **Delay Functions**:
+       - `delay`: Introduces a simple delay for a specified duration in seconds.
+       - `delay_b`: Delays execution for a given time, periodically checking a breaker function that can abort the delay if it returns True.
+       - `delay_b_match`: Similar to `delay_b`, but returns the result of the breaker function once the delay has completed or the breaker condition is met.
+
+    6. **Utility Methods**:
+       - `wait_exec`: Executes a given function and returns the instance of the class itself.
+       - Properties `context`, `motor_ids`, `motor_dirs`, `cmd_queue`, and `serial_client` provide convenient access to internal attributes.
+
+    Overall, the CloseLoopController serves as a central hub for coordinating motor operations, handling communication with the hardware, managing shared data, and introducing controlled delays with breakers in a closed-loop motor control system.
+    """
+
+    def __init__(
+        self,
+        motor_infos: Sequence[MotorInfo] = ClassicMIs,
+        port: Optional[str] = None,
+        context: Optional[Dict[str, Any]] = None,
+        search_available_port: bool = False,
+    ) -> None:
+
+        if len(motor_infos) != len(set(motor_infos)):
+            raise ValueError("Motor infos must be unique.")
+
+        self._serial: SerialClient = SerialClient(port=port, search_available_port=search_available_port)
+        self._motor_infos: Sequence[MotorInfo] = motor_infos
+        self._cmd_queue: Queue[ByteString] = Queue()
+        self._msg_send_thread: Optional[Thread] = None
+        self._msg_send_thread_should_run: bool = True
+        self._context: Dict[str, Any] = context or {}
+
+    def register_context_updater(
+        self, function: Callable[..., Any], input_keys: List[str], output_keys: List[str], freeze_inputs: bool = False
+    ) -> Callable[[], None]:
+        """
+        Registers a context updater function that updates the context with the specified input and output keys.
+
+        Args:
+            function (Callable[..., Any]): The function to register as a context updater.
+            input_keys (List[str]): The list of input keys to use for the context updater.
+            output_keys (List[str]): The list of output keys to update in the context.
+            freeze_inputs (bool, optional): Whether to freeze the input data. Defaults to False.
+
+        Returns:
+            Callable[[], None]: The registered context updater function.
+
+        Raises:
+            ValueError: If either input_keys or output_keys is empty.
+            ValueError: If any input variable is not found in the context.
+            ValueError: If invalid arguments are provided.
+        """
+        if input_keys == [] and output_keys == []:
+            raise ValueError("Either input_keys or output_keys must be non-empty.")
+        # 确保输入和输出变量存在于上下文中
+        if not_included := [var for var in input_keys if var not in self._context]:
+            raise ValueError(f"Input variables {not_included} not found in context.")
+
+        context = self._context
+        input_keys = tuple(input_keys)
+        output_keys = tuple(output_keys)
+        frozen_input_data = tuple(context.get(key) for key in input_keys)
+
+        match freeze_inputs, input_keys, output_keys:
+            case _, (), (output_key,):
+
+                def _updater() -> None:
+                    context[output_key] = function()
+
+            case _, (), all_output_keys:
+
+                def _updater() -> None:
+                    for key, val in zip(all_output_keys, function()):
+                        context[key] = val
+
+            case False, (input_key,), ():
+
+                def _updater() -> None:
+                    function(context.get(input_key))
+
+            case True, (input_key,), ():
+                input_data = context.get(input_key)
+
+                def _updater() -> None:
+                    function(input_data)
+
+            case False, all_input_keys, ():
+
+                def _updater() -> None:
+                    function(*(tuple(context.get(key) for key in all_input_keys)))
+
+            case True, all_input_keys, ():
+
+                def _updater() -> None:
+                    function(*frozen_input_data)
+
+            case False, (input_key,), (output_key,):
+
+                def _updater() -> None:
+                    context[output_key] = function(context.get(input_key))
+
+            case True, (input_key,), (output_key,):
+                input_data = context.get(input_key)
+
+                def _updater() -> None:
+                    context[output_key] = function(input_data)
+
+            case False, all_input_keys, all_output_keys:
+
+                def _updater() -> None:
+                    frozen_input_data = tuple(context.get(key) for key in all_input_keys)
+                    for key, output_data in zip(all_output_keys, function(*frozen_input_data)):
+                        context[key] = output_data
+
+            case True, all_input_keys, all_output_keys:
+
+                def _updater() -> None:
+                    for key, output_data in zip(all_output_keys, function(*frozen_input_data)):
+                        context[key] = output_data
+
+            case _:
+                raise ValueError(
+                    f"Invalid arguments for register_context_updater function. got {input_keys} and {output_keys} and {freeze_inputs}"
+                )
+        return _updater
+
+    def register_context_getter(self, var_key: str) -> Callable[[], Any]:
+        """
+        Register a context getter function for a given variable key.
+
+        Args:
+            var_key (str): The key of the variable.
+
+        Returns:
+            Callable[[], Any]: A function that returns the value of the variable.
+        """
+        context = self._context
+        return lambda: context.get(var_key)
+
+    def wait_exec(self, function: Callable[[], None]) -> Self:
+        """
+        Executes the given function and returns the instance of the class itself.
+
+        Parameters:
+            function (Callable[[], None]): The function to be executed.
+
+        Returns:
+            Self: The instance of the class itself.
+        """
+        function()
+        return self
+
+    @property
+    def context(self) -> Dict[str, Any]:
+        """
+        Returns the context dictionary of the object.
+
+        :return: A dictionary containing the context of the object.
+        :rtype: Dict[str, Any]
+        """
+        return self._context
+
+    @property
+    def motor_ids(self) -> List[int]:
+        """
+        A property that returns a list of motor ids from the motor infos.
+        """
+        return [motor_info.code_sign for motor_info in self._motor_infos]
+
+    @property
+    def motor_dirs(self) -> List[DIRECTION]:
+        """
+        Return the list of directions for each motor in the motor_infos.
+        """
+        return [motor_info.direction for motor_info in self._motor_infos]
+
+    @property
+    def cmd_queue(self) -> Queue[ByteString]:
+        """
+        Return the message queue.
+        """
+        return self._cmd_queue
+
+    @property
+    def serial_client(self) -> SerialClient:
+        """
+        A property that returns the serial client.
+        """
+        return self._serial
+
+    def stop_msg_sending(self) -> Self:
+        """
+        Stop the message sending by setting the _msg_send_thread_should_run flag to False and joining the message send thread.
+        """
+        self._msg_send_thread_should_run = False
+        self._msg_send_thread.join()
+        self._msg_send_thread = None
+        return self
+
+    def start_msg_sending(self) -> Self:
+        """
+        A description of the entire function, its parameters, and its return types.
+        """
+
+        _logger.info("MSG sending thread starting")
+        self._msg_send_thread_should_run = True
+        _logger.info(f"MSG sending thread started")
+        self._msg_send_thread = Thread(name="msg_send_thread", target=self._msg_sending_loop)
+        self._msg_send_thread.daemon = True
+        self._msg_send_thread.start()
+        _logger.info("MSG sending thread stopped")
+        return self
+
+    def _msg_sending_loop(self) -> None:
+        """
+        A function that handles the sending of messages in a loop.
+        It continuously retrieves messages from a queue and writes them to a channel until the thread should stop running.
+        Returns None.
+        """
+
+        while self._msg_send_thread_should_run:
+            temp = self._cmd_queue.get()
+            _logger.debug(f"Writing {temp} to channel,remaining {self._cmd_queue.qsize()}")
+            self._serial.write(temp)
+
+    def set_motors_speed(self, speeds: Sequence[int | float]) -> Self:
+        """
+        Set the speed for each motor based on the provided speed_list.
+
+        Parameters:
+            speeds (Sequence[int|float]): A list of speeds for each motor.
+
+        Returns:
+            None
+        """
+
+        if len(speeds) != len(self._motor_infos):
+            raise ValueError("Length of speed_list must be equal to the number of motors")
+        self._cmd_queue.put(
+            (
+                "".join(
+                    f"{motor_info.code_sign}v{int(speed * motor_info.direction)}\r"
+                    for motor_info, speed in zip(self._motor_infos, speeds)
+                )
+            ).encode("ascii")
+        )
+        return self
+
+    def send_cmd(self, cmd: CMD) -> Self:
+        """
+        Add a command to the command queue.
+
+        Args:
+            cmd (CMD): The command to be added to the queue.
+
+        Returns:
+            Self: Returns the instance of the class.
+        """
+        self._cmd_queue.put(cmd.value)
+        return self
+
+    def delay_b(
+        self,
+        delay_sec: float,
+        breaker: Callable[[], Any],
+        check_interval: float = 0.01,
+    ) -> Self:
+        """
+        Delays the execution of the function by a specified amount of time, while checking a breaker function periodically.
+
+        Parameters:
+            delay_sec (float): The amount of time to delay the execution in seconds.
+            breaker (Callable[[], Any]): A function that returns a boolean value indicating whether the delay should be aborted.
+            check_interval (float, optional): The interval in seconds between each check of the breaker function. Defaults to 0.01.
+
+        Returns:
+            Self: The instance of the class itself.
+
+        Raises:
+            ValueError: If the check_interval is not at least twice as large as the delay_sec.
+
+        Notes:
+            - The delay_sec parameter specifies the total amount of time to delay the execution,
+             including the initial delay and the time spent checking the breaker function.
+            - The check_interval parameter specifies the interval in seconds between each check of the breaker function.
+             It should be at least twice as large as the delay_sec parameter to ensure accurate timing.
+            - The breaker function is called periodically to check if the delay should be aborted.
+            If the breaker function returns True, the delay is aborted and the function returns immediately.
+            - If the breaker function returns False, the function continues to check the breaker function until either
+            the delay is completed or the breaker function returns True.
+            - If the delay is completed before the breaker function returns True, the function returns immediately.
+        """
+        if not (delay_sec > check_interval * 2):
+            raise ValueError(
+                f"check_interval must be 2 times greater than delay_sec, while 2 x {check_interval} > {delay_sec}"
+            )
+
+        ed_time = time() + delay_sec - check_interval
+        # this is to add the first time check, since the timer waits before the check
+        if alarm := breaker():
+            return self
+        while not alarm and time() < ed_time:
+            alarm = breaker()
+            sleep(check_interval)
+        return self
+
+    @staticmethod
+    def delay_b_match(
+        delay_sec: float,
+        breaker: Callable[[], GT],
+        check_interval: float = 0.01,
+    ) -> GT:
+        """
+        Delays the execution of a function until a condition is met.
+
+        Args:
+            delay_sec (float): The number of seconds to delay the execution.
+            breaker (Callable[[], GT]): The function to be executed after the delay.
+            check_interval (float, optional): The interval between each check. Defaults to 0.01.
+
+        Returns:
+            GT: The result of the `breaker` function after the delay.
+
+        Raises:
+            ValueError: If `check_interval` is not 2 times greater than `delay_sec`.
+
+        Note:
+            - The `delay_sec` parameter specifies the total amount of time to delay the execution,
+            including the initial delay and the time spent checking the `breaker` function.
+            - The `check_interval` parameter specifies the interval in seconds between each check.
+            It should be at least twice as large as the `delay_sec` parameter to ensure accurate timing.
+            - The `breaker` function is called periodically to check if the delay should be aborted.
+            If the `breaker` function returns True, the delay is aborted and the function returns immediately.
+            - If the `breaker` function returns False, the function continues to check the `breaker` function until
+            either the delay is completed or the `breaker` function returns True.
+        """
+        if not (delay_sec > check_interval * 2):
+            raise ValueError(
+                f"check_interval must be 2 times greater than delay_sec, while 2 x {check_interval} > {delay_sec}"
+            )
+        ed_time = time() + delay_sec - check_interval
+        # this is to add the first time check, since the timer waits before the check
+        if alarm := breaker():
+            return alarm
+        while not alarm and time() < ed_time:
+            alarm = breaker()
+            sleep(check_interval)
+        return alarm
+
+    def delay(self, delay_sec: float) -> Self:
+        """
+        A function to introduce a delay of a specified time.
+
+        Parameters:
+            delay_sec (float): The time in seconds to delay.
+
+        Returns:
+            Self
+        """
+        sleep(delay_sec)
+        return self
```

### Comparing `bdmc-0.1.5/src/bdmc/modules/debug.py` & `bdmc-0.1.5.1/src/bdmc/modules/debug.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import time
-from typing import Sequence
-
-from bdmc.modules.controller import MotorInfo, CloseLoopController
-from bdmc.modules.seriald import SerialClient
-
-
-def handle_user_input(serial_client: SerialClient) -> None:
-    """
-    A function that handles user input by starting a read thread, processing the input, and putting it into a command queue.
-
-    Parameters:
-    - serial_client (SerialClient): The client for serial communication.
-    - cmd_queue (Queue[ByteString]): The queue to store processed commands.
-
-    Returns:
-    - None
-    """
-    ct = 0
-    print("\n\nuser input channel opened\n" "please enter cmd below, enter [exit] to end the channel")
-
-    serial_client.start_read_thread(lambda s: print(f"\n\rout[{ct}]: {s}"))
-    try:
-
-        while True:
-            user_input = input(f"\n\rin[{ct}]: ")
-            ct += 1
-            # 对输入的内容进行处理
-            compiled_cmd = (user_input + "\r").encode("ascii")
-            serial_client.write(compiled_cmd)
-
-            if user_input.lower() == "exit":
-                break
-    except KeyboardInterrupt:
-        pass
-    finally:
-        serial_client.stop_read_thread()
-        print("\n\ruser input channel closed")
-
-
-def motor_speed_test(
-    port: str,
-    motor_infos: Sequence[MotorInfo],
-    speed_level: int = 11,
-    interval: float = 1,
-    laps: int = 1,
-) -> None:
-    """
-    A function to test the speed of motors connected to a specified port.
-
-    Parameters:
-        port (str): The port where the motors are connected.
-        motor_infos (Sequence[MotorInfo]): Information about the motors being tested.
-        speed_level (int): The level of speed to test, default is 11.
-        interval (float): The time interval between speed level changes, default is 1.
-        laps (int): The number of laps to run the speed test, default is 3.
-
-    Returns:
-        None
-    """
-    motors = len(motor_infos)
-    con = CloseLoopController(motor_infos=motor_infos, port=port).start_msg_sending()
-
-    for _ in range(laps):
-
-        for i in range(speed_level):
-            speed = i * 1000
-            print(f"doing {speed}")
-            con.set_motors_speed([speed] * motors)
-            time.sleep(interval)
-
-    con.set_motors_speed([0] * motors)
-    print("over")
+import time
+from typing import Sequence
+
+from bdmc.modules.controller import MotorInfo, CloseLoopController
+from bdmc.modules.seriald import SerialClient
+
+
+def handle_user_input(serial_client: SerialClient) -> None:
+    """
+    A function that handles user input by starting a read thread, processing the input, and putting it into a command queue.
+
+    Parameters:
+    - serial_client (SerialClient): The client for serial communication.
+    - cmd_queue (Queue[ByteString]): The queue to store processed commands.
+
+    Returns:
+    - None
+    """
+    ct = 0
+    print("\n\nuser input channel opened\n" "please enter cmd below, enter [exit] to end the channel")
+
+    serial_client.start_read_thread(lambda s: print(f"\n\rout[{ct}]: {s}"))
+    try:
+
+        while True:
+            user_input = input(f"\n\rin[{ct}]: ")
+            ct += 1
+            # 对输入的内容进行处理
+            compiled_cmd = (user_input + "\r").encode("ascii")
+            serial_client.write(compiled_cmd)
+
+            if user_input.lower() == "exit":
+                break
+    except KeyboardInterrupt:
+        pass
+    finally:
+        serial_client.stop_read_thread()
+        print("\n\ruser input channel closed")
+
+
+def motor_speed_test(
+    port: str,
+    motor_infos: Sequence[MotorInfo],
+    speed_level: int = 11,
+    interval: float = 1,
+    laps: int = 1,
+) -> None:
+    """
+    A function to test the speed of motors connected to a specified port.
+
+    Parameters:
+        port (str): The port where the motors are connected.
+        motor_infos (Sequence[MotorInfo]): Information about the motors being tested.
+        speed_level (int): The level of speed to test, default is 11.
+        interval (float): The time interval between speed level changes, default is 1.
+        laps (int): The number of laps to run the speed test, default is 3.
+
+    Returns:
+        None
+    """
+    motors = len(motor_infos)
+    con = CloseLoopController(motor_infos=motor_infos, port=port).start_msg_sending()
+
+    for _ in range(laps):
+
+        for i in range(speed_level):
+            speed = i * 1000
+            print(f"doing {speed}")
+            con.set_motors_speed([speed] * motors)
+            time.sleep(interval)
+
+    con.set_motors_speed([0] * motors)
+    print("over")
```

### Comparing `bdmc-0.1.5/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.1/src/bdmc/modules/seriald.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,218 +1,225 @@
-from types import MappingProxyType
-from typing import Callable, Any, Optional, ByteString, Dict
-
-from serial import Serial, EIGHTBITS, PARITY_NONE, STOPBITS_ONE
-from serial.serialutil import SerialException
-from serial.threaded import ReaderThread, Protocol
-
-from bdmc.modules.logger import _logger
-from bdmc.modules.port import find_serial_ports
-
-ReadHandler = Callable[[bytes | bytearray], Optional[Any]]
-DEFAULT_SERIAL_KWARGS = MappingProxyType(
-    {"baudrate": 115200, "bytesize": EIGHTBITS, "parity": PARITY_NONE, "stopbits": STOPBITS_ONE, "timeout": 2}
-)
-
-
-def serial_kwargs_factory(
-    baudrate: int = 115200,
-    bytesize: int = EIGHTBITS,
-    parity: str = PARITY_NONE,
-    stopbits: int = STOPBITS_ONE,
-    timeout: float = 2,
-) -> MappingProxyType:
-    """
-    A function that generates a dictionary of serial port settings with default values.
-
-    Parameters:
-        baudrate (int): The baud rate for the serial port. Default is 115200.
-        bytesize (int): The number of data bits. Default is EIGHTBITS.
-        parity (str): The parity checking scheme. Default is PARITY_NONE.
-        stopbits (int): The number of stop bits. Default is STOPBITS_ONE.
-        timeout (float): The timeout value for the serial port. Default is 2.
-
-    Returns:
-        MappingProxyType: A read-only mapping of the serial port settings.
-    """
-    return MappingProxyType(
-        {"baudrate": baudrate, "bytesize": bytesize, "parity": parity, "stopbits": stopbits, "timeout": timeout}
-    )
-
-
-CODING_METHOD = "ascii"
-
-
-def default_read_handler(data: bytes | bytearray) -> None:
-    print(f"\n##Received:{data.decode(CODING_METHOD)}")
-
-
-class ReadProtocol(Protocol):
-
-    def __init__(self, read_handler: Optional[ReadHandler] = None):
-        self._read_handler: ReadHandler = read_handler if read_handler else lambda data: None
-
-    def connection_made(self, transport):
-        """Called when reader thread is started"""
-        _logger.info("ReadProtocol has been Set")
-
-    def data_received(self, data):
-        """Called with snippets received from the serial port"""
-        self._read_handler(data)
-
-
-def new_ReadProtocol_factory(read_handler: Optional[ReadHandler] = None) -> Callable[[], ReadProtocol]:
-    def factory():
-        return ReadProtocol(read_handler)
-
-    return factory
-
-
-class SerialClient:
-    """
-    create Serial Client
-    """
-
-    def __init__(self, port: Optional[str] = None, serial_config: Optional[Dict] = DEFAULT_SERIAL_KWARGS):
-        """
-        :param serial_config: a dict that contains the critical transport parameters
-        :param port: the serial port to use
-        """
-        self._serial: Serial = Serial(**serial_config)
-
-        if port is not None:
-            # 尝试使用用户提供的端口
-            self._serial.port = port
-            if not self.open():
-                raise ValueError(f"The specified port '{port}' is not available or cannot be opened.")
-
-        else:
-            # 没有提供端口，尝试自动查找并打开可用端口
-            _logger.info("Searching available Ports")
-            available_serial_ports = find_serial_ports()
-            if not available_serial_ports:
-                raise ValueError("No serial ports FOUND!")
-
-            _logger.info(f"Available ports: {available_serial_ports}")
-
-            for ava_port in available_serial_ports:
-                self._serial.port = ava_port
-                _logger.info(f"Trying to open {self._serial.port}")
-                if self.open():
-                    break
-            else:
-                raise ValueError("No available serial ports could be opened.")
-
-        self._read_thread: Optional[ReaderThread] = None
-
-    @property
-    def is_connected(self) -> bool:
-
-        return self._serial.is_open
-
-    @property
-    def port(self) -> str:
-        return self._serial.port
-
-    @port.setter
-    def port(self, value: str):
-        """
-        pyserial will reopen the serial port on the serial port change
-        :param value:
-        :return:
-        """
-        self._serial.port = value
-
-    def open(self) -> bool:
-        """
-        Connect to the serial port with the settings specified in the instance attributes using a thread-safe mechanism.
-        Return True if the connection is successful, else False.
-        """
-        # 如果当前尚未连接
-        try:
-            # 创建一个 `Serial` 实例连接到对应的串口，并根据实例属性设置相关参数
-            self._serial.open() if not self._serial.is_open else None
-            _logger.info(f"Successfully open [{self._serial.port}]")
-            # 如果已经连接，直接返回 True 表示已连接
-            return True
-        except SerialException:
-            _logger.critical(f"Failed to open [{self._serial.port}]")
-            return False
-
-    def close(self):
-        """
-        disconnects the connection
-        :return:
-        """
-        self._serial.close()
-
-    def write(self, data: ByteString) -> bool:
-        """
-        向串口设备中写入二进制数据。
-
-        Args:
-            data: 要写入的二进制数据
-
-        Returns:
-            如果写入成功则返回 True，否则返回 False。
-
-        Raises:
-            无异常抛出。
-
-        Examples:
-            serial = SerialHelper()
-            if serial.write(b'hello world'):
-                print('Data was successfully written to serial port.')
-            else:
-                print('Failed to write data to serial port.')
-
-        Note:
-            1. 此方法需要确保串口设备已经连接并打开，并且调用此方法前应该先检查设备的状态是否正常。
-            2. 在多线程或多进程环境下使用此方法时，需要确保对串口上下文对象（即 SerialPort 类的实例）进行正确的锁定保护，以避免多个线程或进程同时访问串口设备造成不可预期的错误。
-        """
-        try:
-            self._serial.write(data)
-            return True
-        except SerialException:
-            _logger.critical("Serial write error")
-            return False
-
-    def read(self, length: int) -> bytes | bytearray:
-        """
-        从串口设备中读取指定长度的字节数据。
-
-        Args:
-            length: 整数类型，要读取的字节长度。
-
-        Returns:
-            字节串类型，表示所读取的字节数据。如果读取失败，则返回一个空字节串（b''）。
-
-        Raises:
-            无异常抛出。
-
-        Example:
-            data = serial.read(length=10)
-            print(data)
-
-        Note:
-            如果连接断开或者读取过程中发生异常，会在控制台打印错误信息并返回一个空字节串（b''）。
-        """
-        try:
-            return self._serial.read(length)
-        except SerialException:
-            _logger.critical("Serial read error")
-        return b""
-
-    def start_read_thread(self, read_handler: [ReadHandler]) -> None:
-        """
-        Start the thread reading loop.
-        :return:
-        """
-        _logger.info("Start Read Thread")
-        self._read_thread = ReaderThread(
-            serial_instance=self._serial, protocol_factory=new_ReadProtocol_factory(read_handler)
-        )
-        self._read_thread.daemon = True
-        self._read_thread.start()
-
-    def stop_read_thread(self) -> None:
-        self._read_thread.stop()
+from types import MappingProxyType
+from typing import Callable, Any, Optional, ByteString, Dict
+
+from serial import Serial, EIGHTBITS, PARITY_NONE, STOPBITS_ONE
+from serial.serialutil import SerialException
+from serial.threaded import ReaderThread, Protocol
+
+from bdmc.modules.logger import _logger
+from bdmc.modules.port import find_serial_ports
+
+ReadHandler = Callable[[bytes | bytearray], Optional[Any]]
+DEFAULT_SERIAL_KWARGS = MappingProxyType(
+    {"baudrate": 115200, "bytesize": EIGHTBITS, "parity": PARITY_NONE, "stopbits": STOPBITS_ONE, "timeout": 2}
+)
+
+
+def serial_kwargs_factory(
+    baudrate: int = 115200,
+    bytesize: int = EIGHTBITS,
+    parity: str = PARITY_NONE,
+    stopbits: int = STOPBITS_ONE,
+    timeout: float = 2,
+) -> MappingProxyType:
+    """
+    A function that generates a dictionary of serial port settings with default values.
+
+    Parameters:
+        baudrate (int): The baud rate for the serial port. Default is 115200.
+        bytesize (int): The number of data bits. Default is EIGHTBITS.
+        parity (str): The parity checking scheme. Default is PARITY_NONE.
+        stopbits (int): The number of stop bits. Default is STOPBITS_ONE.
+        timeout (float): The timeout value for the serial port. Default is 2.
+
+    Returns:
+        MappingProxyType: A read-only mapping of the serial port settings.
+    """
+    return MappingProxyType(
+        {"baudrate": baudrate, "bytesize": bytesize, "parity": parity, "stopbits": stopbits, "timeout": timeout}
+    )
+
+
+CODING_METHOD = "ascii"
+
+
+def default_read_handler(data: bytes | bytearray) -> None:
+    print(f"\n##Received:{data.decode(CODING_METHOD)}")
+
+
+class ReadProtocol(Protocol):
+
+    def __init__(self, read_handler: Optional[ReadHandler] = None):
+        self._read_handler: ReadHandler = read_handler if read_handler else lambda data: None
+
+    def connection_made(self, transport):
+        """Called when reader thread is started"""
+        _logger.info("ReadProtocol has been Set")
+
+    def data_received(self, data):
+        """Called with snippets received from the serial port"""
+        self._read_handler(data)
+
+
+def new_ReadProtocol_factory(read_handler: Optional[ReadHandler] = None) -> Callable[[], ReadProtocol]:
+    def factory():
+        return ReadProtocol(read_handler)
+
+    return factory
+
+
+class SerialClient:
+    """
+    create Serial Client
+    """
+
+    def __init__(
+        self,
+        port: Optional[str] = None,
+        serial_config: Optional[Dict] = DEFAULT_SERIAL_KWARGS,
+        search_available_port: bool = False,
+    ):
+        """
+        :param serial_config: a dict that contains the critical transport parameters
+        :param port: the serial port to use
+        """
+        self._serial: Serial = Serial(**serial_config)
+
+        if port is not None:
+            # 尝试使用用户提供的端口
+            self._serial.port = port
+            if not self.open():
+                raise ValueError(f"The specified port '{port}' is not available or cannot be opened.")
+
+        elif search_available_port:
+            # 没有提供端口，尝试自动查找并打开可用端口
+            _logger.info("Searching available Ports")
+            available_serial_ports = find_serial_ports()
+            if not available_serial_ports:
+                raise ValueError("No serial ports FOUND!")
+
+            _logger.info(f"Available ports: {available_serial_ports}")
+
+            for ava_port in available_serial_ports:
+                self._serial.port = ava_port
+                if self.open():
+                    break
+            else:
+                raise ValueError("No available serial ports could be opened.")
+        else:
+            pass
+        self._read_thread: Optional[ReaderThread] = None
+
+    @property
+    def is_connected(self) -> bool:
+
+        return self._serial.is_open
+
+    @property
+    def port(self) -> str:
+        return self._serial.port
+
+    @port.setter
+    def port(self, value: str):
+        """
+        pyserial will reopen the serial port on the serial port change
+        :param value:
+        :return:
+        """
+        self._serial.port = value
+
+    def open(self) -> bool:
+        """
+        Connect to the serial port with the settings specified in the instance attributes using a thread-safe mechanism.
+        Return True if the connection is successful, else False.
+        """
+        # 如果当前尚未连接
+        try:
+            _logger.info(f"Trying to open {self._serial.port}")
+
+            # 创建一个 `Serial` 实例连接到对应的串口，并根据实例属性设置相关参数
+            self._serial.open() if not self._serial.is_open else None
+            _logger.info(f"Successfully open [{self._serial.port}]")
+            # 如果已经连接，直接返回 True 表示已连接
+            return True
+        except SerialException:
+            _logger.critical(f"Failed to open [{self._serial.port}]")
+            return False
+
+    def close(self):
+        """
+        disconnects the connection
+        :return:
+        """
+        self._serial.close()
+
+    def write(self, data: ByteString) -> bool:
+        """
+        向串口设备中写入二进制数据。
+
+        Args:
+            data: 要写入的二进制数据
+
+        Returns:
+            如果写入成功则返回 True，否则返回 False。
+
+        Raises:
+            无异常抛出。
+
+        Examples:
+            serial = SerialHelper()
+            if serial.write(b'hello world'):
+                print('Data was successfully written to serial port.')
+            else:
+                print('Failed to write data to serial port.')
+
+        Note:
+            1. 此方法需要确保串口设备已经连接并打开，并且调用此方法前应该先检查设备的状态是否正常。
+            2. 在多线程或多进程环境下使用此方法时，需要确保对串口上下文对象（即 SerialPort 类的实例）进行正确的锁定保护，以避免多个线程或进程同时访问串口设备造成不可预期的错误。
+        """
+        try:
+            self._serial.write(data)
+            return True
+        except SerialException:
+            _logger.critical("Serial write error")
+            return False
+
+    def read(self, length: int) -> bytes | bytearray:
+        """
+        从串口设备中读取指定长度的字节数据。
+
+        Args:
+            length: 整数类型，要读取的字节长度。
+
+        Returns:
+            字节串类型，表示所读取的字节数据。如果读取失败，则返回一个空字节串（b''）。
+
+        Raises:
+            无异常抛出。
+
+        Example:
+            data = serial.read(length=10)
+            print(data)
+
+        Note:
+            如果连接断开或者读取过程中发生异常，会在控制台打印错误信息并返回一个空字节串（b''）。
+        """
+        try:
+            return self._serial.read(length)
+        except SerialException:
+            _logger.critical("Serial read error")
+        return b""
+
+    def start_read_thread(self, read_handler: [ReadHandler]) -> None:
+        """
+        Start the thread reading loop.
+        :return:
+        """
+        _logger.info("Start Read Thread")
+        self._read_thread = ReaderThread(
+            serial_instance=self._serial, protocol_factory=new_ReadProtocol_factory(read_handler)
+        )
+        self._read_thread.daemon = True
+        self._read_thread.start()
+
+    def stop_read_thread(self) -> None:
+        self._read_thread.stop()
```

### Comparing `bdmc-0.1.5/tests/find_tests.py` & `bdmc-0.1.5.1/tests/find_tests.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os
-import sys
-import unittest
-
-
-def discover_tests_in_package(package_path):
-    # 获取package路径
-    package_dir = os.path.dirname(os.path.abspath(__file__))
-
-    # 使用TestLoader的discover方法来查找所有测试
-    loader = unittest.TestLoader()
-    suite = loader.discover(start_dir=package_dir, pattern="test_*.py", top_level_dir=os.getcwd())
-
-    # 执行测试
-    runner = unittest.TextTestRunner(verbosity=2)
-    results = runner.run(suite)
-
-    # 检查是否有失败或错误
-    if not results.wasSuccessful():
-        sys.exit(1)
-
-
-if __name__ == "__main__":
-    # 假设当前位置就是软件包的顶层目录
-    discover_tests_in_package(".")
+import os
+import sys
+import unittest
+
+
+def discover_tests_in_package(package_path):
+    # 获取package路径
+    package_dir = os.path.dirname(os.path.abspath(__file__))
+
+    # 使用TestLoader的discover方法来查找所有测试
+    loader = unittest.TestLoader()
+    suite = loader.discover(start_dir=package_dir, pattern="test_*.py", top_level_dir=os.getcwd())
+
+    # 执行测试
+    runner = unittest.TextTestRunner(verbosity=2)
+    results = runner.run(suite)
+
+    # 检查是否有失败或错误
+    if not results.wasSuccessful():
+        sys.exit(1)
+
+
+if __name__ == "__main__":
+    # 假设当前位置就是软件包的顶层目录
+    discover_tests_in_package(".")
```

### Comparing `bdmc-0.1.5/tests/test_context.py` & `bdmc-0.1.5.1/tests/test_context.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import unittest
-from unittest.mock import MagicMock
-
-from bdmc import CloseLoopController, MotorInfo
-
-
-class TestContextUpdaterRegistration(unittest.TestCase):
-
-    def setUp(self):
-        self.con = CloseLoopController(
-            motor_infos=[MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)],
-            context={"key1": "value1", "key2": "value2"},
-        )
-        # 假设有一个简单的上下文字典
-
-    def test_case_1_no_inputs_and_single_output(self):
-        # 函数无输入，单个输出
-        func = MagicMock(return_value="output_value")
-        updater = self.con.register_context_updater(func, [], ["output"])
-        updater()
-        func.assert_called_once()
-        print(self.con.context)
-        self.assertEqual(self.con.context["output"], "output_value")
-
-    def test_case_2_no_inputs_and_multiple_outputs(self):
-        # 函数无输入，多个输出
-        func = MagicMock(return_value=["out1", "out2"])
-        updater = self.con.register_context_updater(func, [], ["out1", "out2"])
-        updater()
-        func.assert_called_once()
-        self.assertEqual(self.con.context["out1"], "out1")
-        self.assertEqual(self.con.context["out2"], "out2")
-
-    def test_case_3_unfrozen_single_input_no_outputs(self):
-        # 未冻结的单个输入，无输出
-        func = MagicMock()
-        updater = self.con.register_context_updater(func, ["key1"], [])
-        updater()
-        func.assert_called_once_with("value1")
-
-    def test_case_4_frozen_single_input_no_outputs(self):
-        # 冻结的单个输入，无输出
-        func = MagicMock()
-        self.con.register_context_updater(func, ["key1"], [], freeze_inputs=True)
-        # 不检查函数调用，因为在这种情况下函数不会在上下文更新时被调用
-
-    def test_case_5_unfrozen_multiple_inputs_no_outputs(self):
-        # 未冻结的多个输入，无输出
-        func = MagicMock()
-        updater = self.con.register_context_updater(func, ["key1", "key2"], [])
-        updater()
-        func.assert_called_once_with("value1", "value2")
-
-    def test_case_6_frozen_multiple_inputs_no_outputs(self):
-        # 冻结的多个输入，无输出
-        func = MagicMock()
-        frozen_data = ("value1", "value2")
-        updater = self.con.register_context_updater(func, ["key1", "key2"], [], freeze_inputs=True)
-        updater()
-        func.assert_called_once_with(*frozen_data)
-
-    def test_case_7_unfrozen_single_input_single_output(self):
-        # 未冻结的单个输入，单个输出
-        func = MagicMock(return_value="output_value")
-        updater = self.con.register_context_updater(func, ["key1"], ["output"])
-        updater()
-        func.assert_called_once_with("value1")
-        self.assertEqual(self.con.context["output"], "output_value")
-
-    def test_case_8_frozen_single_input_single_output(self):
-        # 冻结的单个输入，单个输出
-        func = MagicMock(return_value="output_value")
-        updater = self.con.register_context_updater(func, ["key1"], ["output"], freeze_inputs=True)
-        updater()
-        func.assert_called_once_with("value1")
-        self.assertEqual(self.con.context["output"], "output_value")
-
-    def test_case_9_unfrozen_multiple_inputs_multiple_outputs(self):
-        # 未冻结的多个输入，多个输出
-        func = MagicMock(return_value=["out1", "out2"])
-        updater = self.con.register_context_updater(func, ["key1", "key2"], ["out1", "out2"])
-        updater()
-        func.assert_called_once_with("value1", "value2")
-        self.assertEqual(self.con.context["out1"], "out1")
-        self.assertEqual(self.con.context["out2"], "out2")
-
-    def test_case_10_frozen_multiple_inputs_multiple_outputs(self):
-        # 冻结的多个输入，多个输出
-        func = MagicMock(side_effect=[("out1", "out2")])
-        updater = self.con.register_context_updater(func, ["key1", "key2"], ["out1", "out2"], freeze_inputs=True)
-        updater()
-        func.assert_called_once_with("value1", "value2")
-        self.assertEqual(self.con.context["out1"], "out1")
-        self.assertEqual(self.con.context["out2"], "out2")
-
-    def test_invalid_arguments_exception(self):
-        with self.assertRaises(ValueError):
-            # 测试无效参数引发的异常
-            self.con.register_context_updater(lambda: None, [], [])
+import unittest
+from unittest.mock import MagicMock
+
+from bdmc import CloseLoopController, MotorInfo
+
+
+class TestContextUpdaterRegistration(unittest.TestCase):
+
+    def setUp(self):
+        self.con = CloseLoopController(
+            motor_infos=[MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)],
+            context={"key1": "value1", "key2": "value2"},
+        )
+        # 假设有一个简单的上下文字典
+
+    def test_case_1_no_inputs_and_single_output(self):
+        # 函数无输入，单个输出
+        func = MagicMock(return_value="output_value")
+        updater = self.con.register_context_updater(func, [], ["output"])
+        updater()
+        func.assert_called_once()
+        print(self.con.context)
+        self.assertEqual(self.con.context["output"], "output_value")
+
+    def test_case_2_no_inputs_and_multiple_outputs(self):
+        # 函数无输入，多个输出
+        func = MagicMock(return_value=["out1", "out2"])
+        updater = self.con.register_context_updater(func, [], ["out1", "out2"])
+        updater()
+        func.assert_called_once()
+        self.assertEqual(self.con.context["out1"], "out1")
+        self.assertEqual(self.con.context["out2"], "out2")
+
+    def test_case_3_unfrozen_single_input_no_outputs(self):
+        # 未冻结的单个输入，无输出
+        func = MagicMock()
+        updater = self.con.register_context_updater(func, ["key1"], [])
+        updater()
+        func.assert_called_once_with("value1")
+
+    def test_case_4_frozen_single_input_no_outputs(self):
+        # 冻结的单个输入，无输出
+        func = MagicMock()
+        self.con.register_context_updater(func, ["key1"], [], freeze_inputs=True)
+        # 不检查函数调用，因为在这种情况下函数不会在上下文更新时被调用
+
+    def test_case_5_unfrozen_multiple_inputs_no_outputs(self):
+        # 未冻结的多个输入，无输出
+        func = MagicMock()
+        updater = self.con.register_context_updater(func, ["key1", "key2"], [])
+        updater()
+        func.assert_called_once_with("value1", "value2")
+
+    def test_case_6_frozen_multiple_inputs_no_outputs(self):
+        # 冻结的多个输入，无输出
+        func = MagicMock()
+        frozen_data = ("value1", "value2")
+        updater = self.con.register_context_updater(func, ["key1", "key2"], [], freeze_inputs=True)
+        updater()
+        func.assert_called_once_with(*frozen_data)
+
+    def test_case_7_unfrozen_single_input_single_output(self):
+        # 未冻结的单个输入，单个输出
+        func = MagicMock(return_value="output_value")
+        updater = self.con.register_context_updater(func, ["key1"], ["output"])
+        updater()
+        func.assert_called_once_with("value1")
+        self.assertEqual(self.con.context["output"], "output_value")
+
+    def test_case_8_frozen_single_input_single_output(self):
+        # 冻结的单个输入，单个输出
+        func = MagicMock(return_value="output_value")
+        updater = self.con.register_context_updater(func, ["key1"], ["output"], freeze_inputs=True)
+        updater()
+        func.assert_called_once_with("value1")
+        self.assertEqual(self.con.context["output"], "output_value")
+
+    def test_case_9_unfrozen_multiple_inputs_multiple_outputs(self):
+        # 未冻结的多个输入，多个输出
+        func = MagicMock(return_value=["out1", "out2"])
+        updater = self.con.register_context_updater(func, ["key1", "key2"], ["out1", "out2"])
+        updater()
+        func.assert_called_once_with("value1", "value2")
+        self.assertEqual(self.con.context["out1"], "out1")
+        self.assertEqual(self.con.context["out2"], "out2")
+
+    def test_case_10_frozen_multiple_inputs_multiple_outputs(self):
+        # 冻结的多个输入，多个输出
+        func = MagicMock(side_effect=[("out1", "out2")])
+        updater = self.con.register_context_updater(func, ["key1", "key2"], ["out1", "out2"], freeze_inputs=True)
+        updater()
+        func.assert_called_once_with("value1", "value2")
+        self.assertEqual(self.con.context["out1"], "out1")
+        self.assertEqual(self.con.context["out2"], "out2")
+
+    def test_invalid_arguments_exception(self):
+        with self.assertRaises(ValueError):
+            # 测试无效参数引发的异常
+            self.con.register_context_updater(lambda: None, [], [])
```

### Comparing `bdmc-0.1.5/tests/test_controller.py` & `bdmc-0.1.5.1/tests/test_controller.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import pathlib
-import time
-import unittest
-
-from viztracer import VizTracer
-
-from bdmc import set_log_level
-from bdmc.modules.controller import MotorInfo, CloseLoopController
-from bdmc.modules.debug import motor_speed_test
-
-VIZ_OUTPUT_DIR = pathlib.Path(__file__).parent / "viz_output"
-VIZ_OUTPUT_DIR.mkdir(exist_ok=True)
-
-
-class TestControllerSend(unittest.TestCase):
-    def setUp(self):
-        self.test_port = None
-        self.tracer = VizTracer()
-
-    def test_send(self):
-        set_log_level(10)
-        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
-        self.tracer.start()
-        motor_speed_test(port=self.test_port, motor_infos=m, interval=0.01)
-        self.tracer.stop()
-        self.tracer.save(output_file=(VIZ_OUTPUT_DIR / "test_send.json").as_posix())
-
-    def test_unique_motor_check(self):
-        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=1, direction=-1)]
-
-        with self.assertRaises(ValueError):
-            CloseLoopController(port=self.test_port, motor_infos=m)
-
-    def test_cmds_align(self):
-        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
-        con = CloseLoopController(port=self.test_port, motor_infos=m)
-        con.set_motors_speed([1000, 2000])
-        with self.assertRaises(ValueError):
-            con.set_motors_speed([100] * 3)
-
-    def test_delays(self):
-        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
-        con = CloseLoopController(port=self.test_port, motor_infos=m)
-        start = time.time()
-        con.delay(1)
-        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
-        start = time.time()
-        con.delay_b(1, lambda: False)
-        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
-        start = time.time()
-        print(con.delay_b(1, lambda: False))
-        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
-
-
-if __name__ == "__main__":
-    pass
+import pathlib
+import time
+import unittest
+
+from viztracer import VizTracer
+
+from bdmc import set_log_level
+from bdmc.modules.controller import MotorInfo, CloseLoopController
+from bdmc.modules.debug import motor_speed_test
+
+VIZ_OUTPUT_DIR = pathlib.Path(__file__).parent / "viz_output"
+VIZ_OUTPUT_DIR.mkdir(exist_ok=True)
+
+
+class TestControllerSend(unittest.TestCase):
+    def setUp(self):
+        self.test_port = None
+        self.tracer = VizTracer()
+
+    def test_send(self):
+        set_log_level(10)
+        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
+        self.tracer.start()
+        motor_speed_test(port=self.test_port, motor_infos=m, interval=0.01)
+        self.tracer.stop()
+        self.tracer.save(output_file=(VIZ_OUTPUT_DIR / "test_send.json").as_posix())
+
+    def test_unique_motor_check(self):
+        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=1, direction=-1)]
+
+        with self.assertRaises(ValueError):
+            CloseLoopController(port=self.test_port, motor_infos=m)
+
+    def test_cmds_align(self):
+        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
+        con = CloseLoopController(port=self.test_port, motor_infos=m)
+        con.set_motors_speed([1000, 2000])
+        with self.assertRaises(ValueError):
+            con.set_motors_speed([100] * 3)
+
+    def test_delays(self):
+        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
+        con = CloseLoopController(port=self.test_port, motor_infos=m)
+        start = time.time()
+        con.delay(1)
+        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
+        start = time.time()
+        con.delay_b(1, lambda: False)
+        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
+        start = time.time()
+        print(con.delay_b(1, lambda: False))
+        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `bdmc-0.1.5/PKG-INFO` & `bdmc-0.1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: bdmc
-Version: 0.1.5
-Summary: An api wrapper lib designed for the uptech BDMC divers
-Author-Email: Whth <88489697+Whth@users.noreply.github.com>
-License: MIT
-Requires-Python: >=3.11
-Requires-Dist: pyserial>=3.5
-Requires-Dist: coloredlogs>=15.0.1
-Description-Content-Type: text/markdown
-
 # bdmc
 ---
 > This lib is especially designed to control the BDMC drivers, which is under the sales of TechStar.
 
 ## TODO
 
 - [x] Basic motor serial controller.
```

