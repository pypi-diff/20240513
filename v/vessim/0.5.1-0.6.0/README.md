# Comparing `tmp/vessim-0.5.1.tar.gz` & `tmp/vessim-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessim-0.5.1.tar", max compression
+gzip compressed data, was "vessim-0.6.0.tar", max compression
```

## Comparing `vessim-0.5.1.tar` & `vessim-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1085 2024-03-14 11:45:56.960181 vessim-0.5.1/LICENSE
--rw-r--r--   0        0        0     5698 2024-03-14 11:45:56.960181 vessim-0.5.1/README.md
--rw-r--r--   0        0        0     3936 2024-03-14 11:45:57.000181 vessim-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      465 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/__init__.py
--rw-r--r--   0        0        0     5023 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/_data.py
--rw-r--r--   0        0        0     4088 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/actor.py
--rw-r--r--   0        0        0     5724 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/controller.py
--rw-r--r--   0        0        0     6100 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/cosim.py
--rw-r--r--   0        0        0      963 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/power_meter.py
--rw-r--r--   0        0        0    16772 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/signal.py
--rw-r--r--   0        0        0     8029 2024-03-14 11:45:57.000181 vessim-0.5.1/vessim/sil.py
--rw-r--r--   0        0        0     5020 2024-03-14 11:45:57.004181 vessim-0.5.1/vessim/storage.py
--rw-r--r--   0        0        0      530 2024-03-14 11:45:57.004181 vessim-0.5.1/vessim/util.py
--rw-r--r--   0        0        0     7561 1970-01-01 00:00:00.000000 vessim-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-13 13:44:39.930082 vessim-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5698 2024-05-13 13:44:39.930082 vessim-0.6.0/README.md
+-rw-r--r--   0        0        0     4087 2024-05-13 13:44:40.034082 vessim-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      429 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/__init__.py
+-rw-r--r--   0        0        0     5023 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/_data.py
+-rw-r--r--   0        0        0     1569 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/_util.py
+-rw-r--r--   0        0        0     4088 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/actor.py
+-rw-r--r--   0        0        0     5549 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/controller.py
+-rw-r--r--   0        0        0     7824 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/cosim.py
+-rw-r--r--   0        0        0     3534 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/policy.py
+-rw-r--r--   0        0        0      963 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/power_meter.py
+-rw-r--r--   0        0        0    16773 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/signal.py
+-rw-r--r--   0        0        0     9469 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/sil.py
+-rw-r--r--   0        0        0     3759 2024-05-13 13:44:40.034082 vessim-0.6.0/vessim/storage.py
+-rw-r--r--   0        0        0     7492 1970-01-01 00:00:00.000000 vessim-0.6.0/PKG-INFO
```

### Comparing `vessim-0.5.1/LICENSE` & `vessim-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vessim-0.5.1/README.md` & `vessim-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `vessim-0.5.1/pyproject.toml` & `vessim-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -39,23 +39,26 @@
     { version = "^1.26.0", python = ">=3.12" }
 ]
 pandas = "^2.0.0"
 mosaik = "^3.2.0"
 mosaik-api-v3 = "^3.0.4"
 loguru = "^0.6.0"
 
+# The docopt, used by the mosaik-api causes some issues in current python versions
+# This dependency can be deleted once the following issue is resolved by mosaik
+# https://gitlab.com/mosaik/api/mosaik-api-python/-/issues/6
+docopt-ng = "^0.6.2"
+
 # Optional dependencies (software-in-the-loop)
 requests = {version = "^2.26.0", optional = true}
 fastapi = {version = "^0.104.0", optional = true}
-docker = {version = "^7.0.0", optional = true}
-redis = {version = "^5.0.0", optional = true}
 uvicorn = {version = "^0.23.0", optional = true}
 
 [tool.poetry.extras]
-sil = ["requests", "fastapi", "docker", "redis", "uvicorn"]
+sil = ["requests", "fastapi", "uvicorn"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 mypy = "*"
@@ -72,14 +75,15 @@
 setuptools = "*"
 sphinx = "*"
 furo = "*"
 sphinx-copybutton = "*"
 nbsphinx = "*"
 pandoc = "*"
 ipython = "*"
+matplotlib = "*"
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 99  # Set the maximum characters per line
```

