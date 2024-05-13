# Comparing `tmp/dflow_galaxy-0.1.8.tar.gz` & `tmp/dflow_galaxy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.8.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.9.tar", max compression
```

## Comparing `dflow_galaxy-0.1.8.tar` & `dflow_galaxy-0.1.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.8/LICENSE
--rw-r--r--   0        0        0     2009 2024-04-22 00:50:41.993871 dflow_galaxy-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.8/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.8/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2498 2024-04-19 08:40:55.003134 dflow_galaxy-0.1.8/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2211 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     7096 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     2050 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4874 2024-04-19 08:41:31.523135 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0     2525 2024-04-11 09:39:14.159344 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/report.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0    16373 2024-04-19 11:59:38.140345 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/report.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.8/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    29475 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/core/dflow_builder.py
--rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.8/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.8/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.8/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-05-09 06:36:33.177848 dflow_galaxy-0.1.8/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.8/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/main.py
--rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.8/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0     1128 2024-04-19 08:58:50.173149 dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/deepmd.json
--rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/tesla_template.yml
--rw-r--r--   0        0        0      906 2024-04-18 09:39:30.561274 dflow_galaxy-0.1.8/dflow_galaxy/util.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.8/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/__init__.py
--rw-r--r--   0        0        0     1172 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/domain.py
--rw-r--r--   0        0        0     1255 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/main.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6347 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9700 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8065 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6342 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     8193 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      740 2024-05-11 02:30:33.739764 dflow_galaxy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2009 2024-04-22 00:50:41.993871 dflow_galaxy-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.9/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.9/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2499 2024-05-13 03:07:22.402618 dflow_galaxy-0.1.9/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.9/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2211 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     7076 2024-05-13 03:06:12.442636 dflow_galaxy-0.1.9/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     2050 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4853 2024-05-13 03:06:27.792632 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0     2525 2024-04-11 09:39:14.159344 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/report.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    16371 2024-05-13 03:06:35.812630 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_tesla/report.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.9/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    29475 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/core/dflow_builder.py
+-rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.9/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.9/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.9/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-05-09 06:36:33.177848 dflow_galaxy-0.1.9/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.9/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.9/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.9/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1128 2024-04-19 08:58:50.173149 dflow_galaxy-0.1.9/dflow_galaxy/res/dynacat/deepmd.json
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.9/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0      906 2024-04-18 09:39:30.561274 dflow_galaxy-0.1.9/dflow_galaxy/util.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.9/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/reweighting/__init__.py
+-rw-r--r--   0        0        0     1172 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/reweighting/domain.py
+-rw-r--r--   0        0        0     1255 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/reweighting/main.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6347 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9700 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8065 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6342 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8193 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      740 2024-05-13 06:47:10.978961 dflow_galaxy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.9/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.8/LICENSE` & `dflow_galaxy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/README.md` & `dflow_galaxy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from dflow.plugins import bohrium
 import dflow
 
 from dflow_galaxy.core.log import get_logger
 logger = get_logger(__name__)
 
 
-class DFlowOptionsMixin:
+class DFlowOptions(BaseModel):
     bh_username: Optional[BohriumUsername]
     bh_ticket: Optional[BohriumTicket]
     bh_project_id: Optional[BohriumProjectId]
 
     dflow_labels: Optional[DflowLabels]
     dflow_argo_api_server: Optional[DflowArgoAPIServer]
     dflow_k8s_api_server: Optional[DflowK8sAPIServer]
     dflow_access_token: Optional[DflowAccessToken]
     dflow_storage_endpoint: Optional[DflowStorageEndpoint]
     dflow_storage_repository: Optional[DflowStorageRepository]
 
 
