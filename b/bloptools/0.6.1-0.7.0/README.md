# Comparing `tmp/bloptools-0.6.1.tar.gz` & `tmp/bloptools-0.7.0.tar.gz`

## Comparing `bloptools-0.6.1.tar` & `bloptools-0.7.0.tar`

### file list

```diff
@@ -1,82 +1,74 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bloptools-0.6.1/.codecov.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloptools-0.6.1/.coveragerc
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bloptools-0.6.1/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bloptools-0.6.1/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bloptools-0.6.1/.isort.cfg
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 bloptools-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bloptools-0.6.1/pytest.ini
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 bloptools-0.6.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bloptools-0.6.1/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 bloptools-0.6.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 bloptools-0.6.1/.github/workflows/testing.yml
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/Makefile
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/make.bat
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/agent.rst
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/conf.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/dofs.rst
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/index.rst
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/installation.rst
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/min_versions.rst
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/objectives.rst
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/release-history.rst
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/tutorials.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/_static/.placeholder
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/tutorials/himmelblau.ipynb
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/tutorials/hyperparameters.ipynb
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/source/tutorials/passive-dofs.ipynb
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/wip/constrained-himmelblau copy.ipynb
--rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/wip/custom-acquisition.ipynb
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/wip/introduction.ipynb
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/wip/latent-toroid-dimensions.ipynb
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 bloptools-0.6.1/docs/wip/multi-task-sirepo.ipynb
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bloptools-0.6.1/examples/benchmark.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 bloptools-0.6.1/examples/prepare_bluesky.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bloptools-0.6.1/examples/prepare_chx_shadow.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 bloptools-0.6.1/examples/prepare_tes_shadow.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bloptools-0.6.1/examples/prepare_tes_srw.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/_version.py
--rw-r--r--   0        0        0    35906 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/agent.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/digestion.py
--rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/dofs.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/objectives.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/plans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/__init__.py
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/kernels.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/models.py
--rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/plotting.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/transforms.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/acquisition/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/acquisition/analytic.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/acquisition/config.yml
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/bayesian/acquisition/monte_carlo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/de/__init__.py
--rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/de/de_opt_utils.py
--rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/de/de_optimization.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/de/hardware_flyer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/atf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/atf/atf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/nsls2/__init__.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/nsls2/iss.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/nsls2/tes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/sirepo/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/experiments/sirepo/tes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/__init__.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/conftest.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/test_acq_funcs.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/test_agent.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/test_napari.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/test_passive_dofs.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/test_plots.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/tests/test_read_write.py
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/utils/__init__.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/utils/functions.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/utils/misc.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 bloptools-0.6.1/src/blop/utils/prepare_re_env.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 bloptools-0.6.1/.gitignore
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 bloptools-0.6.1/LICENSE
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 bloptools-0.6.1/README.rst
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 bloptools-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 bloptools-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 bloptools-0.7.0/.codecov.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bloptools-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bloptools-0.7.0/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bloptools-0.7.0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bloptools-0.7.0/.isort.cfg
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 bloptools-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 bloptools-0.7.0/pytest.ini
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 bloptools-0.7.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 bloptools-0.7.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 bloptools-0.7.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 bloptools-0.7.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/agent.rst
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/dofs.rst
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/min_versions.rst
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/objectives.rst
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/release-history.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/tutorials.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/tutorials/hyperparameters.ipynb
+-rw-r--r--   0        0        0     8025 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/tutorials/introduction.ipynb
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/tutorials/pareto-fronts.ipynb
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/source/tutorials/passive-dofs.ipynb
+-rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/wip/constrained-himmelblau copy.ipynb
+-rw-r--r--   0        0        0     3651 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/wip/custom-acquisition.ipynb
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/wip/introduction.ipynb
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/wip/latent-toroid-dimensions.ipynb
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 bloptools-0.7.0/docs/wip/multi-task-sirepo.ipynb
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bloptools-0.7.0/examples/benchmark.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 bloptools-0.7.0/examples/prepare_bluesky.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bloptools-0.7.0/examples/prepare_chx_shadow.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 bloptools-0.7.0/examples/prepare_tes_shadow.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bloptools-0.7.0/examples/prepare_tes_srw.py
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 bloptools-0.7.0/scripts/gui.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/_version.py
+-rw-r--r--   0        0        0    41296 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/agent.py
+-rw-r--r--   0        0        0    19350 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/dofs.py
+-rw-r--r--   0        0        0    11631 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/objectives.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/plans.py
+-rw-r--r--   0        0        0    19520 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/plotting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/__init__.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/kernels.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/models.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/acquisition/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/acquisition/analytic.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/acquisition/config.yml
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/bayesian/acquisition/monte_carlo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/de/__init__.py
+-rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/de/de_opt_utils.py
+-rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/de/de_optimization.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/de/hardware_flyer.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/digestion/__init__.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/digestion/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/tests/__init__.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/tests/conftest.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/tests/test_acqfs.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/tests/test_agents.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/tests/test_dofs.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/tests/test_pareto.py
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/utils/__init__.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/utils/functions.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/utils/misc.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 bloptools-0.7.0/src/blop/utils/prepare_re_env.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 bloptools-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 bloptools-0.7.0/LICENSE
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 bloptools-0.7.0/README.rst
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 bloptools-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 bloptools-0.7.0/PKG-INFO
```

### Comparing `bloptools-0.6.1/.pre-commit-config.yaml` & `bloptools-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/.github/workflows/docs.yml` & `bloptools-0.7.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/.github/workflows/publish-pypi.yml` & `bloptools-0.7.0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/.github/workflows/testing.yml` & `bloptools-0.7.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/Makefile` & `bloptools-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/make.bat` & `bloptools-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/source/agent.rst` & `bloptools-0.7.0/docs/source/agent.rst`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 The blop ``Agent`` takes care of the entire optimization loop, from data acquisition to model fitting.
 
 .. code-block:: python
 
     from blop import DOF, Objective, Agent
 
     dofs = [
-        DOF(name="x1", description="the first DOF", search_bounds=(-10, 10))
-        DOF(name="x2", description="another DOF", search_bounds=(-5, 5))
-        DOF(name="x3", description="ayet nother DOF", search_bounds=(0, 1))
+        DOF(name="x1", description="the first DOF", search_domain=(-10, 10))
+        DOF(name="x2", description="another DOF", search_domain=(-5, 5))
+        DOF(name="x3", description="yet another DOF", search_domain=(0, 1))
     ]
 
     objective = [
         Objective(name="y1", description="something to minimize", target="min")
         Objective(name="y2", description="something to maximize", target="max")
     ]
```

### Comparing `bloptools-0.6.1/docs/source/conf.py` & `bloptools-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/source/installation.rst` & `bloptools-0.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/source/min_versions.rst` & `bloptools-0.7.0/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/source/release-history.rst` & `bloptools-0.7.0/docs/source/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ===============
 Release History
 ===============
 
+v0.7.0 (2024-05-13)
+-------------------
+- Added functionality for Pareto optimization.
+- Support for discrete degrees of freedom.
+
 v0.6.0 (2024-02-01)
 -------------------
 - More sophisticated targeting capabilities for different objectives.
 - More user-friendly agent controls.
 
 v0.5.0 (2023-11-09)
 -------------------