### Comparing `vessim-0.5.1/vessim/_data.py` & `vessim-0.6.0/vessim/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     },
     "solcast2022_global": {
         "actual": "solcast2022_global_actual.csv",
         "forecast": "solcast2022_global_forecast.csv",
         "fill_method": "bfill",
         "url": "https://raw.githubusercontent.com/dos-group/vessim/main/datasets/solcast2022_global.zip",
     },
-    "watttime2023_casio-north": {
-        "actual": "watttime2023_casio-north_actual.csv",
-        "forecast": "watttime2023_casio-north_forecast.csv",
+    "watttime2023_caiso-north": {
+        "actual": "watttime2023_caiso-north_actual.csv",
+        "forecast": "watttime2023_caiso-north_forecast.csv",
         "fill_method": "ffill",
-        "url": "https://raw.githubusercontent.com/dos-group/vessim/main/datasets/watttime2023_casio-north.zip",
+        "url": "https://raw.githubusercontent.com/dos-group/vessim/main/datasets/watttime2023_caiso-north.zip",
     },
 }
 
 
 def load_dataset(dataset: str, dir_path: Path, params: Optional[dict] = None) -> dict:
     """Downloads a dataset from the vessim repository, unpacks it and loads data."""
     if dataset not in VESSIM_DATASETS:
```

### Comparing `vessim-0.5.1/vessim/actor.py` & `vessim-0.6.0/vessim/actor.py`

 * *Files identical despite different names*

### Comparing `vessim-0.5.1/vessim/controller.py` & `vessim-0.6.0/vessim/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,98 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import datetime
-from typing import Any, TYPE_CHECKING, MutableMapping, Optional, Callable
+from typing import Any, MutableMapping, Optional, Callable, TYPE_CHECKING
 
 import mosaik_api_v3  # type: ignore
 import pandas as pd
 
 from vessim.signal import Signal
-from vessim.util import Clock
+from vessim.storage import Storage
+from vessim.policy import MicrogridPolicy
 
 if TYPE_CHECKING:
     from vessim.cosim import Microgrid
 
 
 class Controller(ABC):
     def __init__(self, step_size: Optional[int] = None):
         self.step_size = step_size
 
-    @abstractmethod
-    def start(self, microgrid: Microgrid, clock: Clock) -> None:
-        """Supplies the controller with objects available after simulation start.
-
-        Args:
-            microgrid: The microgrid under control.
-            clock: The clock of the simulation environment.
-        """
+    def start(self, microgrid: Microgrid):
+        """Function to be executed before simulation is started. Can be overridden."""
+        pass
 
     @abstractmethod
-    def step(self, time: int, p_delta: float, actor_infos: dict) -> None:
+    def step(self, time: datetime, p_delta: float, e_delta: float, actor_states: dict) -> None:
         """Performs a simulation step.
 
         Args:
-            time: Current simulation time.
-            p_delta: Current power delta from the microgrid after the storage has been
-                (de)charged. If negative, this power must be drawn from the public grid.
-                If positive, the power can be fed to the public grid or must be curtailed.
-            actor_infos: Contains the last "info" dictionaries by all actors in the
-                microgrid. The info dictionary is defined by the actor and can contain
+            time: Current datetime.
+            p_delta: Power delta in W based on the consumption and production of all actors.
+            e_delta: Total energy in Ws that has been drawn from/ fed to the utility grid
+                in the previous time step.
+            actor_states: Contains the last state dictionaries by all actors in the
+                microgrid. The state dictionary is defined by the actor and can contain
                 any information about the actor's state.
         """
 
     def finalize(self) -> None:
-        """This method can be overridden clean-up after the simulation finished."""
+        """Function to be executed after simulation has ended. Can be overridden for clean-up."""
+        pass
 
 
 class Monitor(Controller):
     def __init__(
         self,
         step_size: Optional[int] = None,
         grid_signals: Optional[dict[str, Signal]] = None,
+        policy: Optional[MicrogridPolicy] = None,
+        storage: Optional[Storage] = None,
     ):
         super().__init__(step_size=step_size)
-        self.grid_signals = grid_signals
         self.monitor_log: dict[datetime, dict] = defaultdict(dict)
         self.custom_monitor_fns: list[Callable] = []
