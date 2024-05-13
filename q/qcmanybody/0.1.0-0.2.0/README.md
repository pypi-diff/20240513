# Comparing `tmp/qcmanybody-0.1.0.tar.gz` & `tmp/qcmanybody-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcmanybody-0.1.0.tar", last modified: Wed Apr 24 23:07:10 2024, max compression
+gzip compressed data, was "qcmanybody-0.2.0.tar", last modified: Mon May 13 18:07:04 2024, max compression
```

## Comparing `qcmanybody-0.1.0.tar` & `qcmanybody-0.2.0.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.114564 qcmanybody-0.1.0/
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.092564 qcmanybody-0.1.0/.github/
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.095564 qcmanybody-0.1.0/.github/workflows/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5290 2024-04-24 22:59:57.000000 qcmanybody-0.1.0/.github/workflows/ci.yml
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3113 2024-04-24 19:42:31.000000 qcmanybody-0.1.0/.gitignore
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.096564 qcmanybody-0.1.0/.vscode/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       56 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/.vscode/settings.json
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1546 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/LICENSE
--rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4132 2024-04-24 23:07:10.113564 qcmanybody-0.1.0/PKG-INFO
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1426 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/README.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      445 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/codecov.yml
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.097564 qcmanybody-0.1.0/docs/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       35 2024-03-28 22:10:11.000000 qcmanybody-0.1.0/docs/api.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      385 2024-04-24 22:59:57.000000 qcmanybody-0.1.0/docs/changelog.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4231 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/core-interface.md
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.093564 qcmanybody-0.1.0/docs/extensions/
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.098564 qcmanybody-0.1.0/docs/extensions/mdantic_v1/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      241 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/extensions/mdantic_v1/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5334 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/extensions/mdantic_v1/mdantic.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       25 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/high-level-interface.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-03-17 22:44:27.000000 qcmanybody-0.1.0/docs/how-to-guides.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1473 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/index.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1694 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/keywords.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    19797 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/logo.png
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2251 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/qcschema.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/docs/results.md
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.098564 qcmanybody-0.1.0/docs/stylesheets/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      133 2024-03-28 22:10:11.000000 qcmanybody-0.1.0/docs/stylesheets/extra.css
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1816 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/mkdocs.yml
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1505 2024-04-24 22:59:57.000000 qcmanybody-0.1.0/pyproject.toml
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.099564 qcmanybody-0.1.0/qcmanybody/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      218 2024-04-16 17:54:39.000000 qcmanybody-0.1.0/qcmanybody/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7273 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/builder.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.100564 qcmanybody-0.1.0/qcmanybody/hide/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5871 2024-04-24 14:42:51.000000 qcmanybody-0.1.0/qcmanybody/hide/asdf.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1158 2024-04-16 23:10:20.000000 qcmanybody-0.1.0/qcmanybody/hide/hold_test_mbe_keywords.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      658 2024-03-15 16:39:58.000000 qcmanybody-0.1.0/qcmanybody/hide/tsts.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    25486 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/manybody.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.101564 qcmanybody-0.1.0/qcmanybody/models/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      155 2024-04-24 19:42:36.000000 qcmanybody-0.1.0/qcmanybody/models/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    24945 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/models/manybody_pydv1.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    41888 2024-04-24 21:06:27.000000 qcmanybody-0.1.0/qcmanybody/models/qcng_computer.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3120 2024-03-08 22:15:43.000000 qcmanybody-0.1.0/qcmanybody/test_nbody_compute_list.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.103564 qcmanybody-0.1.0/qcmanybody/tests/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2111 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/addons.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3511 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/common.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.107564 qcmanybody-0.1.0/qcmanybody/tests/component_data/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      561 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      386 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7612 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4480 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)   112168 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    61149 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      480 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      176 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5776 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1139 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    77120 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9708 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      335 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_energy_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      316 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_energy_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4448 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4142 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    65348 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    59491 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3936 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/generate_component_data.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.112564 qcmanybody-0.1.0/qcmanybody/tests/ref_data/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      925 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      863 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    30651 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      908 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      729 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    22108 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      931 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      914 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      940 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      540 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26095 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      921 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      499 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9825 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      946 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      924 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      858 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6579 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18555 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      871 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5520 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    17643 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      856 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    86478 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    76866 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      869 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    69847 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    71086 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    45615 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_mbe_he4_multilevel.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    38790 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_mbe_he4_singlelevel.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15056 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_mbe_het4_grad.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    12554 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_mbe_keywords.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1425 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_multi.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1577 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_multi_ss.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1412 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_single.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11514 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/test_utils.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7774 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/tests/utils.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15681 2024-04-24 19:42:44.000000 qcmanybody-0.1.0/qcmanybody/utils.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 23:07:10.112564 qcmanybody-0.1.0/qcmanybody.egg-info/
--rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4132 2024-04-24 23:07:10.000000 qcmanybody-0.1.0/qcmanybody.egg-info/PKG-INFO
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4302 2024-04-24 23:07:10.000000 qcmanybody-0.1.0/qcmanybody.egg-info/SOURCES.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        1 2024-04-24 23:07:10.000000 qcmanybody-0.1.0/qcmanybody.egg-info/dependency_links.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      108 2024-04-24 23:07:10.000000 qcmanybody-0.1.0/qcmanybody.egg-info/requires.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       11 2024-04-24 23:07:10.000000 qcmanybody-0.1.0/qcmanybody.egg-info/top_level.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       38 2024-04-24 23:07:10.114564 qcmanybody-0.1.0/setup.cfg
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.058955 qcmanybody-0.2.0/
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.030955 qcmanybody-0.2.0/.github/
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.035955 qcmanybody-0.2.0/.github/workflows/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5302 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/.github/workflows/ci.yml
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3113 2024-04-27 06:11:03.000000 qcmanybody-0.2.0/.gitignore
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.035955 qcmanybody-0.2.0/.vscode/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       56 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/.vscode/settings.json
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1546 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/LICENSE
+-rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4394 2024-05-13 18:07:04.057955 qcmanybody-0.2.0/PKG-INFO
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1688 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/README.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      445 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/codecov.yml
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.039955 qcmanybody-0.2.0/docs/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       35 2024-03-28 22:10:11.000000 qcmanybody-0.2.0/docs/api.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2150 2024-05-13 18:03:09.000000 qcmanybody-0.2.0/docs/changelog.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4341 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/core-interface.md
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.031955 qcmanybody-0.2.0/docs/extensions/
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.040955 qcmanybody-0.2.0/docs/extensions/mdantic_v1/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      241 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/docs/extensions/mdantic_v1/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5334 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/docs/extensions/mdantic_v1/mdantic.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       25 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/docs/high-level-interface.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-03-17 22:44:27.000000 qcmanybody-0.2.0/docs/how-to-guides.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1737 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/index.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4583 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/keywords.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    19797 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/docs/logo.png
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2573 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/docs/qcschema.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      304 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/results.md
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.040955 qcmanybody-0.2.0/docs/stylesheets/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      133 2024-03-28 22:10:11.000000 qcmanybody-0.2.0/docs/stylesheets/extra.css
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1877 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/mkdocs.yml
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1505 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/pyproject.toml
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.041955 qcmanybody-0.2.0/qcmanybody/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      218 2024-05-03 01:04:53.000000 qcmanybody-0.2.0/qcmanybody/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7273 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/builder.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.043955 qcmanybody-0.2.0/qcmanybody/hide/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5871 2024-04-24 14:42:51.000000 qcmanybody-0.2.0/qcmanybody/hide/asdf.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1158 2024-04-16 23:10:20.000000 qcmanybody-0.2.0/qcmanybody/hide/hold_test_mbe_keywords.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      658 2024-03-15 16:39:58.000000 qcmanybody-0.2.0/qcmanybody/hide/tsts.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    25486 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/manybody.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.044955 qcmanybody-0.2.0/qcmanybody/models/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      266 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/qcmanybody/models/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1330 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/models/generalized_optimization.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11042 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/models/manybody_input_pydv1.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15581 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/models/manybody_output_pydv1.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26556 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/qcng_computer.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.048955 qcmanybody-0.2.0/qcmanybody/tests/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2111 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/addons.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3511 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/common.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.051955 qcmanybody-0.2.0/qcmanybody/tests/component_data/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      561 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      386 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7612 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4480 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)   112168 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    61149 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      480 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      176 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5776 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1139 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    77120 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9708 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      335 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_energy_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      316 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_energy_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4448 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4142 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    65348 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    59491 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3936 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/generate_component_data.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.056955 qcmanybody-0.2.0/qcmanybody/tests/ref_data/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      925 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      863 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    30651 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      908 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      729 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    22108 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      931 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      914 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      940 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      540 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26095 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      921 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      499 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9825 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      946 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      924 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      858 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6579 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18555 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      871 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5520 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    17643 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      856 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    86478 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    76866 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      869 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    69847 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    71086 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    45626 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_multilevel.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    39159 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_singlelevel.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15035 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_het4_grad.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    12835 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_keywords.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1425 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_multi.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1577 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_multi_ss.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1412 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_single.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11514 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_utils.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7774 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/utils.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15683 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/utils.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.056955 qcmanybody-0.2.0/qcmanybody.egg-info/
+-rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4394 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/PKG-INFO
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4352 2024-05-13 18:07:04.000000 qcmanybody-0.2.0/qcmanybody.egg-info/SOURCES.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        1 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/dependency_links.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      108 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/requires.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       11 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/top_level.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       38 2024-05-13 18:07:04.058955 qcmanybody-0.2.0/setup.cfg
```

### Comparing `qcmanybody-0.1.0/.github/workflows/ci.yml` & `qcmanybody-0.2.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             python-version: "3.8"
             runs-on: ubuntu-latest
             pytest: "-m 'not addon'"
 
           - label: Py-max
             python-version: "3.12"
             runs-on: ubuntu-latest