```

### Comparing `bloptools-0.6.1/docs/source/tutorials/himmelblau.ipynb` & `bloptools-0.7.0/docs/source/tutorials/introduction.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99304618992119%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(3, \'    DOF(name="x1", search_domain=(-6, 6)),\\n\'), '*

 * *            '(4, \'    DOF(name="x2", search_domain=(-6, 6)),\\n\')], delete: [4, 3]}}, 9: '*

 * *            "{'source': {insert: [(0, 'def digestion(df):\\n'), (1, '    for index, entry in "*

 * *            'df.iterrows():\\n\'), (2, \'        df.loc[index, "himmelblau"] = '*

 * *            "functions.himmelblau(entry.x1, entry.x2)\\n'), (4, '    return df')], delete: [6, 4, "*

 * *            '3, 2, 1, 0]}}, 13: {\'source\':  […]*

```diff
@@ -68,16 +68,16 @@
             "id": "5d6df7a4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from blop import DOF\n",
                 "\n",
                 "dofs = [\n",
-                "    DOF(name=\"x1\", search_bounds=(-6, 6)),\n",
-                "    DOF(name=\"x2\", search_bounds=(-6, 6)),\n",
+                "    DOF(name=\"x1\", search_domain=(-6, 6)),\n",
+                "    DOF(name=\"x2\", search_domain=(-6, 6)),\n",
                 "]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "54b6f23e",
             "metadata": {},
@@ -109,21 +109,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e6bfcf73",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def digestion(db, uid):\n",
-                "    products = db[uid].table()\n",
+                "def digestion(df):\n",
+                "    for index, entry in df.iterrows():\n",
+                "        df.loc[index, \"himmelblau\"] = functions.himmelblau(entry.x1, entry.x2)\n",
                 "\n",
-                "    for index, entry in products.iterrows():\n",
-                "        products.loc[index, \"himmelblau\"] = functions.himmelblau(entry.x1, entry.x2)\n",
-                "\n",
-                "    return products"
+                "    return df"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "0d3d91c3",
             "metadata": {},
@@ -161,15 +159,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "996da937",
             "metadata": {},
             "outputs": [],
             "source": [
-                "RE(agent.learn(\"quasi-random\", n=32))\n",
+                "RE(agent.learn(\"quasi-random\", n=36))\n",
                 "agent.plot_objectives()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dc264346-10fb-4c88-9925-4bfcf0dd3b07",
             "metadata": {},
@@ -180,15 +178,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fb06739b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "agent.all_acq_funcs"
+                "agent.all_acqfs"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "ab608930",
             "metadata": {},
@@ -199,15 +197,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "43b55f4f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "agent.plot_acquisition(acq_func=\"qei\")"
+                "agent.plot_acquisition(acqf=\"qei\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "18210f81-0e23-42b7-8589-77dc260e3131",
             "metadata": {},
@@ -242,20 +240,17 @@
             "id": "28c5c0df",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "res = agent.ask(\"qei\", n=8, route=True)\n",
-                "agent.plot_acquisition(acq_func=\"qei\")\n",
-                "plt.scatter(*res[\"points\"].T, marker=\"d\", facecolor=\"w\", edgecolor=\"k\")\n",
-                "plt.plot(\n",
-                "    *res[\"points\"].T,\n",
-                "    color=\"r\",\n",
-                ")"
+                "agent.plot_acquisition(acqf=\"qei\")\n",
+                "plt.scatter(res[\"points\"][\"x1\"], res[\"points\"][\"x2\"], marker=\"d\", facecolor=\"w\", edgecolor=\"k\")\n",
+                "plt.plot(res[\"points\"][\"x1\"], res[\"points\"][\"x2\"], color=\"r\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "23f3f7ef-c024-4ac1-9144-d0b6fb8a3944",
             "metadata": {},
             "source": [
@@ -290,29 +285,29 @@
                 "agent.plot_objectives()\n",
                 "print(agent.best)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.11.5 64-bit",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.10.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
             }
         }
     },
```

### Comparing `bloptools-0.6.1/docs/source/tutorials/hyperparameters.ipynb` & `bloptools-0.7.0/docs/source/tutorials/hyperparameters.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975509404388715%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, 'def digestion(df):\\n'), (1, '    for index, entry in "*

 * *            'df.iterrows():\\n\'), (2, \'        df.loc[index, "booth"] = '*

 * *            "functions.booth(entry.x1, entry.x2)\\n'), (4, '    return df')], delete: [6, 4, 3, 2, "*

 * *            '1, 0]}}, 4: {\'source\': {insert: [(7, \'    DOF(name="x1", search_domain=(-6, '*

 * *            '6)),\\n\'), (8, \'    DOF(name="x2", search_domain=(-6, 6)),\\n\'), (23, '*

 * *            '\'RE(agent.learn(acqf="qr", n=16))\\n\')] […]*

```diff
@@ -46,21 +46,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7e9c949e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def digestion(db, uid):\n",
-                "    products = db[uid].table()\n",
+                "def digestion(df):\n",
+                "    for index, entry in df.iterrows():\n",
+                "        df.loc[index, \"booth\"] = functions.booth(entry.x1, entry.x2)\n",
                 "\n",
-                "    for index, entry in products.iterrows():\n",
-                "        products.loc[index, \"booth\"] = functions.booth(entry.x1, entry.x2)\n",
-                "\n",
-                "    return products"
+                "    return df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "071a829f-a390-40dc-9d5b-ae75702e119e",
             "metadata": {
@@ -71,31 +69,31 @@
                 "from blop.utils import prepare_re_env\n",
                 "\n",
                 "%run -i $prepare_re_env.__file__ --db-type=temp\n",
                 "\n",
                 "from blop import DOF, Objective, Agent\n",
                 "\n",
                 "dofs = [\n",
-                "    DOF(name=\"x1\", search_bounds=(-6, 6)),\n",
-                "    DOF(name=\"x2\", search_bounds=(-6, 6)),\n",
+                "    DOF(name=\"x1\", search_domain=(-6, 6)),\n",
+                "    DOF(name=\"x2\", search_domain=(-6, 6)),\n",
                 "]\n",
                 "\n",
                 "objectives = [\n",
                 "    Objective(name=\"booth\", target=\"min\"),\n",
                 "]\n",
                 "\n",
                 "\n",
                 "agent = Agent(\n",
                 "    dofs=dofs,\n",
                 "    objectives=objectives,\n",
                 "    digestion=digestion,\n",
                 "    db=db,\n",
                 ")\n",
                 "\n",
-                "RE(agent.learn(acq_func=\"qr\", n=16))\n",
+                "RE(agent.learn(acqf=\"qr\", n=16))\n",
                 "\n",
                 "agent.plot_objectives()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -110,15 +108,15 @@
             "execution_count": null,
             "id": "bc53bf67",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "agent.plot_acquisition(acq_func=\"qei\")"
+                "agent.plot_acquisition(acqf=\"qei\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ebc65169",
             "metadata": {},
```

### Comparing `bloptools-0.6.1/docs/source/tutorials/passive-dofs.ipynb` & `bloptools-0.7.0/docs/source/tutorials/passive-dofs.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978608630952381%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, 'from blop.digestion.tests import "*

 * *            'constrained_himmelblau_digestion\\n\'), (6, \'    DOF(name="x1", search_domain=(-5.0, '*

 * *            '5.0)),\\n\'), (7, \'    DOF(name="x2", search_domain=(-5.0, 5.0)),\\n\'), (8, \'    '*

 * *            'DOF(name="x3", search_domain=(-5.0, 5.0), active=False),\\n\'), (20, \'    '*

 * *            "digestion=constrained_himmelblau_digestion,\\n')], delete: [20, 8, 7, 6, 0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.1 […]*

```diff
@@ -34,35 +34,35 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4cf5dbd1-e404-4504-b822-3956ca61ef74",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from blop.utils import functions\n",
+                "from blop.digestion.tests import constrained_himmelblau_digestion\n",
                 "from blop import DOF, Agent, Objective\n",
                 "from blop.dofs import BrownianMotion\n",
                 "\n",
                 "\n",
                 "dofs = [\n",
-                "    DOF(name=\"x1\", search_bounds=(-5.0, 5.0)),\n",
-                "    DOF(name=\"x2\", search_bounds=(-5.0, 5.0)),\n",
-                "    DOF(name=\"x3\", search_bounds=(-5.0, 5.0), active=False),\n",
+                "    DOF(name=\"x1\", search_domain=(-5.0, 5.0)),\n",
+                "    DOF(name=\"x2\", search_domain=(-5.0, 5.0)),\n",
+                "    DOF(name=\"x3\", search_domain=(-5.0, 5.0), active=False),\n",
                 "    DOF(device=BrownianMotion(name=\"brownian1\"), read_only=True),\n",
                 "    DOF(device=BrownianMotion(name=\"brownian2\"), read_only=True, active=False),\n",
                 "]\n",
                 "\n",
                 "objectives = [\n",
                 "    Objective(name=\"himmelblau\", target=\"min\"),\n",
                 "]\n",
                 "\n",
                 "agent = Agent(\n",
                 "    dofs=dofs,\n",
                 "    objectives=objectives,\n",
-                "    digestion=functions.constrained_himmelblau_digestion,\n",
+                "    digestion=constrained_himmelblau_digestion,\n",
                 "    db=db,\n",
                 "    verbose=True,\n",
                 "    tolerate_acquisition_errors=False,\n",
                 ")\n",
                 "\n",
                 "RE(agent.learn(\"qr\", n=16))"
             ]
@@ -90,15 +90,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.10.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
             }
         }
     },
```

### Comparing `bloptools-0.6.1/docs/wip/constrained-himmelblau copy.ipynb` & `bloptools-0.7.0/docs/wip/constrained-himmelblau copy.ipynb`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/wip/custom-acquisition.ipynb` & `bloptools-0.7.0/docs/wip/custom-acquisition.ipynb`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/wip/introduction.ipynb` & `bloptools-0.7.0/docs/wip/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/wip/latent-toroid-dimensions.ipynb` & `bloptools-0.7.0/docs/wip/latent-toroid-dimensions.ipynb`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/docs/wip/multi-task-sirepo.ipynb` & `bloptools-0.7.0/docs/wip/multi-task-sirepo.ipynb`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/examples/benchmark.py` & `bloptools-0.7.0/examples/benchmark.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/examples/prepare_bluesky.py` & `bloptools-0.7.0/examples/prepare_bluesky.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/examples/prepare_chx_shadow.py` & `bloptools-0.7.0/examples/prepare_chx_shadow.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/examples/prepare_tes_shadow.py` & `bloptools-0.7.0/examples/prepare_tes_shadow.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/examples/prepare_tes_srw.py` & `bloptools-0.7.0/examples/prepare_tes_srw.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/src/blop/agent.py` & `bloptools-0.7.0/src/blop/agent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import os
+import pathlib
 import time as ttime
 import warnings
 from collections import OrderedDict
 from collections.abc import Mapping
 from typing import Callable, Optional, Sequence, Tuple
 
 import bluesky.plan_stubs as bps  # noqa F401
@@ -11,33 +13,38 @@
 import gpytorch
 import h5py
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 import scipy as sp
 import torch
+
+# from botorch.utils.transforms import normalize
+from botorch.acquisition.objective import ScalarizedPosteriorTransform
 from botorch.models.deterministic import GenericDeterministicModel
 from botorch.models.model_list_gp_regression import ModelListGP
-from botorch.models.transforms.input import AffineInputTransform, ChainedInputTransform, Log10, Normalize
+from botorch.models.transforms.input import Normalize
 from databroker import Broker
 from ophyd import Signal
 
-from . import utils
-from .bayesian import acquisition, models, plotting
-from .bayesian.transforms import TargetingPosteriorTransform
+from . import plotting, utils
+from .bayesian import acquisition, models
+from .bayesian.acquisition import _construct_acqf, parse_acqf_identifier
+
+# from .bayesian.transforms import TargetingPosteriorTransform
 from .digestion import default_digestion_function
 from .dofs import DOF, DOFList
 from .objectives import Objective, ObjectiveList
 from .plans import default_acquisition_plan
 
 warnings.filterwarnings("ignore", category=botorch.exceptions.warnings.InputDataWarning)
 
 mpl.rc("image", cmap="coolwarm")
 
-DEFAULT_MAX_SAMPLES = 2**11
+DEFAULT_MAX_SAMPLES = 3200
 
 
 def _validate_dofs_and_objs(dofs: DOFList, objs: ObjectiveList):
     if len(dofs) == 0:
         raise ValueError("You must supply at least one DOF.")
 
     if len(objs) == 0:
@@ -58,14 +65,15 @@
         self,
         dofs: Sequence[DOF],
         objectives: Sequence[Objective],
         db: Broker = None,
         dets: Sequence[Signal] = [],
         acquistion_plan=default_acquisition_plan,
         digestion: Callable = default_digestion_function,
+        digestion_kwargs: dict = {},
         verbose: bool = False,
         tolerate_acquisition_errors=False,
         sample_center_on_init=False,
         trigger_delay: float = 0,
         train_every: int = 1,
     ):
         """
@@ -78,15 +86,17 @@
         objectives : iterable of Objective objects
             The objectives which the agent will try to optimize.
         dets : iterable of ophyd objects
             Detectors to trigger during acquisition.
         acquisition_plan : optional
             A plan that samples the beamline for some given inputs.
         digestion :
-            A function to digest the output of the acquisition, taking arguments (db, uid).
+            A function to digest the output of the acquisition, taking a DataFrame as an argument.
+        digestion_kwargs :
+            Some kwargs for the digestion function.
         db : optional
             A databroker instance.
         verbose : bool
             To be verbose or not.
         tolerate_acquisition_errors : bool
             Whether to allow errors during acquistion. If `True`, errors will be caught as warnings.
         sample_center_on_init : bool
@@ -119,14 +129,15 @@
         _validate_dofs_and_objs(self.dofs, self.objectives)
 
         self.db = db
 
         self.dets = dets
         self.acquisition_plan = acquistion_plan
         self.digestion = digestion
+        self.digestion_kwargs = digestion_kwargs
 
         self.verbose = verbose
 
         self.tolerate_acquisition_errors = tolerate_acquisition_errors
 
         self.train_every = train_every
         self.trigger_delay = trigger_delay
@@ -135,150 +146,170 @@
         self.table = pd.DataFrame()
 
         self.initialized = False
         self.a_priori_hypers = None
 
         self.n_last_trained = 0
 
-    @property
-    def active_dofs(self):
-        return self.dofs.subset(active=True)
+    def unpack_run(self):
+        return
 
-    @property
-    def active_objs(self):
-        return self.objectives.subset(active=True)
+    def measurement_plan(self):
+        return
 
     def __iter__(self):
         for index in range(len(self)):
             yield self.dofs[index]
 
     def __getattr__(self, attr):
-        acq_func_name = acquisition.parse_acq_func_identifier(attr)
-        if acq_func_name is not None:
-            return self._get_acquisition_function(identifier=acq_func_name)
-
+        acqf_config = acquisition.parse_acqf_identifier(attr, strict=False)
+        if acqf_config is not None:
+            acqf, _ = _construct_acqf(agent=self, acqf_name=acqf_config["name"])
+            return acqf
         raise AttributeError(f"No attribute named '{attr}'.")
 
+    def refresh(self):
+        self._construct_all_models()
+        self._train_all_models()
+
+    def redigest(self):
+        self.table = self.digestion(self.table, **self.digestion_kwargs)
+
     def sample(self, n: int = DEFAULT_MAX_SAMPLES, method: str = "quasi-random") -> torch.Tensor:
         """
         Returns a (..., 1, n_active_dofs) tensor of points sampled within the parameter space.
 
         Parameters
         ----------
         n : int
             How many points to sample.
         method : str
             How to sample the points. Must be one of 'quasi-random', 'random', or 'grid'.
         """
 
+        active_dofs = self.dofs(active=True)
+
         if method == "quasi-random":
-            X = utils.normalized_sobol_sampler(n, d=len(self.active_dofs))
+            X = utils.normalized_sobol_sampler(n, d=len(active_dofs))
 
         elif method == "random":
-            X = torch.rand(size=(n, 1, len(self.active_dofs)))
+            X = torch.rand(size=(n, 1, len(active_dofs)))
 
         elif method == "grid":
-            n_side_if_settable = int(np.power(n, 1 / np.sum(~self.active_dofs.read_only)))
+            n_side_if_settable = int(np.power(n, 1 / np.sum(~active_dofs.read_only)))
             sides = [
-                torch.linspace(0, 1, n_side_if_settable) if not dof.read_only else torch.zeros(1) for dof in self.active_dofs
+                torch.linspace(0, 1, n_side_if_settable) if not dof.read_only else torch.zeros(1) for dof in active_dofs
             ]
             X = torch.cat([x.unsqueeze(-1) for x in torch.meshgrid(sides, indexing="ij")], dim=-1).unsqueeze(-2).double()
 
         else:
             raise ValueError("'method' argument must be one of ['quasi-random', 'random', 'grid'].")
 
-        return self._sample_input_transform.untransform(X)
+        return self.dofs(active=True).untransform(X).double()
 
-    def ask(self, acq_func_identifier="qei", n=1, route=True, sequential=True, upsample=1, **acq_func_kwargs):
+    def ask(self, acqf="qei", n=1, route=True, sequential=True, upsample=1, **acqf_kwargs):
         """Ask the agent for the best point to sample, given an acquisition function.
 
         Parameters
         ----------
