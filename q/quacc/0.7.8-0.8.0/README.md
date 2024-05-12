# Comparing `tmp/quacc-0.7.8.tar.gz` & `tmp/quacc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.8.tar", last modified: Thu May  9 23:37:59 2024, max compression
+gzip compressed data, was "quacc-0.8.0.tar", last modified: Sun May 12 22:33:18 2024, max compression
```

## Comparing `quacc-0.7.8.tar` & `quacc-0.8.0.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:59.001201 quacc-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-09 23:36:36.000000 quacc-0.7.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 23:36:36.000000 quacc-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-05-09 23:37:59.001201 quacc-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-09 23:36:36.000000 quacc-0.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-09 23:36:36.000000 quacc-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:37:59.001201 quacc-0.7.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.969201 quacc-0.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.977201 quacc-0.7.8/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.977201 quacc-0.7.8/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.977201 quacc-0.7.8/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.435920 quacc-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-12 22:31:57.000000 quacc-0.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 22:31:57.000000 quacc-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-12 22:33:18.435920 quacc-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-12 22:31:57.000000 quacc-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-12 22:31:57.000000 quacc-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 22:33:18.435920 quacc-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.403920 quacc-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.407920 quacc-0.8.0/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.407920 quacc-0.8.0/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.411920 quacc-0.8.0/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.415920 quacc-0.8.0/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.419920 quacc-0.8.0/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.423920 quacc-0.8.0/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.427920 quacc-0.8.0/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17135 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-12 22:31:57.000000 quacc-0.8.0/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:33:18.431920 quacc-0.8.0/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 22:33:18.000000 quacc-0.8.0/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.8/LICENSE.md` & `quacc-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/PKG-INFO` & `quacc-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.8
+Version: 0.8.0
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
 Keywords: high-throughput,automated,workflow,dft
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ase>3.22.1
+Requires-Dist: ase>=3.23.0b1
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
-Requires-Dist: covalent>=0.234.0rc0; platform_system != "Windows" and extra == "covalent"
+Requires-Dist: covalent>=0.234.1-rc.0; platform_system != "Windows" and extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; platform_system != "Windows" and extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
 Provides-Extra: defects
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22; extra == "defects"
 Requires-Dist: shakenbreak>=3.2.0; extra == "defects"
@@ -51,15 +51,15 @@
 Requires-Dist: jobflow-remote>=0.1.0; extra == "jobflow"
 Provides-Extra: mlp
 Requires-Dist: matgl>=1.0.0; extra == "mlp"
 Requires-Dist: chgnet>=0.3.3; extra == "mlp"
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
 Provides-Extra: mp
-Requires-Dist: pymatgen-io-validation>=0.0.1; extra == "mp"
+Requires-Dist: atomate2>=0.0.14; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
 Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
```

### Comparing `quacc-0.7.8/README.md` & `quacc-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/pyproject.toml` & `quacc-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.8"
+version = "0.8.0"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: Unix",
     "Operating System :: MacOS",
 ]
-requires-python = ">=3.9, <3.13"
+requires-python = ">=3.9"
 dependencies = [
-    "ase>3.22.1", # for Atoms object and calculators
+    "ase>=3.23.0b1", # for Atoms object and calculators
     "cclib>=1.8", # for I/O parsing of molecular DFT codes
     "custodian>=2024.3.12", # for automated error corrections
     "emmet-core>=0.80.0", # for pre-made schemas
     "maggma>=0.64.0", # for database handling
     "monty>=2024.2.26", # miscellaneous Python utilities
     "numpy>=1.25.0", # for array handling
     "psutil", # for getting compute architecture details
@@ -39,20 +39,20 @@
     "pydantic-settings>=2.2.0", # for settings management
     "pymatgen>=2024.4.13", # for structure manipulation
     "ruamel.yaml>=0.17.40", # for YAML
     "typer>=0.12.1", # for the CLI
 ]
 
 [project.optional-dependencies]
-covalent = ["covalent>=0.234.0rc0; platform_system!='Windows'", "covalent-cloud>=0.39.0; platform_system!='Windows'"]
+covalent = ["covalent>=0.234.1-rc.0; platform_system!='Windows'", "covalent-cloud>=0.39.0; platform_system!='Windows'"]
 dask = ["dask[distributed]>=2023.12.1", "dask-jobqueue>=0.8.2"]
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
 jobflow = ["jobflow[fireworks]>=0.1.14", "jobflow-remote>=0.1.0"]
 mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0"]
-mp = ["pymatgen-io-validation>=0.0.1"]
+mp = ["atomate2>=0.0.14"]
 newtonnet = ["newtonnet>=1.1"]
 parsl = ["parsl[monitoring]>=2023.10.23; platform_system!='Windows'"]
 phonons = ["phonopy>=2.20.0", "seekpath>=2.1.0"]
 prefect = ["prefect>=2.14.14", "prefect-dask>=0.2.6", "dask-jobqueue>=0.8.2"]
 redun = ["redun>=0.16.2"]
 sella = ["sella>=2.3.3"]
 tblite = ["tblite>=0.3.0; platform_system=='Linux'"]
```

### Comparing `quacc-0.7.8/src/quacc/__init__.py` & `quacc-0.8.0/src/quacc/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 
 import logging
 from importlib.metadata import version
 
 from ase.atoms import Atoms
 from pymatgen.io.ase import MSONAtoms
 
-from quacc.settings import QuaccSettings
+from quacc.settings import QuaccSettings, change_settings
 from quacc.utils.dicts import Remove
 from quacc.wflow_tools.customizers import redecorate, strip_decorator
 from quacc.wflow_tools.decorators import Flow, Job, Subflow, flow, job, subflow
 
 __all__ = [
     "flow",
     "job",
     "subflow",
     "Flow",
     "Job",
     "Subflow",
     "redecorate",
+    "change_settings",
     "strip_decorator",
     "Remove",
 ]
 
 
 # Load the quacc version
 __version__ = version("quacc")
```

### Comparing `quacc-0.7.8/src/quacc/_cli/quacc.py` & `quacc-0.8.0/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/atoms/core.py` & `quacc-0.8.0/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/atoms/defects.py` & `quacc-0.8.0/src/quacc/atoms/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/atoms/deformation.py` & `quacc-0.8.0/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/atoms/phonons.py` & `quacc-0.8.0/src/quacc/atoms/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/atoms/slabs.py` & `quacc-0.8.0/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/espresso/espresso.py` & `quacc-0.8.0/src/quacc/calculators/espresso/espresso.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.8.0/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.8.0/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/espresso/utils.py` & `quacc-0.8.0/src/quacc/calculators/espresso/utils.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/qchem/io.py` & `quacc-0.8.0/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/qchem/params.py` & `quacc-0.8.0/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/qchem/qchem.py` & `quacc-0.8.0/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.8.0/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/io.py` & `quacc-0.8.0/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/params.py` & `quacc-0.8.0/src/quacc/calculators/vasp/params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """Parameter-related utilities for the Vasp calculator."""
 
 from __future__ import annotations
 
 import logging
+from importlib import util
 from typing import TYPE_CHECKING
 
 import numpy as np
 from ase.calculators.vasp import Vasp as Vasp_
