# Comparing `tmp/crayopt-0.4.3.tar.gz` & `tmp/crayopt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crayopt-0.4.3.tar", last modified: Fri Nov 24 23:28:05 2023, max compression
+gzip compressed data, was "crayopt-0.5.0.tar", last modified: Mon May 13 14:32:57 2024, max compression
```

## Comparing `crayopt-0.4.3.tar` & `crayopt-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.060277 crayopt-0.4.3/
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-11-24 23:27:49.000000 crayopt-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3406 2023-11-24 23:28:05.059277 crayopt-0.4.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1216 2023-11-24 23:27:49.000000 crayopt-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.048277 crayopt-0.4.3/crayopt/
--rwxrwxrwx   0 root         (0) root         (0)      154 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.051277 crayopt-0.4.3/crayopt/blackbox/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/blackbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/blackbox/evolution_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/blackbox/lax.py
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/blackbox/lin.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/blackbox/meta.py
--rw-rw-rw-   0 root         (0) root         (0)    13763 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/blackbox/random_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.054277 crayopt-0.4.3/crayopt/gradient/
--rwxrwxrwx   0 root         (0) root         (0)      495 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2170 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/adabelief.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/adadelta.py
--rwxrwxrwx   0 root         (0) root         (0)     1175 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/adagrad.py
--rwxrwxrwx   0 root         (0) root         (0)     4948 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/adam.py
--rwxrwxrwx   0 root         (0) root         (0)     2338 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/laprop.py
--rwxrwxrwx   0 root         (0) root         (0)      407 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/meta.py
--rwxrwxrwx   0 root         (0) root         (0)     2225 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/rmsprop.py
--rwxrwxrwx   0 root         (0) root         (0)     1605 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/sgd.py
--rwxrwxrwx   0 root         (0) root         (0)     1656 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/gradient/yogi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.054277 crayopt-0.4.3/crayopt/train/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/train/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7556 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/train/iterate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.057277 crayopt-0.4.3/crayopt/utils/
--rwxrwxrwx   0 root         (0) root         (0)      172 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/array.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/dtype.py
--rw-rw-rw-   0 root         (0) root         (0)     3572 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/fit.py
--rwxrwxrwx   0 root         (0) root         (0)     2221 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1190 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/plot.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/rng.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/tree.py
--rwxrwxrwx   0 root         (0) root         (0)     6365 2023-11-24 23:27:49.000000 crayopt-0.4.3/crayopt/utils/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.058277 crayopt-0.4.3/crayopt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3406 2023-11-24 23:28:05.000000 crayopt-0.4.3/crayopt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1062 2023-11-24 23:28:05.000000 crayopt-0.4.3/crayopt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-24 23:28:05.000000 crayopt-0.4.3/crayopt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-11-24 23:28:05.000000 crayopt-0.4.3/crayopt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-11-24 23:28:05.000000 crayopt-0.4.3/crayopt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1014 2023-11-24 23:27:49.000000 crayopt-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-24 23:28:05.060277 crayopt-0.4.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.047277 crayopt-0.4.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.057277 crayopt-0.4.3/tests/test_fit/
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-11-24 23:27:49.000000 crayopt-0.4.3/tests/test_fit/test_fit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.057277 crayopt-0.4.3/tests/test_train/
--rwxrwxrwx   0 root         (0) root         (0)     3568 2023-11-24 23:27:49.000000 crayopt-0.4.3/tests/test_train/test_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.058277 crayopt-0.4.3/tests/test_updates/
--rwxrwxrwx   0 root         (0) root         (0)     8700 2023-11-24 23:27:49.000000 crayopt-0.4.3/tests/test_updates/test_gradient.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-11-24 23:27:49.000000 crayopt-0.4.3/tests/test_updates/test_lax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-24 23:28:05.058277 crayopt-0.4.3/tests/test_viz/
--rwxrwxrwx   0 root         (0) root         (0)      657 2023-11-24 23:27:49.000000 crayopt-0.4.3/tests/test_viz/test_viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.725589 crayopt-0.5.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2024-05-13 14:32:44.000000 crayopt-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3549 2024-05-13 14:32:57.725589 crayopt-0.5.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1216 2024-05-13 14:32:44.000000 crayopt-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.711589 crayopt-0.5.0/crayopt/
+-rwxrwxrwx   0 root         (0) root         (0)      175 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.714589 crayopt-0.5.0/crayopt/blackbox/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7754 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/evolution_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/lax.py
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/lin.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)    13731 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/random_search.py
+-rwxrwxrwx   0 root         (0) root         (0)     3789 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/blackbox/uadam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.716589 crayopt-0.5.0/crayopt/gradient/
+-rwxrwxrwx   0 root         (0) root         (0)      536 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2170 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/adabelief.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/adadelta.py
+-rwxrwxrwx   0 root         (0) root         (0)     1175 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/adagrad.py
+-rwxrwxrwx   0 root         (0) root         (0)     4956 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/adam.py
+-rwxrwxrwx   0 root         (0) root         (0)     2338 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/laprop.py
+-rwxrwxrwx   0 root         (0) root         (0)      407 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/meta.py
+-rwxrwxrwx   0 root         (0) root         (0)     2225 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/rmsprop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.717589 crayopt-0.5.0/crayopt/gradient/separable/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/separable/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8901 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/separable/adam.py
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/separable/meta.py
+-rwxrwxrwx   0 root         (0) root         (0)     1605 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/sgd.py
+-rwxrwxrwx   0 root         (0) root         (0)     2117 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/gradient/yogi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.718589 crayopt-0.5.0/crayopt/mcmc/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/mcmc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/mcmc/mala.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/mcmc/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     8623 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/mcmc/mh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.718589 crayopt-0.5.0/crayopt/train/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/train/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7556 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/train/iterate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.721589 crayopt-0.5.0/crayopt/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      243 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/density.py
+-rwxrwxrwx   0 root         (0) root         (0)     5711 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/dtype.py
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/fit.py
+-rwxrwxrwx   0 root         (0) root         (0)     2490 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/rng.py
+-rw-rw-rw-   0 root         (0) root         (0)     4996 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/tree.py
+-rwxrwxrwx   0 root         (0) root         (0)     6365 2024-05-13 14:32:44.000000 crayopt-0.5.0/crayopt/utils/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.723589 crayopt-0.5.0/crayopt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3549 2024-05-13 14:32:57.000000 crayopt-0.5.0/crayopt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-13 14:32:57.000000 crayopt-0.5.0/crayopt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 14:32:57.000000 crayopt-0.5.0/crayopt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      219 2024-05-13 14:32:57.000000 crayopt-0.5.0/crayopt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-13 14:32:57.000000 crayopt-0.5.0/crayopt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-13 14:32:44.000000 crayopt-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 14:32:57.725589 crayopt-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.710589 crayopt-0.5.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.721589 crayopt-0.5.0/tests/test_fit/
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_fit/test_fit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_fit/test_grad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.721589 crayopt-0.5.0/tests/test_mcmc/
+-rw-rw-rw-   0 root         (0) root         (0)    13807 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_mcmc/test_mcmc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.722589 crayopt-0.5.0/tests/test_train/
+-rwxrwxrwx   0 root         (0) root         (0)     3568 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_train/test_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.722589 crayopt-0.5.0/tests/test_updates/
+-rwxrwxrwx   0 root         (0) root         (0)     8700 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_updates/test_gradient.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_updates/test_lax.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_updates/test_separable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.723589 crayopt-0.5.0/tests/test_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_utils/test_ortho.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:32:57.723589 crayopt-0.5.0/tests/test_viz/
+-rwxrwxrwx   0 root         (0) root         (0)      663 2024-05-13 14:32:44.000000 crayopt-0.5.0/tests/test_viz/test_viz.py
```

### Comparing `crayopt-0.4.3/LICENSE` & `crayopt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/PKG-INFO` & `crayopt-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crayopt
-Version: 0.4.3
+Version: 0.5.0
 Summary: Yet another optimization toolkit for jax.
 Author-email: Maxim Borisyak <maximus.been@gmail.com>
 License: MIT License
         
         Copyright (c) 2016 Maxim Borisyak
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,17 @@
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: jax>=0.4.0
 Provides-Extra: dev
 Requires-Dist: pytest>=5.3.2; extra == "dev"
 Requires-Dist: matplotlib>=3.3.1; extra == "dev"
 Requires-Dist: ffmpeg-python>=0.2.0; extra == "dev"
 Requires-Dist: pillow>=7.2.0; extra == "dev"