-        self.clock: Optional[Clock] = None
-
-    def start(self, microgrid: Microgrid, clock: Clock) -> None:
-        self.clock = clock
-        if microgrid.storage is not None:
-            storage_state = microgrid.storage.state()
-            self.add_monitor_fn(lambda _: {"storage": storage_state})
 
-        if self.grid_signals is not None:
-            for signal_name, signal_api in self.grid_signals.items():
+        if grid_signals is not None:
+            for signal_name, signal_api in grid_signals.items():
 
                 def fn(time):
-                    return {signal_name: signal_api.at(clock.to_datetime(time))}
+                    return {signal_name: signal_api.at(time)}
 
                 self.add_monitor_fn(fn)
 
+        if policy is not None:
+
+            def fn(time):
+                return policy.state()
+
+            self.add_monitor_fn(fn)
+
+        if storage is not None:
+
+            def fn(time):
+                return storage.state()
+
+            self.add_monitor_fn(fn)
+
     def add_monitor_fn(self, fn: Callable[[float], dict[str, Any]]):
         self.custom_monitor_fns.append(fn)
 
-    def step(self, time: int, p_delta: float, actor_infos: dict) -> None:
+    def step(self, time: datetime, p_delta: float, e_delta: float, actor_states: dict) -> None:
         log_entry = dict(
             p_delta=p_delta,
-            actor_infos=actor_infos,
+            e_delta=e_delta,
+            actor_states=actor_states,
         )
         for monitor_fn in self.custom_monitor_fns:
             log_entry.update(monitor_fn(time))
-        assert self.clock is not None  # clock is initialized at this point
-        self.monitor_log[self.clock.to_datetime(time)] = log_entry
+        self.monitor_log[time] = log_entry
 
     def to_csv(self, out_path: str):
         df = pd.DataFrame({k: _flatten_dict(v) for k, v in self.monitor_log.items()}).T
         df.to_csv(out_path)
 
 
 def _flatten_dict(d: MutableMapping, parent_key: str = "") -> MutableMapping:
@@ -114,51 +119,51 @@
         },
     }
 
     def __init__(self):
         super().__init__(self.META)
         self.eid = "Controller"
         self.step_size = None
-        self.controller: Optional[Controller] = None
+        self.clock = None
+        self.controller = None
+        self.e = 0.0
 
     def init(self, sid, time_resolution=1.0, **sim_params):
         self.step_size = sim_params["step_size"]
+        self.clock = sim_params["clock"]
         return self.meta
 
     def create(self, num, model, **model_params):
         assert num == 1, "Only one instance per simulation is supported"
         self.controller = model_params["controller"]
         return [{"eid": self.eid, "type": model}]
 
     def step(self, time, inputs, max_advance):
         assert self.controller is not None
-        try:
-            self.controller.step(time, *_parse_controller_inputs(inputs[self.eid]))
-        except KeyError:
-            self.controller.step(time, p_delta=0, actor_infos={})
+        now = self.clock.to_datetime(time)
+        self.controller.step(now, *self._parse_controller_inputs(inputs[self.eid]))
         return time + self.step_size
 
     def get_data(self, outputs):
         return {}  # TODO so far unused
 
     def finalize(self) -> None:
         """Stops the api server and the collector thread when the simulation finishes."""
         assert self.controller is not None
         self.controller.finalize()
 
-
-def _parse_controller_inputs(inputs: dict[str, dict[str, Any]]) -> tuple[float, dict]:
-    try:
+    def _parse_controller_inputs(
+            self, inputs: dict[str, dict[str, Any]]
+    ) -> tuple[float,float, dict]:
         p_delta = _get_val(inputs, "p_delta")
-    except KeyError:
-        p_delta = None  # in case there has not yet been any power reported by actors
-    actor_keys = [k for k in inputs.keys() if k.startswith("actor")]
-    actors: defaultdict[str, Any] = defaultdict(dict)
-    for k in actor_keys:
-        _, actor_name = k.split(".")
-        actors[actor_name] = _get_val(inputs, k)
-    assert p_delta is not None
-    return p_delta, dict(actors)
+        last_e = self.e
+        self.e = _get_val(inputs, "e")
+        actor_keys = [k for k in inputs.keys() if k.startswith("actor")]
+        actors: defaultdict[str, Any] = defaultdict(dict)
+        for k in actor_keys:
+            _, actor_name = k.split(".")
+            actors[actor_name] = _get_val(inputs, k)
+        return p_delta, self.e - last_e, dict(actors)
 
 
 def _get_val(inputs: dict, key: str) -> Any:
     return list(inputs[key].values())[0]