+from monty.dev import requires
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from quacc.atoms.core import check_is_metal
 from quacc.utils.kpts import convert_pmg_kpts
 
+has_atomate2 = util.find_spec("atomate2")
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
     from pymatgen.io.vasp.sets import DictSet
 
+    from quacc.utils.files import SourceDirectory
     from quacc.utils.kpts import PmgKpts
 
+    if has_atomate2:
+        from atomate2.vasp.jobs.base import BaseVaspMaker
+
 logger = logging.getLogger(__name__)
 
 
 def get_param_swaps(
     user_calc_params: dict[str, Any],
     pmg_kpts: dict[Literal["line_density", "kppvol", "kppa"], float],
     input_atoms: Atoms,
@@ -365,49 +372,114 @@
         user_calc_params["reciprocal"] = reciprocal
     if user_calc_params.get("gamma") is None:
         user_calc_params["gamma"] = gamma
 
     return user_calc_params
 
 
-def get_pmg_input_set_params(dict_set: DictSet, atoms: Atoms) -> tuple[dict, Atoms]:
+class MPtoASEConverter:
+    """
+    Convert an MP-formatted input set to an ASE-formatted input set.
     """
-    Convert a Pymatgen VASP input set into an ASE-compatible set of
-    calculator parameters.
-
-    Parameters
-    ----------
-    dict_set
-        The Pymatgen VASP input set.
-    atoms
-        The input atoms.
 
-    Returns
-    -------
-    dict
-        The ASE-compatible set of calculator parameters.
-    Atoms
-        The input atoms to match the pymatgen input set.
-    """
-    structure = AseAtomsAdaptor.get_structure(atoms)
-    pmg_input_set = dict_set(structure=structure, sort_structure=False)
-    incar_dict = {k.lower(): v for k, v in pmg_input_set.incar.items()}
-
-    potcar_symbols = pmg_input_set.potcar_symbols
-    potcar_setups = {symbol.split("_")[0]: symbol for symbol in potcar_symbols}
-    for k, v in potcar_setups.items():
-        if k in v:
-            potcar_setups[k] = v.split(k)[-1]
-
-    pp = pmg_input_set.potcar_functional.split("_")[0]
-
-    full_input_params = incar_dict | {"setups": potcar_setups, "pp": pp}
-
-    pmg_kpts = pmg_input_set.kpoints
-    if pmg_kpts is not None:
-        kpoints_dict = pmg_input_set.kpoints.as_dict()
-        full_input_params |= {
-            "kpts": kpoints_dict["kpoints"][0],
-            "gamma": kpoints_dict["generation_style"] == "Gamma",
-        }
+    def __init__(
+        self, atoms: Atoms | None = None, prev_dir: SourceDirectory | None = None
+    ) -> None:
+        """
+        Initialize the converter.
+
+        Parameters
+        ----------
+        atoms
+            The ASE atoms object.
+        prev_dir
+            The previous directory.
+
+        Returns
+        -------
+        None
+        """
+        if atoms is None and prev_dir is None:
+            raise ValueError("Either atoms or prev_dir must be provided.")
+        self.atoms = atoms
+        self.prev_dir = prev_dir
+        self.structure = AseAtomsAdaptor.get_structure(atoms)
+
+    def convert_dict_set(self, dict_set: DictSet) -> dict:
+        """
+        Convert a Pymatgen DictSet to a dictionary of ASE VASP parameters.
+
+        Parameters
+        ----------
+        dict_set
+            The pymatgen DictSet.
+
+        Returns
+        -------
+        dict
+            The ASE VASP parameters.
+        """
+        input_set = dict_set(sort_structure=False)
+        vasp_input = input_set.get_input_set(
+            structure=self.structure, potcar_spec=True, prev_dir=self.prev_dir
+        )
+        self.incar_dict = vasp_input["INCAR"]
+        self.pmg_kpts = vasp_input.get("KPOINTS")
+        self.potcar_symbols = vasp_input["POTCAR"]
+        self.potcar_functional = input_set.potcar_functional
+        self.poscar = vasp_input["POSCAR"]
+        return self._convert()
+
+    @requires(has_atomate2, "atomate2 is not installed.")
+    def convert_vasp_maker(self, VaspMaker: BaseVaspMaker) -> dict:
+        """
+        Convert an atomate2 VaspMaker to a dictionary of ASE VASP parameters.
+
+        Parameters
+        ----------
+        VaspMaker
+            The atomate2 VaspMaker.
+
+        Returns
+        -------
+        dict
+            The ASE VASP parameters.
+        """
+        input_set_generator = VaspMaker().input_set_generator
+        assert hasattr(input_set_generator, "sort_structure")
+        input_set_generator.sort_structure = False
+        input_set = input_set_generator.get_input_set(
+            structure=self.structure, potcar_spec=True, prev_dir=self.prev_dir
+        )
+        self.incar_dict = input_set.incar
+        self.pmg_kpts = input_set.kpoints
+        self.potcar_symbols = input_set.potcar
+        self.potcar_functional = input_set_generator.potcar_functional
+        self.poscar = input_set.poscar
+        return self._convert()
+
+    def _convert(self) -> dict:
+        """
+        Convert the MP input to a dictionary of ASE VASP parameters.
+
+        Returns
+        -------
+        dict
+            The ASE VASP parameters.
+        """
+        self.incar_dict = {k.lower(): v for k, v in self.incar_dict.items()}
+        pp = self.potcar_functional.split("_")[0]
+        potcar_setups = {symbol.split("_")[0]: symbol for symbol in self.potcar_symbols}
+        for k, v in potcar_setups.items():
+            if k in v:
+                potcar_setups[k] = v.split(k)[-1]
+
+        full_input_params = self.incar_dict | {"setups": potcar_setups, "pp": pp}
+
+        if self.pmg_kpts:
+            kpts_dict = self.pmg_kpts.as_dict()
+            full_input_params |= {
+                "kpts": kpts_dict["kpoints"][0],
+                "gamma": kpts_dict["generation_style"].lower() == "gamma",
+            }
 
-    return full_input_params, pmg_input_set.poscar.structure.to_ase_atoms()
+        return full_input_params
```

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.8.0/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.8.0/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/vasp.py` & `quacc-0.8.0/src/quacc/calculators/vasp/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,27 @@
 from ase.calculators.vasp import Vasp as Vasp_
 from ase.calculators.vasp import setups as ase_setups
 from ase.constraints import FixAtoms
 
 from quacc.calculators.vasp.io import load_vasp_yaml_calc
 from quacc.calculators.vasp.params import (
     get_param_swaps,
-    get_pmg_input_set_params,
     normalize_params,
     remove_unused_flags,
     set_auto_dipole,
     set_pmg_kpts,
 )
 from quacc.calculators.vasp.vasp_custodian import run_custodian
 from quacc.schemas.prep import set_magmoms
 from quacc.utils.dicts import sort_dict
 
 if TYPE_CHECKING:
     from typing import Literal
 
     from ase.atoms import Atoms
-    from pymatgen.io.vasp.sets import DictSet
 
 _DEFAULT_SETTING = ()
 
 
 class Vasp(Vasp_):
     """This is a wrapper around the ASE Vasp calculator that adjusts INCAR parameters
     on-the-fly, allows for ASE to run VASP via Custodian, and supports several automatic
@@ -52,15 +50,14 @@
         elemental_magmoms: dict[str, float] | None = None,
         pmg_kpts: (
             dict[Literal["line_density", "kppvol", "kppa"], float]
             | dict[Literal["length_densities"], list[float]]
             | None
         ) = None,
         auto_dipole: bool | None = None,
-        pmg_input_set: DictSet | None = None,
         **kwargs,
     ) -> None:
         """
         Initialize the VASP calculator.
 
         Parameters
         ----------
@@ -97,17 +94,14 @@
             [quacc.schemas.prep.set_magmoms][], e.g. `{"Fe": 5, "Ni": 4}`.
         pmg_kpts
             An automatic k-point generation scheme from Pymatgen. See
             [quacc.utils.kpts.convert_pmg_kpts][] for details.
         auto_dipole
             If True, will automatically set dipole moment correction parameters
             based on the center of mass (in the c dimension by default).
-        pmg_input_set
-            A Pymatgen input set to use for the VASP calculation, taken from a
-            `pymatgen.io.vasp.sets.DictSet` object.
         **kwargs
             Additional arguments to be passed to the VASP calculator, e.g.
             `xc='PBE'`, `encut=520`. Takes all valid ASE calculator arguments.
 
         Returns
         -------
         None
@@ -146,15 +140,14 @@
         self.incar_copilot = incar_copilot
         self.copy_magmoms = copy_magmoms
         self.preset_mag_default = preset_mag_default
         self.mag_cutoff = mag_cutoff
         self.elemental_magmoms = elemental_magmoms
         self.pmg_kpts = pmg_kpts
         self.auto_dipole = auto_dipole
-        self.pmg_input_set = pmg_input_set
         self.kwargs = kwargs
 
         # Initialize for later
         self.user_calc_params = {}
 
         # Cleanup parameters
         self._cleanup_params()
@@ -214,33 +207,25 @@
             self.use_custodian
             and self.input_atoms.constraints
             and not all(isinstance(c, FixAtoms) for c in self.input_atoms.constraints)
         ):
             msg = "Atoms object has a constraint that is not compatible with Custodian."
             raise ValueError(msg)
 
-        # Get Pymatgen VASP input set parameters
-        if self.pmg_input_set:
-            pmg_calc_params, self.input_atoms = get_pmg_input_set_params(
-                self.pmg_input_set, self.input_atoms
-            )
-        else:
-            pmg_calc_params = {}
-
         # Get user-defined preset parameters for the calculator
         if self.preset:
             calc_preset = load_vasp_yaml_calc(SETTINGS.VASP_PRESET_DIR / self.preset)[
                 "inputs"
             ]
         else:
             calc_preset = {}
 
         # Collect all the calculator parameters and prioritize the kwargs in the
         # case of duplicates.
-        self.user_calc_params = pmg_calc_params | calc_preset | self.kwargs
+        self.user_calc_params = calc_preset | self.kwargs
 
         # Allow the user to use setups='mysetups.yaml' to load in a custom
         # setups from a YAML file
         if (
             isinstance(self.user_calc_params.get("setups"), (str, Path))
             and self.user_calc_params["setups"] not in ase_setups.setups_defaults
         ):
```

### Comparing `quacc-0.7.8/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.8.0/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/common/defects.py` & `quacc-0.8.0/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/common/elastic.py` & `quacc-0.8.0/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/common/phonons.py` & `quacc-0.8.0/src/quacc/recipes/common/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/common/slabs.py` & `quacc-0.8.0/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/dftb/_base.py` & `quacc-0.8.0/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/dftb/core.py` & `quacc-0.8.0/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/emt/core.py` & `quacc-0.8.0/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/emt/defects.py` & `quacc-0.8.0/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/emt/elastic.py` & `quacc-0.8.0/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/emt/phonons.py` & `quacc-0.8.0/src/quacc/recipes/emt/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/emt/slabs.py` & `quacc-0.8.0/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/espresso/_base.py` & `quacc-0.8.0/src/quacc/recipes/espresso/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/espresso/bands.py` & `quacc-0.8.0/src/quacc/recipes/espresso/bands.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/espresso/core.py` & `quacc-0.8.0/src/quacc/recipes/espresso/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/espresso/dos.py` & `quacc-0.8.0/src/quacc/recipes/espresso/dos.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/espresso/phonons.py` & `quacc-0.8.0/src/quacc/recipes/espresso/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/gaussian/_base.py` & `quacc-0.8.0/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/gaussian/core.py` & `quacc-0.8.0/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/gulp/_base.py` & `quacc-0.8.0/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/gulp/core.py` & `quacc-0.8.0/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/lj/core.py` & `quacc-0.8.0/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/mlp/_base.py` & `quacc-0.8.0/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/mlp/core.py` & `quacc-0.8.0/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/mlp/phonons.py` & `quacc-0.8.0/src/quacc/recipes/mlp/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/newtonnet/core.py` & `quacc-0.8.0/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.8.0/src/quacc/recipes/newtonnet/ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
-from quacc import SETTINGS, job, strip_decorator
+from quacc import SETTINGS, change_settings, job, strip_decorator
 from quacc.recipes.newtonnet.core import _add_stdev_and_hess, freq_job, relax_job
 from quacc.runners.ase import run_opt
 from quacc.schemas.ase import summarize_opt_run
 from quacc.utils.dicts import recursive_dict_merge
 
 try:
     from sella import IRC, Sella
@@ -157,15 +157,14 @@
     Returns
     -------
     IRCSchema
         A dictionary containing the IRC summary and thermodynamic summary.
         See the type-hint for the data structure.
     """
     freq_job_kwargs = freq_job_kwargs or {}