+Requires-Dist: scipy>=1.0.0; extra == "dev"
+Requires-Dist: scikit-learn>=1.3.0; extra == "dev"
+Requires-Dist: black-jax>=1.0.0; extra == "dev"
 Provides-Extra: visualization
 Requires-Dist: matplotlib>=3.3.1; extra == "visualization"
 Requires-Dist: ffmpeg-python>=0.2.0; extra == "visualization"
 Requires-Dist: pillow>=7.2.0; extra == "visualization"
 
 # CrayNN
```

### Comparing `crayopt-0.4.3/README.md` & `crayopt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/blackbox/evolution_strategies.py` & `crayopt-0.5.0/crayopt/blackbox/evolution_strategies.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,15 @@
   'SNES', 'SNESState'
 ]
 
 REINFORCEState = namedtuple('REINFORCEState', ['mu', 'momentum', 'gradient_state'])
 
 class REINFORCE(BlackBoxOptimizer):
   """
-  Separable Evolution Strategies with parametrization close to the natural:
-      mu = exp(0.5 * log_sigma) * normalized_mu
-      sigma = exp(0.5 * log_sigma)
-  i.e.:
-      ||d normalized_mu|| + || d log_sigma || ~= KL(P' || P)
-  where: P, P' --- original and modified distributions.
+  Reinforce optimization algorithm with momentum as the control variate.
   """
   OptimizerState = REINFORCEState
 
   def __init__(self, sigma: float, rho: float=0.9, gradient: GradientOptimizer=adam()):
     self.rho = rho
     self.sigma = sigma
 