-def setup_dflow_context(opts: DFlowOptionsMixin):
+def setup_dflow_context(opts: DFlowOptions):
     """
     setup dflow context based on:
     https://dptechnology.feishu.cn/docx/HYjmdDj36oAksixbviKcbgUinUf
     """
 
     dflow_config = {
         'host': opts.dflow_argo_api_server,
```

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath, Optional
 from dp.launching.typing import Int, String, Enum, Float, Boolean, Set
 from dp.launching.cli import to_runner
 
-from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context
+from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context
 from dflow_galaxy.res import get_cp2k_data_dir
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
 from ai2_kit.tool.ase import AseTool
 from ai2_kit.tool.dpdata import DpdataTool
 
 from pathlib import Path
@@ -71,15 +71,15 @@
     ECP_POTENTIALS_pob_TZVP_rev2 = "ECP_POTENTIALS_pob-TZVP-rev2"
     ECP_POTENTIALS = "ECP_POTENTIALS"
     NLCC_POTENTIALS = "NLCC_POTENTIALS"
     AcPP1_POTENTIALS = "AcPP1_POTENTIALS"
     LnPP1_POTENTIALS = "LnPP1_POTENTIALS"
 
 
-class Cp2kLightningArgs(BaseModel, DFlowOptionsMixin):
+class Cp2kLightningArgs(DFlowOptions):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
         description="A system file as the initial structure of AIMD simulation, can be xyz, cif, POSCAR format")
@@ -118,24 +118,24 @@
         description="Output directory for the simulation results")
 
     cp2k_image: String = Field(
         default='registry.dp.tech/dptech/cp2k:11',
         description="Docker image for running CP2K simulation")
 
     cp2k_device_model: String = Field(
-        default='c32_m64_cpu',
+        default='c64_m256_cpu',
         description="Device model for CP2K simulation")
 
     cp2k_script: String = Field(
         default= '\n'.join([
             '# 1. the output file must be named as `output`',
             '# 2. cp2k.aimd.inp for aimd and cp2k.dft.inp for dft',
             '# Note that different container may have different setup',
             'source /opt/cp2k-toolchain/install/setup',
-            'mpirun -n 32 cp2k.popt -i cp2k.aimd.inp &> output',
+            'mpirun -n 64 cp2k.popt -i cp2k.aimd.inp &> output',
             'rm *.wfn  # reduce the size of output file',
         ]),
         format='multi-line',
         description="Script to run CP2K simulation, note that it depends on the docker image")
 
 
 def launch_app(args: Cp2kLightningArgs) -> int:
```

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath, Optional, Dict
 from dp.launching.typing import Int, String, Enum, Float, Boolean
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 
-from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context, EnsembleOptions
+from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context, EnsembleOptions
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
 from ai2_kit.core.util import dump_text, dump_json
 
 
 from pathlib import Path
 import shutil
@@ -15,15 +15,15 @@
 
 from .dflow import run_lammps_workflow
 from .report import gen_report
 
 logger = get_logger(__name__)
 
 
-class DynaCatMdArgs(BaseModel, DFlowOptionsMixin):
+class DynaCatMdArgs(DFlowOptions):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
         description="A system file as the initial structure of LAMMPS simulation, can be xyz, cif, POSCAR, etc.")