```

### Comparing `vessim-0.5.1/vessim/power_meter.py` & `vessim-0.6.0/vessim/power_meter.py`

 * *Files identical despite different names*

### Comparing `vessim-0.5.1/vessim/signal.py` & `vessim-0.6.0/vessim/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Any, Optional, Literal
 
 import pandas as pd
 import numpy as np
 
 from vessim._data import load_dataset
-from vessim.util import DatetimeLike
+from vessim._util import DatetimeLike
 
 
 class Signal(ABC):
     """Abstract base class for signals."""
 
     @abstractmethod
     def at(self, dt: DatetimeLike, **kwargs):
```

### Comparing `vessim-0.5.1/vessim/storage.py` & `vessim-0.6.0/vessim/storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from __future__ import annotations
-
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from loguru import logger
 
 
 class Storage(ABC):
     @abstractmethod
     def update(self, power: float, duration: int) -> float:
         """Feed or draw energy for specified duration.
 
         Args:
-            power: Charging if positive, discharging if negative.
+            power: Power to be (dis)charged in W. Charging if positive, discharging if negative.
             duration: Duration in seconds for which the storage will be (dis)charged.
 
         Returns:
-            The power delta, in case not all requested power could be discharged from or
-            charged into the battery. This can happen either if the batter is full/empty
-            or if the C-rate was exceeded.
-            If 0, all power was successfully (dis)charged.
+            The total energy in Ws that has been charged/discharged.
         """
 
-    @abstractmethod
-    def soc(self) -> float:
-        """Returns the current State of Charge (SoC)."""
-
-    @abstractmethod
     def state(self) -> dict:
-        """Returns information about the current state of the storage."""
+        """Returns information about the current state of the storage. Should be overridden."""
+        return {}
 
 
 class SimpleBattery(Storage):
     """(Way too) simple battery.
 
     Args:
-        capacity: Battery capacity in watt-hours (Wh).
-        charge_level: Initial charge level in watt-hours (Wh).
+        capacity: Battery capacity in watt-seconds (Ws).
+        charge_level: Initial charge level in watt-seconds (Ws). Defaults to 0Ws.
         min_soc: Minimum allowed state of charge (SoC) for the battery.
-        c_rate: C-rate, which defines the charge and discharge rate of the battery.
+            Defaults to 0%. Can be altered during simulation.
+        c_rate: Optional C-rate, which defines the charge and discharge rate of the battery.
             For more information on C-rate, see `C-rate explanation <https://www.batterydesign.net/electrical/c-rate/>`_.
+            Defaults to None.
     """
 
     def __init__(
         self,
         capacity: float,
         charge_level: float = 0,
         min_soc: float = 0,
@@ -56,90 +50,54 @@
         self.min_soc = min_soc
         self.c_rate = c_rate
 
     def update(self, power: float, duration: int) -> float:
         if duration <= 0.0:
             raise ValueError("Duration needs to be a positive value")
 
-        max_charge_p_delta, p_delta = 0.0, 0.0
-
+        assert self.min_soc <= self.soc(), "Minimum SoC can not be smaller than the current SoC"
         if self.c_rate is not None:
-            max_rate = self.c_rate * self.capacity / 3600
-            if power >= max_rate:
+            max_power = self.c_rate * self.capacity / 3600
+            if power >= max_power:
+                # Too high charge rate
                 logger.info(
                     f"Trying to charge storage '{self.__class__.__name__}' with "
-                    f"{power} W but only {max_rate} W are supported."
+                    f"{power} W but only {max_power} W are supported."
                 )
-                max_charge_p_delta = power - max_rate
-                power = max_rate
+                power = max_power
 
-            if power <= -max_rate:
+            if power <= -max_power:
+                # Too high discharge rate
                 logger.info(
                     f"Trying to discharge storage '{self.__class__.__name__}' "
-                    f"with {power} W but only {max_rate} W are supported."
+                    f"with {power} W but only {max_power} W are supported."
                 )
-                max_charge_p_delta = power + max_rate
-                power = -self.c_rate
+                power = -max_power
 
-        charge_energy = power * duration
-        new_charge_level = self.charge_level + power * duration
+        charged_energy = power * duration  # Total energy to be (dis)charged in Ws
+        new_charge_level = self.charge_level + charged_energy
 
         abs_min_soc = self.min_soc * self.capacity
         if new_charge_level < abs_min_soc:
-            p_delta = (new_charge_level - abs_min_soc) / duration
+            # Battery can not be discharged further than the minimum state-of-charge
+            charged_energy = abs_min_soc - self.charge_level
             self.charge_level = abs_min_soc
         elif new_charge_level > self.capacity:
-            p_delta = (new_charge_level - self.capacity) / duration
+            # Battery can not be charged past its capacity
+            charged_energy = self.capacity - self.charge_level
             self.charge_level = self.capacity
         else:
-            self.charge_level += charge_energy
+            self.charge_level = new_charge_level
 
-        return p_delta + max_charge_p_delta
+        return charged_energy
 
     def soc(self) -> float:
         return self.charge_level / self.capacity
 
     def state(self) -> dict:
         return {
+            "soc": self.soc(),
             "charge_level": self.charge_level,
             "capacity": self.capacity,
             "min_soc": self.min_soc,
             "c_rate": self.c_rate,
         }
-
-
-class StoragePolicy(ABC):
-    @abstractmethod
-    def apply(self, storage: Storage, p_delta: float, time_since_last_step: int) -> float:
-        """(Dis)charge the storage according to the policy."""
-
-    @abstractmethod
-    def state(self) -> dict:
-        """Returns information about the current state of the storage policy."""
-
-
-class DefaultStoragePolicy(StoragePolicy):
-    """Storage policy which tries to (dis)charge as much of the delta as possible.
-
-    Args:
-        grid_power: If not 0, the battery is in "charge mode" and will draw the
-            provided power from the grid. In this case, the delta simply returned
-            together with the demand for charging.
-    """
-
-    def __init__(self, grid_power: float = 0):
-        self.grid_power = grid_power
-
-    def apply(self, storage: Storage, p_delta: float, time_since_last_step: int) -> float:
-        if self.grid_power == 0:
-            return storage.update(power=p_delta, duration=time_since_last_step)
-        else:
-            excess_energy = storage.update(
-                power=self.grid_power, duration=time_since_last_step
-            )
-            real_charge_power = self.grid_power - excess_energy
-            return p_delta - real_charge_power
-
-    def state(self) -> dict:
-        return {
-            "grid_power": self.grid_power,
-        }
```

### Comparing `vessim-0.5.1/PKG-INFO` & `vessim-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vessim
-Version: 0.5.1
+Version: 0.6.0
 Summary: A simulator for carbon-aware applications and systems.
 Home-page: https://github.com/dos-group/vessim
 License: MIT
 Keywords: simulation,energy system,testbed,carbon-aware computing,software-in-the-loop
 Author: Philipp Wiesner
 Author-email: wiesner@tu-berlin.de
 Requires-Python: >=3.8,<3.13
@@ -19,23 +19,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Testing
 Provides-Extra: sil
-Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "sil"
+Requires-Dist: docopt-ng (>=0.6.2,<0.7.0)
 Requires-Dist: fastapi (>=0.104.0,<0.105.0) ; extra == "sil"
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: mosaik (>=3.2.0,<4.0.0)
 Requires-Dist: mosaik-api-v3 (>=3.0.4,<4.0.0)
 Requires-Dist: numpy (>=1.22.0,<2.0.0) ; python_version < "3.12"
 Requires-Dist: numpy (>=1.26.0,<2.0.0) ; python_version >= "3.12"
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: redis (>=5.0.0,<6.0.0) ; extra == "sil"
 Requires-Dist: requests (>=2.26.0,<3.0.0) ; extra == "sil"
 Requires-Dist: uvicorn (>=0.23.0,<0.24.0) ; extra == "sil"
 Project-URL: Bug Reports, https://github.com/dos-group/vessim/issues
 Project-URL: Documentation, https://github.com/dos-group/vessim
 Project-URL: Repository, https://github.com/dos-group/vessim
 Description-Content-Type: text/markdown
```