-        acq_func_identifier :
-            Which acquisition function to use. Supported values can be found in `agent.all_acq_funcs`
+        acqf_identifier :
+            Which acquisition function to use. Supported values can be found in `agent.all_acqfs`
         n : int
             How many points you want
         route : bool
             Whether to route the supplied points to make a more efficient path.
         sequential : bool
             Whether to generate points sequentially (as opposed to in parallel). Sequential generation involves
             finding one points and constructing a fantasy posterior about its value to generate the next point.
         """
 
-        acq_func_name = acquisition.parse_acq_func_identifier(acq_func_identifier)
-        acq_func_type = acquisition.config[acq_func_name]["type"]
+        acqf_config = parse_acqf_identifier(acqf)
+        if acqf_config is None:
+            raise ValueError(f"'{acqf}' is an invalid acquisition function.")
 
         start_time = ttime.monotonic()
 
-        if acq_func_name in ["quasi-random", "random", "grid"]:
-            candidates = self.sample(n=n, method=acq_func_name).squeeze(1).numpy()
+        active_dofs = self.dofs(active=True)
+        active_objs = self.objectives(active=True)
 
-            # define dummy acqf objective
-            acqf_obj = torch.zeros(len(candidates))
+        # these are the fake acquisiton functions that we don't need to construct
+        if acqf_config["name"] in ["quasi-random", "random", "grid"]:
+            candidates = self.sample(n=n, method=acqf_config["name"]).squeeze(1).numpy()
 
-        elif acq_func_type in ["analytic", "monte_carlo"]:
-            if not all(hasattr(obj, "model") for obj in self.objectives):
+            # define dummy acqf kwargs and objective
+            acqf_kwargs, acqf_obj = {}, torch.zeros(len(candidates))
+
+        else:
+            # check that all the objectives have models
+            if not all(hasattr(obj, "model") for obj in active_objs):
                 raise RuntimeError(
-                    f"Can't construct non-trivial acquisition function '{acq_func_identifier}'"
-                    f" (the agent is not initialized!)"
+                    f"Can't construct non-trivial acquisition function '{acqf}' as the agent is not initialized."
                 )
 
-            for obj in self.active_objs:
-                if obj.model_dofs != set(self.active_dofs.names):
+            # if the model for any active objective mismatches the active dofs, reconstrut and train it
+            for obj in active_objs:
+                if obj.model_dofs != set(active_dofs.names):
                     self._construct_model(obj)
                     self._train_model(obj.model)
 
-            if acq_func_type == "analytic" and n > 1:
+            if acqf_config["type"] == "analytic" and n > 1:
                 raise ValueError("Can't generate multiple design points for analytic acquisition functions.")
 
-            acq_func, _ = self._get_acquisition_function(
-                identifier=acq_func_identifier, return_metadata=True, **acq_func_kwargs
-            )
+            # we may pick up some more kwargs
+            acqf, acqf_kwargs = _construct_acqf(self, acqf_name=acqf_config["name"], **acqf_kwargs)
 
             NUM_RESTARTS = 8
             RAW_SAMPLES = 256
 
             candidates, acqf_obj = botorch.optim.optimize_acqf(
-                acq_function=acq_func,
-                bounds=self._sample_bounds,
+                acq_function=acqf,
+                bounds=self.sample_domain,
                 q=n,
                 sequential=sequential,
                 num_restarts=NUM_RESTARTS,
                 raw_samples=RAW_SAMPLES,  # used for intialization heuristic
+                fixed_features={i: dof._transform(dof.readback) for i, dof in enumerate(active_dofs) if dof.read_only},
             )
 
-            # this includes both RO and non-RO DOFs
-            candidates = candidates.numpy()
+            # this includes both RO and non-RO DOFs.
+            # and is in the transformed model space
+            candidates = self.dofs(active=True).untransform(candidates).numpy()
+
+        # p = self.posterior(candidates) if hasattr(self, "model") else None
 
-        acq_points = candidates[..., ~self.active_dofs.read_only]
-        read_only_values = candidates[..., self.active_dofs.read_only]
+        active_dofs = self.dofs(active=True)
+
+        points = candidates[..., ~active_dofs.read_only]
+        read_only_values = candidates[..., active_dofs.read_only]
 
         duration = 1e3 * (ttime.monotonic() - start_time)
 
         if route and n > 1:
-            routing_index = utils.route(self.dofs.subset(active=True, read_only=False).readback, acq_points)
-            acq_points = acq_points[routing_index]
+            current_points = np.array([dof.readback for dof in active_dofs if not dof.read_only])
+            travel_expenses = np.array([dof.travel_expense for dof in active_dofs if not dof.read_only])
+            routing_index = utils.route(current_points, points, dim_weights=travel_expenses)
+            points = points[routing_index]
 
         if upsample > 1:
-            idx = np.arange(len(acq_points))
+            if n == 1:
+                raise ValueError("Cannot upsample points unless n > 1.")
+            idx = np.arange(len(points))
             upsampled_idx = np.linspace(0, len(idx) - 1, upsample * len(idx) - 1)
-            acq_points = sp.interpolate.interp1d(idx, acq_points, axis=0)(upsampled_idx)
-
-        p = self.posterior(candidates) if hasattr(self, "model") else None
+            points = sp.interpolate.interp1d(idx, points, axis=0)(upsampled_idx)
 
         res = {
-            "points": acq_points,
-            "acq_func": acq_func_name,
-            "acq_func_kwargs": acq_func_kwargs,
-            "acq_func_obj": np.atleast_1d(acqf_obj.numpy()),
+            "points": {dof.name: list(points[..., i]) for i, dof in enumerate(active_dofs(read_only=False))},
+            "acqf_name": acqf_config["name"],
+            "acqf_obj": list(np.atleast_1d(acqf_obj.numpy())),
+            "acqf_kwargs": acqf_kwargs,
             "duration_ms": duration,
             "sequential": sequential,
             "upsample": upsample,
             "read_only_values": read_only_values,
-            "posterior": p,
+            # "posterior": p,
         }
 
         return res
 
     def tell(
         self,
         data: Optional[Mapping] = {},
@@ -320,21 +351,21 @@
             raise ValueError("All supplies values must be the same length!")
 
         new_table = pd.DataFrame(data)
         self.table = pd.concat([self.table, new_table]) if append else new_table
         self.table.index = np.arange(len(self.table))
 
         if update_models:
-            for obj in self.active_objs:
+            for obj in self.objectives(active=True):
                 t0 = ttime.monotonic()
 
                 cached_hypers = obj.model.state_dict() if hasattr(obj, "model") else None
-                n_before_tell = obj.n
+                n_before_tell = obj.n_valid
                 self._construct_model(obj)
-                n_after_tell = obj.n
+                n_after_tell = obj.n_valid
 
                 if train is None:
                     train = int(n_after_tell / self.train_every) > int(n_before_tell / self.train_every)
 
                 if len(obj.model.train_targets) >= 4:
                     if train:
                         t0 = ttime.monotonic()
@@ -343,33 +374,34 @@
                             print(f"trained model '{obj.name}' in {1e3*(ttime.monotonic() - t0):.00f} ms")
 
                     else:
                         self._train_model(obj.model, hypers=cached_hypers)
 
     def learn(
         self,
-        acq_func: str = "qei",
+        acqf: str = "qei",
         n: int = 1,
         iterations: int = 1,
         upsample: int = 1,
         train: bool = None,
         append: bool = True,
         hypers: str = None,
         route: bool = True,
+        **acqf_kwargs,
     ):
         """This returns a Bluesky plan which iterates the learning algorithm, looping over ask -> acquire -> tell.
 
         For example:
 
         RE(agent.learn('qr', n=16))
         RE(agent.learn('qei', n=4, iterations=4))
 
         Parameters
         ----------
-        acq_func : str
+        acqf : str
             A valid identifier for an implemented acquisition function.
         n : int
             How many points to sample on each iteration.
         iterations: int
             How many iterations of the learning loop to perform.
         train: bool
             Whether to train the models upon telling the agent.
@@ -379,28 +411,31 @@
             If supplied, read a saved data file instead of running the acquisition plan.
         hypers_file: str
             If supplied, read a saved hyperparameter file instead of fitting models. NOTE: The agent will assume these
             hyperparameters a priori for the rest of the run, and not try to fit a model.
         """
 
         if self.sample_center_on_init and not self.initialized:
-            center_inputs = np.atleast_2d(self.dofs.subset(active=True, read_only=False).search_bounds.mean(axis=1))
+            center_inputs = np.atleast_2d(self.dofs(active=True, read_only=False).search_domain.mean(axis=1))
             new_table = yield from self.acquire(center_inputs)
-            new_table.loc[:, "acq_func"] = "sample_center_on_init"
+            new_table.loc[:, "acqf"] = "sample_center_on_init"
 
         for i in range(iterations):
-            print(f"running iteration {i + 1} / {iterations}")
-            for single_acq_func in np.atleast_1d(acq_func):
-                res = self.ask(n=n, acq_func_identifier=single_acq_func, upsample=upsample, route=route)
+            if self.verbose:
+                print(f"running iteration {i + 1} / {iterations}")
+            for single_acqf in np.atleast_1d(acqf):
+                res = self.ask(n=n, acqf=single_acqf, upsample=upsample, route=route, **acqf_kwargs)
                 new_table = yield from self.acquire(res["points"])
-                new_table.loc[:, "acq_func"] = res["acq_func"]
+                new_table.loc[:, "acqf"] = res["acqf_name"]
 
-                x = {key: new_table.pop(key).tolist() for key in self.dofs.names}
-                y = {key: new_table.pop(key).tolist() for key in self.objectives.names}
-                metadata = new_table.to_dict(orient="list")
+                x = {key: new_table.loc[:, key].tolist() for key in self.dofs.names}
+                y = {key: new_table.loc[:, key].tolist() for key in self.objectives.names}
+                metadata = {
+                    key: new_table.loc[:, key].tolist() for key in new_table.columns if (key not in x) and (key not in y)
+                }
                 self.tell(x=x, y=y, metadata=metadata, append=append, train=train)
 
     def view(self, item: str = "mean", cmap: str = "turbo", max_inputs: int = 2**16):
         """
         Use napari to see a high-dimensional array.
 
         Parameters
@@ -412,155 +447,224 @@
         import napari  # noqa E402
 
         test_grid = self.sample(n=max_inputs, method="grid")
 
         self.viewer = napari.Viewer()
 
         if item in ["mean", "error"]:
-            for obj in self.active_objs:
+            for obj in self.objectives(active=True):
                 p = obj.model.posterior(test_grid)
 
                 if item == "mean":
                     mean = p.mean.detach().numpy()[..., 0, 0]
                     self.viewer.add_image(data=mean, name=f"{obj.name}_mean", colormap=cmap)
 
                 if item == "error":
                     error = np.sqrt(p.variance.detach().numpy()[..., 0, 0])
                     self.viewer.add_image(data=error, name=f"{obj.name}_error", colormap=cmap)
 
         else:
             try:
-                acq_func_identifier = acquisition.parse_acq_func_identifier(identifier=item)
+                acqf_identifier = acquisition.parse_acqf_identifier(identifier=item)
             except Exception:
                 raise ValueError("'item' must be either 'mean', 'error', or a valid acq func.")
 
-            acq_func, acq_func_meta = self._get_acquisition_function(identifier=acq_func_identifier, return_metadata=True)
-            a = acq_func(test_grid).detach().numpy()
+            acqf, acqf_meta = self._get_acquisition_function(identifier=acqf_identifier, return_metadata=True)
+            a = acqf(test_grid).detach().numpy()
 
-            self.viewer.add_image(data=a, name=f"{acq_func_identifier}", colormap=cmap)
+            self.viewer.add_image(data=a, name=f"{acqf_identifier}", colormap=cmap)
 
         self.viewer.dims.axis_labels = self.dofs.names
 
-    def acquire(self, acquisition_inputs):
+    def acquire(self, points):
         """Acquire and digest according to the self's acquisition and digestion plans.
 
         Parameters
         ----------
         acquisition_inputs :
             A 2D numpy array comprising inputs for the active and non-read-only DOFs to sample.
         """
 
         if self.db is None:
             raise ValueError("Cannot run acquistion without databroker instance!")
 
+        acquisition_dofs = self.dofs(active=True, read_only=False)
+        for dof in acquisition_dofs:
+            if dof.name not in points:
+                raise ValueError(f"Cannot acquire points; missing values for {dof.name}.")
+
+        n = len(points[dof.name])
+
         try:
-            acquisition_devices = self.dofs.subset(active=True, read_only=False).devices
             uid = yield from self.acquisition_plan(
-                acquisition_devices,
-                acquisition_inputs.astype(float),
+                acquisition_dofs,
+                points,
                 [*self.dets, *self.dofs.devices],
                 delay=self.trigger_delay,
             )
-
-            products = self.digestion(self.db, uid)
+            products = self.digestion(self.db[uid].table(), **self.digestion_kwargs)
 
         except KeyboardInterrupt as interrupt:
             raise interrupt
 
         except Exception as error:
             if not self.tolerate_acquisition_errors:
                 raise error
             logging.warning(f"Error in acquisition/digestion: {repr(error)}")
-            products = pd.DataFrame(acquisition_inputs, columns=self.dofs.subset(active=True, read_only=False).names)
-            for obj in self.active_objs:
+            products = pd.DataFrame(points)
+            for obj in self.objectives(active=True):
                 products.loc[:, obj.name] = np.nan
 
-        if not len(acquisition_inputs) == len(products):
+        if len(products) != n:
             raise ValueError("The table returned by the digestion function must be the same length as the sampled inputs!")
 
         return products
 
-    def load_data(self, data_file, append=True, train=True):
+    def load_data(self, data_file, append=True):
         new_table = pd.read_hdf(data_file, key="table")
-        x = {key: new_table.pop(key).tolist() for key in self.dofs.names}
-        y = {key: new_table.pop(key).tolist() for key in self.objectives.names}
-        metadata = new_table.to_dict(orient="list")
-        self.tell(x=x, y=y, metadata=metadata, append=append, train=train)
+        self.table = pd.concat([self.table, new_table]) if append else new_table
+        self.refresh()
 
     def reset(self):
         """Reset the agent."""
         self.table = pd.DataFrame()
 