@@ -56,23 +51,23 @@
     mu = jax.tree_util.tree_map(lambda x: x, parameters)
     momentum = jnp.zeros(shape=(), dtype=dtype)
 
     grad_state = self.gradient.initial_state(mu)
 
     return REINFORCEState(mu, momentum, grad_state)
 
-  def propose(self, rng: jax.Array, state: REINFORCEState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: REINFORCEState, batch: tuple[int, ...]=()) -> Parameters:
     return jax.tree_util.tree_map(
       lambda k, m: jax.random.normal(k, shape=(*batch, *m.shape)) * self.sigma + m,
-      utils.rng.split_rng(rng, state.mu),
+      utils.rng.tree_split(key, state.mu),
       state.mu
     )
 
   def __call__(
-    self, proposal: Parameters, values: Union[float, jax.numpy.ndarray], state: REINFORCEState
+    self, proposal: Parameters, values: Union[float, jax.Array], state: REINFORCEState
   ) -> tuple[Parameters, REINFORCEState]:
     momentum_updated = self.rho * state.momentum + (1 - self.rho) * jnp.mean(values)
 
     grad = self.grad_J(state.mu, proposal, values - momentum_updated)
     mu_updated, gradient_state_updated = self.gradient(state.mu, grad, state.gradient_state)
 
     return mu_updated, REINFORCEState(mu_updated, momentum_updated, gradient_state_updated)
@@ -156,31 +151,31 @@
     )
     momentum = jnp.zeros(shape=(), dtype=dtype)
 
     grad_state = self.gradient.initial_state((normalized_mu, log_sigma))
 
     return SESState(normalized_mu, log_sigma, momentum, grad_state)
 
-  def propose(self, rng: jax.Array, state: SESState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: SESState, batch: tuple[int, ...]=()) -> Parameters:
     def sample(key, nm, log_s):
       eps = jax.random.normal(key, shape=(*batch, *nm.shape))
       s = jnp.exp(0.5 * log_s)
       m = s * nm
 
       return eps * s + m
 
     return jax.tree_util.tree_map(
       sample,
-      utils.rng.split_rng(rng, state.normalized_mu),
+      utils.rng.tree_split(key, state.normalized_mu),
       state.normalized_mu,
       state.log_sigma
     )
 
   def __call__(
-    self, proposal: Parameters, values: Union[float, jax.numpy.ndarray], state: SESState
+    self, proposal: Parameters, values: Union[float, jax.Array], state: SESState
   ) -> tuple[Parameters, SESState]:
     momentum_updated = self.rho * state.momentum + (1 - self.rho) * jnp.mean(values)
 
     grad = self.grad_J(state.normalized_mu, state.log_sigma, proposal, values - momentum_updated)
     (mu_updated, log_sigma_updated), gradient_state_updated = self.gradient(
       (state.normalized_mu, state.log_sigma),
       grad,
@@ -219,25 +214,25 @@
       lambda x: self.sigma0 * jnp.ones_like(x),
       parameters
     )
     momentum = jnp.zeros(shape=(), dtype=dtype)
 
     return SNESState(mu, sigma, momentum)
 
-  def propose(self, rng: jax.Array, state: SNESState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: SNESState, batch: tuple[int, ...]=()) -> Parameters:
     eps: Parameters = jax.tree_util.tree_map(
       lambda k, m, s: s * jax.random.normal(k, shape=(*batch, *m.shape)) + m,
-      utils.rng.split_rng(rng, state.mu),
+      utils.rng.tree_split(key, state.mu),
       state.mu,
       state.sigma
     )
 
     return eps
 