-            pytest: "-k 'not (he4 and (3b or 4b))'"
+            pytest: "-k 'not (he4 and (3b or 4b) and not sio)'"
 
     name: "🐍 ${{ matrix.cfg.python-version }} • ${{ matrix.cfg.label }} • ${{ matrix.cfg.runs-on }}"
     runs-on: ${{ matrix.cfg.runs-on }}
 
     steps:
     - uses: actions/checkout@v4
       with:
```

### Comparing `qcmanybody-0.1.0/.gitignore` & `qcmanybody-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/LICENSE` & `qcmanybody-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/PKG-INFO` & `qcmanybody-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcmanybody
-Version: 0.1.0
+Version: 0.2.0
 Summary: QCManyBody
 Author-email: Benjamin Pritchard <bpp4@vt.edu>, "Lori A. Burns" <lori.burns@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, The Molecular Sciences Software Institute
         All rights reserved.
         
@@ -52,15 +52,15 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 QCManyBody
 ==========
 
-<p align="center">
+<p align="left">
     <picture>
     <img alt="QCManyBody Logo" src="https://github.com/MolSSI/QCManyBody/blob/main/docs/logo.png" height="150px">
     </picture>
 </p>
 
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/MolSSI/QCManyBody/ci.yml?logo=github)](https://github.com/MolSSI/QCManyBody/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/loriab/QCManyBody/graph/badge.svg?token=E4S0706HJ0)](https://codecov.io/gh/loriab/QCManyBody)
@@ -69,16 +69,27 @@
 ![python](https://img.shields.io/badge/python-3.8+-blue.svg)
 
 QCManyBody is a python package for running quantum chemistry manybody expansions and interaction calculations in a
 package-independent way.
 
 ## Installation
 
-Currently, the package is only available on [GitHub](https://github.com/MolSSI/QCManyBody). To install directly
-from GitHub, use the following command:
+QCManyBody is available from [PyPI](https://pypi.org/project/qcmanybody) and from
+[conda-forge](https://anaconda.org/conda-forge/qcmanybody).
+
+```bash
+# Installation from PyPI
+pip install qcmanybody
+
+# Installation from conda-forge
+conda install -c conda-forge qcmanybody
+```
+
+To install the latest development version directly from
+[GitHub](https://github.com/MolSSI/QCManyBody), you can use the following command:
 
 ```bash
 pip install git+https://github.com/MolSSI/QCManyBody.git
 ```
 
 ## Documentation
```

### Comparing `qcmanybody-0.1.0/README.md` & `qcmanybody-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 QCManyBody
 ==========
 
-<p align="center">
+<p align="left">
     <picture>
     <img alt="QCManyBody Logo" src="https://github.com/MolSSI/QCManyBody/blob/main/docs/logo.png" height="150px">
     </picture>
 </p>
 
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/MolSSI/QCManyBody/ci.yml?logo=github)](https://github.com/MolSSI/QCManyBody/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/loriab/QCManyBody/graph/badge.svg?token=E4S0706HJ0)](https://codecov.io/gh/loriab/QCManyBody)
@@ -14,16 +14,27 @@
 ![python](https://img.shields.io/badge/python-3.8+-blue.svg)
 
 QCManyBody is a python package for running quantum chemistry manybody expansions and interaction calculations in a
 package-independent way.
 
 ## Installation
 
-Currently, the package is only available on [GitHub](https://github.com/MolSSI/QCManyBody). To install directly
-from GitHub, use the following command:
+QCManyBody is available from [PyPI](https://pypi.org/project/qcmanybody) and from
+[conda-forge](https://anaconda.org/conda-forge/qcmanybody).
+
+```bash
+# Installation from PyPI
+pip install qcmanybody
+
+# Installation from conda-forge
+conda install -c conda-forge qcmanybody
+```
+
+To install the latest development version directly from
+[GitHub](https://github.com/MolSSI/QCManyBody), you can use the following command:
 
 ```bash
 pip install git+https://github.com/MolSSI/QCManyBody.git
 ```
 
 ## Documentation
```

### Comparing `qcmanybody-0.1.0/docs/core-interface.md` & `qcmanybody-0.2.0/docs/core-interface.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
 
 ## Using the core interface
 
 The core interface is accessed through the [`ManyBodyCalculator`][qcmanybody.manybody.ManyBodyCalculator]
 class.
 
-The first step is to create a molecule. This molecule is a QCElemental molecule object, and must contain fragments.
+The first step is to create a molecule. This molecule is a
+[QCElemental molecule object](https://molssi.github.io/QCElemental/model_molecule.html), and must contain fragments.
+(see also: [moleule input](keywords.md#molecule))
 
 ```python
 import qcmanybody as qcmb
 import qcelemental as qcel
 
 # Create a molecule with 3 hydrogen atoms, each as its own fragment
 mol = qcel.models.Molecule(symbols=['h', 'h', 'h'],
@@ -38,18 +40,18 @@
     return_total_data=True,
     supersystem_ie_only=False
 )
 ```
 
 The `levels` option is a dictionary that specifies the n-body level as a key, then an arbitrary
 string as the description of the calculation to be performed at the n-body level. This string is
-termed the 'model chemistry' is completely arbitrary; it only has meaning to the user, and the user is expected to map these strings
-to some meaningful definition of a calculation.
+termed the 'model chemistry' is completely arbitrary; it only has meaning to the user, and the user is expected to
+map these strings to some meaningful definition of a calculation.
 
-**Note**: The core interface is less flexible than the high-level interface when it comes to the `levels` option.
+**Note:** The core interface is less flexible than the high-level interface when it comes to the `levels` option.
     In the core interface, all levels must be accounted for (that is, keys must go from 1 to the maximum
     nbody you would like to calculate). All levels must be present even if the model chemistry
     is the same for all levels.
 
 For a complete discussion of the other options available in the `ManyBodyCalculator` object, see the
 [keywords discussion](keywords.md)
 the [`ManyBodyCalculator API documentation`][qcmanybody.manybody.ManyBodyCalculator].
```

### Comparing `qcmanybody-0.1.0/docs/extensions/mdantic_v1/mdantic.py` & `qcmanybody-0.2.0/docs/extensions/mdantic_v1/mdantic.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/docs/index.md` & `qcmanybody-0.2.0/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 # QCManyBody Documentation
 
 QCManyBody is a python package for running quantum chemistry manybody expansions and interaction calculations in a
 package-independent way.
 
 ## Installation
 
-Currently, the package is only available on [GitHub](https://github.com/MolSSI/QCManyBody). To install directly
-from GitHub, use the following command:
+QCManyBody is available from [PyPI](https://pypi.org/project/qcmanybody) and from
+[conda-forge](https://anaconda.org/conda-forge/qcmanybody).
+
+```bash
+# Installation from PyPI
+pip install qcmanybody
+
+# Installation from conda-forge
+conda install -c conda-forge qcmanybody
+```
+
+To install the latest development version directly from
+[GitHub](https://github.com/MolSSI/QCManyBody), you can use the following command:
 
 ```bash
 pip install git+https://github.com/MolSSI/QCManyBody.git
 ```
 
 ## Package Overview
 
 The package has two main interfaces. The high-level interface allows for a comprehensive workflow, where the user
 provides complete information about the calculation, including the full specification (method, basis set, etc.) of the
 manybody calculation. This is designed to work with [QCEngine](https://github.com/MolSSI/QCEngine) or other packages
 that implement the [QCSchema](https://github.com/MolSSI/QCSchema).
 
-For more information, see (High-level interface)(high-level-interface.md).
+For more information, see [High-level interface](high-level-interface.md).
 
 QCManyBody also has a core low-level interface that allows for more flexibility in how the calculations are run. This
 interface generally takes a molecule and an arbitrary definition of quantum chemistry specifications, and expects
 the user to run them themselves.
 
-For more information, see (Core interface)(core-interface.md).
+For more information, see [Core interface](core-interface.md).
 
 ## Table of Contents
 
 1. [Common Keywords and Options](keywords.md)
 2. [High-level Interface](high-level-interface.md)
 3. [Core Interface](core-interface.md)
 4. [Results](results.md)
```

### Comparing `qcmanybody-0.1.0/docs/logo.png` & `qcmanybody-0.2.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/docs/qcschema.md` & `qcmanybody-0.2.0/docs/qcschema.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 
 <!-- ====  Inputs  ================================================================= -->
 
 ::: qcmanybody.models.BsseEnum
+    options:
+        show_root_heading: true
 
 
 ::: qcmanybody.models.ManyBodyKeywords
     options:
         show_root_heading: true
 
-$pydantic: qcmanybody.models.manybody_pydv1.ManyBodyKeywords
+$pydantic: qcmanybody.models.manybody_input_pydv1.ManyBodyKeywords
 
 
-::: qcmanybody.models.manybody_pydv1.ManyBodySpecification
+::: qcmanybody.models.ManyBodySpecification
     options:
         show_root_heading: true
 
-$pydantic: qcmanybody.models.manybody_pydv1.ManyBodySpecification
+$pydantic: qcmanybody.models.manybody_input_pydv1.ManyBodySpecification
 
 
 ::: qcmanybody.models.ManyBodyInput
     options:
         show_root_heading: true
 
-$pydantic: qcmanybody.models.manybody_pydv1.ManyBodyInput
+$pydantic: qcmanybody.models.manybody_input_pydv1.ManyBodyInput
 
 
 <!-- ====  Protocols  ============================================================== -->
 
 <!--
 ::: qcmanybody.models.manybody_pydv1.ManyBodyProtocolEnum
 
 
-::: qcmanybody.models.manybody_pydv1.ManyBodyProtocols
+::: qcmanybody.models.manybody_input_pydv1.ManyBodyProtocols
     options:
         show_root_heading: true
 
-$pydantic: qcmanybody.models.manybody_pydv1.ManyBodyProtocols
+$pydantic: qcmanybody.models.manybody_input_pydv1.ManyBodyProtocols
 -->
 
 
 <!-- ====  Properties/Outputs  ===================================================== -->
 
+!!! note
+
+    The properties model is generated dynamically based on a constant
+    ``MAX_NBODY``. To not overload the docs table, this is set to 5, which
+    covers full calculations on tetramers. To use a larger
+    ``ManyBodyKeywords.max_nbody``, reset this value.
+
+        import qcmanybody as qcmb
+        qcmb.models.MAX_NBODY = 8
+
+
 ::: qcmanybody.models.ManyBodyResultProperties
     options:
         show_root_heading: true
 
 $pydantic: qcmanybody.models.ManyBodyResultProperties
 
 
@@ -86,11 +99,7 @@
           - model_post_init
           - model_rebuild
           - model_validate
           - model_validate_json
           - copy
 -->
 
-::: qcmanybody.resize_gradient
-    options:
-        show_root_heading: true
-
```

### Comparing `qcmanybody-0.1.0/mkdocs.yml` & `qcmanybody-0.2.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,17 @@
           - https://matplotlib.org/stable/objects.inv
           - https://molssi.github.io/QCElemental/objects.inv
           - https://molssi.github.io/QCEngine/objects.inv
           - https://molssi.github.io/QCFractal/objects.inv
 
 markdown_extensions:
   - mdantic_v1
+  - admonition
+  - pymdownx.details
+  - pymdownx.superfences
 
 nav:
   - Home: index.md
   - high-level-interface.md
   - core-interface.md
   - QCSchema: qcschema.md
   - How-To Guides: how-to-guides.md
```

### Comparing `qcmanybody-0.1.0/pyproject.toml` & `qcmanybody-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/builder.py` & `qcmanybody-0.2.0/qcmanybody/builder.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/hide/asdf.py` & `qcmanybody-0.2.0/qcmanybody/hide/asdf.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/hide/hold_test_mbe_keywords.py` & `qcmanybody-0.2.0/qcmanybody/hide/hold_test_mbe_keywords.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/hide/tsts.py` & `qcmanybody-0.2.0/qcmanybody/hide/tsts.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/manybody.py` & `qcmanybody-0.2.0/qcmanybody/manybody.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/models/manybody_pydv1.py` & `qcmanybody-0.2.0/qcmanybody/models/manybody_output_pydv1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,243 +1,22 @@
 from __future__ import annotations
 
-from enum import Enum, IntEnum
-from typing import Any, Dict, List, Optional, Literal, Tuple, Union, TYPE_CHECKING
+from typing import Any, Dict, Literal, Optional, TYPE_CHECKING, Union
 
 # v2: from pydantic import create_model, Field, field_validator, FieldValidationInfo
 try:
     from pydantic.v1 import create_model, Field, validator
 except ImportError:
     from pydantic import create_model, Field, validator
 
 from qcelemental.models.types import Array
-#from .basemodels import ExtendedConfigDict, ProtoModel
-from qcelemental.models.common_models import Model
-from qcelemental.models.molecule import Molecule
-from qcelemental.models.results import AtomicResultProperties, AtomicResultProtocols
-from qcelemental.models import DriverEnum, ProtoModel, Provenance
-
-
-# ====  Misplaced & Next Models  ================================================
-
-class AtomicSpecification(ProtoModel):
-    """Specification for a single point QC calculation"""
-
-    keywords: Dict[str, Any] = Field({}, description="The program specific keywords to be used.")
-    program: str = Field(..., description="The program for which the Specification is intended.")
-
-    schema_name: Literal["qcschema_atomicspecification"] = "qcschema_atomicspecification"
-    driver: DriverEnum = Field(..., description=DriverEnum.__doc__)
-    model: Model = Field(..., description=Model.__doc__)
-    protocols: AtomicResultProtocols = Field(
-        AtomicResultProtocols(),
-        description=AtomicResultProtocols.__doc__,
-    )
-
-
-class ResultBase(ProtoModel):
-    """Base class for all result classes"""
-
-    #input_data: InputBase = Field(..., description=InputBase.__doc__)
-    input_data: Any
-    success: bool = Field(
-        ...,
-        description="A boolean indicator that the operation succeeded or failed. Allows programmatic assessment of "
-        "all results regardless of if they failed or succeeded by checking `result.success`.",
-    )
-    stdout: Optional[str] = Field(
-        None,
-        description="The primary logging output of the program, whether natively standard output or a file. Presence vs. absence (or null-ness?) configurable by protocol.",
-    )
-    stderr: Optional[str] = Field(None, description="The standard error of the program execution.")
+from qcelemental.models.results import AtomicResult, AtomicResultProperties
+from qcelemental.models import ProtoModel, Provenance
 
-
-class SuccessfulResultBase(ResultBase):
-    """Base object for any successful result"""
-
-    success: Literal[True] = Field(True, description="Always `True` for a successful result")
-
-
-# ====  Inputs  =================================================================
-
-class BsseEnum(str, Enum):
-#class BsseEnum(IntEnum):
-    """Available basis-set superposition error (BSSE) treatments."""
-
-    nocp = "nocp"  # plain supramolecular interaction energy
-    cp = "cp"      # Boys-Bernardi counterpoise correction; site-site functional counterpoise (SSFC)
-    vmfc = "vmfc"  # Valiron-Mayer function counterpoise
-    ssfc = "cp"
-
-    def formal(self):
-        return {
-            "nocp": "Non-Counterpoise Corrected",
-            "cp": "Counterpoise Corrected",
-            "vmfc": "Valiron-Mayer Function Counterpoise",
-        }[self]
-
-    def abbr(self):
-        return {
-            "nocp": "NoCP",
-            "cp": "CP",
-            "vmfc": "VMFC",
-        }[self]
-
-
-FragBasIndex = Tuple[Tuple[int], Tuple[int]]
-
-
-class ManyBodyKeywords(ProtoModel):
-    """The many-body-specific keywords for user control."""
-
-    bsse_type: List[BsseEnum] = Field(
-        [BsseEnum.cp],
-        # definitive description
-        description="Requested BSSE treatments. First in list determines which interaction or total "
-            "energy/gradient/Hessian returned.",
-    )
-    embedding_charges: Dict[int, List[float]] = Field(
-        {},
-        description="Atom-centered point charges to be used on molecule fragments whose basis sets are not included in "
-            "the computation. Keys: 1-based index of fragment. Values: list of atom charges for that fragment.",
-            # TODO embedding charges should sum to fragment charge, right? enforce?
-            # TODO embedding charges irrelevant to CP (basis sets always present)?
-        json_schema_extra={
-            "shape": ["nfr", "<varies: nat in ifr>"],
-        },
-    )
-    return_total_data: Optional[bool] = Field(
-        None,
-        validate_default=True,
-        # definitive description
-        description="When True, returns the total data (energy/gradient/Hessian) of the system, otherwise returns "
-            "interaction data. Default is False for energies, True for gradients and Hessians. Note that the calculation "
-            "of counterpoise corrected total energies implies the calculation of the energies of monomers in the monomer "
-            "basis, hence specifying ``return_total_data = True`` may carry out more computations than "
-            "``return_total_data = False``. For gradients and Hessians, ``return_total_data = False`` is rarely useful.",
-    )
-    levels: Optional[Dict[Union[int, Literal["supersystem"]], str]] = Field(
-        None,
-        # definitive description. appended in Computer
-        description="Dictionary of different levels of theory for different levels of expansion. Note that the primary "
-            "method_string is not used when this keyword is given. ``supersystem`` computes all higher order n-body "
-            "effects up to the number of fragments; this higher-order correction uses the nocp basis, regardless of "
-            "bsse_type. A method fills in for any lower unlisted nbody levels. Note that if "
-            "both this and max_nbody are provided, they must be consistent. Examples: "
-            "SUPERSYSTEM definition suspect"
-            "* {1: 'ccsd(t)', 2: 'mp2', 'supersystem': 'scf'} "
-            "* {2: 'ccsd(t)/cc-pvdz', 3: 'mp2'} "
-            "* Now invalid: {1: 2, 2: 'ccsd(t)/cc-pvdz', 3: 'mp2'} ",
-    )
-    max_nbody: Optional[int] = Field(
-        None,
-        validate_default=True,
-        # definitive description
-        description="Maximum number of bodies to include in the many-body treatment. Possible: max_nbody <= nfragments. "
-            "Default: max_nbody = nfragments.",
-    )
-    supersystem_ie_only: Optional[bool] = Field(
-        False,
-        validate_default=True,
-        # definitive description
-        description="Target the supersystem total/interaction energy (IE) data over the many-body expansion (MBE) "
-            "analysis, thereby omitting intermediate-body calculations. When False (default), compute each n-body level "
-            "in the MBE up through ``max_nbody``. When True (only allowed for ``max_nbody = nfragments``), only compute "
-            "enough for the overall interaction/total energy: max_nbody-body and 1-body. When True, properties "
-            "``INTERACTION {driver} THROUGH {max_nbody}-BODY`` will always be available; ``TOTAL {driver} THROUGH "
-            "{max_nbody}-BODY`` will be available depending on ``return_total_data``; and ``{max_nbody}-BODY "
-            "CONTRIBUTION TO {driver}`` won't be available (except for dimers). This keyword produces no savings for a "
-            "two-fragment molecule. But for the interaction energy of a three-fragment molecule, for example, 2-body "
-            "subsystems can be skipped with ``supersystem_ie_only=True`` Do not use with ``vmfc`` in ``bsse_type``"
-            "as it cannot produce savings."
-    )
-
-    # v2: @field_validator("bsse_type", mode="before")
-    @validator("bsse_type", pre=True)
-    @classmethod
-    def set_bsse_type(cls, v: Any) -> List[BsseEnum]:
-        if not isinstance(v, list):
-            v = [v]
-        # emulate ordered set
-        # * bt.lower() as return (w/i `list(dict.fromkeys([bt.lower() ...`)
-        #   works until aliases added to BsseEnum
-        # * BsseEnum[bt].value as return works for good vals, but passing bad
-        #   vals through as bt lets pydantic raise a clearer error message
-        return list(dict.fromkeys([(BsseEnum[bt.lower()].value if bt.lower() in BsseEnum.__members__ else bt.lower()) for bt in v]))
-
-
-class ManyBodySpecification(ProtoModel):
-
-    schema_name: Literal["qcschema_manybodyspecification"] = "qcschema_manybodyspecification"
-    #provenance: Provenance = Field(Provenance(**provenance_stamp(__name__)), description=Provenance.__doc__)
-    keywords: ManyBodyKeywords = Field(..., description=ManyBodyKeywords.__doc__)
-    #program: str = Field(..., description="The program for which the Specification is intended.")
-    driver: DriverEnum = Field(
-        ...,
-        description="The computation driver; i.e., energy, gradient, hessian.",
-    )
-    #specification: Union[AtomicSpecification, Dict[str, AtomicSpecification]] = Field(
-    specification: Dict[str, AtomicSpecification] = Field(
-        ...,
-        description="??? TODO expand to cbs, fd",
-    )
-
-    # v2: @field_validator("specification", mode="before")
-    @validator("specification", pre=True)
-    @classmethod
-    def set_specification(cls, v: Any) -> Dict[str, AtomicSpecification]:
-        #print(f"hit atomicspecification validator with {type(v)=} {v}", end="")
-        # v could be model instance or dict
-        if isinstance(v, AtomicSpecification) or "model" in v:
-            v = {"(auto)": v}
-        #print(f" ... setting v={v}")
-        return v
-
-
-class ManyBodyInput(ProtoModel):
-
-    schema_name: Literal["qcschema_manybodyinput"] = "qcschema_manybodyinput"
-    #provenance: Provenance = Field(Provenance(**provenance_stamp(__name__)), description=Provenance.__doc__)
-    specification: ManyBodySpecification = Field(
-        ...,
-        description="???",
-    )
-    molecule: Molecule = Field(
-        ...,
-        description="Target molecule for many-body expansion (MBE) or interaction energy (IE) analysis.",
-    )
-    #protocols
-
-
-# ====  Protocols  ==============================================================
-
-class ManyBodyProtocolEnum(str, Enum):
-    """
-    Which atomic evaluations to keep in a many body evaluation.
-    """
-
-    all = "all"
-    all_real = "all_real"
-    largest_body = "largest_body"
-    none = "none"
-
-
-class ManyBodyProtocols(ProtoModel):
-    """
-    Protocols regarding the manipulation of a ManyBody output data.
-    """
-
-    atomics: ManyBodyProtocolEnum = Field(
-        ManyBodyProtocolEnum.all,
-        description=str(ManyBodyProtocolEnum.__doc__),
-    )
-
-    # v2: model_config = ExtendedConfigDict(force_skip_defaults=True)
-    class Config:
-        force_skip_defaults = True
+from .manybody_input_pydv1 import ManyBodyInput, SuccessfulResultBase
 
 
 # ====  Properties  =============================================================
 
 # class ManyBodyResultProperties defined through create_model
 
 manybodyresultproperties_doc = """
@@ -497,15 +276,15 @@
     class Config(ProtoModel.Config):
         serialize_skip_defaults = True
         force_skip_defaults = True
 
 if TYPE_CHECKING:
     ManyBodyResultProperties = ProtoModelSkipDefaults
 else:
-    # if/else suppresses a warning about using dynamically generated class as Field type in ManyBodyResults
+    # if/else suppresses a warning about using a dynamically generated class as Field type in ManyBodyResults
     ManyBodyResultProperties = create_model(
     "ManyBodyResultProperties",
     #__doc__=manybodyresultproperties_doc,  # needs later pydantic
     __base__=ProtoModelSkipDefaults,
     **mbprop,
 )
 
@@ -537,17 +316,28 @@
     )
     properties: ManyBodyResultProperties = Field(..., description=str(ManyBodyResultProperties.__doc__))
     component_properties: Dict[str, AtomicResultProperties] = Field(
         ...,
         description="The key results for each subsystem species computed. Keys contain modelchem, real and ghost information (e.g., `'[\"(auto)\", [2], [1, 2, 3]]'`). Values are total e/g/H/property results. Array values, if present, are sized and shaped for the full supersystem.",
 
     )
+    component_results: Dict[str, AtomicResult] = Field({}, description="Detailed results")
     return_result: Union[float, Array[float], Dict[str, Any]] = Field(
         ...,
         description="The primary return specified by the :attr:`~qcelemental.models.AtomicInput.driver` field. Scalar if energy; array if gradient or hessian; dictionary with property keys if properties.",
     )
     stdout: Optional[str] = Field(
         None,
         description="The primary logging output of the program, whether natively standard output or a file. Presence vs. absence (or null-ness?) configurable by protocol.",
     )
     stderr: Optional[str] = Field(None, description="The standard error of the program execution.")
     success: Literal[True] = Field(True, description="Always `True` for a successful result")
+
+    @validator("component_results")
+    def _component_results(cls, value, values):
+        crp = values["input_data"].specification.protocols.component_results
+        if crp == "all":
+            return value
+        elif crp == "none":
+            return {}
+        else:
+            raise ValueError(f"Protocol `component_resutls:{crp}` is not understood")
```

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/addons.py` & `qcmanybody-0.2.0/qcmanybody/tests/addons.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/common.py` & `qcmanybody-0.2.0/qcmanybody/tests/common.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/generate_component_data.py` & `qcmanybody-0.2.0/qcmanybody/tests/generate_component_data.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst` & `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_mbe_he4_multilevel.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_multilevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pytest
 
 from qcelemental import constants
 from qcelemental.models import Molecule
 # v2: from qcelemental.models.procedures_manybody import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
 from qcelemental.testing import compare_values, compare_recursive
 
-from qcmanybody.models.manybody_pydv1 import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
-from qcmanybody.models.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
+from qcmanybody.models import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
+from qcmanybody.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
 
 import qcengine as qcng
 from .addons import using
 from .test_mbe_he4_singlelevel import sumdict as sumdict_single
 
 def skprop(qcvar):
     # qcng: return qcng.procedures.manybody.qcvars_to_manybodyproperties[qcvar]
@@ -722,15 +722,15 @@
 
     mbe_keywords = ManyBodyKeywords(levels=levels, **mbe_keywords)
     mbe_data_multilevel_631g["molecule"] = he_tetramer
     mbe_data_multilevel_631g["specification"]["keywords"] = mbe_keywords
     mbe_model = ManyBodyInput(**mbe_data_multilevel_631g)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_qcschema_ben(mbe_model)
+    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
     print(f"MMMMMMM {request.node.name}")
     pprint.pprint(ret.dict(), width=200)
 
     refs = he4_refs_conv_multilevel_631g[pattern]
     ans = refs[anskey]
     ref_nmbe = calcinfo_nmbe[pattern]
     ref_bodykeys = bodykeys[pattern] if pattern in bodykeys else bodykeys
@@ -815,15 +815,15 @@
 
     mbe_keywords = ManyBodyKeywords(levels=levels, **mbe_keywords)
     mbe_data_multilevel_631g["molecule"] = he_tetramer
     mbe_data_multilevel_631g["specification"]["keywords"] = mbe_keywords
     mbe_model = ManyBodyInput(**mbe_data_multilevel_631g)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_qcschema_ben(mbe_model)
+    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
     print(f"MMMMMMM {request.node.name}")
     pprint.pprint(ret.dict(), width=200)
 
     refs = he4_refs_conv_multilevel_631g[pattern]
     ans = refs[anskey]
     ref_nmbe = calcinfo_nmbe[pattern]
     ref_bodykeys = bodykeys[pattern] if pattern in bodykeys else bodykeys
@@ -892,14 +892,15 @@
        },
        id="3b_vmfc"),
 ])
 def test_count_he4_multi(mbe_keywords, ref_count, he_tetramer, request):
     atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": "mybas"}, program="myqc", driver="energy")
     mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy"}, molecule=he_tetramer)
 
-    ret = ManyBodyComputerQCNG.from_qcschema_ben(mbe_model, build_tasks=False)
+    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model, build_tasks=False)
+    ret = ret.qcmb_calculator
 
     text, dcount = ret.format_calc_plan()
     assert compare_recursive(ref_count["all"], dcount, atol=1.e-6)
     for sset in ["all", "cp", "nocp", "vmfc_compute"]:
         text, dcount = ret.format_calc_plan(sset)
         assert compare_recursive(ref_count[sset], dcount, atol=1.e-6)
```

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_mbe_he4_singlelevel.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_singlelevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import pytest
 
 from qcelemental import constants
 from qcelemental.models import Molecule
 # v2: from qcelemental.models.procedures_manybody import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
 from qcelemental.testing import compare_values, compare_recursive
 
-from qcmanybody.models.manybody_pydv1 import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
-from qcmanybody.models.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
+from qcmanybody.models import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
+from qcmanybody.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
 
 import qcengine as qcng
 from .addons import using
 
 def skprop(qcvar):
     # qcng: return qcng.procedures.manybody.qcvars_to_manybodyproperties[qcvar]
     return qcvars_to_manybodyproperties[qcvar]
@@ -165,15 +165,15 @@
     "vmfc4b_tot": r"""
    ==> N-Body: Valiron-Mayer Function Counterpoise \(VMFC\) energies <==
 
 ^\s+n-Body     Total Energy            Interaction Energy                          N-body Contribution to Interaction Energy
 ^\s+\[Eh\]                    \[Eh\]                  \[kcal/mol\]            \[Eh\]                  \[kcal/mol\]
 ^\s+1\s+-11.5306687\d+        0.0000000\d+        0.00\d+        0.0000000\d+        0.00\d+
 ^\s+2\s+-11.5224489\d+        0.0082197\d+        5.15\d+        0.0082197\d+        5.15\d+
-^\s+3\s+-11.5226845\d+        0.0079841\d+        5.01\d+       -0.0002356\d+       -0.14\d+
+^\s+3\s+-11.5226845\d+        0.0079841\d+        5.01\d+       -0.000235\d+       -0.14\d+
 ^\s+FULL/RTN\s+4\s+-11.5226215\d+        0.0080471\d+        5.04\d+        0.0000629\d+        0.03\d+
 """,
     "cp3b_tot": r"""
    ==> N-Body: Counterpoise Corrected \(CP\) energies <==
 
 ^\s+n-Body     Total Energy            Interaction Energy                          N-body Contribution to Interaction Energy
 ^\s+\[Eh\]                    \[Eh\]                  \[kcal/mol\]            \[Eh\]                  \[kcal/mol\]
@@ -617,19 +617,19 @@
         id="1b_vmfc"),
 ])
 def test_nbody_he4_single(program, basis, keywords, mbe_keywords, anskey, bodykeys, outstrs, calcinfo_nmbe, he_tetramer, request):
     #! MP2/aug-cc-pvDZ many body energies of an arbitrary Helium complex,
     #   addressing 4-body formulas
     # e, wfn = energy('MP2/aug-cc-pVDZ', molecule=he_tetramer, ...)
 
-    atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": basis}, program=program, driver="energy", keywords=keywords)
-    mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy"}, molecule=he_tetramer)
+    atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": basis}, program=program, driver="energy", keywords=keywords, protocols={"stdout": False})
+    mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy", "protocols": {"component_results": "all"}}, molecule=he_tetramer)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_qcschema_ben(mbe_model)
+    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
     print(f"SSSSSSS {request.node.name}")
     # v2: pprint.pprint(ret.model_dump(), width=200)
     pprint.pprint(ret.dict(), width=200)
 
     _inner = request.node.name.split("[")[1].split("]")[0]
     kwdsln, progln = _inner.split("-")
     refs = he4_refs_df if progln == "psi4_df" else he4_refs_conv
@@ -665,14 +665,18 @@
     }.items():
         skp = skprop(qcv)
         assert compare_values(ref, ret.extras["qcvars"][qcv], atol=atol, label=f"[e] qcvars {qcv}")
         assert compare_values(ref, getattr(ret.properties, skp), atol=atol, label=f"[f] skprop {skp}")
     assert compare_values(ans, ret.return_result, atol=atol, label=f"[g] ret")
 
     assert ret.properties.calcinfo_nmbe == ref_nmbe, f"[i] {ret.properties.calcinfo_nmbe=} != {ref_nmbe}"
+    assert len(ret.component_results) == ref_nmbe, f"[k] {len(ret.component_results)=} != {ref_nmbe}; mbe protocol did not take"
+    if ref_nmbe > 0:
+        an_atres = next(iter(ret.component_results.values()))
+        assert an_atres.stdout is None, f"[l] atomic protocol did not take"
 
     if outstrs and progln != "psi4_df":
         for stdoutkey in outstrs:
             assert re.search(sumstr[stdoutkey], ret.stdout, re.MULTILINE), f"[j] N-Body pattern not found: {sumstr[stdoutkey]}"
 
 
 @pytest.mark.parametrize("mbe_keywords,ref_count", [
@@ -704,14 +708,15 @@
         },
         id="3b_vmfc"),
 ])
 def test_count_he4_single(mbe_keywords, ref_count, he_tetramer):
     atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": "mybas"}, program="myqc", driver="energy")
     mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy"}, molecule=he_tetramer)
 
-    ret = ManyBodyComputerQCNG.from_qcschema_ben(mbe_model, build_tasks=False)
+    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model, build_tasks=False)
+    ret = ret.qcmb_calculator
 
     text, dcount = ret.format_calc_plan()
     assert compare_recursive(ref_count["all"], dcount, atol=1.e-6)
     for sset in ["all", "cp", "nocp", "vmfc_compute"]:
         text, dcount = ret.format_calc_plan(sset)
         assert compare_recursive(ref_count[sset], dcount, atol=1.e-6)
```

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_mbe_het4_grad.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_het4_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import pytest
 import numpy as np
 
 from qcelemental.models import Molecule
 from qcelemental.testing import compare_values
 
-from qcmanybody.models.manybody_pydv1 import ManyBodyKeywords, ManyBodyInput
-from qcmanybody.models.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
+from qcmanybody.models import ManyBodyKeywords, ManyBodyInput
+from qcmanybody.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
 
 from .addons import uusing
 
 def skprop(qcvar):
     # qcng: return qcng.procedures.manybody.qcvars_to_manybodyproperties[qcvar]
     return qcvars_to_manybodyproperties[qcvar]
 
@@ -254,15 +254,15 @@
     mbe_keywords = ManyBodyKeywords(**mbe_keywords)
     mbe_data_grad_dtz["molecule"] = het_tetramer
     mbe_data_grad_dtz["specification"]["driver"] = "gradient"
     mbe_data_grad_dtz["specification"]["keywords"] = mbe_keywords
     mbe_model = ManyBodyInput(**mbe_data_grad_dtz)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_qcschema_ben(mbe_model)
+    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
     print(f"MMMMMMM {request.node.name}")
     pprint.pprint(ret.dict(), width=200)
 
     refs = het4_refs_conv_grad_dtz[kwdsln]
     ansE = refs[anskeyE]
     ansG = refs[anskeyG]
     ref_nmbe = calcinfo_nmbe
```

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_mbe_keywords.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_keywords.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 try:
     from pydantic.v1 import ValidationError
 except ImportError:
     from pydantic import ValidationError
 
 import qcelemental
 from qcelemental.models import DriverEnum, Molecule
-from qcmanybody.models.manybody_pydv1 import BsseEnum, ManyBodyInput
+from qcmanybody.models import BsseEnum, ManyBodyInput
 
 import qcengine as qcng
 
 # qcng: from qcengine.procedures.manybody import ManyBodyComputerQCNG
-from qcmanybody.models.qcng_computer import ManyBodyComputerQCNG
+from qcmanybody.qcng_computer import ManyBodyComputerQCNG
 from qcmanybody import ManyBodyCalculator
 
 
 @pytest.fixture(scope="function")
 def mbe_data():
     henehh = Molecule(symbols=["He", "Ne", "H", "H"], fragments=[[0], [1], [2, 3]], geometry=[0, 0, 0, 2, 0, 0, 0, 1, 0, 0, -1, 0])
     return {
@@ -99,15 +99,15 @@
     pytest.param("hessian", {"return_total_data": False}, False),
 ])
 def test_mbe_rtd(mbe_data, driver, kws, ans):
     mbe_data["specification"]["driver"] = driver
     mbe_data["specification"]["keywords"] = kws
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_qcschema(input_model)
+    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.driver == driver
     assert comp_model.return_total_data == ans
 
 
 @pytest.mark.parametrize("kws,ans", [
     pytest.param({}, [3, {3: "(auto)"}, [[1, 2, 3]] ]),
@@ -146,15 +146,15 @@
 
     #pytest.param({}, [ , {}, [] ]),
 ])
 def test_mbe_level_bodies(mbe_data, kws, ans):
     mbe_data["specification"]["keywords"] = kws
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_qcschema(input_model)
+    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.nfragments == 3
     assert comp_model.max_nbody == ans[0]
     assert list(comp_model.levels.items()) == list(ans[1].items())  # compare as OrderedDict
     assert comp_model.nbodies_per_mc_level == ans[2]
 
 
@@ -174,15 +174,15 @@
 ])
 def test_mbe_level_5mer(mbe_data, kws, ans):
     he3ne2 = Molecule(symbols=["He", "He", "He", "Ne", "Ne"], fragments=[[0], [1], [2], [3], [4]], geometry=[0, 0, 0, 2, 0, 0, -2, 0, 0, 0, 2, 0, 0, -2, 0])
     mbe_data["molecule"] = he3ne2
     mbe_data["specification"]["keywords"] = kws
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_qcschema(input_model)
+    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.nfragments == 5
     assert comp_model.max_nbody == ans[0]
     assert list(comp_model.levels.items()) == list(ans[1].items())  # compare as OrderedDict
     assert comp_model.nbodies_per_mc_level == ans[2]
 
 
@@ -196,45 +196,47 @@
 ])
 def test_mbe_level_fails(mbe_data, kws, errmsg):
     mbe_data["specification"]["keywords"] = kws
 
     # v2: with pytest.raises(Exception):
     with pytest.raises(ValidationError) as e:
         input_model = ManyBodyInput(**mbe_data)
-        ManyBodyComputerQCNG.from_qcschema(input_model)
+        ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
     assert errmsg in str(e.value), e.value
 
 
 @pytest.mark.parametrize("kws,ans", [
     pytest.param({}, [BsseEnum.cp]),
     pytest.param({"bsse_type": "CP"}, [BsseEnum.cp]),
     pytest.param({"bsse_type": "nocp"}, [BsseEnum.nocp]),
     pytest.param({"bsse_type": ["vmfc"]}, [BsseEnum.vmfc]),
     pytest.param({"bsse_type": ["vmfc", "nocp"]}, [BsseEnum.vmfc, BsseEnum.nocp]),
     pytest.param({"bsse_type": ["ssFC", "nocp"]}, [BsseEnum.cp, BsseEnum.nocp]),
     pytest.param({"bsse_type": ["ssfc", "cp"]}, [BsseEnum.cp]),
     pytest.param({"bsse_type": ["ssfc", "vmfc", "nocp", "cp"]}, [BsseEnum.cp, BsseEnum.vmfc, BsseEnum.nocp]),
+    pytest.param({"bsse_type": "mbE"}, [BsseEnum.nocp]),
+    pytest.param({"bsse_type": ["ssfc", "cp"]}, [BsseEnum.cp]),
     pytest.param({"bsse_type": "mycp"}, "error"),
     pytest.param({"bsse_type": ["CP", "mycp"]}, "error"),
 ])
 def test_mbe_bsse_type(mbe_data, kws, ans):
     mbe_data["specification"]["keywords"] = kws
 
     if ans == "error":
         with pytest.raises(ValidationError) as e:
             input_model = ManyBodyInput(**mbe_data)
 
         assert "not a valid enumeration member; permitted: 'nocp', 'cp', 'vmfc'" in str(e.value)
         return
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_qcschema(input_model)
+    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
-    assert comp_model.bsse_type == ans
+    assert comp_model.bsse_type == ans, f"{comp_model=} != {ans}"
 
 
 @pytest.mark.parametrize("kws,ans", [
     pytest.param({}, False),
     pytest.param({"max_nbody": 3, "supersystem_ie_only": True}, True),
     pytest.param({"supersystem_ie_only": False}, False),
     pytest.param({"max_nbody": 1, "supersystem_ie_only": True},
@@ -246,21 +248,21 @@
 ])
 def test_mbe_sie(mbe_data, kws, ans):
     mbe_data["specification"]["keywords"] = kws
 
     if isinstance(ans, str):
         input_model = ManyBodyInput(**mbe_data)
         with pytest.raises(ValidationError) as e:
-            comp_model = ManyBodyComputerQCNG.from_qcschema(input_model)
+            ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
         assert ans in str(e.value)
         return
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_qcschema(input_model)
+    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.supersystem_ie_only == ans
 
 
 def test_noncontiguous_fragments_ordinary():
     with pytest.raises(qcelemental.exceptions.ValidationError) as e:
         Molecule(symbols=["H", "Ne", "Cl"], geometry=[0, 0, 0, 2, 0, 0, 0, 2, 0], fragments=[[0, 2], [1]])
```

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_multi.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_multi_ss.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_multi_ss.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_single.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_single.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/test_utils.py` & `qcmanybody-0.2.0/qcmanybody/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/tests/utils.py` & `qcmanybody-0.2.0/qcmanybody/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.1.0/qcmanybody/utils.py` & `qcmanybody-0.2.0/qcmanybody/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                 else:
                     info += f"""  {lbl:>11} {nb:3}        {"N/A":14}  {int_e:20.12f}  {int_e_kcal:20.12f}  {delta_e:20.12f}  {delta_e_kcal:20.12f}\n"""
             previous_e = energy_body_dict[nb]
         else:
             info += f"""  {lbl:>11} {nb:3}        {"N/A":20}  {"N/A":20}  {"N/A":20}  {"N/A":20}  {"N/A":20}\n"""
 
     info += "\n"
-    print(info)
+    # print(info)
     return info
 
 
 def collect_vars(
         bsse: str,
         prop: str,
         body_dict: Mapping[int, Union[float, np.ndarray]],
```

### Comparing `qcmanybody-0.1.0/qcmanybody.egg-info/PKG-INFO` & `qcmanybody-0.2.0/qcmanybody.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcmanybody
-Version: 0.1.0
+Version: 0.2.0
 Summary: QCManyBody
 Author-email: Benjamin Pritchard <bpp4@vt.edu>, "Lori A. Burns" <lori.burns@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, The Molecular Sciences Software Institute
         All rights reserved.
         
@@ -52,15 +52,15 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings[python]; extra == "docs"
 Requires-Dist: tabulate; extra == "docs"
 
 QCManyBody
 ==========
 
-<p align="center">
+<p align="left">
     <picture>
     <img alt="QCManyBody Logo" src="https://github.com/MolSSI/QCManyBody/blob/main/docs/logo.png" height="150px">
     </picture>
 </p>
 
 [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/MolSSI/QCManyBody/ci.yml?logo=github)](https://github.com/MolSSI/QCManyBody/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/loriab/QCManyBody/graph/badge.svg?token=E4S0706HJ0)](https://codecov.io/gh/loriab/QCManyBody)
@@ -69,16 +69,27 @@
 ![python](https://img.shields.io/badge/python-3.8+-blue.svg)
 
 QCManyBody is a python package for running quantum chemistry manybody expansions and interaction calculations in a
 package-independent way.
 
 ## Installation
 
-Currently, the package is only available on [GitHub](https://github.com/MolSSI/QCManyBody). To install directly
-from GitHub, use the following command:
+QCManyBody is available from [PyPI](https://pypi.org/project/qcmanybody) and from
+[conda-forge](https://anaconda.org/conda-forge/qcmanybody).
+
+```bash
+# Installation from PyPI
+pip install qcmanybody
+
+# Installation from conda-forge
+conda install -c conda-forge qcmanybody
+```
+
+To install the latest development version directly from
+[GitHub](https://github.com/MolSSI/QCManyBody), you can use the following command:
 
 ```bash
 pip install git+https://github.com/MolSSI/QCManyBody.git
 ```
 
 ## Documentation
```

### Comparing `qcmanybody-0.1.0/qcmanybody.egg-info/SOURCES.txt` & `qcmanybody-0.2.0/qcmanybody.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 docs/results.md
 docs/extensions/mdantic_v1/__init__.py
 docs/extensions/mdantic_v1/mdantic.py
 docs/stylesheets/extra.css
 qcmanybody/__init__.py
 qcmanybody/builder.py
 qcmanybody/manybody.py
-qcmanybody/test_nbody_compute_list.py
+qcmanybody/qcng_computer.py
 qcmanybody/utils.py
 qcmanybody.egg-info/PKG-INFO
 qcmanybody.egg-info/SOURCES.txt
 qcmanybody.egg-info/dependency_links.txt
 qcmanybody.egg-info/requires.txt
 qcmanybody.egg-info/top_level.txt
 qcmanybody/hide/asdf.py
 qcmanybody/hide/hold_test_mbe_keywords.py
 qcmanybody/hide/tsts.py
 qcmanybody/models/__init__.py
-qcmanybody/models/manybody_pydv1.py
-qcmanybody/models/qcng_computer.py
+qcmanybody/models/generalized_optimization.py
+qcmanybody/models/manybody_input_pydv1.py
+qcmanybody/models/manybody_output_pydv1.py
 qcmanybody/tests/__init__.py
 qcmanybody/tests/addons.py
 qcmanybody/tests/common.py
 qcmanybody/tests/generate_component_data.py
 qcmanybody/tests/test_mbe_he4_multilevel.py
 qcmanybody/tests/test_mbe_he4_singlelevel.py
 qcmanybody/tests/test_mbe_het4_grad.py
```