-        for obj in self.active_objs:
+        for obj in self.objectives(active=True):
             if hasattr(obj, "model"):
                 del obj.model
 
         self.n_last_trained = 0
 
     def benchmark(
-        self, output_dir="./", runs=16, n_init=64, learning_kwargs_list=[{"acq_func": "qei", "n": 4, "iterations": 16}]
+        self,
+        output_dir="./",
+        iterations=16,
+        per_iter_learn_kwargs_list=[{"acqf": "qr", "n": 32}, {"acqf": "qei", "n": 1, "iterations": 4}],
     ):
         """Iterate over having the agent learn from scratch, and save the results to an output directory.
 
         Parameters
         ----------
         output_dir :
             Where to save the agent output.
-        runs : int
+        iterations : int
             How many benchmarks to run
-        learning_kwargs_list:
-            A list of kwargs to pass to the learn method which the agent will run sequentially for each run.
+        per_iter_learn_kwargs_list:
+            A list of kwargs to pass to the agent.learn() method that the agent will run sequentially for each iteration.
         """
 
-        for run in range(runs):
+        for _ in range(iterations):
             self.reset()
 
-            for kwargs in learning_kwargs_list:
+            for kwargs in per_iter_learn_kwargs_list:
                 yield from self.learn(**kwargs)
 
-            self.save_data(output_dir + f"benchmark-{int(ttime.time())}.h5")
+            self.save_data(f"{output_dir}/blop_benchmark_{int(ttime.time())}.h5")
 
     @property
     def model(self):
-        """A model encompassing all the objectives. A single GP in the single-objective case, or a model list."""
-        return (
-            ModelListGP(*[obj.model for obj in self.active_objs]) if len(self.active_objs) > 1 else self.active_objs[0].model
-        )
+        """A model encompassing all the fitnesses and constraints."""
+        active_objs = self.objectives(active=True)
+        if all(hasattr(obj, "model") for obj in active_objs):
+            return ModelListGP(*[obj.model for obj in active_objs]) if len(active_objs) > 1 else active_objs[0].model
+        raise ValueError("Not all active objectives have models.")
 
     def posterior(self, x):
         """A model encompassing all the objectives. A single GP in the single-objective case, or a model list."""
-        return self.model.posterior(torch.tensor(x))
+        return self.model.posterior(self.dofs(active=True).transform(torch.tensor(x)))
 
     @property
-    def targeting_transform(self):
-        return TargetingPosteriorTransform(
-            weights=torch.tensor(self.active_objs.weights, dtype=torch.double), targets=self.active_objs.targets
-        )
+    def fitness_model(self):
+        active_fitness_models = self.objectives(active=True, kind="fitness")
+        if len(active_fitness_models) == 0:
+            return GenericDeterministicModel(f=lambda x: torch.ones(x.shape[:-1]).unsqueeze(-1))
+        if len(active_fitness_models) == 1:
+            return active_fitness_models[0].model
+        return ModelListGP(*[obj.model for obj in active_fitness_models])
 
     @property
-    def scalarized_objectives(self):
-        """Returns a (n_obs,) array of scalarized objectives"""
-        return self.targeting_transform.evaluate(self.train_targets(active=True)).sum(axis=-1)
+    def evaluated_constraints(self):
+        constraint_objectives = self.objectives(kind="constraint")
+        if len(constraint_objectives):
+            return torch.cat([obj.constrain(self.raw_targets(obj.name)) for obj in constraint_objectives], dim=-1)
+        else:
+            return torch.ones(size=(len(self.table), 0), dtype=torch.bool)
+
+    def fitness_scalarization(self, weights="default"):
+        fitness_objectives = self.objectives(active=True, kind="fitness")
+        if weights == "default":
+            weights = torch.tensor([obj.weight for obj in fitness_objectives], dtype=torch.double)
+        elif weights == "equal":
+            weights = torch.ones(len(fitness_objectives), dtype=torch.double)
+        elif weights == "random":
+            weights = torch.rand(len(fitness_objectives), dtype=torch.double)
+            weights *= len(fitness_objectives) / weights.sum()
+        elif not isinstance(weights, torch.Tensor):
+            raise ValueError(f"'weights' must be a Tensor or one of ['default', 'equal', 'random'], and not {weights}.")
+        return ScalarizedPosteriorTransform(weights=weights)
+
+    def scalarized_fitnesses(self, weights="default", constrained=True):
+        """
+        Return the scalar fitness for each sample, scalarized by the weighting scheme.
+
+        If constrained=True, the points that satisfy the most constraints are automatically better than the others.
+        """
+        fitness_objs = self.objectives(kind="fitness")
+        if len(fitness_objs) >= 1:
+            f = self.fitness_scalarization(weights=weights).evaluate(self.train_targets(active=True, kind="fitness"))
+            f = torch.where(f.isnan(), -np.inf, f)  # remove all nans
+        else:
+            f = torch.zeros(len(self.table), dtype=torch.double)  # if there are no fitnesses, use a constant dummy fitness
+        if constrained:
+            # how many constraints are satisfied?
+            c = self.evaluated_constraints.sum(axis=-1)
+            f = torch.where(c < c.max(), -np.inf, f)
+        return f
+
+    def argmax_best_f(self, weights="default"):
+        return int(self.scalarized_fitnesses(weights=weights, constrained=True).argmax())
+
+    def best_f(self, weights="default"):
+        return float(self.scalarized_fitnesses(weights=weights, constrained=True).max())
 
     @property
-    def max_scalarized_objective(self):
-        """Returns the value of the best scalarized objective seen so far."""
-        f = self.scalarized_objectives
-        return np.max(np.where(np.isnan(f), -np.inf, f))
+    def pareto_mask(self):
+        """
+        Returns a mask of all points that satisfy all constraints and are Pareto efficient.
+        A point is Pareto efficient if it is there is no other point that is better at every objective.
+        """
+        Y = self.train_targets(active=True, kind="fitness")
+
+        # nuke the bad points
+        Y[~self.evaluated_constraints.all(axis=-1)] = -np.inf
+        if Y.shape[-1] < 2:
+            raise ValueError("Computing the Pareto front requires at least 2 fitness objectives.")
+        in_pareto_front = ~(Y.unsqueeze(1) > Y.unsqueeze(0)).all(axis=-1).any(axis=0)
+        return in_pareto_front & self.evaluated_constraints.all(axis=-1)
 
     @property
-    def argmax_scalarized_objective(self):
-        """Returns the index of the best scalarized objective seen so far."""
-        f = self.scalarized_objectives
-        return np.argmax(np.where(np.isnan(f), -np.inf, f))
+    def pareto_front(self):
+        """
+        A subset of the data table containing only points on the Pareto front.
+        """
+        return self.table.loc[self.pareto_mask.numpy()]
+
+    @property
+    def min_ref_point(self):
+        y = self.train_targets()[:, self.objectives.type == "fitness"]
+        return y[y.argmax(axis=0)].min(axis=0).values
+
+    @property
+    def random_ref_point(self):
+        return self.train_targets(active=True, kind="fitness")[self.argmax_best_f(weights="random")]
 
     @property
     def all_objectives_valid(self):
         """A mask of whether all objectives are valid for each data point."""
-        return ~torch.isnan(self.scalarized_objectives)
+        return ~torch.isnan(self.scalarized_fitnesses())
 
     def _train_model(self, model, hypers=None, **kwargs):
         """Fit all of the agent's models. All kwargs are passed to `botorch.fit.fit_gpytorch_mll`."""
         if hypers is not None:
             model.load_state_dict(hypers)
         else:
             botorch.fit.fit_gpytorch_mll(gpytorch.mlls.ExactMarginalLogLikelihood(model.likelihood, model), **kwargs)
@@ -591,130 +695,124 @@
         trusted = inputs_are_trusted & targets_are_trusted
 
         obj.model = models.LatentGP(
             train_inputs=train_inputs[trusted],
             train_targets=train_targets[trusted],
             likelihood=likelihood,
             skew_dims=skew_dims,
-            input_transform=self._model_input_transform,
+            input_transform=self.input_normalization,
             outcome_transform=outcome_transform,
         )
 
-        obj.model_dofs = set(self.active_dofs.names)  # if these change, retrain the model on self.ask()
+        obj.model_dofs = set(self.dofs(active=True).names)  # if these change, retrain the model on self.ask()
 
         if trusted.all():
             obj.validity_conjugate_model = None
             obj.validity_constraint = GenericDeterministicModel(f=lambda x: torch.ones(size=x.size())[..., -1])
 
         else:
             dirichlet_likelihood = gpytorch.likelihoods.DirichletClassificationLikelihood(
                 trusted.long(), learn_additional_noise=True
             )
 