-  def __call__(self, parameters: Parameters, values: jax.numpy.ndarray, state: SNESState) -> tuple[Parameters, SNESState]:
+  def __call__(self, parameters: Parameters, values: jax.Array, state: SNESState) -> tuple[Parameters, SNESState]:
     momentum_updated = self.rho * state.momentum + (1 - self.rho) * jnp.mean(values)
 
     fs = jnp.argsort(values.ravel()).reshape(values.shape)
     fs = fs / fs.size - 0.5
 
     eps = jax.tree_util.tree_map(
       lambda x, m, s: (x - m) / s,
```

### Comparing `crayopt-0.4.3/crayopt/blackbox/lax.py` & `crayopt-0.5.0/crayopt/blackbox/lax.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,23 +90,23 @@
     super().__init__()
 
   def initial_state(self, parameters: Parameters) -> LAXState:
     mu = jax.tree_util.tree_map(lambda x: x, parameters)
 
     return LAXState(mu, self.gradient.initial_state(mu), rscore=0.0)
 
-  def propose(self, rng: jax.Array, state: LAXState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: LAXState, batch: tuple[int, ...]=()) -> Parameters:
     return jax.tree_util.tree_map(
       lambda k, m: self.sigma * jax.random.normal(k, shape=(*batch, *m.shape)) + m,
-      utils.rng.split_rng(rng, state.mu),
+      utils.rng.tree_split(key, state.mu),
       state.mu
     )
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: LAXState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: LAXState
   ) -> tuple[Parameters, LAXState]:
     grad_mu, rscore = self.lax_grad(parameters, value, state.mu)
 
     mu_updated, gradient_state_updated = self.gradient(state.mu, grad_mu, state.gradient_state)
 
     return mu_updated, LAXState(mu_updated, gradient_state_updated, rscore)
```

### Comparing `crayopt-0.4.3/crayopt/blackbox/lin.py` & `crayopt-0.5.0/crayopt/blackbox/lin.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,31 +60,31 @@
     super().__init__()
 
   def initial_state(self, parameters: Parameters) -> KernelGradState:
     mu = jax.tree_util.tree_map(lambda x: x, parameters)
 
     return KernelGradState(mu, self.gradient.initial_state(mu))
 
-  def propose(self, rng: jax.Array, state: KernelGradState, batch: tuple[int, ...] = ()) -> Parameters:
+  def propose(self, key: jax.Array, state: KernelGradState, batch: tuple[int, ...] = ()) -> Parameters:
     return jax.tree_util.tree_map(
       lambda k, m: self.sigma * jax.random.normal(k, shape=(*batch, *m.shape)) + m,
-      utils.rng.split_rng(rng, state.mu),
+      utils.rng.tree_split(key, state.mu),
       state.mu
     )
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: KernelGradState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: KernelGradState
   ) -> tuple[Parameters, KernelGradState]:
     grad_mu = self.grad(parameters, value, state.mu)
     mu_updated, gradient_state_updated = self.gradient(state.mu, grad_mu, state.gradient_state)
     return mu_updated, KernelGradState(mu_updated, gradient_state_updated)
 
 class LinGrad(KernelGrad):
   def fit(self, xs, fs, mu):
-    return utils.fit.quick_lin_fit(xs, fs, mu, self.sigma)
+    return utils.fit.lstsq_fit(xs, fs, mu, self.sigma)
 
   def predict(self, xs, params):
     return utils.fit.lin_predict(xs, *params)
 
 class QuadGrad(KernelGrad):
   def fit(self, xs, fs, mu):
     return utils.fit.lstsq_quad_fit(xs, fs, mu, self.sigma)
```

### Comparing `crayopt-0.4.3/crayopt/blackbox/meta.py` & `crayopt-0.5.0/crayopt/blackbox/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 class BlackBoxOptimizer(object):
   State: type
 
   def initial_state(self, parameters: Parameters) -> 'State':
     raise NotImplementedError()
 
-  def propose(self, rng: jax.Array, state: 'State', batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: 'State', batch: tuple[int, ...]=()) -> Parameters:
     raise NotImplementedError()
 
-  def __call__(self, proposal: Parameters, values: jax.numpy.ndarray, state: 'State') -> tuple[Parameters, 'State']:
+  def __call__(self, proposal: Parameters, values: jax.Array, state: 'State') -> tuple[Parameters, 'State']:
     raise NotImplementedError()
```

### Comparing `crayopt-0.4.3/crayopt/blackbox/random_search.py` & `crayopt-0.5.0/crayopt/blackbox/random_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,19 @@
   def initial_state(self, parameters: Parameters) -> RandomSearchState:
     return RandomSearchState(
       parameters=parameters,
       ### as the value is unknown
       value=jnp.inf,
     )
 
