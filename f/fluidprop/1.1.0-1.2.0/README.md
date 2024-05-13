# Comparing `tmp/fluidprop-1.1.0.tar.gz` & `tmp/fluidprop-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidprop-1.1.0.tar", last modified: Sun May 12 12:14:57 2024, max compression
+gzip compressed data, was "fluidprop-1.2.0.tar", last modified: Mon May 13 13:56:15 2024, max compression
```

## Comparing `fluidprop-1.1.0.tar` & `fluidprop-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 12:14:57.521348 fluidprop-1.1.0/
--rw-rw-rw-   0        0        0       76 2024-05-11 11:03:33.000000 fluidprop-1.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0      220 2024-05-12 12:04:18.000000 fluidprop-1.1.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1098 2024-05-11 11:03:33.000000 fluidprop-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      289 2020-07-01 17:41:38.000000 fluidprop-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9690 2024-05-12 12:14:57.520350 fluidprop-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2024-05-12 12:06:40.000000 fluidprop-1.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-12 12:14:57.521348 fluidprop-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2349 2024-05-12 11:55:11.000000 fluidprop-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:14:57.514347 fluidprop-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 12:14:57.519348 fluidprop-1.1.0/src/fluidprop.egg-info/
--rw-rw-rw-   0        0        0     9690 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 21:28:56.000000 fluidprop-1.1.0/src/fluidprop.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 12:14:57.000000 fluidprop-1.1.0/src/fluidprop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17154 2024-05-12 12:06:46.000000 fluidprop-1.1.0/src/fluidprop.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:56:15.778072 fluidprop-1.2.0/
+-rw-rw-rw-   0        0        0       76 2024-05-11 11:03:33.000000 fluidprop-1.2.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0      475 2024-05-13 13:54:41.000000 fluidprop-1.2.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1098 2024-05-11 11:03:33.000000 fluidprop-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      289 2020-07-01 17:41:38.000000 fluidprop-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10187 2024-05-13 13:56:15.778072 fluidprop-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8533 2024-05-13 13:54:41.000000 fluidprop-1.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:56:15.779073 fluidprop-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2349 2024-05-13 13:54:41.000000 fluidprop-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:56:15.772075 fluidprop-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 13:56:15.777074 fluidprop-1.2.0/src/fluidprop.egg-info/
+-rw-rw-rw-   0        0        0    10187 2024-05-13 13:56:15.000000 fluidprop-1.2.0/src/fluidprop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-13 13:56:15.000000 fluidprop-1.2.0/src/fluidprop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:56:15.000000 fluidprop-1.2.0/src/fluidprop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 13:56:15.000000 fluidprop-1.2.0/src/fluidprop.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-05-13 13:56:15.000000 fluidprop-1.2.0/src/fluidprop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 13:56:15.000000 fluidprop-1.2.0/src/fluidprop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17472 2024-05-13 13:54:41.000000 fluidprop-1.2.0/src/fluidprop.py
+-rw-rw-rw-   0        0        0    11021 2024-05-13 13:54:41.000000 fluidprop-1.2.0/src/rbc.py
```

### Comparing `fluidprop-1.1.0/LICENSE.txt` & `fluidprop-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidprop-1.1.0/PKG-INFO` & `fluidprop-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidprop
-Version: 1.1.0
+Version: 1.2.0
 Summary: Easy access to thermodynamic fluid properties as a function of temperature and pressure. With a minimal command-line interface.
 Home-page: https://github.com/Dennis-van-Gils/python-fluidprop/
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-fluidprop/issues
 Keywords: CoolProp,fluids,thermodynamic
@@ -55,16 +55,16 @@
 
     pip3 install fluidprop
 
 EOS models
 ----------
 
 Thermodynamic properties are provided by CoolProp, the open-source alternative
-to `NIST refprop <https://www.nist.gov/srd/refprop>`_, with most of the calculations relying on the same
-equation-of-state (EOS) models as refprop.
+to `NIST refprop <https://www.nist.gov/srd/refprop>`_, with most of the
+calculations relying on the same equation-of-state (EOS) models as refprop.
 
 * http://www.coolprop.org/
 * http://pubs.acs.org/doi/abs/10.1021/ie4033999
 
 Command-line interface
 ======================
 
@@ -76,15 +76,22 @@
 
     python3 -m fluidprop
 
 It will show a minimal command-line interface which guides the user to enter a
 fluid, temperature and pressure. It will print out its thermodynamic properties
 as a table to the terminal.
 