-            obj.validity_conjugate_model = models.LatentDirichletModel(
+            obj.validity_conjugate_model = models.LatentDirichletClassifier(
                 train_inputs=train_inputs[inputs_are_trusted],
                 train_targets=dirichlet_likelihood.transformed_targets.transpose(-1, -2)[inputs_are_trusted].double(),
                 skew_dims=skew_dims,
                 likelihood=dirichlet_likelihood,
-                input_transform=self._model_input_transform,
+                input_transform=self.input_normalization,
             )
 
             obj.validity_constraint = GenericDeterministicModel(
                 f=lambda x: obj.validity_conjugate_model.probabilities(x)[..., -1]
             )
 
     def _construct_all_models(self):
         """Construct a model for each objective."""
-        for obj in self.active_objs:
+        for obj in self.objectives(active=True):
             self._construct_model(obj)
 
     def _train_all_models(self, **kwargs):
         """Fit all of the agent's models. All kwargs are passed to `botorch.fit.fit_gpytorch_mll`."""
         t0 = ttime.monotonic()
-        for obj in self.active_objs:
+        for obj in self.objectives(active=True):
             self._train_model(obj.model)
             if obj.validity_conjugate_model is not None:
                 self._train_model(obj.validity_conjugate_model)
 
         if self.verbose:
             print(f"trained models in {ttime.monotonic() - t0:.01f} seconds")
 
         self.n_last_trained = len(self.table)
 
     def _get_acquisition_function(self, identifier, return_metadata=False):
         """Returns a BoTorch acquisition function for a given identifier. Acquisition functions can be
-        found in `agent.all_acq_funcs`.
+        found in `agent.all_acqfs`.
         """
-        return acquisition.get_acquisition_function(self, identifier=identifier, return_metadata=return_metadata)
+
+        acquisition._construct_acqf(self, identifier=identifier, return_metadata=return_metadata)
+
+        return
 
     def _latent_dim_tuples(self, obj_index=None):
         """
         For the objective indexed by 'obj_index', return a list of tuples, where each tuple represents
         a group of DOFs to fit a latent representation to.
         """
 
         if obj_index is None:
             return {obj.name: self._latent_dim_tuples(obj_index=obj.name) for obj in self.objectives}
 
         obj = self.objectives[obj_index]
 
         latent_group_index = {}
-        for dof in self.active_dofs:
+        for dof in self.dofs(active=True):
             latent_group_index[dof.name] = dof.name
             for group_index, latent_group in enumerate(obj.latent_groups):
                 if dof.name in latent_group:
                     latent_group_index[dof.name] = group_index
 
         u, uinv = np.unique(list(latent_group_index.values()), return_inverse=True)
         return [tuple(np.where(uinv == i)[0]) for i in range(len(u))]
 
     @property
-    def _sample_bounds(self):
-        return torch.tensor(self.active_dofs.search_bounds, dtype=torch.double).T
-
-    @property
-    def _sample_input_transform(self):
-        tf1 = Log10(indices=list(np.where(self.active_dofs.log)[0]))
-
-        transformed_sample_bounds = tf1.transform(self._sample_bounds)
-
-        offset = transformed_sample_bounds.min(dim=0).values
-        coefficient = (transformed_sample_bounds.max(dim=0).values - offset).clamp(min=1e-16)
-
-        tf2 = AffineInputTransform(d=len(offset), coefficient=coefficient, offset=offset)
-
-        return ChainedInputTransform(tf1=tf1, tf2=tf2)
+    def sample_domain(self):
+        """
+        Returns a (2, n_active_dof) array of lower and upper bounds for dofs.
+        Read-only DOFs are set to exactly their last known value.
+        Discrete DOFs are relaxed to some continuous domain.
+        """
+        return self.dofs(active=True).transform(self.dofs(active=True).search_domain.T)
 
     @property
-    def _model_input_transform(self):
+    def input_normalization(self):
         """
         Suitably transforms model inputs to the unit hypercube.
 
         For modeling:
 
-        Always normalize between min and max values. This is always inside the trust bounds, sometimes smaller.
+        Always normalize between min and max values. This is always inside the trust domain, sometimes smaller.
 
         For sampling:
 
         Settable: normalize between search bounds
         Read-only: constrain to the readback value
         """
 
-        tf1 = Log10(indices=list(np.where(self.active_dofs.log)[0]))
-        tf2 = Normalize(d=len(self.active_dofs))
+        return Normalize(d=self.dofs.active.sum())
 
-        return ChainedInputTransform(tf1=tf1, tf2=tf2)
-
-    def save_data(self, filepath="./self_data.h5"):
+    def save_data(self, path="./data.h5"):
         """
         Save the sampled inputs and targets of the agent to a file, which can be used
-        to initialize a future self.
+        to initialize a future agent.
         """
 
-        self.table.to_hdf(filepath, key="table")
+        save_dir, _ = os.path.split(path)
+        pathlib.Path(save_dir).mkdir(parents=True, exist_ok=True)
+        self.table.to_hdf(path, key="table")
 
     def forget(self, last=None, index=None, train=True):
         """
         Make the agent forget some data.
 
         Parameters
         ----------
@@ -735,28 +833,30 @@
             if train:
                 self._train_all_models()
 
         else:
             raise ValueError("Must supply either 'last' or 'index'.")
 
     def _set_hypers(self, hypers):
-        for obj in self.active_objs:
+        for obj in self.objectives(active=True):
             obj.model.load_state_dict(hypers[obj.name])
         self.validity_constraint.load_state_dict(hypers["validity_constraint"])
 
     def constraint(self, x):
+        x = self.dofs(active=True).transform(x)
+
         p = torch.ones(x.shape[:-1])
-        for obj in self.active_objs:
+        for obj in self.objectives(active=True):
             # if the targeting constraint is non-trivial
-            if obj.use_as_constraint:
-                p *= obj.targeting_constraint(x)
+            # if obj.kind == "constraint":
+            #     p *= obj.targeting_constraint(x)
             # if the validity constaint is non-trivial
             if obj.validity_conjugate_model is not None:
                 p *= obj.validity_constraint(x)
-        return p
+        return p  # + 1e-6 * normalize(x, self.sample_domain).square().sum(axis=-1)
 
     @property
     def hypers(self) -> dict:
         """Returns a dict of all the hyperparameters for each model in each objective."""
         hypers = {}
         for obj in self.objectives:
             hypers[obj.name] = {"model": {}, "validity_conjugate_model": {}}
@@ -798,68 +898,75 @@
 
                 for key, value in f[obj_name]["validity_conjugate_model"].items():
                     hypers[obj_name]["validity_conjugate_model"][key] = torch.tensor(np.atleast_1d(value[()]))
 
         return hypers
 
     @property
-    def all_acq_funcs(self):
-        """Description and identifiers for all supported acquisition functions."""
-        entries = []
-        for k, d in acquisition.config.items():
-            ret = ""
-            ret += f"{d['pretty_name'].upper()} (identifiers: {d['identifiers']})\n"
-            ret += f"-> {d['description']}"
-            entries.append(ret)
+    def all_acqfs(self):
+        """
+        Description and identifiers for all supported acquisition functions.
+        """
+        return acquisition.all_acqfs()
 
-        print("\n\n".join(entries))
+    def raw_inputs(self, index=None, **subset_kwargs):
+        """
+        Get the raw, untransformed inputs for a DOF (or for a subset).
+        """
+        if index is None:
+            return torch.cat([self.raw_inputs(dof.name) for dof in self.dofs(**subset_kwargs)], dim=-1)
+        return torch.tensor(self.table.loc[:, self.dofs[index].name].values, dtype=torch.double).unsqueeze(-1)
 
     def train_inputs(self, index=None, **subset_kwargs):
         """A two-dimensional tensor of all DOF values."""
 
         if index is None:
-            return torch.cat([self.train_inputs(dof.name) for dof in self.dofs.subset(**subset_kwargs)], dim=-1)
+            return torch.cat([self.train_inputs(index=dof.name) for dof in self.dofs(**subset_kwargs)], dim=-1)
 
         dof = self.dofs[index]
-        inputs = self.table.loc[:, dof.name].values.copy()
+        raw_inputs = self.raw_inputs(index=index, **subset_kwargs)
 
         # check that inputs values are inside acceptable values
-        valid = (inputs >= dof._trust_bounds[0]) & (inputs <= dof._trust_bounds[1])
-        inputs = np.where(valid, inputs, np.nan)
+        valid = (raw_inputs >= dof._trust_domain[0]) & (raw_inputs <= dof._trust_domain[1])
+        raw_inputs = torch.where(valid, raw_inputs, np.nan)
 
-        return torch.tensor(inputs, dtype=torch.double).unsqueeze(-1)
+        return dof._transform(raw_inputs)
+
+    def raw_targets(self, index=None, **subset_kwargs):
+        """
+        Get the raw, untransformed inputs for an objective (or for a subset).
+        """
+        if index is None:
+            return torch.cat([self.raw_targets(index=obj.name) for obj in self.objectives(**subset_kwargs)], dim=-1)
+        return torch.tensor(self.table.loc[:, self.objectives[index].name].values, dtype=torch.double).unsqueeze(-1)
 
     def train_targets(self, index=None, **subset_kwargs):
         """Returns the values associated with an objective name."""
 
         if index is None:
-            return torch.cat([self.train_targets(obj.name) for obj in self.objectives], dim=-1)
+            return torch.cat([self.train_targets(obj.name) for obj in self.objectives(**subset_kwargs)], dim=-1)
 
         obj = self.objectives[index]
-        targets = self.table.loc[:, obj.name].values.copy()
+        raw_targets = self.raw_targets(index=index, **subset_kwargs)
 
         # check that targets values are inside acceptable values
-        valid = (targets >= obj._trust_bounds[0]) & (targets <= obj._trust_bounds[1])
-        targets = np.where(valid, targets, np.nan)
-
-        # transform if needed
-        if obj.log:
-            targets = np.where(targets > 0, np.log(targets), np.nan)
+        valid = (raw_targets >= obj._trust_domain[0]) & (raw_targets <= obj._trust_domain[1])
+        raw_targets = torch.where(valid, raw_targets, np.nan)
 
-        return torch.tensor(targets, dtype=torch.double).unsqueeze(-1)
+        return obj._transform(raw_targets)
 
     @property
     def best(self):
         """Returns all data for the best point."""
-        return self.table.loc[self.argmax_scalarized_objective]
+        return self.table.loc[self.argmax_best_f()]
 
     @property
     def best_inputs(self):
         """Returns the value of each DOF at the best point."""
-        return self.table.loc[self.argmax_scalarized_objective, self.dofs.names].to_dict()
+        return self.table.loc[self.argmax_best_f(), self.dofs.names].to_dict()
 
     def go_to(self, **positions):
         """Set all settable DOFs to a given position. DOF/value pairs should be supplied as kwargs, e.g. as
 
         RE(agent.go_to(some_dof=x1, some_other_dof=x2, ...))
         """
         mv_args = []
@@ -882,49 +989,57 @@
         """Plot the sampled objectives
 
         Parameters
         ----------
         axes :
             A tuple specifying which DOFs to plot as a function of. Can be either an int or the name of DOFs.
         """
-        if len(self.dofs.subset(active=True, read_only=False)) == 1:
-            plotting._plot_objs_one_dof(self, **kwargs)
+
+        if len(self.dofs(active=True, read_only=False)) == 1:
+            if len(self.objectives(active=True, kind="fitness")) > 0:
+                plotting._plot_fitness_objs_one_dof(self, **kwargs)
+            if len(self.objectives(active=True, kind="constraint")) > 0:
+                plotting._plot_constraint_objs_one_dof(self, **kwargs)
         else:
             plotting._plot_objs_many_dofs(self, axes=axes, **kwargs)
 
-    def plot_acquisition(self, acq_func="ei", axes: Tuple = (0, 1), **kwargs):
+    def plot_acquisition(self, acqf="ei", axes: Tuple = (0, 1), **kwargs):
         """Plot an acquisition function over test inputs sampling the limits of the parameter space.
 
         Parameters
         ----------
-        acq_func :
+        acqf :
             Which acquisition function to plot. Can also take a list of acquisition functions.
         axes :
             A tuple specifying which DOFs to plot as a function of. Can be either an int or the name of DOFs.
         """
-        if len(self.dofs.subset(active=True, read_only=False)) == 1:
-            plotting._plot_acqf_one_dof(self, acq_funcs=np.atleast_1d(acq_func), **kwargs)
+        if len(self.dofs(active=True, read_only=False)) == 1:
+            plotting._plot_acqf_one_dof(self, acqfs=np.atleast_1d(acqf), **kwargs)
 
         else:
-            plotting._plot_acqf_many_dofs(self, acq_funcs=np.atleast_1d(acq_func), axes=axes, **kwargs)
+            plotting._plot_acqf_many_dofs(self, acqfs=np.atleast_1d(acqf), axes=axes, **kwargs)
 
     def plot_validity(self, axes: Tuple = (0, 1), **kwargs):
         """Plot the modeled constraint over test inputs sampling the limits of the parameter space.
 
         Parameters
         ----------
         axes :
             A tuple specifying which DOFs to plot as a function of. Can be either an int or the name of DOFs.
         """
-        if len(self.dofs.subset(active=True, read_only=False)) == 1:
+        if len(self.dofs(active=True, read_only=False)) == 1:
             plotting._plot_valid_one_dof(self, **kwargs)
 
         else:
             plotting._plot_valid_many_dofs(self, axes=axes, **kwargs)
 
     def plot_history(self, **kwargs):
         """Plot the improvement of the agent over time."""
         plotting._plot_history(self, **kwargs)
 
     @property
     def latent_transforms(self):
-        return {obj.name: obj.model.covar_module.latent_transform for obj in self.active_objs}
+        return {obj.name: obj.model.covar_module.latent_transform for obj in self.objectives(active=True)}
+
+    def plot_pareto_front(self, **kwargs):
+        """Plot the improvement of the agent over time."""
+        plotting._plot_pareto_front(self, **kwargs)
```

### Comparing `bloptools-0.6.1/src/blop/plans.py` & `bloptools-0.7.0/src/blop/plans.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import bluesky.plan_stubs as bps
 import bluesky.plans as bp
-import numpy as np
 
 
 def list_scan_with_delay(*args, delay=0, **kwargs):
     "Accepts all the normal 'scan' parameters, plus an optional delay."
 
     def one_nd_step_with_delay(detectors, step, pos_cache):
         "This is a copy of bluesky.plan_stubs.one_nd_step with a sleep added."
@@ -15,15 +14,25 @@
 
     kwargs.setdefault("per_step", one_nd_step_with_delay)
     uid = yield from bp.list_scan(*args, **kwargs)
     return uid
 
 
 def default_acquisition_plan(dofs, inputs, dets, **kwargs):
+    """
+    Parameters
+    ----------
+    x : list of DOFs or DOFList
+        A list of DOFs
+    inputs: dict
+        A dict of a list of inputs per dof, keyed by dof.name
+    dets: list
+        A list of detectors to trigger
+    """
     delay = kwargs.get("delay", 0)
     args = []
-    for dof, points in zip(dofs, np.atleast_2d(inputs).T):
-        args.append(dof)
-        args.append(list(points))
+    for dof in dofs:
+        args.append(dof.device)
+        args.append(inputs[dof.name])
 
     uid = yield from list_scan_with_delay(dets, *args, delay=delay)
     return uid
```

### Comparing `bloptools-0.6.1/src/blop/bayesian/kernels.py` & `bloptools-0.7.0/src/blop/bayesian/kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,18 @@
     def latent_transform(self):
         return torch.matmul(self.diag_matrix, self.skew_matrix)
 
     def forward(self, x1, x2, diag=False, **params):
         # adapted from the Matern kernel
         mean = x1.reshape(-1, x1.size(-1)).mean(0)[(None,) * (x1.dim() - 1)]
 
-        trans_x1 = torch.matmul(self.latent_transform.unsqueeze(1), (x1 - mean).unsqueeze(-1)).squeeze(-1)
-        trans_x2 = torch.matmul(self.latent_transform.unsqueeze(1), (x2 - mean).unsqueeze(-1)).squeeze(-1)
+        transform = self.latent_transform.unsqueeze(1)
+
+        trans_x1 = torch.matmul(transform, (x1 - mean).unsqueeze(-1)).squeeze(-1)
+        trans_x2 = torch.matmul(transform, (x2 - mean).unsqueeze(-1)).squeeze(-1)
 
         distance = self.covar_dist(trans_x1, trans_x2, diag=diag, **params)
 
         if self.num_outputs == 1:
             distance = distance.squeeze(0)
 
         outputscale = self.outputscale if self.scale_output else 1.0
```

### Comparing `bloptools-0.6.1/src/blop/bayesian/models.py` & `bloptools-0.7.0/src/blop/bayesian/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import botorch
 import gpytorch
 import torch
+from botorch.models.gp_regression import SingleTaskGP
 
 from . import kernels
 
 
-class LatentGP(botorch.models.gp_regression.SingleTaskGP):
+class LatentGP(SingleTaskGP):
     def __init__(self, train_inputs, train_targets, skew_dims=True, *args, **kwargs):
         super().__init__(train_inputs, train_targets, *args, **kwargs)
 
         self.mean_module = gpytorch.means.ConstantMean(constant_prior=gpytorch.priors.NormalPrior(loc=0, scale=1))
 
         self.covar_module = kernels.LatentKernel(
             num_inputs=train_inputs.shape[-1],
@@ -19,15 +19,30 @@
             scale=True,
             **kwargs,
         )
 
         self.trained = False
 
 
-class LatentDirichletModel(LatentGP):
+class LatentConstraintModel(LatentGP):
+    def __init__(self, train_inputs, train_targets, skew_dims=True, *args, **kwargs):
+        super().__init__(train_inputs, train_targets, skew_dims, *args, **kwargs)
+
+        self.trained = False
+
+    def fitness(self, x, n_samples=1024):
+        """
+        Takes in a (..., m) dimension tensor and returns a (..., n_classes) tensor
+        """
+        *input_shape, n_dim = x.shape
+        samples = self.posterior(x.reshape(-1, n_dim)).sample(torch.Size((n_samples,))).exp()
+        return (samples / samples.sum(-1, keepdim=True)).mean(0).reshape(*input_shape, -1)
+
+
+class LatentDirichletClassifier(LatentGP):
     def __init__(self, train_inputs, train_targets, skew_dims=True, *args, **kwargs):
         super().__init__(train_inputs, train_targets, skew_dims, *args, **kwargs)
 
         self.trained = False
 
     def probabilities(self, x, n_samples=1024):
         """
```

### Comparing `bloptools-0.6.1/src/blop/bayesian/plotting.py` & `bloptools-0.7.0/src/blop/plotting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import matplotlib as mpl
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.patches import Patch
 
-from . import acquisition
+from .bayesian.acquisition import _construct_acqf, parse_acqf_identifier
 
 DEFAULT_COLOR_LIST = ["dodgerblue", "tomato", "mediumseagreen", "goldenrod"]
-DEFAULT_COLORMAP = "magma"
+# Note: the values near 1 are hard to see on a white background. Turbo goes from red to blue and isn't white in the middle.
+DEFAULT_COLORMAP = "turbo"
 DEFAULT_SCATTER_SIZE = 16
 
 MAX_TEST_INPUTS = 2**11
 
 
-def _plot_objs_one_dof(agent, size=16, lw=1e0):
+def _plot_fitness_objs_one_dof(agent, size=16, lw=1e0):
+    fitness_objs = agent.objectives(kind="fitness")
+
     agent.obj_fig, agent.obj_axes = plt.subplots(
-        len(agent.objectives),
+        len(fitness_objs),
         1,
-        figsize=(6, 4 * len(agent.objectives)),
+        figsize=(6, 4 * len(fitness_objs)),
         sharex=True,
         constrained_layout=True,
     )
 
     agent.obj_axes = np.atleast_1d(agent.obj_axes)
 
-    x_dof = agent.dofs.subset(active=True)[0]
+    x_dof = agent.dofs(active=True)[0]
     x_values = agent.table.loc[:, x_dof.device.name].values
 
-    for obj_index, obj in enumerate(agent.objectives):
+    test_inputs = agent.sample(method="grid")
+    test_model_inputs = agent.dofs(active=True).transform(test_inputs)
+
+    for obj_index, obj in enumerate(fitness_objs):
         obj_values = agent.train_targets(obj.name).squeeze(-1).numpy()
 
         color = DEFAULT_COLOR_LIST[obj_index]
 
         test_inputs = agent.sample(method="grid")
         test_x = test_inputs[..., 0].detach().numpy()
 
-        test_posterior = obj.model.posterior(test_inputs)
+        test_posterior = obj.model.posterior(test_model_inputs)
         test_mean = test_posterior.mean[..., 0].detach().numpy()
         test_sigma = test_posterior.variance.sqrt()[..., 0].detach().numpy()
 
         agent.obj_axes[obj_index].scatter(x_values, obj_values, s=size, color=color)
 
         for z in [0, 1, 2]:
             agent.obj_axes[obj_index].fill_between(
@@ -46,25 +52,88 @@
                 (test_mean - z * test_sigma).ravel(),
                 (test_mean + z * test_sigma).ravel(),
                 lw=lw,
                 color=color,
                 alpha=0.5**z,
             )
 
-        agent.obj_axes[obj_index].set_xlim(*x_dof.search_bounds)
-        agent.obj_axes[obj_index].set_xlabel(x_dof.label)
-        agent.obj_axes[obj_index].set_ylabel(obj.label)
+        agent.obj_axes[obj_index].set_xlim(*x_dof.search_domain)
+        agent.obj_axes[obj_index].set_xlabel(x_dof.label_with_units)
+        agent.obj_axes[obj_index].set_ylabel(obj.label_with_units)
+
+
+def _plot_constraint_objs_one_dof(agent, size=16, lw=1e0):
+    constraint_objs = agent.objectives(kind="constraint")
+
+    agent.obj_fig, agent.obj_axes = plt.subplots(
+        len(constraint_objs),
+        2,
+        figsize=(8, 4 * len(constraint_objs)),
+        sharex=True,
+        constrained_layout=True,
+    )
+
+    agent.obj_axes = np.atleast_2d(agent.obj_axes)
+
+    x_dof = agent.dofs(active=True)[0]
+    x_values = agent.table.loc[:, x_dof.device.name].values
+
+    test_inputs = agent.sample(method="grid")
+    test_model_inputs = agent.dofs(active=True).transform(test_inputs)
+
+    for obj_index, obj in enumerate(constraint_objs):
+        val_ax = agent.obj_axes[obj_index, 0]
+        con_ax = agent.obj_axes[obj_index, 1]
+
+        obj_values = agent.train_targets(obj.name).squeeze(-1).numpy()
+
+        color = DEFAULT_COLOR_LIST[obj_index]
+
+        test_inputs = agent.sample(method="grid")
+        test_x = test_inputs[..., 0].detach().numpy()
+
+        test_posterior = obj.model.posterior(test_model_inputs)
+        test_mean = test_posterior.mean[..., 0].detach().numpy()
+        test_sigma = test_posterior.variance.sqrt()[..., 0].detach().numpy()
+
+        val_ax.scatter(x_values, obj_values, s=size, color=color)
+
+        con_ax.plot(test_x, obj.targeting_constraint(test_model_inputs).detach())
+
+        for z in [0, 1, 2]:
+            val_ax.fill_between(
+                test_x.ravel(),
+                (test_mean - z * test_sigma).ravel(),
+                (test_mean + z * test_sigma).ravel(),
+                lw=lw,
+                color=color,
+                alpha=0.5**z,
+            )
+
+        ymin, ymax = val_ax.get_ylim()
+
+        val_ax.fill_between(
+            test_x.ravel(), y1=np.maximum(obj.target[0], ymin), y2=np.minimum(obj.target[1], ymax), alpha=0.2
+        )
+        val_ax.set_ylim(ymin, ymax)
+
+        con_ax.set_ylabel(r"P(constraint)")
+        val_ax.set_ylabel(obj.label_with_units)
+
+        for ax in [val_ax, con_ax]:
+            ax.set_xlim(*x_dof.search_domain)
+            ax.set_xlabel(x_dof.label_with_units)
 
 
 def _plot_objs_many_dofs(agent, axes=(0, 1), shading="nearest", cmap=DEFAULT_COLORMAP, gridded=None, size=32, grid_zoom=1):
     """
     Axes represents which active, non-read-only axes to plot with
     """
 
-    plottable_dofs = agent.dofs.subset(active=True, read_only=False)
+    plottable_dofs = agent.dofs(active=True, read_only=False)
 
     if gridded is None:
         gridded = len(plottable_dofs) == 2
 
     agent.obj_fig, agent.obj_axes = plt.subplots(
         len(agent.objectives),
         4,
@@ -82,88 +151,146 @@
 
     # test_inputs has shape (*input_shape, 1, n_active_dofs)
     # test_x and test_y should be squeezeable
     test_inputs = agent.sample(method="grid") if gridded else agent.sample(n=1024)
     test_x = test_inputs[..., 0, axes[0]].detach().squeeze().numpy()
     test_y = test_inputs[..., 0, axes[1]].detach().squeeze().numpy()
 
+    model_inputs = agent.dofs(active=True).transform(test_inputs)
+
     for obj_index, obj in enumerate(agent.objectives):
         targets = agent.train_targets(obj.name).squeeze(-1).numpy()
 
-        obj_vmin, obj_vmax = np.nanpercentile(targets, q=[1, 99])
+        values = obj._untransform(targets)
+
+        val_vmin, val_vmax = np.nanquantile(values, q=[0.01, 0.99])
+        val_norm = (
+            mpl.colors.LogNorm(val_vmin, val_vmax) if obj.transform == "log" else mpl.colors.Normalize(val_vmin, val_vmax)
+        )
+
+        obj_vmin, obj_vmax = np.nanquantile(targets, q=[0.01, 0.99])
         obj_norm = mpl.colors.Normalize(obj_vmin, obj_vmax)
 
-        data_ax = agent.obj_axes[obj_index, 0].scatter(x_values, y_values, c=targets, s=size, norm=obj_norm, cmap=cmap)
+        val_ax = agent.obj_axes[obj_index, 0].scatter(x_values, y_values, c=values, s=size, norm=val_norm, cmap=cmap)
 
         # mean and sigma will have shape (*input_shape,)
-        test_posterior = obj.model.posterior(test_inputs)
+        test_posterior = obj.model.posterior(model_inputs)
         test_mean = test_posterior.mean[..., 0, 0].detach().squeeze().numpy()
         test_sigma = test_posterior.variance.sqrt()[..., 0, 0].detach().squeeze().numpy()
 
+        # test_values = obj.fitness_inverse(test_mean) if obj.kind == "fitness" else test_mean
+
+        test_constraint = None
+        if not obj.kind == "fitness":
+            test_constraint = obj.targeting_constraint(model_inputs).detach().squeeze().numpy()
+
         if gridded:
-            _ = agent.obj_axes[obj_index, 1].pcolormesh(
-                test_x,
-                test_y,
-                test_mean,
-                shading=shading,
-                cmap=cmap,
-                norm=obj_norm,
-            )
-            sigma_ax = agent.obj_axes[obj_index, 2].pcolormesh(
-                test_x,
-                test_y,
-                test_sigma,
-                shading=shading,
-                cmap=cmap,
-                norm=mpl.colors.LogNorm(),
-            )
+            # _ = agent.obj_axes[obj_index, 1].pcolormesh(
+            #     test_x,
+            #     test_y,
+            #     test_values,
+            #     shading=shading,
+            #     cmap=cmap,
+            #     norm=val_norm,
+            # )
+            if obj.kind == "fitness":
+                fitness_ax = agent.obj_axes[obj_index, 1].pcolormesh(
+                    test_x,
+                    test_y,
+                    test_mean,
+                    shading=shading,
+                    cmap=cmap,
+                    norm=obj_norm,
+                )
+                fit_err_ax = agent.obj_axes[obj_index, 2].pcolormesh(
+                    test_x,
+                    test_y,
+                    test_sigma,
+                    shading=shading,
+                    cmap=cmap,
+                    norm=mpl.colors.LogNorm(),
+                )
+
+            if test_constraint is not None:
+                constraint_ax = agent.obj_axes[obj_index, 3].pcolormesh(
+                    test_x,
+                    test_y,
+                    test_constraint,
+                    shading=shading,
+                    cmap=cmap,
+                    # norm=mpl.colors.LogNorm(),
+                )
 
         else:
-            _ = agent.obj_axes[obj_index, 1].scatter(
-                test_x,
-                test_y,
-                c=test_mean,
-                s=size,
-                norm=obj_norm,
-                cmap=cmap,
-            )
-            sigma_ax = agent.obj_axes[obj_index, 2].scatter(
-                test_x,
-                test_y,
-                c=test_sigma,
-                s=size,
-                cmap=cmap,
-                norm=mpl.colors.LogNorm(),
+            # _ = agent.obj_axes[obj_index, 1].scatter(
+            #     test_x,
+            #     test_y,
+            #     c=test_values,
+            #     s=size,
+            #     norm=val_norm,
+            #     cmap=cmap,
+            # )
+            if obj.kind == "fitness":
+                fitness_ax = agent.obj_axes[obj_index, 1].scatter(
+                    test_x,
+                    test_y,
+                    c=test_mean,
+                    s=size,
+                    norm=obj_norm,
+                    cmap=cmap,
+                )
+                fit_err_ax = agent.obj_axes[obj_index, 2].scatter(
+                    test_x,
+                    test_y,
+                    c=test_sigma,
+                    s=size,
+                    cmap=cmap,
+                    norm=mpl.colors.LogNorm(),
+                )
+
+            if test_constraint is not None:
+                constraint_ax = agent.obj_axes[obj_index, 3].scatter(
+                    test_x,
+                    test_y,
+                    c=test_constraint,
+                    s=size,
+                    cmap=cmap,
+                    norm=mpl.colors.LogNorm(),
+                )
+
+        val_cbar = agent.obj_fig.colorbar(val_ax, ax=agent.obj_axes[obj_index, 0], location="bottom", aspect=32, shrink=0.8)
+        val_cbar.set_label(f"{obj.units or ''}")
+
+        if obj.kind == "fitness":
+            _ = agent.obj_fig.colorbar(fitness_ax, ax=agent.obj_axes[obj_index, 1], location="bottom", aspect=32, shrink=0.8)
+            _ = agent.obj_fig.colorbar(fit_err_ax, ax=agent.obj_axes[obj_index, 2], location="bottom", aspect=32, shrink=0.8)
+
+            # obj_cbar.set_label(f"{obj.label}")
+            # err_cbar.set_label(f"{obj.label}")
+
+        if test_constraint is not None:
+            constraint_cbar = agent.obj_fig.colorbar(
+                constraint_ax, ax=agent.obj_axes[obj_index, 3], location="bottom", aspect=32, shrink=0.8
             )
 
-        obj_cbar = agent.obj_fig.colorbar(
-            data_ax, ax=agent.obj_axes[obj_index, :2], location="bottom", aspect=32, shrink=0.8
-        )
-        err_cbar = agent.obj_fig.colorbar(
-            sigma_ax, ax=agent.obj_axes[obj_index, 2], location="bottom", aspect=32, shrink=0.8
-        )
-        obj_cbar.set_label(obj.label)
-        err_cbar.set_label(f"{obj.label} error")
+            constraint_cbar.set_label(f"{obj.label_with_units} constraint")
 
-    col_names = ["samples", "posterior mean", "posterior std. dev.", "fitness"]
-
-    pad = 5
-
-    for column_index, ax in enumerate(agent.obj_axes[0]):
-        ax.annotate(
-            col_names[column_index],
-            xy=(0.5, 1),
-            xytext=(0, pad),
-            color="k",
-            xycoords="axes fraction",
-            textcoords="offset points",
-            size="large",
-            ha="center",
-            va="baseline",
-        )
+        col_names = [
+            f"{obj.description} samples",
+            f"pred. {obj.description} fitness",
+            f"pred. {obj.description} fitness error",
+            f"{obj.description} constraint",
+        ]
+
+        pad = 5
+
+        for column_index, ax in enumerate(agent.obj_axes[obj_index]):
+            ax.set_title(
+                col_names[column_index],
+            )
 
     if len(agent.objectives) > 1:
         for row_index, ax in enumerate(agent.obj_axes[:, 0]):
             ax.annotate(
                 agent.objectives[row_index].name,
                 xy=(0, 0.5),
                 xytext=(-ax.yaxis.labelpad - pad, 0),
@@ -173,146 +300,151 @@
                 size="large",
                 ha="right",
                 va="center",
                 rotation=90,
             )
 
     for ax in agent.obj_axes.ravel():
-        ax.set_xlabel(x_dof.label)
-        ax.set_ylabel(y_dof.label)
-        ax.set_xlim(*x_dof.search_bounds)
-        ax.set_ylim(*y_dof.search_bounds)
-        if x_dof.log:
+        ax.set_xlabel(x_dof.label_with_units)
+        ax.set_ylabel(y_dof.label_with_units)
+        ax.set_xlim(*x_dof.search_domain)
+        ax.set_ylim(*y_dof.search_domain)
+        if x_dof.transform == "log":
             ax.set_xscale("log")
-        if y_dof.log:
+        if y_dof.transform == "log":
             ax.set_yscale("log")
 
 
-def _plot_acqf_one_dof(agent, acq_funcs, lw=1e0, **kwargs):
+def _plot_acqf_one_dof(agent, acqfs, lw=1e0, **kwargs):
     agent.acq_fig, agent.acq_axes = plt.subplots(
         1,
-        len(acq_funcs),
-        figsize=(4 * len(acq_funcs), 4),
+        len(acqfs),
+        figsize=(4 * len(acqfs), 4),
         sharex=True,
         constrained_layout=True,
     )
 
     agent.acq_axes = np.atleast_1d(agent.acq_axes)
-    x_dof = agent.dofs.subset(active=True)[0]
+    x_dof = agent.dofs(active=True)[0]
 
     test_inputs = agent.sample(method="grid")
+    model_inputs = agent.dofs.transform(test_inputs)
+
+    for iacqf, acqf_identifier in enumerate(acqfs):
+        color = DEFAULT_COLOR_LIST[iacqf]
 
-    for iacq_func, acq_func_identifier in enumerate(acq_funcs):
-        color = DEFAULT_COLOR_LIST[iacq_func]
+        acqf_config = parse_acqf_identifier(acqf_identifier)
+        acqf, _ = _construct_acqf(agent, acqf_config["name"])
 
-        acq_func, acq_func_meta = acquisition.get_acquisition_function(agent, acq_func_identifier)
-        test_acqf = acq_func(test_inputs).detach().numpy()
+        test_acqf_value = acqf(model_inputs).detach().numpy()
 
-        agent.acq_axes[iacq_func].plot(test_inputs.squeeze(-2), test_acqf, lw=lw, color=color)
+        agent.acq_axes[iacqf].plot(test_inputs.squeeze(-2), test_acqf_value, lw=lw, color=color)
 
-        agent.acq_axes[iacq_func].set_xlim(*x_dof.search_bounds)
-        agent.acq_axes[iacq_func].set_xlabel(x_dof.label)
-        agent.acq_axes[iacq_func].set_ylabel(acq_func_meta["name"])
+        agent.acq_axes[iacqf].set_xlim(*x_dof.search_domain)
+        agent.acq_axes[iacqf].set_xlabel(x_dof.label_with_units)
+        agent.acq_axes[iacqf].set_ylabel(acqf_config["name"])
 
 
 def _plot_acqf_many_dofs(
-    agent, acq_funcs, axes=[0, 1], shading="nearest", cmap=DEFAULT_COLORMAP, gridded=None, size=16, **kwargs
+    agent, acqfs, axes=[0, 1], shading="nearest", cmap=DEFAULT_COLORMAP, gridded=None, size=16, **kwargs
 ):
     agent.acq_fig, agent.acq_axes = plt.subplots(
         1,
-        len(acq_funcs),
-        figsize=(4 * len(acq_funcs), 4),
+        len(acqfs),
+        figsize=(4 * len(acqfs), 4),
         sharex=True,
         sharey=True,
         constrained_layout=True,
     )
 
-    plottable_dofs = agent.dofs.subset(active=True, read_only=False)
+    plottable_dofs = agent.dofs(active=True, read_only=False)
 
     if gridded is None:
         gridded = len(plottable_dofs) == 2
 
     agent.acq_axes = np.atleast_1d(agent.acq_axes)
 
     x_dof, y_dof = plottable_dofs[axes[0]], plottable_dofs[axes[1]]
 
     # test_inputs has shape (..., 1, n_active_dofs)
     test_inputs = agent.sample(n=1024, method="grid") if gridded else agent.sample(n=1024)
+    model_inputs = agent.dofs.transform(test_inputs)
     *test_dim, input_dim = test_inputs.shape
     test_x = test_inputs[..., 0, axes[0]].detach().squeeze().numpy()
     test_y = test_inputs[..., 0, axes[1]].detach().squeeze().numpy()
 
-    for iacq_func, acq_func_identifier in enumerate(acq_funcs):
-        acq_func, acq_func_meta = acquisition.get_acquisition_function(agent, acq_func_identifier)
+    for iacqf, acqf_identifier in enumerate(acqfs):
+        acqf_config = parse_acqf_identifier(acqf_identifier)
+        acqf, _ = _construct_acqf(agent, acqf_config["name"])
 
-        test_acqf = acq_func(test_inputs.reshape(-1, 1, input_dim)).detach().reshape(test_dim).squeeze().numpy()
+        test_acqf_value = acqf(model_inputs.reshape(-1, 1, input_dim)).detach().reshape(test_dim).squeeze().numpy()
 
         if gridded:
-            agent.acq_axes[iacq_func].set_title(acq_func_meta["name"])
-            obj_ax = agent.acq_axes[iacq_func].pcolormesh(
+            agent.acq_axes[iacqf].set_title(acqf_config["name"])
+            obj_ax = agent.acq_axes[iacqf].pcolormesh(
                 test_x,
                 test_y,
-                test_acqf,
+                test_acqf_value,
                 shading=shading,
                 cmap=cmap,
             )
 
-            agent.acq_fig.colorbar(obj_ax, ax=agent.acq_axes[iacq_func], location="bottom", aspect=32, shrink=0.8)
+            agent.acq_fig.colorbar(obj_ax, ax=agent.acq_axes[iacqf], location="bottom", aspect=32, shrink=0.8)
 
         else:
-            agent.acq_axes[iacq_func].set_title(acq_func_meta["name"])
-            obj_ax = agent.acq_axes[iacq_func].scatter(
+            agent.acq_axes[iacqf].set_title(acqf_config["name"])
+            obj_ax = agent.acq_axes[iacqf].scatter(
                 test_x,
                 test_y,
-                c=test_acqf,
+                c=test_acqf_value,
             )
 
-            agent.acq_fig.colorbar(obj_ax, ax=agent.acq_axes[iacq_func], location="bottom", aspect=32, shrink=0.8)
+            agent.acq_fig.colorbar(obj_ax, ax=agent.acq_axes[iacqf], location="bottom", aspect=32, shrink=0.8)
 
     for ax in agent.acq_axes.ravel():
-        ax.set_xlabel(x_dof.label)
-        ax.set_ylabel(y_dof.label)
-        ax.set_xlim(*x_dof.search_bounds)
-        ax.set_ylim(*y_dof.search_bounds)
-        if x_dof.log:
+        ax.set_xlabel(x_dof.label_with_units)
+        ax.set_ylabel(y_dof.label_with_units)
+        ax.set_xlim(*x_dof.search_domain)
+        ax.set_ylim(*y_dof.search_domain)
+        if x_dof.transform == "log":
             ax.set_xscale("log")
-        if y_dof.log:
+        if y_dof.transform == "log":
             ax.set_yscale("log")
 
 
 def _plot_valid_one_dof(agent, size=16, lw=1e0):
     agent.valid_fig, agent.valid_ax = plt.subplots(1, 1, figsize=(6, 4 * len(agent.objectives)), constrained_layout=True)
 
-    x_dof = agent.dofs.subset(active=True)[0]
+    x_dof = agent.dofs(active=True)[0]
     x_values = agent.table.loc[:, x_dof.device.name].values
 
     test_inputs = agent.sample(method="grid")
-    constraint = agent.constraint(test_inputs)[..., 0]
+    constraint = agent.constraint(agent.dofs.transform(test_inputs))[..., 0]
 
     agent.valid_ax.scatter(x_values, agent.all_objectives_valid, s=size)
     agent.valid_ax.plot(test_inputs.squeeze(-2), constraint, lw=lw)
-    agent.valid_ax.set_xlim(*x_dof.search_bounds)
+    agent.valid_ax.set_xlim(*x_dof.search_domain)
 
 
 def _plot_valid_many_dofs(agent, axes=[0, 1], shading="nearest", cmap=DEFAULT_COLORMAP, size=16, gridded=None):
     agent.valid_fig, agent.valid_axes = plt.subplots(1, 2, figsize=(8, 4), constrained_layout=True)
 
-    plottable_dofs = agent.dofs.subset(active=True, read_only=False)
+    plottable_dofs = agent.dofs(active=True, read_only=False)
 
     if gridded is None:
         gridded = len(plottable_dofs) == 2
 
     x_dof, y_dof = plottable_dofs[axes[0]], plottable_dofs[axes[1]]
 
     # test_inputs has shape (..., 1, n_active_dofs)
     test_inputs = agent.sample(method="grid") if gridded else agent.sample(n=1024)
     test_x = test_inputs[..., 0, axes[0]].detach().squeeze().numpy()
     test_y = test_inputs[..., 0, axes[1]].detach().squeeze().numpy()
 
-    constraint = agent.constraint(test_inputs)[..., 0].squeeze().numpy()
+    constraint = agent.constraint(agent.dofs.transform(test_inputs))[..., 0].squeeze().numpy()
 
     if gridded:
         _ = agent.valid_axes[1].pcolormesh(
             test_x,
             test_y,
             constraint,
             shading=shading,
@@ -329,21 +461,21 @@
             s=size,
             cmap=cmap,
             vmin=0,
             vmax=0,
         )
 
     for ax in agent.valid_axes.ravel():
-        ax.set_xlabel(x_dof.label)
-        ax.set_ylabel(y_dof.label)
-        ax.set_xlim(*x_dof.search_bounds)
-        ax.set_ylim(*y_dof.search_bounds)
-        if x_dof.log:
+        ax.set_xlabel(x_dof.label_with_units)
+        ax.set_ylabel(y_dof.label_with_units)
+        ax.set_xlim(*x_dof.search_domain)
+        ax.set_ylim(*y_dof.search_domain)
+        if x_dof.transform == "log":
             ax.set_xscale("log")
-        if y_dof.log:
+        if y_dof.transform == "log":
             ax.set_yscale("log")
 
 
 def _plot_history(agent, x_key="index", show_all_objs=False):
     x = getattr(agent.table, x_key).values
 
     num_obj_plots = 1
@@ -353,42 +485,40 @@
     len(agent.objectives) + 1 if len(agent.objectives) > 1 else 1
 
     hist_fig, hist_axes = plt.subplots(
         num_obj_plots, 1, figsize=(6, 4 * num_obj_plots), sharex=True, constrained_layout=True, dpi=200
     )
     hist_axes = np.atleast_1d(hist_axes)
 
-    unique_strategies, acq_func_index, acq_func_inverse = np.unique(
-        agent.table.acq_func, return_index=True, return_inverse=True
-    )
+    unique_strategies, acqf_index, acqf_inverse = np.unique(agent.table.acqf, return_index=True, return_inverse=True)
 
-    sample_colors = np.array(DEFAULT_COLOR_LIST)[acq_func_inverse]
+    sample_colors = np.array(DEFAULT_COLOR_LIST)[acqf_inverse]
 
     if show_all_objs:
         for obj_index, obj in enumerate(agent.objectives):
             y = agent.table.loc[:, f"{obj.key}_fitness"].values
             hist_axes[obj_index].scatter(x, y, c=sample_colors)
             hist_axes[obj_index].plot(x, y, lw=5e-1, c="k")
             hist_axes[obj_index].set_ylabel(obj.key)
 
-    y = agent.scalarized_objectives
+    y = agent.scalarized_fitnesses()
 
     cummax_y = np.array([np.nanmax(y[: i + 1]) for i in range(len(y))])
 
     hist_axes[-1].scatter(x, y, c=sample_colors)
     hist_axes[-1].plot(x, y, lw=5e-1, c="k")
 
     hist_axes[-1].plot(x, cummax_y, lw=5e-1, c="k", ls=":")
 
     hist_axes[-1].set_ylabel("total_fitness")
     hist_axes[-1].set_xlabel(x_key)
 
     handles = []
-    for i_acq_func, acq_func in enumerate(unique_strategies):
-        handles.append(Patch(color=DEFAULT_COLOR_LIST[i_acq_func], label=acq_func))
+    for i_acqf, acqf in enumerate(unique_strategies):
+        handles.append(Patch(color=DEFAULT_COLOR_LIST[i_acqf], label=acqf))
     legend = hist_axes[0].legend(handles=handles, fontsize=8)
     legend.set_title("acquisition function")
 
 
 def inspect_beam(agent, index, border=None):
     im = agent.images[index]
 
@@ -402,7 +532,31 @@
     plt.figure()
     plt.imshow(im, cmap="gray_r")
     plt.plot(bbx, bby, lw=4e0, c="r")
 
     if border is not None:
         plt.xlim(x_min - border * width_x, x_min + border * width_x)
         plt.ylim(y_min - border * width_y, y_min + border * width_y)
+
+
+def _plot_pareto_front(agent, obj_indices=(0, 1)):
+    f_objs = agent.objectives(kind="fitness")
+    (i, j) = obj_indices
+
+    if len(f_objs) < 2:
+        raise ValueError("Cannot plot Pareto front for agents with fewer than two fitness objectives")
+
+    fig, ax = plt.subplots(1, 1, figsize=(6, 6))
+
+    y = agent.train_targets(kind="fitness")
+
+    pareto_mask = agent.pareto_mask
+    constraint = agent.evaluated_constraints.all(axis=-1)
+
+    ax.scatter(*y[(~pareto_mask) & constraint].T[[i, j]], c="k")
+    ax.scatter(*y[~constraint].T[[i, j]], c="r", marker="x", label="invalid")
+    ax.scatter(*y[pareto_mask].T[[i, j]], c="b", label="Pareto front")
+
+    ax.set_xlabel(f"{f_objs[i].name} fitness")
+    ax.set_ylabel(f"{f_objs[j].name} fitness")
+
+    ax.legend()
```

### Comparing `bloptools-0.6.1/src/blop/bayesian/acquisition/analytic.py` & `bloptools-0.7.0/src/blop/bayesian/acquisition/analytic.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/src/blop/bayesian/acquisition/config.yml` & `bloptools-0.7.0/src/blop/bayesian/acquisition/config.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,101 @@
 expected_improvement:
   pretty_name: Expected improvement
   description: The expected value of max(f(x) - \nu, 0), where \nu is the current maximum.
-  identifiers:
-  - ei
+  identifier: ei
   multitask_only: false
   type: analytic
 
 monte_carlo_expected_improvement:
   description: The expected value of max(f(x) - \nu, 0), where \nu is the current maximum.
-  identifiers:
-  - qei
+  identifier: qei
   multitask_only: false
   pretty_name: Monte Carlo Expected improvement
   type: monte_carlo
 
 expected_mean:
   description: The expected value at each input.
-  identifiers:
-  - em
+  identifier: em
   multitask_only: false
   pretty_name: Expected mean
   type: analytic
 
 monte_carlo_expected_mean:
   description: The expected value at each input.
-  identifiers:
-  - qem
+  identifier: qem
   multitask_only: false
   pretty_name: Monte Carlo expected mean
   type: monte_carlo
 
 lower_bound_max_value_entropy:
   description: Max entropy search, basically
-  identifiers:
-  - lbmve
-  - lbmes
-  - gibbon
+  identifier: lbmve
   multitask_only: false
   pretty_name: Lower bound max value entropy
   type: monte_carlo
 
 noisy_expected_hypervolume_improvement:
   description: It's like a big box. How big is the box?
-  identifiers:
-  - nehvi
+  identifier: nehvi
   multitask_only: true
   pretty_name: Noisy expected hypervolume improvement
   type: analytic
 
+monte_carlo_noisy_expected_hypervolume_improvement:
+  description: It's like a big box. How big is the box?
+  identifier: qnehvi
+  multitask_only: true
+  pretty_name: Noisy expected hypervolume improvement
+  type: monte_carlo
+
 probability_of_improvement:
   description: The probability that this input improves on the current maximum.
-  identifiers:
-  - pi
+  identifier: pi
   multitask_only: false
   pretty_name: Probability of improvement
   type: analytic
 
 monte_carlo_probability_of_improvement:
   description: The probability that this input improves on the current maximum.
-  identifiers:
-  - qpi
+  identifier: qpi
   multitask_only: false
   pretty_name: Monte Carlo probability of improvement
   type: monte_carlo
 
 random:
   description: Uniformly-sampled random points.
-  identifiers:
-  - r
+  identifier: r
   multitask_only: false
   pretty_name: Random
-  type: none
+  type: random
 
 quasi-random:
   description: Sobol-sampled quasi-random points.
-  identifiers:
-  - qr
+  identifier: qr
   multitask_only: false
   pretty_name: Quasi-random
-  type: none
+  type: random
 
 grid:
   description: A grid scan over the parameters.
-  identifiers:
-  - g
-  - gs
+  identifier: g
   multitask_only: false
   pretty_name: Grid scan
-  type: none
+  type: random
 
 upper_confidence_bound:
-  default_args:
+  default_kwargs:
     beta: 4
   description: The expected value, plus some multiple of the uncertainty (typically \mu + 2\sigma).
-  identifiers:
-  - ucb
+  identifier: ucb
   multitask_only: false
   pretty_name: Upper confidence bound
   type: analytic
 
 monte_carlo_upper_confidence_bound:
-  default_args:
+  default_kwargs:
     beta: 4
   description: The expected value, plus some multiple of the uncertainty (typically \mu + 2\sigma).
-  identifiers:
-  - qucb
+  identifier: qucb
   multitask_only: false
   pretty_name: Monte Carlo upper confidence bound
   type: monte_carlo
```

### Comparing `bloptools-0.6.1/src/blop/bayesian/acquisition/monte_carlo.py` & `bloptools-0.7.0/src/blop/bayesian/acquisition/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/src/blop/de/de_opt_utils.py` & `bloptools-0.7.0/src/blop/de/de_opt_utils.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/src/blop/de/de_optimization.py` & `bloptools-0.7.0/src/blop/de/de_optimization.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/src/blop/de/hardware_flyer.py` & `bloptools-0.7.0/src/blop/de/hardware_flyer.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/src/blop/utils/__init__.py` & `bloptools-0.7.0/src/blop/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import botorch
 import numpy as np
 import scipy as sp
 import torch
 from ortools.constraint_solver import pywrapcp, routing_enums_pb2
 
 
-def cummax(x):
-    return [np.nanmax(x[: i + 1]) for i in range(len(np.atleast_1d(x)))]
-
-
 def sobol_sampler(bounds, n, q=1):
     """
     Returns $n$ quasi-randomly sampled points within the bounds (a 2 by d tensor)
     and batch size $q$
     """
     return botorch.utils.sampling.draw_sobol_samples(bounds, n=n, q=q)
```

### Comparing `bloptools-0.6.1/src/blop/utils/misc.py` & `bloptools-0.7.0/src/blop/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import botorch
 import numpy as np
 import scipy as sp
 import torch
 from ortools.constraint_solver import pywrapcp, routing_enums_pb2
 
 
+def cummax(x):
+    return [np.nanmax(x[: i + 1]) for i in range(len(np.atleast_1d(x)))]
+
+
 def sobol_sampler(bounds, n, q=1):
     """
     Returns $n$ quasi-randomly sampled points within the bounds (a 2 by d tensor)
     and batch size $q$
     """
     return botorch.utils.sampling.draw_sobol_samples(bounds, n=n, q=q)
 
@@ -40,29 +44,29 @@
 def mprod(*M):
     res = M[0]
     for m in M[1:]:
         res = np.matmul(res, m)
     return res
 
 
-def route(start_point, points):
+def route(start_point, points, dim_weights=1):
     """
     Returns the indices of the most efficient way to visit `points`, starting from `start_point`.
     """
 
     total_points = np.r_[np.atleast_2d(start_point), points]
     points_scale = total_points.ptp(axis=0)
     dim_mask = points_scale > 0
 
     if dim_mask.sum() == 0:
         return np.arange(len(points))
 
-    normalized_points = (total_points - total_points.min(axis=0))[:, dim_mask] / points_scale[dim_mask]
+    scaled_points = (total_points - total_points.min(axis=0)) * (dim_weights / np.where(points_scale > 0, points_scale, 1))
 
-    delay_matrix = np.sqrt(np.square(normalized_points[:, None, :] - normalized_points[None, :, :]).sum(axis=-1))
+    delay_matrix = np.sqrt(np.square(scaled_points[:, None, :] - scaled_points[None, :, :]).sum(axis=-1))
     delay_matrix = (1e4 * delay_matrix).astype(int)  # it likes integers idk
 
     manager = pywrapcp.RoutingIndexManager(len(total_points), 1, 0)  # number of depots, number of salesmen, starting index
     routing = pywrapcp.RoutingModel(manager)
 
     def delay_callback(from_index, to_index):
         to_node = manager.IndexToNode(to_index)
```

### Comparing `bloptools-0.6.1/src/blop/utils/prepare_re_env.py` & `bloptools-0.7.0/src/blop/utils/prepare_re_env.py`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/.gitignore` & `bloptools-0.7.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-blop/_version.py
+# setuptools_scm
+src/*/_version.py
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `bloptools-0.6.1/LICENSE` & `bloptools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloptools-0.6.1/pyproject.toml` & `bloptools-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     "matplotlib",
     "numpy",
     "ophyd",
     "ortools",
     "scipy",
     "tables",
     "torch",
-    "zict<3.0.0",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.9",
@@ -48,14 +47,18 @@
     "sirepo-bluesky"
 ]
 
 napari = [
     "napari"
 ]
 
+gui = [
+    "nicegui"
+]
+
 dev = [
     "black",
     "pytest-codecov",
     "coverage",
     "flake8",
     "furo",
     "isort",
```

### Comparing `bloptools-0.6.1/PKG-INFO` & `bloptools-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bloptools
-Version: 0.6.1
+Version: 0.7.0
 Summary: Beamline optimization with machine learning
 Project-URL: Homepage, https://github.com/NSLS-II/blop
 Project-URL: Documentation, https://nsls-ii.github.io/blop
 Project-URL: Bug Reports, https://github.com/NSLS-II/blop/issues
 Author-email: Brookhaven National Laboratory <tmorris@bnl.gov>
 Maintainer-email: Brookhaven National Laboratory <tmorris@bnl.gov>
 License-File: LICENSE
@@ -24,15 +24,14 @@
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: ophyd
 Requires-Dist: ortools
 Requires-Dist: scipy
 Requires-Dist: tables
 Requires-Dist: torch
-Requires-Dist: zict<3.0.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: furo; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
@@ -46,14 +45,16 @@
 Requires-Dist: pre-commit-hooks; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-codecov; extra == 'dev'
 Requires-Dist: sphinx; extra == 'dev'
 Requires-Dist: sphinx-copybutton; extra == 'dev'
 Requires-Dist: sphinx-rtd-theme; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
+Provides-Extra: gui
+Requires-Dist: nicegui; extra == 'gui'
 Provides-Extra: napari
 Requires-Dist: napari; extra == 'napari'
 Provides-Extra: sirepo
 Requires-Dist: sirepo-bluesky; extra == 'sirepo'
 Description-Content-Type: text/x-rst
 
 =========
```