-    default_settings = SETTINGS.model_copy()
 
     calc_defaults = {
         "model_path": SETTINGS.NEWTONNET_MODEL_PATH,
         "settings_path": SETTINGS.NEWTONNET_CONFIG_PATH,
     }
     opt_defaults = {
         "optimizer": IRC,
@@ -176,22 +175,21 @@
     calc_flags = recursive_dict_merge(calc_defaults, calc_kwargs)
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
     # Define calculator
     atoms.calc = NewtonNet(**calc_flags)
 
     # Run IRC
-    SETTINGS.CHECK_CONVERGENCE = False
-    dyn = run_opt(atoms, **opt_flags)
-    opt_irc_summary = _add_stdev_and_hess(
-        summarize_opt_run(
-            dyn, additional_fields={"name": f"NewtonNet IRC: {direction}"}
+    with change_settings({"CHECK_CONVERGENCE": False}):
+        dyn = run_opt(atoms, **opt_flags)
+        opt_irc_summary = _add_stdev_and_hess(
+            summarize_opt_run(
+                dyn, additional_fields={"name": f"NewtonNet IRC: {direction}"}
+            )
         )
-    )
-    SETTINGS.CHECK_CONVERGENCE = default_settings.CHECK_CONVERGENCE
 
     # Run frequency job
     freq_summary = (
         strip_decorator(freq_job)(opt_irc_summary["atoms"], **freq_job_kwargs)
         if run_freq
         else None
     )
```

### Comparing `quacc-0.7.8/src/quacc/recipes/onetep/_base.py` & `quacc-0.8.0/src/quacc/recipes/onetep/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/onetep/core.py` & `quacc-0.8.0/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/orca/_base.py` & `quacc-0.8.0/src/quacc/recipes/orca/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/orca/core.py` & `quacc-0.8.0/src/quacc/recipes/orca/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/psi4/_base.py` & `quacc-0.8.0/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/psi4/core.py` & `quacc-0.8.0/src/quacc/recipes/psi4/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/qchem/_base.py` & `quacc-0.8.0/src/quacc/recipes/qchem/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/qchem/core.py` & `quacc-0.8.0/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/qchem/ts.py` & `quacc-0.8.0/src/quacc/recipes/qchem/ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
-from quacc import SETTINGS, job, strip_decorator
+from quacc import change_settings, job, strip_decorator
 from quacc.atoms.core import perturb
 from quacc.recipes.qchem._base import run_and_summarize_opt
 from quacc.recipes.qchem.core import _BASE_SET, relax_job
 from quacc.utils.dicts import recursive_dict_merge
 
 try:
     from sella import IRC, Sella
@@ -201,16 +201,14 @@
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
     OptSchema
         Dictionary of results from [quacc.schemas.ase.summarize_opt_run][]
     """
-    default_settings = SETTINGS.model_copy()
-
     irc_job_defaults = {
         "charge": charge,
         "spin_multiplicity": spin_multiplicity,
         "direction": direction,
         "method": method,
         "basis": basis,
         "opt_params": {"max_steps": 10},
@@ -221,20 +219,18 @@
         "spin_multiplicity": spin_multiplicity,
         "method": method,
         "basis": basis,
     }
     irc_job_kwargs = recursive_dict_merge(irc_job_defaults, irc_job_kwargs)
     relax_job_kwargs = recursive_dict_merge(relax_job_defaults, relax_job_kwargs)
 
-    SETTINGS.CHECK_CONVERGENCE = False
-    irc_summary = strip_decorator(irc_job)(atoms, **irc_job_kwargs)
+    with change_settings({"CHECK_CONVERGENCE": False}):
+        irc_summary = strip_decorator(irc_job)(atoms, **irc_job_kwargs)
 
-    SETTINGS.CHECK_CONVERGENCE = default_settings.CHECK_CONVERGENCE
     relax_summary = strip_decorator(relax_job)(irc_summary["atoms"], **relax_job_kwargs)
-
     relax_summary["initial_irc"] = irc_summary
 
     return relax_summary
 
 
 @job
 @requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
```

### Comparing `quacc-0.7.8/src/quacc/recipes/tblite/core.py` & `quacc-0.8.0/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/tblite/phonons.py` & `quacc-0.8.0/src/quacc/recipes/tblite/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/vasp/_base.py` & `quacc-0.8.0/src/quacc/recipes/vasp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/vasp/core.py` & `quacc-0.8.0/src/quacc/recipes/vasp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/recipes/vasp/mp.py` & `quacc-0.8.0/src/quacc/recipes/vasp/mp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,336 +1,255 @@
 """
 Materials Project-compatible recipes.
 
-This set of recipes is meant to be compatible with the Materials Project
-
 !!! Important
 
     Make sure that you use the Materials Project-compatible pseudpotential
     versions. The GGA workflows use the old (no version) PAW PBE potentials.
     The meta-GGA workflows currently use the v.54 PAW PBE potentials.
-
-!!! Info
-    The one true source of Materials Project workflows is
-    [atomate2](https://github.com/materialsproject/atomate2).
 """
 
 from __future__ import annotations
 
-import logging
-from functools import partial
+from importlib import util
 from typing import TYPE_CHECKING
 
-from pymatgen.io.vasp.sets import MPRelaxSet, MPScanRelaxSet, MPStaticSet
+from monty.dev import requires
 
-from quacc import flow, job
+from quacc import change_settings, flow, job
+from quacc.calculators.vasp.params import MPtoASEConverter
 from quacc.recipes.vasp._base import run_and_summarize
 from quacc.wflow_tools.customizers import customize_funcs
 
-try:
-    from pymatgen.io.validation import ValidationDoc
-except ImportError:
-    ValidationDoc = None
+has_atomate2 = util.find_spec("atomate2")
+if has_atomate2:
+    from atomate2.vasp.jobs.mp import (
+        MPGGARelaxMaker,
+        MPGGAStaticMaker,
+        MPMetaGGARelaxMaker,
+        MPMetaGGAStaticMaker,
+        MPPreRelaxMaker,
+    )
 
 if TYPE_CHECKING:
-    from pathlib import Path
     from typing import Any, Callable
 
     from ase.atoms import Atoms
-    from emmet.core.base import EmmetBaseModel
 
     from quacc.schemas._aliases.vasp import (
         MPGGARelaxFlowSchema,
         MPMetaGGARelaxFlowSchema,
         VaspSchema,
     )
-    from quacc.utils.files import Filenames, SourceDirectory
+    from quacc.utils.files import SourceDirectory
 
-logger = logging.getLogger(__name__)
-
-
-def _validate_mp_compatability(directory: Path | str) -> EmmetBaseModel | None:
-    """
-    Validate the output of a VASP calculation for Materials Project compatibility.
-
-    Parameters
-    ----------
-    directory
-        Path to the directory containing the VASP calculation.
-
-    Returns
-    -------
-    EmmetBaseModel | None
-        The validation document.
-    """
-    if ValidationDoc is None:
-        logger.warning(
-            "pymatgen-io-validation is not installed. Skipping MP compatability check."
-        )
-        return None
-    validation_doc = ValidationDoc.from_directory(dir_name=directory)
-    if not validation_doc.valid:
-        logger.warning(
-            f"Calculation in {directory} is not MP-compatible for the following reasons: {validation_doc.reasons}"
-        )
-    if validation_doc.warnings:
-        logger.warning(
-            f"Calculation in {directory} has the following MP-related warnings: {validation_doc.warnings}"
-        )
-    return validation_doc
+_MP_SETTINGS = {"VASP_INCAR_COPILOT": "off", "VASP_USE_CUSTODIAN": True}
 
 
 @job
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_gga_relax_job(
-    atoms: Atoms,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **calc_kwargs,
+    atoms: Atoms, prev_dir: SourceDirectory | None = None, **calc_kwargs
 ) -> VaspSchema:
     """
     Function to relax a structure with the original Materials Project GGA(+U) settings.
 
     Parameters
     ----------
     atoms
         Atoms object
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+    prev_dir
+        A previous directory for a prior step in the workflow.
     **calc_kwargs
         Custom kwargs for the Vasp calculator. Set a value to
         `None` to remove a pre-existing key entirely. For a list of available
         keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
     VaspSchema
         Dictionary of results.
     """
-    calc_defaults = {"pmg_input_set": MPRelaxSet}
-    output = run_and_summarize(
-        atoms,
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP GGA Relax"},
-        copy_files=copy_files,
+    calc_defaults = MPtoASEConverter(atoms=atoms, prev_dir=prev_dir).convert_vasp_maker(
+        MPGGARelaxMaker
     )
-    _validate_mp_compatability(output["dir_name"])
-
-    return output
+    with change_settings(_MP_SETTINGS):
+        return run_and_summarize(
+            atoms,
+            calc_defaults=calc_defaults,
+            calc_swaps=calc_kwargs,
+            report_mp_corrections=True,
+            additional_fields={"name": "MP GGA Relax"},
+            copy_files={prev_dir: ["CHGCAR*", "WAVECAR*"]},
+        )
 
 
 @job
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_gga_static_job(
-    atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **calc_kwargs,
+    atoms: Atoms, prev_dir: SourceDirectory | None = None, **calc_kwargs
 ) -> VaspSchema:
     """
     Function to run a static calculation on a structure with the original Materials Project GGA(+U) settings.
 
     Parameters
     ----------
     atoms
         Atoms object
-    bandgap
-        The bandgap in eV, if known from a prior calculation.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+    prev_dir
+        A previous directory for a prior step in the workflow.
     **calc_kwargs
         Custom kwargs for the Vasp calculator. Set a value to
         `None` to remove a pre-existing key entirely. For a list of available
         keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
     VaspSchema
         Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPStaticSet, bandgap=bandgap, small_gap_multiply=[1e-4, 3.125]
-        ),
-        "algo": "fast",
-        "lwave": True,  # Deviation from MP (but logical)
-        "lreal": False,
-    }
-    output = run_and_summarize(
-        atoms,
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP GGA Static"},
-        copy_files=copy_files,
+    calc_defaults = MPtoASEConverter(atoms=atoms, prev_dir=prev_dir).convert_vasp_maker(
+        MPGGAStaticMaker
     )
-    _validate_mp_compatability(output["dir_name"])
-
-    return output
+    with change_settings(_MP_SETTINGS):
+        return run_and_summarize(
+            atoms,
+            calc_defaults=calc_defaults,
+            calc_swaps=calc_kwargs,
+            report_mp_corrections=True,
+            additional_fields={"name": "MP GGA Static"},
+            copy_files={prev_dir: ["CHGCAR*", "WAVECAR*"]},
+        )
 
 
 @job
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_metagga_prerelax_job(
-    atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **calc_kwargs,
+    atoms: Atoms, prev_dir: SourceDirectory | None = None, **calc_kwargs
 ) -> VaspSchema:
     """
     Function to pre-relax a structure with Materials Project r2SCAN workflow settings. By default, this
     uses a PBEsol pre-relax step.
 
     Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
 
     Parameters
     ----------
     atoms
         Atoms object
-    bandgap
-        Estimate for the bandgap in eV.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+    prev_dir
+        A previous directory for a prior step in the workflow.
     **calc_kwargs
         Custom kwargs for the Vasp calculator. Set a value to
         `None` to remove a pre-existing key entirely. For a list of available
         keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
     VaspSchema
         Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
-        ),
-        "ediffg": -0.05,
-        "gga": "PS",
-        "laechg": False,  # Deviation from MP (but logical)
-        "lvtot": False,  # Deviation from MP (but logical)
-        "lwave": True,
-        "metagga": None,
-    }
-    output = run_and_summarize(
-        atoms,
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP Meta-GGA Pre-Relax"},
-        copy_files=copy_files,
+    calc_defaults = MPtoASEConverter(atoms=atoms, prev_dir=prev_dir).convert_vasp_maker(
+        MPPreRelaxMaker
     )
-    _validate_mp_compatability(output["dir_name"])
-    return output
+    with change_settings(_MP_SETTINGS):
+        return run_and_summarize(
+            atoms,
+            calc_defaults=calc_defaults,
+            calc_swaps=calc_kwargs,
+            report_mp_corrections=True,
+            additional_fields={"name": "MP Meta-GGA Pre-Relax"},
+            copy_files={prev_dir: ["CHGCAR*", "WAVECAR*"]},
+        )
 
 
 @job
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_metagga_relax_job(
-    atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **calc_kwargs,
+    atoms: Atoms, prev_dir: SourceDirectory | None = None, **calc_kwargs
 ) -> VaspSchema:
     """
     Function to relax a structure with Materials Project r2SCAN workflow settings. By default, this uses
     an r2SCAN relax step.
 
     Reference: https://doi.org/10.1103/PhysRevMaterials.6.013801
 
     Parameters
     ----------
     atoms
         Atoms object
-    bandgap
-        Estimate for the bandgap in eV.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+    prev_dir
+        A previous directory for a prior step in the workflow.
     **calc_kwargs
         Dictionary of custom kwargs for the Vasp calculator. Set a value to
         `None` to remove a pre-existing key entirely. For a list of available
         keys, refer to [quacc.calculators.vasp.vasp.Vasp][].
 
     Returns
     -------
     VaspSchema
         Dictionary of results.
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
-        ),
-        "laechg": False,  # Deviation from MP (but logical)
-        "lvtot": False,  # Deviation from MP (but logical)
-        "lwave": True,
-    }
-    output = run_and_summarize(
-        atoms,
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP Meta-GGA Relax"},
-        copy_files=copy_files,
+    calc_defaults = MPtoASEConverter(atoms=atoms, prev_dir=prev_dir).convert_vasp_maker(
+        MPMetaGGARelaxMaker
     )
-    _validate_mp_compatability(output["dir_name"])
-
-    return output
+    with change_settings(_MP_SETTINGS):
+        return run_and_summarize(
+            atoms,
+            calc_defaults=calc_defaults,
+            calc_swaps=calc_kwargs,
+            report_mp_corrections=True,
+            additional_fields={"name": "MP Meta-GGA Relax"},
+            copy_files={prev_dir: ["CHGCAR*", "WAVECAR*"]},
+        )
 
 
 @job
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_metagga_static_job(
-    atoms: Atoms,
-    bandgap: float | None = None,
-    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-    **calc_kwargs,
+    atoms: Atoms, prev_dir: SourceDirectory | None = None, **calc_kwargs
 ) -> VaspSchema:
     """
     Function to run a static calculation on a structure with r2SCAN workflow Materials Project settings.
     By default, this uses an r2SCAN static step.
 
     Parameters
     ----------
     atoms
         Atoms object
-    bandgap
-        Estimate for the bandgap in eV.
-    copy_files
-        Files to copy (and decompress) from source to the runtime directory.
+    prev_dir
+        A previous directory for a prior step in the workflow.
     **calc_kwargs
         Dictionary of custom kwargs for the Vasp calculator. Set a value to
         `None` to remove a pre-existing key entirely. For a list of available
         keys, refer to `ase.calculators.vasp.vasp.Vasp`.
 
     Returns
     -------
     VaspSchema
         Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
         See the type-hint for the data structure.
     """
-    calc_defaults = {
-        "pmg_input_set": partial(
-            MPScanRelaxSet, bandgap=bandgap or 0.0, auto_ismear=False
-        ),
-        "algo": "fast",
-        "ismear": -5,
-        "lreal": False,
-        "lwave": True,  # Deviation from MP (but logical)
-        "nsw": 0,
-    }
-    output = run_and_summarize(
-        atoms,
-        calc_defaults=calc_defaults,
-        calc_swaps=calc_kwargs,
-        report_mp_corrections=True,
-        additional_fields={"name": "MP Meta-GGA Static"},
-        copy_files=copy_files,
+    calc_defaults = MPtoASEConverter(atoms=atoms, prev_dir=prev_dir).convert_vasp_maker(
+        MPMetaGGAStaticMaker
     )
-    _validate_mp_compatability(output["dir_name"])
-    return output
+    with change_settings(_MP_SETTINGS):
+        return run_and_summarize(
+            atoms,
+            calc_defaults=calc_defaults,
+            calc_swaps=calc_kwargs,
+            report_mp_corrections=True,
+            additional_fields={"name": "MP Meta-GGA Static"},
+            copy_files={prev_dir: ["CHGCAR*", "WAVECAR*"]},
+        )
 
 
 @flow
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_gga_relax_flow(
     atoms: Atoms,
     job_params: dict[str, dict[str, Any]] | None = None,
     job_decorators: dict[str, Callable | None] | None = None,
 ) -> MPGGARelaxFlowSchema:
     """
     Materials Project GGA workflow consisting of:
@@ -371,33 +290,31 @@
     )
 
     # Run the relax
     relax_results = mp_gga_relax_job_(atoms)
 
     # Run the second relax
     double_relax_results = mp_gga_relax_job_(
-        relax_results["atoms"],
-        copy_files={relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+        relax_results["atoms"], prev_dir=relax_results["dir_name"]
     )
 
     # Run the static
     static_results = mp_gga_static_job_(
-        double_relax_results["atoms"],
-        bandgap=double_relax_results["output"]["bandgap"],
-        copy_files={double_relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+        double_relax_results["atoms"], prev_dir=double_relax_results["dir_name"]
     )
 
     return {
         "relax1": relax_results,
         "relax2": double_relax_results,
         "static": static_results,
     }
 
 
 @flow
+@requires(has_atomate2, "atomate2 is not installed. Run `pip install quacc[mp]`")
 def mp_metagga_relax_flow(
     atoms: Atoms,
     job_params: dict[str, dict[str, Any]] | None = None,
     job_decorators: dict[str, Callable | None] | None = None,
 ) -> MPMetaGGARelaxFlowSchema:
     """
     Materials Project r2SCAN workflow consisting of:
@@ -450,31 +367,25 @@
     )
 
     # Run the prerelax
     prerelax_results = mp_metagga_prerelax_job_(atoms)
 
     # Run the relax
     relax_results = mp_metagga_relax_job_(
-        prerelax_results["atoms"],
-        bandgap=prerelax_results["output"]["bandgap"],
-        copy_files={prerelax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+        prerelax_results["atoms"], prev_dir=prerelax_results["dir_name"]
     )
 
     # Run the second relax
     double_relax_results = mp_metagga_relax_job_(
-        relax_results["atoms"],
-        bandgap=relax_results["output"]["bandgap"],
-        copy_files={relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+        relax_results["atoms"], prev_dir=relax_results["dir_name"]
     )
 
     # Run the static
     static_results = mp_metagga_static_job_(
-        double_relax_results["atoms"],
-        bandgap=double_relax_results["output"]["bandgap"],
-        copy_files={double_relax_results["dir_name"]: ["CHGCAR*", "WAVECAR*"]},
+        double_relax_results["atoms"], prev_dir=double_relax_results["dir_name"]
     )
 
     return {
         "prerelax": prerelax_results,
         "relax1": relax_results,
         "relax2": double_relax_results,
         "static": static_results,
```

### Comparing `quacc-0.7.8/src/quacc/recipes/vasp/qmof.py` & `quacc-0.8.0/src/quacc/recipes/vasp/qmof.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,34 +3,38 @@
 
 This set of recipes is meant to be compatible with the QMOF Database workflow.
 Reference: https://doi.org/10.1016/j.matt.2021.02.015
 """
 
 from __future__ import annotations
 
+import logging
 from typing import TYPE_CHECKING
 
 from ase.optimize import BFGSLineSearch
 
-from quacc import job
+from quacc import change_settings, job
 from quacc.recipes.vasp._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.ase import OptSchema
     from quacc.schemas._aliases.vasp import QMOFRelaxSchema, VaspSchema
+    from quacc.utils.files import Filenames, SourceDirectory
+
+LOGGER = logging.getLogger(__name__)
 
 
 @job
 def qmof_relax_job(
     atoms: Atoms,
-    preset: str | None = "QMOFSet",
     relax_cell: bool = True,
     run_prerelax: bool = True,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> QMOFRelaxSchema:
     """
     Relax a structure in a multi-step process for increased computational efficiency.
     This is all done in a single compute job. Settings are such that they are compatible
     with the QMOF Database.
 
@@ -44,77 +48,87 @@
 
     5. Static calculation.
 
     Parameters
     ----------
     atoms
         Atoms object
-    preset
-        Preset to use from `quacc.calculators.vasp.presets`. Applies for all jobs.
     relax_cell
         True if a volume relaxation should be performed. False if only the
         positions should be updated.
     run_prerelax
         If True, a pre-relax will be carried out with BFGSLineSearch.
         Recommended if starting from hypothetical structures or materials with
         very high starting forces.
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
         Custom kwargs for the calculator. Set a value to `None` to remove
         a pre-existing key entirely. Applies for all jobs.
 
     Returns
     -------
     QMOFRelaxSchema
         Dictionary of results. See the type-hint for the data structure.
     """
-    # 1. Pre-relaxation
-    if run_prerelax:
-        summary1 = _prerelax(atoms, preset, fmax=5.0, **calc_kwargs)
-        atoms = summary1["atoms"]
-
-    # 2. Position relaxation (loose)
-    summary2 = _loose_relax_positions(atoms, preset, **calc_kwargs)
-    atoms = summary2["atoms"]
-
-    # 3. Optional: Volume relaxation (loose)
-    if relax_cell:
-        summary3 = _loose_relax_cell(atoms, preset, **calc_kwargs)
-        atoms = summary3["atoms"]
-
-    # 4. Double Relaxation This is done for two reasons: a) because it can
-    # resolve repadding issues when dV is large; b) because we can use LREAL =
-    # Auto for the first relaxation and the default LREAL for the second.
-    summary4 = _double_relax(atoms, preset, relax_cell=relax_cell, **calc_kwargs)
-    atoms = summary4[1]["atoms"]
-
-    # 5. Static Calculation
-    summary5 = _static(atoms, preset, **calc_kwargs)
-    summary5["prerelax_lowacc"] = summary1 if run_prerelax else None
-    summary5["position_relax_lowacc"] = summary2
-    summary5["volume_relax_lowacc"] = summary3 if relax_cell else None
-    summary5["double_relax"] = summary4
+    with change_settings({"VASP_USE_CUSTODIAN": True}):
+        copy_files = None
+
+        # 1. Pre-relaxation
+        if run_prerelax:
+            summary1 = _prerelax(atoms, **calc_kwargs)
+            atoms = summary1["atoms"]
+            copy_files = {summary1["dir_name"]: ["WAVECAR*"]}
+
+        # 2. Position relaxation (loose)
+        summary2 = _loose_relax_positions(atoms, copy_files=copy_files, **calc_kwargs)
+        atoms = summary2["atoms"]
+        copy_files = {summary2["dir_name"]: ["WAVECAR*"]}
+
+        # 3. Optional: Volume relaxation (loose)
+        if relax_cell:
+            summary3 = _loose_relax_cell(atoms, copy_files=copy_files, **calc_kwargs)
+            atoms = summary3["atoms"]
+            copy_files = {summary3["dir_name"]: ["WAVECAR*"]}
+
+        # 4. Double Relaxation
+        # This is done for two reasons: a) because it can
+        # resolve repadding issues when dV is large; b) because we can use LREAL =
+        # Auto for the first relaxation and the default LREAL for the second.
+        summary4 = _double_relax(
+            atoms, relax_cell=relax_cell, copy_files=copy_files, **calc_kwargs
+        )
+        atoms = summary4[-1]["atoms"]
+        copy_files = {summary4[-1]["dir_name"]: ["WAVECAR*"]}
+
+        # 5. Static Calculation
+        summary5 = _static(atoms, copy_files=copy_files, **calc_kwargs)
+        summary5["prerelax_lowacc"] = summary1 if run_prerelax else None
+        summary5["position_relax_lowacc"] = summary2
+        summary5["volume_relax_lowacc"] = summary3 if relax_cell else None
+        summary5["double_relax"] = summary4
 
-    return summary5
+        return summary5
 
 
 def _prerelax(
-    atoms: Atoms, preset: str | None = "QMOFSet", fmax: float = 5.0, **calc_kwargs
+    atoms: Atoms,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
 ) -> OptSchema:
     """
     A "pre-relaxation" with BFGSLineSearch to resolve very high forces.
 
     Parameters
     ----------
     atoms
         Atoms object
-    preset
-        Preset to use from `quacc.calculators.vasp.presets`.
-    fmax
-        Maximum force in eV/A.
-    **kwargs
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
         Custom kwargs for the calculator. Set a value to `None` to remove
         a pre-existing key entirely.
 
     Returns
     -------
     OptSchema
         Dictionary of results from [quacc.schemas.ase.summarize_opt_run][].
@@ -128,35 +142,38 @@
         "lreal": "auto",
         "lwave": True,
         "nelm": 225,
         "nsw": 0,
     }
     return run_and_summarize_opt(
         atoms,
-        preset=preset,
+        preset="QMOFSet",
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
-        opt_defaults={"fmax": fmax, "optimizer": BFGSLineSearch},
+        opt_defaults={"fmax": 5.0, "optimizer": BFGSLineSearch},
         additional_fields={"name": "QMOF Prerelax"},
+        copy_files=copy_files,
     )
 
 
 def _loose_relax_positions(
-    atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs
+    atoms: Atoms,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
 ) -> VaspSchema:
     """
     Position relaxation with default ENCUT and coarse k-point grid.
 
     Parameters
     ----------
     atoms
         Atoms object
-    preset
-        Preset to use from `quacc.calculators.vasp.presets`.
-    **kwargs
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
         Custom kwargs for the calculator. Set a value to `None` to remove
         a pre-existing key entirely.
 
     Returns
     -------
     VaspSchema
         Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
@@ -172,33 +189,36 @@
         "lcharg": False,
         "lreal": "auto",
         "lwave": True,
         "nsw": 250,
     }
     return run_and_summarize(
         atoms,
-        preset=preset,
+        preset="QMOFSet",
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         additional_fields={"name": "QMOF Loose Relax"},
+        copy_files=copy_files,
     )
 
 
 def _loose_relax_cell(
-    atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs
+    atoms: Atoms,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
 ) -> VaspSchema:
     """
     Volume relaxation with coarse k-point grid.
 
     Parameters
     ----------
     atoms
         Atoms object
-    preset
-        Preset to use from `quacc.calculators.vasp.presets`.
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
         Custom kwargs for the calculator. Set a value to `None` to remove
         a pre-existing key entirely.
 
     Returns
     -------
     VaspSchema
@@ -213,35 +233,39 @@
         "lcharg": False,
         "lreal": "auto",
         "lwave": True,
         "nsw": 500,
     }
     return run_and_summarize(
         atoms,
-        preset=preset,
+        preset="QMOFSet",
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         additional_fields={"name": "QMOF Loose Relax Volume"},
+        copy_files=copy_files,
     )
 
 
 def _double_relax(
-    atoms: Atoms, preset: str | None = "QMOFSet", relax_cell: bool = True, **calc_kwargs
+    atoms: Atoms,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    relax_cell: bool = True,
+    **calc_kwargs,
 ) -> list[VaspSchema]:
     """
     Double relaxation using production-quality settings.
 
     Parameters
     ----------
     atoms
         Atoms object
-    preset
-        Preset to use from `quacc.calculators.vasp.presets`.
     relax_cell
         True if a volume relaxation should be performed.
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
     **calc_kwargs
         Dictionary of custom kwargs for the calculator. Set a value to `None` to remove
         a pre-existing key entirely.
 
     Returns
     -------
     list[VaspSchema]
@@ -256,48 +280,54 @@
         "lcharg": False,
         "lreal": "auto",
         "lwave": True,
         "nsw": 500 if relax_cell else 250,
     }
     summary1 = run_and_summarize(
         atoms,
-        preset=preset,
+        preset="QMOFSet",
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         additional_fields={"name": "QMOF DoubleRelax 1"},
+        copy_files=copy_files,
     )
 
     # Update atoms for Relaxation 2
     atoms = summary1["atoms"]
 
     # Reset LREAL
     del calc_defaults["lreal"]
 
     # Run second relaxation
     summary2 = run_and_summarize(
         summary1["atoms"],
-        preset=preset,
+        preset="QMOFSet",
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         additional_fields={"name": "QMOF DoubleRelax 2"},
+        copy_files={summary1["dir_name"]: ["WAVECAR*"]},
     )
     return [summary1, summary2]
 
 
-def _static(atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs) -> VaspSchema:
+def _static(
+    atoms: Atoms,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
+) -> VaspSchema:
     """
     Static calculation using production-quality settings.
 
     Parameters
     ----------
     atoms
         Atoms object
-    preset
-        Preset to use from `quacc.calculators.presets.vasp`.
-    **kwargs
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
         Custom kwargs for the calculator. Set a value to `None` to remove
         a pre-existing key entirely.
 
     Returns
     -------
     VaspSchema
         Dictionary of results from [quacc.schemas.vasp.vasp_summarize_run][].
@@ -308,12 +338,13 @@
         "lcharg": True,
         "lreal": False,
         "lwave": True,
         "nsw": 0,
     }
     return run_and_summarize(
         atoms,
-        preset=preset,
+        preset="QMOFSet",
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         additional_fields={"name": "QMOF Static"},
+        copy_files=copy_files,
     )
```

### Comparing `quacc-0.7.8/src/quacc/recipes/vasp/slabs.py` & `quacc-0.8.0/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/runners/ase.py` & `quacc-0.8.0/src/quacc/runners/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/runners/phonons.py` & `quacc-0.8.0/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/runners/prep.py` & `quacc-0.8.0/src/quacc/runners/prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 
     # Copy files to tmpdir and decompress them if needed
     if copy_files:
         if isinstance(copy_files, (str, Path)):
             copy_files = {copy_files: "*"}
 
         for source_directory, filenames in copy_files.items():
-            copy_decompress_files(source_directory, filenames, tmpdir)
+            if source_directory is not None:
+                copy_decompress_files(source_directory, filenames, tmpdir)
 
     return tmpdir, job_results_dir
 
 
 def calc_cleanup(
     atoms: Atoms | None, tmpdir: Path | str, job_results_dir: Path | str
 ) -> None:
```

### Comparing `quacc-0.7.8/src/quacc/runners/thermo.py` & `quacc-0.8.0/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/_aliases/ase.py` & `quacc-0.8.0/src/quacc/schemas/_aliases/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.8.0/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.8.0/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.8.0/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.8.0/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.8.0/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/ase.py` & `quacc-0.8.0/src/quacc/schemas/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/atoms.py` & `quacc-0.8.0/src/quacc/schemas/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/cclib.py` & `quacc-0.8.0/src/quacc/schemas/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/phonons.py` & `quacc-0.8.0/src/quacc/schemas/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/prep.py` & `quacc-0.8.0/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/schemas/vasp.py` & `quacc-0.8.0/src/quacc/schemas/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/settings.py` & `quacc-0.8.0/src/quacc/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,25 @@
 """Settings for quacc."""
 
 from __future__ import annotations
 
 import os
-from importlib import util
+from contextlib import contextmanager
 from pathlib import Path
 from shutil import which
 from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import psutil
 from maggma.core import Store
 from pydantic import Field, field_validator, model_validator
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 if TYPE_CHECKING:
     from typing import Any
 
-
-installed_engine = next(
-    (
-        wflow_engine
-        for wflow_engine in ["parsl", "covalent", "prefect", "dask", "redun", "jobflow"]
-        if util.find_spec(wflow_engine)
-    ),
-    None,
-)
 _DEFAULT_CONFIG_FILE_PATH = Path("~", ".quacc.yaml").expanduser().resolve()
 
 
 class QuaccSettings(BaseSettings):
     """
     Settings for quacc.
 
@@ -63,15 +54,15 @@
 
     # ---------------------------
     # Workflow Engine
     # ---------------------------
 
     WORKFLOW_ENGINE: Optional[
         Literal["covalent", "dask", "parsl", "prefect", "redun", "jobflow"]
-    ] = Field(installed_engine, description=("The workflow manager to use, if any."))
+    ] = Field(None, description=("The workflow manager to use, if any."))
 
     # ---------------------------
     # General Settings
     # ---------------------------
 
     RESULTS_DIR: Path = Field(
         Path.cwd(),
@@ -288,15 +279,15 @@
             """
             Default initial magmom to use for a given element if a preset
             with magmoms is provided but an element is missing from the list.
             """
         ),
     )
     VASP_MAG_CUTOFF: float = Field(
-        0.05,
+        0.02,
         description=(
             """
             If the absolute value of all magnetic moments are below this value,
             they will be set to 0 such that a spin-unpolarized calculation will be performed.
             """
         ),
     )
@@ -512,15 +503,15 @@
 
 def _type_handler(settings: dict[str, Any]) -> dict[str, Any]:
     """
     Convert common strings to their proper types.
 
     Parameters
     ----------
-    settings : dict
+    settings
         Initial settings.
 
     Returns
     -------
     dict
         Updated settings.
     """
@@ -528,7 +519,36 @@
         if isinstance(value, str):
             if value.lower() in {"null", "none"}:
                 settings[key] = None
             elif value.lower() in {"true", "false"}:
                 settings[key] = value.lower() == "true"
 
     return settings
+
+
+@contextmanager
+def change_settings(changes: dict[str, Any]) -> QuaccSettings:  # type: ignore
+    """
+    Temporarily change an attribute of an object.
+
+    Parameters
+    ----------
+    changes
+        Dictionary of changes to make formatted as attribute: value.
+
+    Returns
+    -------
+    QuaccSettings
+        Updated settings.
+    """
+    from quacc import SETTINGS
+
+    original_values = {attr: getattr(SETTINGS, attr) for attr in changes}
+
+    for attr, new_value in changes.items():
+        setattr(SETTINGS, attr, new_value)
+
+    try:
+        yield
+    finally:
+        for attr, original_value in original_values.items():
+            setattr(SETTINGS, attr, original_value)
```

### Comparing `quacc-0.7.8/src/quacc/utils/dicts.py` & `quacc-0.8.0/src/quacc/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/utils/files.py` & `quacc-0.8.0/src/quacc/utils/files.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/utils/kpts.py` & `quacc-0.8.0/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/utils/lists.py` & `quacc-0.8.0/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/wflow_tools/customizers.py` & `quacc-0.8.0/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/wflow_tools/db.py` & `quacc-0.8.0/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc/wflow_tools/decorators.py` & `quacc-0.8.0/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc.egg-info/PKG-INFO` & `quacc-0.8.0/src/quacc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.8
+Version: 0.8.0
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
 Keywords: high-throughput,automated,workflow,dft
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.13,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ase>3.22.1
+Requires-Dist: ase>=3.23.0b1
 Requires-Dist: cclib>=1.8
 Requires-Dist: custodian>=2024.3.12
 Requires-Dist: emmet-core>=0.80.0
 Requires-Dist: maggma>=0.64.0
 Requires-Dist: monty>=2024.2.26
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
-Requires-Dist: covalent>=0.234.0rc0; platform_system != "Windows" and extra == "covalent"
+Requires-Dist: covalent>=0.234.1-rc.0; platform_system != "Windows" and extra == "covalent"
 Requires-Dist: covalent-cloud>=0.39.0; platform_system != "Windows" and extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
 Provides-Extra: defects
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22; extra == "defects"
 Requires-Dist: shakenbreak>=3.2.0; extra == "defects"
@@ -51,15 +51,15 @@
 Requires-Dist: jobflow-remote>=0.1.0; extra == "jobflow"
 Provides-Extra: mlp
 Requires-Dist: matgl>=1.0.0; extra == "mlp"
 Requires-Dist: chgnet>=0.3.3; extra == "mlp"
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
 Provides-Extra: mp
-Requires-Dist: pymatgen-io-validation>=0.0.1; extra == "mp"
+Requires-Dist: atomate2>=0.0.14; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
 Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
```

### Comparing `quacc-0.7.8/src/quacc.egg-info/SOURCES.txt` & `quacc-0.8.0/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.7.8/src/quacc.egg-info/requires.txt` & `quacc-0.8.0/src/quacc.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ase>3.22.1
+ase>=3.23.0b1
 cclib>=1.8
 custodian>=2024.3.12
 emmet-core>=0.80.0
 maggma>=0.64.0
 monty>=2024.2.26
 numpy>=1.25.0
 psutil
@@ -11,15 +11,15 @@
 pymatgen>=2024.4.13
 ruamel.yaml>=0.17.40
 typer>=0.12.1
 
 [covalent]
 
 [covalent:platform_system != "Windows"]
-covalent>=0.234.0rc0
+covalent>=0.234.1-rc.0
 covalent-cloud>=0.39.0
 
 [dask]
 dask[distributed]>=2023.12.1
 dask-jobqueue>=0.8.2
 
 [defects]
@@ -47,15 +47,15 @@
 [mlp]
 matgl>=1.0.0
 chgnet>=0.3.3
 mace-torch>=0.3.3
 torch-dftd>=0.4.0
 
 [mp]
-pymatgen-io-validation>=0.0.1
+atomate2>=0.0.14
 
 [newtonnet]
 newtonnet>=1.1
 
 [parsl]
 
 [parsl:platform_system != "Windows"]
```