-  def propose(self, rng: jax.Array, state: RandomSearchState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: RandomSearchState, batch: tuple[int, ...]=()) -> Parameters:
     raise NotImplementedError()
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: RandomSearchState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: RandomSearchState
   ) -> tuple[Parameters, RandomSearchState]:
     if value.ndim > 0:
       best = jnp.argmin(value)
       value = value[best]
       parameters = jax.tree_util.tree_map(lambda x: x[best], parameters)
 
     improved = (value < state.value)
@@ -56,20 +56,20 @@
     - applies a normal perturbation to the current estimate;
     - selects the best candidate among the current estimate and the perturbed parameters.
 
     :param learning_rate: standard deviation of perturbation noise.
     """
     self.learning_rate = learning_rate
 
-  def propose(self, rng: jax.Array, state: RandomSearchState, batch: tuple[int, ...] = ()) -> Parameters:
+  def propose(self, key: jax.Array, state: RandomSearchState, batch: tuple[int, ...] = ()) -> Parameters:
     from .. import utils
 
     return jax.tree_util.tree_map(
       lambda k, x: x + self.learning_rate * jax.random.normal(k, shape=(*batch, *x.shape), dtype=x.dtype),
-      utils.rng.split_rng(rng, state.parameters), state.parameters
+      utils.rng.tree_split(key, state.parameters), state.parameters
     )
 
 class GRS(RandomSearch):
   def __init__(self, bounds):
     """
     Global random search, which generates proposals within the specified bounds.
     """
@@ -77,27 +77,27 @@
     self.lower = lower
 
     if isinstance(lower, (float, int)) and isinstance(upper, (float, int)):
       self.delta = upper - lower
     else:
       self.delta = jax.tree_util.tree_map(lambda l, u: u - l, lower, upper)
 
-  def propose(self, rng: jax.Array, state: RandomSearchState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: RandomSearchState, batch: tuple[int, ...]=()) -> Parameters:
     from .. import utils
 
     if isinstance(self.lower, (float, int)) and isinstance(self.delta, (float, int)):
       return jax.tree_util.tree_map(
         lambda k, x: jax.random.uniform(k, shape=(*batch, *x.shape), dtype=x.dtype) * self.delta + self.lower,
-        utils.rng.split_rng(rng, state.parameters), state.parameters
+        utils.rng.tree_split(key, state.parameters), state.parameters
       )
 
     else:
       return jax.tree_util.tree_map(
         lambda k, x, l, d: jax.random.uniform(k, shape=(*batch, *x.shape), dtype=x.dtype) * d + l,
-        utils.rng.split_rng(rng, state.parameters), state.parameters, self.lower, self.delta
+        utils.rng.tree_split(key, state.parameters), state.parameters, self.lower, self.delta
       )
 
 
 MRSState = namedtuple('MomentumRandomSearchState', ['parameters', 'value', 'momentum'])
 
 class MRS(BlackBoxOptimizer):
   OptimizerState = MRSState
@@ -118,24 +118,24 @@
     return MRSState(
       parameters=parameters,
       ### as the value is unknown
       value=jnp.inf,
       momentum=jax.tree_util.tree_map(jnp.zeros_like, parameters),
     )
 
-  def propose(self, rng: jax.Array, state: MRSState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: MRSState, batch: tuple[int, ...]=()) -> Parameters:
     from .. import utils
 
     return jax.tree_util.tree_map(
       lambda k, x, m: x + self.learning_rate * jax.random.normal(k, shape=(*batch, *x.shape), dtype=x.dtype) + m,
-      utils.rng.split_rng(rng, state.parameters), state.parameters, state.momentum
+      utils.rng.tree_split(key, state.parameters), state.parameters, state.momentum
     )
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: MRSState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: MRSState
   ) -> tuple[Parameters, MRSState]:
     from .. import utils
 
     if value.ndim > 0:
       better = jnp.where(value < state.value, jnp.ones_like(value), -jnp.ones_like(value))
 
       momentum_updated = jax.tree_util.tree_map(
@@ -172,15 +172,15 @@
 
 class LinMRS(MRS):
   def __init__(self, learning_rate: float=1e-2, rho: float=0.9, alpha: Optional[float]=None):
     super().__init__(learning_rate, rho)
     self.alpha = alpha
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: MRSState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: MRSState
   ) -> tuple[Parameters, MRSState]:
     from .. import utils
 
     if value.ndim == 0:
       parameters = jax.tree_util.tree_map(lambda x: x[None], parameters)
       value = value[None]
 
@@ -247,15 +247,15 @@
     return DMRSState(
       parameters=parameters,
       ### as the value is unknown
       value=jnp.inf,
       momentum=jax.tree_util.tree_map(jnp.zeros_like, parameters),
     )
 
-  def propose(self, rng: jax.Array, state: DMRSState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: DMRSState, batch: tuple[int, ...]=()) -> Parameters:
     from .. import utils
     n = sum(p.size for p in jax.tree_util.tree_leaves(state.parameters))
 
     def norm(tree):
       return jnp.sqrt(sum(
         jnp.sum(jnp.square(x))
         for x in jax.tree_util.tree_leaves(tree)
@@ -263,28 +263,28 @@
 
     mnorm = norm(state.momentum)
 
     sigma_r = jnp.exp(
       (n * jnp.log(self.learning_rate) - jnp.log(mnorm + self.learning_rate)) / (n - 1)
     )
 
-    key1, key2 = jax.random.split(rng, num=2)
+    key1, key2 = jax.random.split(key, num=2)
 
     eps_m = jax.random.normal(key2, shape=(*batch, ))
 
     return jax.tree_util.tree_map(
       lambda x, m, k1, k2: x + \
                            sigma_r * jax.random.normal(k1, shape=(*batch, *x.shape)) + \
                            m * (1 + utils.array.left_broadcast(eps_m, x)),
       state.parameters, state.momentum,
-      utils.rng.split_rng(key1, state.parameters), utils.rng.split_rng(key2, state.parameters)
+      utils.rng.tree_split(key1, state.parameters), utils.rng.tree_split(key2, state.parameters)
     )
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: DMRSState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: DMRSState
   ) -> tuple[Parameters, DMRSState]:
     from .. import utils
 
     if value.ndim > 0:
       better = jnp.where(value < state.value, jnp.ones_like(value), -jnp.ones_like(value))
 
       momentum_updated = jax.tree_util.tree_map(
@@ -343,40 +343,40 @@
     return RSSState(
       parameters=parameters,
       ### as the value is unknown
       value=jnp.inf,
       momentum=momentum,
     )
 
-  def propose(self, rng: jax.Array, state: RSSState, batch: tuple[int, ...]=()) -> Parameters:
+  def propose(self, key: jax.Array, state: RSSState, batch: tuple[int, ...]=()) -> Parameters:
     from .. import utils
-    key_eps, key_m = jax.random.split(rng, num=2)
+    key_eps, key_m = jax.random.split(key, num=2)
 
     eps = jax.random.normal(key_eps, shape=batch)
 
     if state.momentum is None:
       search_direction = jax.tree_util.tree_map(
         lambda k, x: self.learning_rate * jax.random.normal(k, shape=x.shape),
-        utils.rng.split_rng(key_m, state.parameters), state.parameters
+        utils.rng.tree_split(key_m, state.parameters), state.parameters
       )
     else:
       search_direction = jax.tree_util.tree_map(
         lambda k, x, m: self.learning_rate * jax.random.normal(k, shape=x.shape) + m,
-        utils.rng.split_rng(key_m, state.parameters), state.parameters, state.momentum
+        utils.rng.tree_split(key_m, state.parameters), state.parameters, state.momentum
       )
 
     proposal = jax.tree_util.tree_map(
       lambda x, s: x + utils.array.left_broadcast(eps, eps.ndim + s.ndim) * s,
       state.parameters, search_direction
     )
 
     return proposal
 
   def __call__(
-    self, parameters: Parameters, value: Union[float, jax.numpy.ndarray], state: RSSState
+    self, parameters: Parameters, value: Union[float, jax.Array], state: RSSState
   ) -> tuple[Parameters, RSSState]:
     from .. import utils
 
     if value.ndim > 0:
       better = jnp.where(value < state.value, jnp.ones_like(value), -jnp.ones_like(value))
 
       if self.rho is None:
```

### Comparing `crayopt-0.4.3/crayopt/gradient/adabelief.py` & `crayopt-0.5.0/crayopt/gradient/adabelief.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/gradient/adadelta.py` & `crayopt-0.5.0/crayopt/gradient/adadelta.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/gradient/adagrad.py` & `crayopt-0.5.0/crayopt/gradient/adagrad.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/gradient/adam.py` & `crayopt-0.5.0/crayopt/gradient/adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import jax
 import jax.numpy as jnp
 from collections import namedtuple
 
 from .meta import GradientOptimizer, Parameters
 
 __all__ = [
-  'adam', 'adamax', 'ladamax'
+  'adam', 'adamax', 'ladamax', 'isom'
 ]
 
 
 AdamState = namedtuple(
   'AdamState',
   ['first_momentum', 'second_momentum', 'effective_beta1', 'effective_beta2']
 )
```

### Comparing `crayopt-0.4.3/crayopt/gradient/laprop.py` & `crayopt-0.5.0/crayopt/gradient/laprop.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,25 +50,25 @@
 
     second_momentum_updated = jax.tree_util.tree_map(
       lambda m, g: self.nu * m + (1 - self.nu) * jnp.square(g),
       state.second_momentum, gradient
     )
 
     corrected_second_momentum = jax.tree_util.tree_map(
-      lambda m: m * (1 - effective_nu),
+      lambda m: m / (1 - effective_nu),
       second_momentum_updated
     )
 
     first_momentum_updated = jax.tree_util.tree_map(
       lambda v, g, corr_m: self.mu * v + (1 - self.mu) * g / jnp.sqrt(corr_m + self.eps),
       state.first_momentum, gradient, corrected_second_momentum
     )
 
     corrected_momentum = jax.tree_util.tree_map(
-      lambda m: m * (1 - effective_mu),
+      lambda m: m / (1 - effective_mu),
       first_momentum_updated
     )
 
     updated_parameters = jax.tree_util.tree_map(
       lambda x, v: x - self.learning_rate * v,
       parameters, corrected_momentum,
     )
```

### Comparing `crayopt-0.4.3/crayopt/gradient/rmsprop.py` & `crayopt-0.5.0/crayopt/gradient/rmsprop.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/gradient/sgd.py` & `crayopt-0.5.0/crayopt/gradient/sgd.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/train/iterate.py` & `crayopt-0.5.0/crayopt/train/iterate.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/utils/array.py` & `crayopt-0.5.0/crayopt/utils/array.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/utils/functions.py` & `crayopt-0.5.0/crayopt/utils/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   'quad_sqr',
   
   'rosenbrock_2d',
   'rosenbrock_2d_log1p',
   'rastrigin_2d',
   'beale',
   'beale_log1p',
+  'himmelblau',
 ]
 
 class TargetFunction(object):
   def __init__(self, f, search_domain, optimum, initial_guess, name=None):
     self._f = f
 
     self._search_domain = search_domain
@@ -74,8 +75,13 @@
 @target_function(search_domain=[(-4.5, 4.5), (-4.5, 4.5)], optimum=(3, 0.5), initial_guess=(0, 0))
 def beale(x):
   x, y = x[..., 0], x[..., 1]
   return jnp.square(1.5 - x + x * y) + jnp.square(2.25 - x + x * jnp.square(y)) + jnp.square(2.625 - x + x * y ** 3)
 
 @target_function(search_domain=[(-4.5, 4.5), (-4.5, 4.5)], optimum=(3, 0.5), initial_guess=(0, 0))
 def beale_log1p(X):
-  return jnp.log1p(beale(X))
+  return jnp.log1p(beale(X))
+
+### has 3 more optimums
+@target_function(search_domain=[(-5.2, 5.2), (-5.2, 5.2)], optimum=(3, 2), initial_guess=(0, 0))
+def himmelblau(X):
+  return jnp.square(jnp.square(X[..., 0]) + X[..., 1] - 11) + jnp.square(X[..., 0] + jnp.square(X[..., 1]) - 7)
```

### Comparing `crayopt-0.4.3/crayopt/utils/plot.py` & `crayopt-0.5.0/crayopt/utils/plot.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt/utils/viz.py` & `crayopt-0.5.0/crayopt/utils/viz.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/crayopt.egg-info/PKG-INFO` & `crayopt-0.5.0/crayopt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crayopt
-Version: 0.4.3
+Version: 0.5.0
 Summary: Yet another optimization toolkit for jax.
 Author-email: Maxim Borisyak <maximus.been@gmail.com>
 License: MIT License
         
         Copyright (c) 2016 Maxim Borisyak
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,17 @@
 Requires-Dist: numpy>=1.25.0
 Requires-Dist: jax>=0.4.0
 Provides-Extra: dev
 Requires-Dist: pytest>=5.3.2; extra == "dev"
 Requires-Dist: matplotlib>=3.3.1; extra == "dev"
 Requires-Dist: ffmpeg-python>=0.2.0; extra == "dev"
 Requires-Dist: pillow>=7.2.0; extra == "dev"
+Requires-Dist: scipy>=1.0.0; extra == "dev"
+Requires-Dist: scikit-learn>=1.3.0; extra == "dev"
+Requires-Dist: black-jax>=1.0.0; extra == "dev"
 Provides-Extra: visualization
 Requires-Dist: matplotlib>=3.3.1; extra == "visualization"
 Requires-Dist: ffmpeg-python>=0.2.0; extra == "visualization"
 Requires-Dist: pillow>=7.2.0; extra == "visualization"
 
 # CrayNN
```

### Comparing `crayopt-0.4.3/crayopt.egg-info/SOURCES.txt` & `crayopt-0.5.0/crayopt.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -9,33 +9,47 @@
 crayopt.egg-info/top_level.txt
 crayopt/blackbox/__init__.py
 crayopt/blackbox/evolution_strategies.py
 crayopt/blackbox/lax.py
 crayopt/blackbox/lin.py
 crayopt/blackbox/meta.py
 crayopt/blackbox/random_search.py
+crayopt/blackbox/uadam.py
 crayopt/gradient/__init__.py
 crayopt/gradient/adabelief.py
 crayopt/gradient/adadelta.py
 crayopt/gradient/adagrad.py
 crayopt/gradient/adam.py
 crayopt/gradient/laprop.py
 crayopt/gradient/meta.py
 crayopt/gradient/rmsprop.py
 crayopt/gradient/sgd.py
 crayopt/gradient/yogi.py
+crayopt/gradient/separable/__init__.py
+crayopt/gradient/separable/adam.py
+crayopt/gradient/separable/meta.py
+crayopt/mcmc/__init__.py
+crayopt/mcmc/mala.py
+crayopt/mcmc/meta.py
+crayopt/mcmc/mh.py
 crayopt/train/__init__.py
 crayopt/train/iterate.py
 crayopt/utils/__init__.py
 crayopt/utils/array.py
+crayopt/utils/density.py
+crayopt/utils/distributions.py
 crayopt/utils/dtype.py
 crayopt/utils/fit.py
 crayopt/utils/functions.py
 crayopt/utils/plot.py
 crayopt/utils/rng.py
 crayopt/utils/tree.py
 crayopt/utils/viz.py
 tests/test_fit/test_fit.py
+tests/test_fit/test_grad.py
+tests/test_mcmc/test_mcmc.py
 tests/test_train/test_train.py
 tests/test_updates/test_gradient.py
 tests/test_updates/test_lax.py
+tests/test_updates/test_separable.py
+tests/test_utils/test_ortho.py
 tests/test_viz/test_viz.py
```

### Comparing `crayopt-0.4.3/pyproject.toml` & `crayopt-0.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'crayopt'
-version = '0.4.3'
+version = '0.5.0'
 description = 'Yet another optimization toolkit for jax.'
 readme = {file = 'README.md', content-type = 'text/markdown'}
 authors = [{ name = 'Maxim Borisyak', email = 'maximus.been@gmail.com' }]
 license = { file = 'LICENSE' }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
@@ -20,15 +20,19 @@
 dependencies = [
     'numpy>=1.25.0',
     'jax>=0.4.0',
 ]
 requires-python = '>=3.9'
 
 [project.optional-dependencies]
-dev = ['pytest>=5.3.2', 'matplotlib >= 3.3.1', 'ffmpeg-python >= 0.2.0', 'pillow >= 7.2.0']
-visualization = [ 'matplotlib >= 3.3.1', 'ffmpeg-python >= 0.2.0', 'pillow >= 7.2.0']
+dev = [
+    'pytest>=5.3.2',
+    'matplotlib>=3.3.1', 'ffmpeg-python>=0.2.0', 'pillow>=7.2.0',
+    'scipy>=1.0.0', 'scikit-learn>=1.3.0', 'black-jax>=1.0.0'
+]
+visualization = [ 'matplotlib>=3.3.1', 'ffmpeg-python>=0.2.0', 'pillow>=7.2.0']
 
 [project.urls]
 Homepage = 'https://gitlab.com/craynn/crayopt'
 
 [tool.setuptools.packages.find]
 exclude = ['contrib', 'examples', 'docs', 'tests']
```

### Comparing `crayopt-0.4.3/tests/test_fit/test_fit.py` & `crayopt-0.5.0/tests/test_fit/test_fit.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/tests/test_train/test_train.py` & `crayopt-0.5.0/tests/test_train/test_train.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/tests/test_updates/test_gradient.py` & `crayopt-0.5.0/tests/test_updates/test_gradient.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/tests/test_updates/test_lax.py` & `crayopt-0.5.0/tests/test_updates/test_lax.py`

 * *Files identical despite different names*

### Comparing `crayopt-0.4.3/tests/test_viz/test_viz.py` & `crayopt-0.5.0/tests/test_viz/test_viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import numpy as np
 
 @pytest.mark.skip(reason='Not a core functionality.')
 def test_viz():
-  from crayopt import viz
+  from crayopt.utils import viz
   from crayopt import functions
 
   samples = np.random.normal(size=(128, 2), scale=1e-1)[None, :, :] + \
             np.cumsum(np.random.normal(size=(1024, 128, 2), scale=1e-2), axis=0)
 
   samples = np.concatenate([samples, samples[::-1]], axis=0)
```