-Example output::
+BONUS for the Rayleigh-Bénard convection community. Running::
+
+    python -m rbc
+
+will show a command-line interface acting as a 'pocket calculator' to calculate
+the Rayleigh and other numbers based on the user input.
+
+Example output of `fluidprop`::
 
     https://github.com/Dennis-van-Gils/python-fluidprop
     Thermodynamic properties by CoolProp v6.6.0
     http://pubs.acs.org/doi/abs/10.1021/ie4033999
 
     All known fluids:
         0 | 1-Butene             41 | MD4M                 82 | R1233zd(E)
@@ -214,20 +221,26 @@
 
     Cv      (ndarray): Isochoric heat capacity        [J/(kg K)]
 
     comp    (ndarray): Isothermal compressibility     [1/Pa]
 
     Pr      (ndarray): Prandtl number                 [-]
 
-Dennis van Gils, 12-05-2024
+Dennis van Gils, 13-05-2024
 
 Changelog
 =========
 
+1.2.0 (2024-05-13)
+------------------
+* Added ``rbc.py``: A quick 'pocket calculator' for Rayleigh-Bénard Convection.
+* ``show_cli()`` will not show an end report by itself anymore. You'll have to
+  call ``report()`` afterwards yourselves.
+
 1.1.0 (2024-05-12)
 ------------------
-* Added field `Cv`: Isochoric heat capacity
-* Added field `comp`: Isothermal compressibility
+* Added field ``Cv``: Isochoric heat capacity.
+* Added field ``comp``: Isothermal compressibility.
 
 1.0.0 (2024-05-11)
 ------------------
-* Initial release
+* Initial release.
```

### Comparing `fluidprop-1.1.0/README.rst` & `fluidprop-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
     pip3 install fluidprop
 
 EOS models
 ----------
 
 Thermodynamic properties are provided by CoolProp, the open-source alternative
-to `NIST refprop <https://www.nist.gov/srd/refprop>`_, with most of the calculations relying on the same
-equation-of-state (EOS) models as refprop.
+to `NIST refprop <https://www.nist.gov/srd/refprop>`_, with most of the
+calculations relying on the same equation-of-state (EOS) models as refprop.
 
 * http://www.coolprop.org/
 * http://pubs.acs.org/doi/abs/10.1021/ie4033999
 
 Command-line interface
 ======================
 
@@ -48,15 +48,22 @@
 
     python3 -m fluidprop
 
 It will show a minimal command-line interface which guides the user to enter a
 fluid, temperature and pressure. It will print out its thermodynamic properties
 as a table to the terminal.
 
-Example output::
+BONUS for the Rayleigh-Bénard convection community. Running::
+
+    python -m rbc
+
+will show a command-line interface acting as a 'pocket calculator' to calculate
+the Rayleigh and other numbers based on the user input.
+
+Example output of `fluidprop`::
 
     https://github.com/Dennis-van-Gils/python-fluidprop
     Thermodynamic properties by CoolProp v6.6.0
     http://pubs.acs.org/doi/abs/10.1021/ie4033999
 
     All known fluids:
         0 | 1-Butene             41 | MD4M                 82 | R1233zd(E)
@@ -186,8 +193,8 @@
 
     Cv      (ndarray): Isochoric heat capacity        [J/(kg K)]
 
     comp    (ndarray): Isothermal compressibility     [1/Pa]
 
     Pr      (ndarray): Prandtl number                 [-]
 
