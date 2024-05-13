# Comparing `tmp/janus_core-0.3.0b1.tar.gz` & `tmp/janus_core-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.3.0b1.tar", max compression
+gzip compressed data, was "janus_core-0.4.0b0.tar", max compression
```

## Comparing `janus_core-0.3.0b1.tar` & `janus_core-0.4.0b0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1533 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/LICENSE
--rw-r--r--   0        0        0     9036 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/README.md
--rw-r--r--   0        0        0      132 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/__init__.py
--rw-r--r--   0        0        0     4814 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/calculations/geom_opt.py
--rw-r--r--   0        0        0    34723 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/calculations/md.py
--rw-r--r--   0        0        0    12143 2024-04-29 13:16:03.595586 janus_core-0.3.0b1/janus_core/calculations/single_point.py
--rw-r--r--   0        0        0     6958 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/geomopt.py
--rw-r--r--   0        0        0      839 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/janus.py
--rw-r--r--   0        0        0    13206 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/md.py
--rw-r--r--   0        0        0     5203 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/singlepoint.py
--rw-r--r--   0        0        0     3481 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/types.py
--rw-r--r--   0        0        0     3274 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/cli/utils.py
--rw-r--r--   0        0        0     1686 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/janus_types.py
--rw-r--r--   0        0        0     4053 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/log.py
--rw-r--r--   0        0        0     3532 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/mlip_calculators.py
--rw-r--r--   0        0        0     5838 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/stats.py
--rw-r--r--   0        0        0     1544 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/janus_core/helpers/utils.py
--rw-r--r--   0        0        0     2558 2024-04-29 13:16:03.599586 janus_core-0.3.0b1/pyproject.toml
--rw-r--r--   0        0        0    10095 1970-01-01 00:00:00.000000 janus_core-0.3.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-13 13:13:50.085032 janus_core-0.4.0b0/LICENSE
+-rw-r--r--   0        0        0     9907 2024-05-13 13:13:50.085032 janus_core-0.4.0b0/README.md
+-rw-r--r--   0        0        0      132 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/__init__.py
+-rw-r--r--   0        0        0     4814 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/calculations/geom_opt.py
+-rw-r--r--   0        0        0    36040 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/calculations/md.py
+-rw-r--r--   0        0        0    12143 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/calculations/single_point.py
+-rw-r--r--   0        0        0     6958 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/geomopt.py
+-rw-r--r--   0        0        0     1000 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/janus.py
+-rw-r--r--   0        0        0    13636 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/md.py
+-rw-r--r--   0        0        0     5203 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/singlepoint.py
+-rw-r--r--   0        0        0     1701 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/train.py
+-rw-r--r--   0        0        0     3481 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/types.py
+-rw-r--r--   0        0        0     3274 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/cli/utils.py
+-rw-r--r--   0        0        0     1686 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/janus_types.py
+-rw-r--r--   0        0        0     4053 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/log.py
+-rw-r--r--   0        0        0     3532 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/mlip_calculators.py
+-rw-r--r--   0        0        0     5838 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/stats.py
+-rw-r--r--   0        0        0     2272 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/train.py
+-rw-r--r--   0        0        0     1544 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/janus_core/helpers/utils.py
+-rw-r--r--   0        0        0     2558 2024-05-13 13:13:50.089032 janus_core-0.4.0b0/pyproject.toml
+-rw-r--r--   0        0        0    10966 1970-01-01 00:00:00.000000 janus_core-0.4.0b0/PKG-INFO
```

### Comparing `janus_core-0.3.0b1/LICENSE` & `janus_core-0.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/README.md` & `janus_core-0.4.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 - [x] Molecular Dynamics
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
 - [ ] Nudge Elastic Band
 - [ ] Phonons
   - vibroscopy
-- [ ] Training ML potentials
+- [x] Training ML potentials
   - MACE
-- [ ] Fine tunning MLIPs
+- [x] Fine tunning MLIPs
   - MACE
 - [ ] Rare events simulations
   - PLUMED
 
 The code relies heavily on ASE, unless something else is mentioned.
 
 ## Development
@@ -194,14 +194,34 @@
 This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
 
 
 > [!NOTE]
 > `properties` must be passed as a Yaml list, as above, not as a string.
 
 