```

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/report.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_md/report.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/main.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_tesla/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath
 from dp.launching.typing import Int, String, Enum, Float, Boolean, List, Optional, Dict
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 from dp.launching.report import Report, ReportSection, ChartReportElement
 
-from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context, EnsembleOptions
+from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context, EnsembleOptions
 from dflow_galaxy.res import get_res_path
 from dflow_galaxy.core.log import get_logger
 from dflow_galaxy.core.util import parse_string_array, str_or_none
 
 from dflow_galaxy.workflow.tesla.main import build_tesla_workflow
 
 from ai2_kit.core.util import dump_json, load_text, load_json
@@ -32,15 +32,15 @@
     'image_name': 'registry.dp.tech/dptech/dpmd:2.2.8-cuda12.0',
     'scass_type': 'c8_m32_1 * NVIDIA V100',
 }
 BH_LAMMPS_DEFAULT = BH_DEEPMD_DEFAULT
 
 BH_CP2K_DEFAULT = {
     'image_name': 'registry.dp.tech/dptech/cp2k:11',
-    'scass_type': 'c32_m64_cpu',
+    'scass_type': 'c64_m256_cpu',
 }
 
 BH_PYTHON_DEFAULT = {
     'image_name': 'registry.dp.tech/dptech/prod-13325/dflow-galaxy:0.1.7-main-07745fb',
     'scass_type': 'c2_m4_cpu',
 }
 
@@ -128,15 +128,15 @@
         description='Sampling frequency of LAMMPS simulation')
 
     no_pbc: Boolean = Field(
         default=False,
         description='Whether to use periodic boundary condition')
 
     concurrency: Int = Field(
-        default=5,
+        default=20,
         description="Number of concurrent run")
 
     cmd: String = Field(
         default='lmp',
         description="Command to run LAMMPS, note that it depends on the docker image you used")
 
     setup_script: String = Field(
@@ -162,35 +162,35 @@
 class Cp2kSettings(BaseModel):
 
     limit: Int = Field(
         default=50,
         description="Limit of the number of structures to be labeled for each iteration")
 
     concurrency: Int = Field(
-        default=5,
+        default=20,
         description="Number of concurrent run")
 
     cmd: String = Field(
-        default='mpirun -np 32 cp2k.popt',
+        default='mpirun -np 64 cp2k.popt',
         description="Script to run CP2K simulation, note that it depends on the docker image")
 
     setup_script: String = Field(
         default = '\n'.join([
             '# guess cp2k data dir',
             '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k || which cp2k.psmp)")/../../data" || true',
             'source /opt/cp2k-toolchain/install/setup',
         ]),
         format='multi-line',
         description="Setup script for CP2K simulation, note that it depends on the docker image you used")
 
 
-class DynacatTeslaArgs(BaseModel, DFlowOptionsMixin):
+class DynacatTeslaArgs(DFlowOptions):
     deepmd_dataset : InputFilePath = Field(
         title='DeepMD Dataset',
-        description="DeepMD in zip or tgz format, for example: deepmd-dataset.tgz")
+        description="DeepMD in zip or tgz format, for example: deepmd-dataset.tgz, dp-dataset.zip")
 
     deepmd_input_template: Optional[InputFilePath] = Field(
         title='DeepMD Input Template',
         description="Input template file for DeepMD training, in json format, for example: deepmd.json, if not provided, the build-in template will be used")
 
     lammps_system_file: InputFilePath = Field(
         description="Structure file in xyz format use for LAMMPS simulation, for example h2o.xyz, the xyz file may contain multiple structures")
```

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/report.py` & `dflow_galaxy-0.1.9/dflow_galaxy/app/dynacat_tesla/report.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/core/dflow_builder.py` & `dflow_galaxy-0.1.9/dflow_galaxy/core/dflow_builder.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.9/dflow_galaxy/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.9/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.9/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.9/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/deepmd.json` & `dflow_galaxy-0.1.9/dflow_galaxy/res/dynacat/deepmd.json`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/tesla_template.yml` & `dflow_galaxy-0.1.9/dflow_galaxy/res/dynacat/tesla_template.yml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/util.py` & `dflow_galaxy-0.1.9/dflow_galaxy/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/domain.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/reweighting/domain.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/main.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/reweighting/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.9/dflow_galaxy/workflow/tesla/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.8/pyproject.toml` & `dflow_galaxy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydflow = "1.8.60"
 dpdispatcher = "^0.6.4"
-ai2-kit= "0.18.1"
+ai2-kit= "0.18.3"
 dp-launching-sdk = "^0.12.0"
 lbg = "^1.2.24"
 cp2kdata = "^0.6.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.0"
```

### Comparing `dflow_galaxy-0.1.8/PKG-INFO` & `dflow_galaxy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ai2-kit (==0.18.1)
+Requires-Dist: ai2-kit (==0.18.3)
 Requires-Dist: cp2kdata (>=0.6.6,<0.7.0)
 Requires-Dist: dp-launching-sdk (>=0.12.0,<0.13.0)
 Requires-Dist: dpdispatcher (>=0.6.4,<0.7.0)
 Requires-Dist: lbg (>=1.2.24,<2.0.0)
 Requires-Dist: pydflow (==1.8.60)
 Description-Content-Type: text/markdown
```