-Dennis van Gils, 12-05-2024
+Dennis van Gils, 13-05-2024
```

### Comparing `fluidprop-1.1.0/setup.py` & `fluidprop-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ) as fh:
         return fh.read()
 
 
 setup(
     name="fluidprop",
     license="MIT",
-    version="1.1.0",
+    version="1.2.0",
     description="Easy access to thermodynamic fluid properties as a function of temperature and pressure. With a minimal command-line interface.",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
```

### Comparing `fluidprop-1.1.0/src/fluidprop.egg-info/PKG-INFO` & `fluidprop-1.2.0/src/fluidprop.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidprop
-Version: 1.1.0
+Version: 1.2.0
 Summary: Easy access to thermodynamic fluid properties as a function of temperature and pressure. With a minimal command-line interface.
 Home-page: https://github.com/Dennis-van-Gils/python-fluidprop/
 Author: Dennis van Gils
 Author-email: vangils.dennis@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Dennis-van-Gils/python-fluidprop/issues
 Keywords: CoolProp,fluids,thermodynamic
@@ -55,16 +55,16 @@
 
     pip3 install fluidprop
 
 EOS models
 ----------
 
 Thermodynamic properties are provided by CoolProp, the open-source alternative
-to `NIST refprop <https://www.nist.gov/srd/refprop>`_, with most of the calculations relying on the same
-equation-of-state (EOS) models as refprop.
+to `NIST refprop <https://www.nist.gov/srd/refprop>`_, with most of the
+calculations relying on the same equation-of-state (EOS) models as refprop.
 
 * http://www.coolprop.org/
 * http://pubs.acs.org/doi/abs/10.1021/ie4033999
 
 Command-line interface
 ======================
 
@@ -76,15 +76,22 @@
 
     python3 -m fluidprop
 
 It will show a minimal command-line interface which guides the user to enter a
 fluid, temperature and pressure. It will print out its thermodynamic properties
 as a table to the terminal.
 
-Example output::
+BONUS for the Rayleigh-Bénard convection community. Running::
+
+    python -m rbc
+
+will show a command-line interface acting as a 'pocket calculator' to calculate
+the Rayleigh and other numbers based on the user input.
+
+Example output of `fluidprop`::
 
     https://github.com/Dennis-van-Gils/python-fluidprop
     Thermodynamic properties by CoolProp v6.6.0
     http://pubs.acs.org/doi/abs/10.1021/ie4033999
 
     All known fluids:
         0 | 1-Butene             41 | MD4M                 82 | R1233zd(E)
@@ -214,20 +221,26 @@
 
     Cv      (ndarray): Isochoric heat capacity        [J/(kg K)]
 
     comp    (ndarray): Isothermal compressibility     [1/Pa]
 
     Pr      (ndarray): Prandtl number                 [-]
 
-Dennis van Gils, 12-05-2024
+Dennis van Gils, 13-05-2024
 
 Changelog
 =========
 
+1.2.0 (2024-05-13)
+------------------
+* Added ``rbc.py``: A quick 'pocket calculator' for Rayleigh-Bénard Convection.
+* ``show_cli()`` will not show an end report by itself anymore. You'll have to
+  call ``report()`` afterwards yourselves.
+
 1.1.0 (2024-05-12)
 ------------------
-* Added field `Cv`: Isochoric heat capacity
-* Added field `comp`: Isothermal compressibility
+* Added field ``Cv``: Isochoric heat capacity.
+* Added field ``comp``: Isothermal compressibility.
 
 1.0.0 (2024-05-11)
 ------------------
-* Initial release
+* Initial release.
```

### Comparing `fluidprop-1.1.0/src/fluidprop.py` & `fluidprop-1.2.0/src/fluidprop.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 Thermodynamic properties are provided by CoolProp:
 * http://www.coolprop.org/
 * http://pubs.acs.org/doi/abs/10.1021/ie4033999
 """
 __author__ = "Dennis van Gils"
 __authoremail__ = "vangils.dennis@gmail.com"
 __url__ = "https://github.com/Dennis-van-Gils/python-fluidprop"
-__date__ = "12-05-2024"
-__version__ = "1.1.0"
+__date__ = "13-05-2024"
+__version__ = "1.2.0"
 
 import re
 from typing import Union
 
 import numpy.typing as npt
 import numpy as np
 import CoolProp
@@ -360,18 +360,25 @@
         text,
     )
 
     return text
 
 
 # ------------------------------------------------------------------------------
-#   main
+#   show_cli
 # ------------------------------------------------------------------------------
 
-if __name__ == "__main__":
+
+def show_cli() -> FluidProperties:
+    """Show a minimal command-line interface which guides the user to enter a
+    fluid, temperature and pressure.
+
+    Returns:
+        The resulting `FluidProperties()` class instance.
+    """
     print(__url__)
     print(f"Thermodynamic properties by CoolProp v{CoolProp.__version__}")
     print("http://pubs.acs.org/doi/abs/10.1021/ie4033999")
 
     # Table of predefined subselection of fluids
     table_1 = ""
     for idx, item in enumerate(FLUID_SELECTION):
@@ -505,19 +512,22 @@
             except ValueError:
                 print("Not a valid number.")
                 continue
 
         # Made it successfully till the end
         break
 
-    # ----------------------------------
-    #   Calculate and report to screen
-    # ----------------------------------
-
-    fluid = FluidProperties(
+    return FluidProperties(
         coolprop_name=fluid_name,
         T_in_deg_C=temperature_deg_C,
         P_in_bar=pressure_bar,
     )
 
+
+# ------------------------------------------------------------------------------
+#   main
+# ------------------------------------------------------------------------------
+
+if __name__ == "__main__":
+    fluid = show_cli()
     print()
     fluid.report()
```