+### Training and fine-tuning MACE models
+
+> [!NOTE]
+> This currently requires use of the [develop branch of MACE](https://github.com/ACEsuit/mace/tree/develop).
+> This can be installed by running `poetry add git+https://github.com/ACEsuit/mace.git#develop`, followed by `poetry install`.
+
+MACE models can be trained by passing a configuration file to the [MACE CLI](https://github.com/ACEsuit/mace/blob/main/mace/cli/run_train.py):
+
+```shell
+janus train --mlip-config /path/to/training/config.yml
+```
+
+This will create `logs`, `checkpoints` and `results` folders, as well as saving the trained model, and a compiled version of the model.
+
+Foundational models can also be fine-tuned, by including the `foundation_model` option in your configuration file, and using `--fine-tune` option:
+
+```shell
+janus train --mlip-config /path/to/fine/tuning/config.yml --fine-tune
+```
+
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
 
 Contributors to this project were funded by
```

### Comparing `janus_core-0.3.0b1/janus_core/calculations/geom_opt.py` & `janus_core-0.4.0b0/janus_core/calculations/geom_opt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/calculations/md.py` & `janus_core-0.4.0b0/janus_core/calculations/md.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=too-many-lines
 """Run molecular dynamics simulations."""
 
 import datetime
+from math import isclose
 from pathlib import Path
 import random
 from typing import Any, Optional
 from warnings import warn
 
 from ase import Atoms, units
 from ase.io import write
@@ -288,24 +289,33 @@
 
         # Check temperatures for heating differ
         if self.temp_start is not None and self.temp_start == self.temp_end:
             raise ValueError("Start and end temperatures must be different")
 
         # Warn if mix of None and not None
         self.ramp_temp = (
-            self.temp_start and self.temp_end and self.temp_step and self.temp_time
+            self.temp_start is not None
+            and self.temp_end is not None
+            and self.temp_step
+            and self.temp_time
         )
         if (
-            self.temp_start or self.temp_end or self.temp_step or self.temp_time
+            self.temp_start is not None
+            or self.temp_end is not None
+            or self.temp_step
+            or self.temp_time
         ) and not self.ramp_temp:
             warn(
                 "`temp_start`, `temp_end` and `temp_step` must all be specified for "
                 "heating to run"
             )
 
+        if self.ramp_temp and (self.temp_start < 0 or self.temp_end < 0):
+            raise ValueError("Start and end temperatures must be positive")
+
         self.minimize_kwargs = minimize_kwargs if minimize_kwargs else {}
         self.restart_files = []
         self.dyn = None
         self.n_atoms = len(self.struct)
 
         # Infer names for structure and if not specified
         if not self.struct_name:
@@ -331,20 +341,24 @@
     def _set_velocity_distribution(self) -> None:
         """
         Set velocities to current target temperature.
 
         Sets Maxwell-Boltzmann velocity distribution, as well as removing
         centre-of-mass momentum, and (optionally) total angular momentum.
         """
-        MaxwellBoltzmannDistribution(self.struct, temperature_K=self.temp)
-        Stationary(self.struct)
+        atoms = self.struct
+        if self.dyn.nsteps >= 0:
+            atoms = self.dyn.atoms
+
+        MaxwellBoltzmannDistribution(atoms, temperature_K=self.temp)
+        Stationary(atoms)
         if self.logger:
             self.logger.info("Velocities reset at step %s", self.dyn.nsteps)
         if self.remove_rot:
-            ZeroRotation(self.struct)
+            ZeroRotation(atoms)
             if self.logger:
                 self.logger.info("Rotation reset at step %s", self.dyn.nsteps)
 
     def _reset_velocities(self) -> None:
         """Reset velocities and (optionally) rotation of system while equilibrating."""
         if self.dyn.nsteps < self.equil_steps:
             self._set_velocity_distribution()
@@ -369,15 +383,15 @@
         Returns
         -------
         str
            Formatted temperature range if heating and target temp if running md.
         """
 
         temperature_prefix = ""
-        if self.temp_start and self.temp_end:
+        if self.temp_start is not None and self.temp_end is not None:
             temperature_prefix = f"-T{self.temp_start}-T{self.temp_end}"
 
         if self.steps > 0:
             temperature_prefix += f"-T{self.temp}"
 
         return temperature_prefix
 
@@ -597,31 +611,48 @@
         # Set velocities to match current temperature
         self._set_velocity_distribution()
 
         # Run temperature ramp
         if self.ramp_temp:
             heating_steps = int(self.temp_time // self.timestep)
 
-            n_temps = int(1 + (self.temp_end - self.temp_start) // self.temp_step)
-            temps = [self.temp_start + i * self.temp_step for i in range(n_temps)]
+            # Always include start temperature in ramp, and include end temperature
+            # if separated by an integer number of temperature steps
+            n_temps = int(1 + abs(self.temp_end - self.temp_start) // self.temp_step)
+
+            # Add or subtract temperatures
+            ramp_sign = 1 if (self.temp_end - self.temp_start) > 0 else -1
+            temps = [
+                self.temp_start + ramp_sign * i * self.temp_step for i in range(n_temps)
+            ]
 
             if self.logger:
                 self.logger.info("Beginning temperature ramp at %sK", temps[0])
             for temp in temps:
                 self.temp = temp
+                self._set_velocity_distribution()
+                if isclose(temp, 0.0):
+                    self._write_final_state()
+                    continue
+                if not isinstance(self, NVE):
+                    self.dyn.set_temperature(temperature_K=self.temp)
                 self.dyn.run(heating_steps)
                 self._write_final_state()
             if self.logger:
                 self.logger.info("Temperature ramp complete at %sK", temps[-1])
 
         # Run MD
         if self.steps > 0:
             if self.logger:
                 self.logger.info("Starting molecular dynamics simulation")
             self.temp = md_temp
+            if self.ramp_temp:
+                self._set_velocity_distribution()
+                if not isinstance(self, NVE):
+                    self.dyn.set_temperature(temperature_K=self.temp)
             self.dyn.run(self.steps)
             self._write_final_state()
             if self.logger:
                 self.logger.info("Molecular dynamics simulation complete")
 
 
 class NPT(MolecularDynamics):
@@ -688,20 +719,24 @@
         **kwargs
             Additional keyword arguments.
         """
         self.pressure = pressure
         super().__init__(ensemble=ensemble, file_prefix=file_prefix, *args, **kwargs)
 
         self.ttime = thermostat_time * units.fs
-        scaled_bulk_modulus = bulk_modulus * units.GPa
+
         if barostat_time:
-            pfactor = (barostat_time * units.fs) ** 2 * scaled_bulk_modulus
+            pfactor = barostat_time**2 * bulk_modulus
+            if self.logger:
+                self.logger.info("NPT pfactor=%s GPa fs^2", pfactor)
+
+            # convert the pfactor to ASE internal units
+            pfactor *= units.fs**2 * units.GPa
         else:
             pfactor = None
-
         self.dyn = ASE_NPT(
             self.struct,
             timestep=self.timestep,
             temperature_K=self.temp,
             ttime=self.ttime,
             pfactor=pfactor,
             append_trajectory=self.traj_append,
```

### Comparing `janus_core-0.3.0b1/janus_core/calculations/single_point.py` & `janus_core-0.4.0b0/janus_core/calculations/single_point.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/cli/geomopt.py` & `janus_core-0.4.0b0/janus_core/cli/geomopt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/cli/janus.py` & `janus_core-0.4.0b0/janus_core/cli/janus.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 from janus_core.cli.md import md
 from janus_core.cli.singlepoint import singlepoint
 
 app = Typer(name="janus", no_args_is_help=True)
 app.command()(singlepoint)
 app.command()(geomopt)
 app.command()(md)
+# Train not imlpemented in older versions of MACE
+try:
+    from janus_core.cli.train import train
+
+    app.command()(train)
+except NotImplementedError:
+    pass
 
 
 @app.callback(invoke_without_command=True, help="")
 def print_version(
     version: Annotated[
         bool, Option("--version", help="Print janus version and exit.")
     ] = None,
```

### Comparing `janus_core-0.3.0b1/janus_core/cli/md.py` & `janus_core-0.4.0b0/janus_core/cli/md.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,25 @@
 @use_config(yaml_converter_callback)
 def md(
     # pylint: disable=too-many-arguments,too-many-locals,invalid-name,duplicate-code
     # numpydoc ignore=PR02
     ctx: Context,
     ensemble: Annotated[str, Option(help="Name of thermodynamic ensemble.")],
     struct: StructPath,
+    struct_name: Annotated[
+        str,
+        Option(
+            help=(
+                """
+                Name of structure to simulate. Default is inferred from filepath or
+                chemical formula.
+                """
+            )
+        ),
+    ] = None,
     steps: Annotated[int, Option(help="Number of steps in simulation.")] = 0,
     timestep: Annotated[float, Option(help="Timestep for integrator, in fs.")] = 1.0,
     temp: Annotated[float, Option(help="Temperature, in K.")] = 300.0,
     thermostat_time: Annotated[
         float,
         Option(
             help="Thermostat time for NPT, NVT Nosé-Hoover, or NPH simulation, in fs."
@@ -170,14 +181,17 @@
     ----------
     ctx : Context
         Typer (Click) Context. Automatically set.
     ensemble : str
         Name of thermodynamic ensemble.
     struct : Path
         Path of structure to simulate.
+    struct_name : str
+        Name of structure to simulate. Default is inferred from filepath or chemical
+        formula.
     steps : int
         Number of steps in simulation. Default is 0.
     timestep : float
         Timestep for integrator, in fs. Default is 1.0.
     temp : float
         Temperature, in K. Default is 300.
     thermostat_time : float
@@ -271,14 +285,15 @@
 
     if not ensemble in get_args(Ensembles):
         raise ValueError(f"ensemble must be in {get_args(Ensembles)}")
 
     # Set up single point calculator
     s_point = SinglePoint(
         struct_path=struct,
+        struct_name=struct_name,
         architecture=arch,
         device=device,
         read_kwargs=read_kwargs,
         calc_kwargs=calc_kwargs,
         log_kwargs={"filename": log, "filemode": "w"},
     )
```

### Comparing `janus_core-0.3.0b1/janus_core/cli/singlepoint.py` & `janus_core-0.4.0b0/janus_core/cli/singlepoint.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/cli/types.py` & `janus_core-0.4.0b0/janus_core/cli/types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/cli/utils.py` & `janus_core-0.4.0b0/janus_core/cli/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/helpers/janus_types.py` & `janus_core-0.4.0b0/janus_core/helpers/janus_types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/helpers/log.py` & `janus_core-0.4.0b0/janus_core/helpers/log.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/helpers/mlip_calculators.py` & `janus_core-0.4.0b0/janus_core/helpers/mlip_calculators.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/helpers/stats.py` & `janus_core-0.4.0b0/janus_core/helpers/stats.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/janus_core/helpers/utils.py` & `janus_core-0.4.0b0/janus_core/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.3.0b1/pyproject.toml` & `janus_core-0.4.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.3.0b1"
+version = "0.4.0b0"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
```

### Comparing `janus_core-0.3.0b1/PKG-INFO` & `janus_core-0.4.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.3.0b1
+Version: 0.4.0b0
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -48,17 +48,17 @@
 - [x] Molecular Dynamics
   - NVE
   - NVT (Langevin(Eijnden/Ciccotti flavour) and Nosé-Hoover (Melchionna flavour))
   - NPT (Nosé-Hoover (Melchiona flavour))
 - [ ] Nudge Elastic Band
 - [ ] Phonons
   - vibroscopy
-- [ ] Training ML potentials
+- [x] Training ML potentials
   - MACE
-- [ ] Fine tunning MLIPs
+- [x] Fine tunning MLIPs
   - MACE
 - [ ] Rare events simulations
   - PLUMED
 
 The code relies heavily on ASE, unless something else is mentioned.
 
 ## Development
@@ -220,14 +220,34 @@
 This will run a singlepoint energy calculation on `KCl.cif` using the [MACE-MP](https://github.com/ACEsuit/mace-mp) "medium" force-field, saving the results to `KCl-results.cif`.
 
 
 > [!NOTE]
 > `properties` must be passed as a Yaml list, as above, not as a string.
 
 
+### Training and fine-tuning MACE models
+
+> [!NOTE]
+> This currently requires use of the [develop branch of MACE](https://github.com/ACEsuit/mace/tree/develop).
+> This can be installed by running `poetry add git+https://github.com/ACEsuit/mace.git#develop`, followed by `poetry install`.
+
+MACE models can be trained by passing a configuration file to the [MACE CLI](https://github.com/ACEsuit/mace/blob/main/mace/cli/run_train.py):
+
+```shell
+janus train --mlip-config /path/to/training/config.yml
+```
+
+This will create `logs`, `checkpoints` and `results` folders, as well as saving the trained model, and a compiled version of the model.
+
+Foundational models can also be fine-tuned, by including the `foundation_model` option in your configuration file, and using `--fine-tune` option:
+
+```shell
+janus train --mlip-config /path/to/fine/tuning/config.yml --fine-tune
+```
+
 ## License
 
 [BSD 3-Clause License](LICENSE)
 
 ## Funding
 
 Contributors to this project were funded by
```

