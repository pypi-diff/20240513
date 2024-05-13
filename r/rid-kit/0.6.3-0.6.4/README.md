# Comparing `tmp/rid-kit-0.6.3.tar.gz` & `tmp/rid-kit-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rid-kit-0.6.3.tar", last modified: Mon May 13 08:39:23 2024, max compression
+gzip compressed data, was "rid-kit-0.6.4.tar", last modified: Mon May 13 08:54:37 2024, max compression
```

## Comparing `rid-kit-0.6.3.tar` & `rid-kit-0.6.4.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.265521 rid-kit-0.6.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/.eggs/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.229522 rid-kit-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.github/workflows/pipy_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-13 08:39:17.000000 rid-kit-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-13 08:39:23.265521 rid-kit-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-13 08:39:17.000000 rid-kit-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/docs/.eggs/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/.eggs/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (127)   567861 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/pics/mcmc_ala_1cv.png
--rw-r--r--   0 runner    (1001) docker     (127)   738823 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/pics/mcmc_ala_2cv.png
--rw-r--r--   0 runner    (1001) docker     (127)   639421 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/pics/rid_workflow.jpg
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/_static/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (127)     2693 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/install_dp.md
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/mcmc_configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/prepare_files.md
--rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/rid_configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/rid_download.md
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/rid_machine.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/source/troubleshooting/
--rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/minikube.md
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/submit.md
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/examples/JSON/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/JSON/rid.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3448 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/install-linux-cn.sh
--rw-r--r--   0 runner    (1001) docker     (127)    49439 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/quick-start-postgres-stable-cn.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    25032 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/install/
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/DeePFE.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/gmx_exploration.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/gmx_plumed.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/gmx_tf.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/lmp_exploration_dp.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/tf_cpu.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/tf_gpu.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 08:39:17.000000 rid-kit-0.6.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/common/gromacs/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/gmx_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/mdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/trjconv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/common/lammps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/lammps/command.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/lammps/lmp_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/mol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/mol_dpdata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/common/plumed/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/check_plumed.py
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/make_plumed.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/plumed_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/common/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/sampler/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/common/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/tensorflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/redim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/relabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/reredim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/resubmit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/flow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/flow/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/mcmc/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.249522 rid-kit-0.6.3/rid/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/train_net.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.249522 rid-kit-0.6.3/rid/op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/adjust_trust_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/label_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/mcmc_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/mcmc_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_rid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_model_devi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.249522 rid-kit-0.6.3/rid/select/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/conf_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/model_devi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/superop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27192 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10888 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/exploration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11594 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/mcmc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12664 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/task/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/template/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5900 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_bohrium.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     5116 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_bohrium_k8s.json
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_bohrium_k8s_mcmc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_local_k8s.json
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_k8s.json
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_k8s_mcmc.json
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_local.json
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_local_mcmc.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     1999 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_custom.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     2026 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_dih.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     2031 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_dis.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     1505 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_lmp_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     3013 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_lmp_gmx_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_mcmc_cv_dih.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_mcmc_cv_dis.json
--rwxr-xr-x   0 runner    (1001) docker     (127)     1160 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_mcmc_path.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/tools/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.257521 rid-kit-0.6.3/rid/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/set_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.257521 rid-kit-0.6.3/rid_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:39:23.265521 rid-kit-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 08:39:19.000000 rid-kit-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.257521 rid-kit-0.6.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/000/
--rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/000/conf.gro
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/000/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/001/
--rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/001/conf.gro
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/001/plumed.dat
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/001/topol.top
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/centers.out
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/cls_sel.ndx
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/cls_sel.out
--rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/conf.gro
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/cv_forces.out
--rwxr-xr-x   0 runner    (1001) docker     (127)        7 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/kappa.out
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/models/
--rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_000.pb
--rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_001.pb
--rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_002.pb
--rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_003.pb
--rwxr-xr-x   0 runner    (1001) docker     (127)     4238 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/plm.out
--rwxr-xr-x   0 runner    (1001) docker     (127)    15119 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/plm_label.out
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/plumed.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)     1493 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/rid.json
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/topol.top
--rw-r--r--   0 runner    (1001) docker     (127)   217160 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/traj_comp.xtc
--rwxr-xr-x   0 runner    (1001) docker     (127)    12799 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/mocked_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.265521 rid-kit-0.6.3/tests/op/
--rwxr-xr-x   0 runner    (1001) docker     (127)      113 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/context.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1470 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_adjust_trust_l.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2507 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_rid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_select.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      874 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4405 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6897 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_init-block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_iter-block.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6882 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.736698 rid-kit-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.708698 rid-kit-0.6.4/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:54:32.000000 rid-kit-0.6.4/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.700698 rid-kit-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.708698 rid-kit-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 08:54:32.000000 rid-kit-0.6.4/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 08:54:32.000000 rid-kit-0.6.4/.github/workflows/pipy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 08:54:32.000000 rid-kit-0.6.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 08:54:32.000000 rid-kit-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-13 08:54:32.000000 rid-kit-0.6.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-13 08:54:32.000000 rid-kit-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-13 08:54:37.736698 rid-kit-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-13 08:54:32.000000 rid-kit-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.708698 rid-kit-0.6.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.708698 rid-kit-0.6.4/docs/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/.eggs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.708698 rid-kit-0.6.4/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)   567861 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/pics/mcmc_ala_1cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)   738823 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/pics/mcmc_ala_2cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)   639421 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/pics/rid_workflow.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.712698 rid-kit-0.6.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.712698 rid-kit-0.6.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/_static/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2693 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/install_dp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/mcmc_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/prepare_files.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/rid_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/rid_download.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/rid_machine.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.712698 rid-kit-0.6.4/docs/source/troubleshooting/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/troubleshooting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/troubleshooting/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/troubleshooting/minikube.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/troubleshooting/submit.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-13 08:54:32.000000 rid-kit-0.6.4/docs/source/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.712698 rid-kit-0.6.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.712698 rid-kit-0.6.4/examples/JSON/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 08:54:32.000000 rid-kit-0.6.4/examples/JSON/rid.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3448 2024-05-13 08:54:32.000000 rid-kit-0.6.4/examples/install-linux-cn.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    49439 2024-05-13 08:54:32.000000 rid-kit-0.6.4/examples/quick-start-postgres-stable-cn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    25032 2024-05-13 08:54:32.000000 rid-kit-0.6.4/examples/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/DeePFE.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/gmx_exploration.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/gmx_plumed.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/gmx_tf.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/lmp_exploration_dp.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/tf_cpu.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 08:54:32.000000 rid-kit-0.6.4/install/tf_gpu.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 08:54:32.000000 rid-kit-0.6.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/common/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/gromacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/gromacs/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/gromacs/gmx_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/gromacs/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/gromacs/trjconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/common/lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/lammps/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/lammps/lmp_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/mol_dpdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/common/plumed/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/plumed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/plumed/check_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/plumed/make_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/plumed/plumed_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/common/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/sampler/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.716698 rid-kit-0.6.4/rid/common/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/common/tensorflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.720698 rid-kit-0.6.4/rid/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/redim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/relabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/reredim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/entrypoint/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.720698 rid-kit-0.6.4/rid/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/flow/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.720698 rid-kit-0.6.4/rid/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/mcmc/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.720698 rid-kit-0.6.4/rid/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/nn/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/nn/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/nn/train_net.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.724698 rid-kit-0.6.4/rid/op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/adjust_trust_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/label_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/mcmc_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/mcmc_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/prep_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/prep_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/prep_rid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/prep_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/run_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/run_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/run_model_devi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/run_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/op/run_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.724698 rid-kit-0.6.4/rid/select/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/select/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/select/conf_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/select/model_devi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.724698 rid-kit-0.6.4/rid/superop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27192 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10888 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/exploration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11594 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/mcmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12664 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/superop/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.724698 rid-kit-0.6.4/rid/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/task/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.728698 rid-kit-0.6.4/rid/template/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5900 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_bohrium.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5116 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_bohrium_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_bohrium_k8s_mcmc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_local_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_slurm_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_slurm_k8s_mcmc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_slurm_local.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/machine_slurm_local_mcmc.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1999 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_gmx_custom.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2026 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_gmx_dih.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2031 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_gmx_dis.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_gmx_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1505 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_lmp_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3013 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_lmp_gmx_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_mcmc_cv_dih.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_mcmc_cv_dis.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1160 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/template/rid_mcmc_path.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.728698 rid-kit-0.6.4/rid/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/tools/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.728698 rid-kit-0.6.4/rid/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 08:54:32.000000 rid-kit-0.6.4/rid/utils/set_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.728698 rid-kit-0.6.4/rid_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-13 08:54:37.000000 rid-kit-0.6.4/rid_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-13 08:54:37.000000 rid-kit-0.6.4/rid_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:54:37.000000 rid-kit-0.6.4/rid_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 08:54:37.000000 rid-kit-0.6.4/rid_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 08:54:37.000000 rid-kit-0.6.4/rid_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 08:54:37.000000 rid-kit-0.6.4/rid_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:54:37.736698 rid-kit-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 08:54:34.000000 rid-kit-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.728698 rid-kit-0.6.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.732698 rid-kit-0.6.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.732698 rid-kit-0.6.4/tests/data/000/
+-rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/000/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/000/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.732698 rid-kit-0.6.4/tests/data/001/
+-rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/001/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/001/plumed.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/001/topol.top
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/centers.out
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/cls_sel.ndx
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/cls_sel.out
+-rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/cv_forces.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)        7 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/kappa.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.736698 rid-kit-0.6.4/tests/data/models/
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/models/model_000.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/models/model_001.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/models/model_002.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/models/model_003.pb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4238 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/plm.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15119 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/plm_label.out
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/plumed.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1493 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/rid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/topol.top
+-rw-r--r--   0 runner    (1001) docker     (127)   217160 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/data/traj_comp.xtc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12799 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/mocked_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:54:37.736698 rid-kit-0.6.4/tests/op/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      113 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1470 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_adjust_trust_l.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2507 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_prep_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_prep_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_prep_rid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_prep_select.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      874 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_run_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_run_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_run_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/test_run_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/op/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4405 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6897 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/test_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/test_init-block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/test_iter-block.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6882 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-13 08:54:32.000000 rid-kit-0.6.4/tests/test_select.py
```

### Comparing `rid-kit-0.6.3/.github/workflows/pipy_release.yml` & `rid-kit-0.6.4/.github/workflows/pipy_release.yml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/.readthedocs.yaml` & `rid-kit-0.6.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/LICENSE` & `rid-kit-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/PKG-INFO` & `rid-kit-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rid-kit
-Version: 0.6.3
+Version: 0.6.4
 Summary: RiD package for enhanced sampling
 Home-page: https://github.com/deepmodeling/rid-kit
 Author: Yanze Wang, Jiahao Fan
 Author-email: yanze039@mit.edu,jiahaofan@pku.edu.cn
 License: UNKNOWN
 Keywords: enhanced sampling reinforced dynamics RiD
 Platform: UNKNOWN
```

### Comparing `rid-kit-0.6.3/README.md` & `rid-kit-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/Makefile` & `rid-kit-0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/make.bat` & `rid-kit-0.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/pics/mcmc_ala_1cv.png` & `rid-kit-0.6.4/docs/pics/mcmc_ala_1cv.png`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/pics/mcmc_ala_2cv.png` & `rid-kit-0.6.4/docs/pics/mcmc_ala_2cv.png`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/pics/rid_workflow.jpg` & `rid-kit-0.6.4/docs/pics/rid_workflow.jpg`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/conf.py` & `rid-kit-0.6.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/index.rst` & `rid-kit-0.6.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/install.md` & `rid-kit-0.6.4/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/install_dp.md` & `rid-kit-0.6.4/docs/source/install_dp.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/mcmc_configuration.md` & `rid-kit-0.6.4/docs/source/mcmc_configuration.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/prepare_files.md` & `rid-kit-0.6.4/docs/source/prepare_files.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/rid_configuration.md` & `rid-kit-0.6.4/docs/source/rid_configuration.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/rid_download.md` & `rid-kit-0.6.4/docs/source/rid_download.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/rid_machine.md` & `rid-kit-0.6.4/docs/source/rid_machine.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/troubleshooting/installation.md` & `rid-kit-0.6.4/docs/source/troubleshooting/installation.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/troubleshooting/minikube.md` & `rid-kit-0.6.4/docs/source/troubleshooting/minikube.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/troubleshooting/submit.md` & `rid-kit-0.6.4/docs/source/troubleshooting/submit.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/tutorial.ipynb` & `rid-kit-0.6.4/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/docs/source/tutorial.md` & `rid-kit-0.6.4/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/examples/install-linux-cn.sh` & `rid-kit-0.6.4/examples/install-linux-cn.sh`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/examples/quick-start-postgres-stable-cn.yaml` & `rid-kit-0.6.4/examples/quick-start-postgres-stable-cn.yaml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/examples/tutorial.ipynb` & `rid-kit-0.6.4/examples/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/install/DeePFE.cpp` & `rid-kit-0.6.4/install/DeePFE.cpp`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/install/gmx_exploration.dockerfile` & `rid-kit-0.6.4/install/gmx_exploration.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/install/gmx_plumed.dockerfile` & `rid-kit-0.6.4/install/gmx_plumed.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/install/gmx_tf.Dockerfile` & `rid-kit-0.6.4/install/gmx_tf.Dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/install/lmp_exploration_dp.dockerfile` & `rid-kit-0.6.4/install/lmp_exploration_dp.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/gromacs/command.py` & `rid-kit-0.6.4/rid/common/gromacs/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/gromacs/gmx_constant.py` & `rid-kit-0.6.4/rid/common/gromacs/gmx_constant.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/gromacs/mdp.py` & `rid-kit-0.6.4/rid/common/gromacs/mdp.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/gromacs/trjconv.py` & `rid-kit-0.6.4/rid/common/gromacs/trjconv.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/mol.py` & `rid-kit-0.6.4/rid/common/mol.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/mol_dpdata.py` & `rid-kit-0.6.4/rid/common/mol_dpdata.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/plumed/check_plumed.py` & `rid-kit-0.6.4/rid/common/plumed/check_plumed.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/plumed/make_plumed.py` & `rid-kit-0.6.4/rid/common/plumed/make_plumed.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/plumed/plumed_constant.py` & `rid-kit-0.6.4/rid/common/plumed/plumed_constant.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/sampler/command.py` & `rid-kit-0.6.4/rid/common/sampler/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/common/tensorflow/graph.py` & `rid-kit-0.6.4/rid/common/tensorflow/graph.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/constants.py` & `rid-kit-0.6.4/rid/constants.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/cli.py` & `rid-kit-0.6.4/rid/entrypoint/cli.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/download.py` & `rid-kit-0.6.4/rid/entrypoint/download.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/explore.py` & `rid-kit-0.6.4/rid/entrypoint/explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/info.py` & `rid-kit-0.6.4/rid/entrypoint/info.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/label.py` & `rid-kit-0.6.4/rid/entrypoint/label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/main.py` & `rid-kit-0.6.4/rid/entrypoint/main.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/redim.py` & `rid-kit-0.6.4/rid/entrypoint/redim.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/relabel.py` & `rid-kit-0.6.4/rid/entrypoint/relabel.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/reredim.py` & `rid-kit-0.6.4/rid/entrypoint/reredim.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/resubmit.py` & `rid-kit-0.6.4/rid/entrypoint/resubmit.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/server.py` & `rid-kit-0.6.4/rid/entrypoint/server.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/submit.py` & `rid-kit-0.6.4/rid/entrypoint/submit.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/entrypoint/train.py` & `rid-kit-0.6.4/rid/entrypoint/train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/flow/loop.py` & `rid-kit-0.6.4/rid/flow/loop.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/mcmc/walker.py` & `rid-kit-0.6.4/rid/mcmc/walker.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/nn/freeze.py` & `rid-kit-0.6.4/rid/nn/freeze.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/nn/model.py` & `rid-kit-0.6.4/rid/nn/model.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/nn/train_net.py` & `rid-kit-0.6.4/rid/nn/train_net.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/adjust_trust_level.py` & `rid-kit-0.6.4/rid/op/adjust_trust_level.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/label_stats.py` & `rid-kit-0.6.4/rid/op/label_stats.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/mcmc_plot.py` & `rid-kit-0.6.4/rid/op/mcmc_plot.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/mcmc_run.py` & `rid-kit-0.6.4/rid/op/mcmc_run.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/prep_data.py` & `rid-kit-0.6.4/rid/op/prep_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/prep_exploration.py` & `rid-kit-0.6.4/rid/op/prep_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/prep_label.py` & `rid-kit-0.6.4/rid/op/prep_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/prep_rid.py` & `rid-kit-0.6.4/rid/op/prep_rid.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/prep_select.py` & `rid-kit-0.6.4/rid/op/prep_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/recorder.py` & `rid-kit-0.6.4/rid/op/recorder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/run_exploration.py` & `rid-kit-0.6.4/rid/op/run_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/run_label.py` & `rid-kit-0.6.4/rid/op/run_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/run_model_devi.py` & `rid-kit-0.6.4/rid/op/run_model_devi.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/run_select.py` & `rid-kit-0.6.4/rid/op/run_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/op/run_train.py` & `rid-kit-0.6.4/rid/op/run_train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/select/cluster.py` & `rid-kit-0.6.4/rid/select/cluster.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/select/conf_select.py` & `rid-kit-0.6.4/rid/select/conf_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/select/model_devi.py` & `rid-kit-0.6.4/rid/select/model_devi.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/superop/blocks.py` & `rid-kit-0.6.4/rid/superop/blocks.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/superop/data.py` & `rid-kit-0.6.4/rid/superop/data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/superop/exploration.py` & `rid-kit-0.6.4/rid/superop/exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/superop/label.py` & `rid-kit-0.6.4/rid/superop/label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/superop/mcmc.py` & `rid-kit-0.6.4/rid/superop/mcmc.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/superop/selector.py` & `rid-kit-0.6.4/rid/superop/selector.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/task/builder.py` & `rid-kit-0.6.4/rid/task/builder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/task/task.py` & `rid-kit-0.6.4/rid/task/task.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_bohrium.json` & `rid-kit-0.6.4/rid/template/machine_bohrium.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_bohrium_k8s.json` & `rid-kit-0.6.4/rid/template/machine_bohrium_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_bohrium_k8s_mcmc.json` & `rid-kit-0.6.4/rid/template/machine_bohrium_k8s_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_local_k8s.json` & `rid-kit-0.6.4/rid/template/machine_local_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_slurm_k8s.json` & `rid-kit-0.6.4/rid/template/machine_slurm_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_slurm_k8s_mcmc.json` & `rid-kit-0.6.4/rid/template/machine_slurm_k8s_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_slurm_local.json` & `rid-kit-0.6.4/rid/template/machine_slurm_local.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/machine_slurm_local_mcmc.json` & `rid-kit-0.6.4/rid/template/machine_slurm_local_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_gmx_custom.json` & `rid-kit-0.6.4/rid/template/rid_gmx_custom.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_gmx_dih.json` & `rid-kit-0.6.4/rid/template/rid_gmx_dih.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_gmx_dis.json` & `rid-kit-0.6.4/rid/template/rid_gmx_dis.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_gmx_dp.json` & `rid-kit-0.6.4/rid/template/rid_gmx_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_lmp_dp.json` & `rid-kit-0.6.4/rid/template/rid_lmp_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_lmp_gmx_dp.json` & `rid-kit-0.6.4/rid/template/rid_lmp_gmx_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_mcmc_cv_dis.json` & `rid-kit-0.6.4/rid/template/rid_mcmc_cv_dis.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/template/rid_mcmc_path.json` & `rid-kit-0.6.4/rid/template/rid_mcmc_path.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/tools/estimator.py` & `rid-kit-0.6.4/rid/tools/estimator.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/utils/command.py` & `rid-kit-0.6.4/rid/utils/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/utils/files.py` & `rid-kit-0.6.4/rid/utils/files.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/utils/path.py` & `rid-kit-0.6.4/rid/utils/path.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid/utils/set_config.py` & `rid-kit-0.6.4/rid/utils/set_config.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/rid_kit.egg-info/PKG-INFO` & `rid-kit-0.6.4/rid_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rid-kit
-Version: 0.6.3
+Version: 0.6.4
 Summary: RiD package for enhanced sampling
 Home-page: https://github.com/deepmodeling/rid-kit
 Author: Yanze Wang, Jiahao Fan
 Author-email: yanze039@mit.edu,jiahaofan@pku.edu.cn
 License: UNKNOWN
 Keywords: enhanced sampling reinforced dynamics RiD
 Platform: UNKNOWN
```

### Comparing `rid-kit-0.6.3/rid_kit.egg-info/SOURCES.txt` & `rid-kit-0.6.4/rid_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/setup.py` & `rid-kit-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 readme_file = Path(__file__).parent / "README.md"
 readme = readme_file.read_text(encoding="utf-8")
 
 setuptools.setup(
     name='rid-kit',
     author="Yanze Wang, Jiahao Fan",
     author_email="yanze039@mit.edu,jiahaofan@pku.edu.cn",
-    version='0.6.3',
+    version='0.6.4',
     description="RiD package for enhanced sampling",
     setup_requires=['setuptools_scm'],
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/rid-kit",
     python_requires=">=3.6",
     packages=[
```

### Comparing `rid-kit-0.6.3/tests/context.py` & `rid-kit-0.6.4/tests/context.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/000/conf.gro` & `rid-kit-0.6.4/tests/data/000/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/000/topol.top` & `rid-kit-0.6.4/tests/data/000/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/001/conf.gro` & `rid-kit-0.6.4/tests/data/001/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/001/topol.top` & `rid-kit-0.6.4/tests/data/001/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/conf.gro` & `rid-kit-0.6.4/tests/data/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/models/model_000.pb` & `rid-kit-0.6.4/tests/data/models/model_000.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/models/model_001.pb` & `rid-kit-0.6.4/tests/data/models/model_001.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/models/model_002.pb` & `rid-kit-0.6.4/tests/data/models/model_002.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/models/model_003.pb` & `rid-kit-0.6.4/tests/data/models/model_003.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/plm.out` & `rid-kit-0.6.4/tests/data/plm.out`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/plm_label.out` & `rid-kit-0.6.4/tests/data/plm_label.out`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/rid.json` & `rid-kit-0.6.4/tests/data/rid.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/topol.top` & `rid-kit-0.6.4/tests/data/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/data/traj_comp.xtc` & `rid-kit-0.6.4/tests/data/traj_comp.xtc`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/mocked_ops.py` & `rid-kit-0.6.4/tests/mocked_ops.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_adjust_trust_l.py` & `rid-kit-0.6.4/tests/op/test_adjust_trust_l.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_prep_data.py` & `rid-kit-0.6.4/tests/op/test_prep_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_prep_explore.py` & `rid-kit-0.6.4/tests/op/test_prep_explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_prep_label.py` & `rid-kit-0.6.4/tests/op/test_prep_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_prep_rid.py` & `rid-kit-0.6.4/tests/op/test_prep_rid.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_prep_select.py` & `rid-kit-0.6.4/tests/op/test_prep_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_recorder.py` & `rid-kit-0.6.4/tests/op/test_recorder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_run_explore.py` & `rid-kit-0.6.4/tests/op/test_run_explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_run_label.py` & `rid-kit-0.6.4/tests/op/test_run_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_run_select.py` & `rid-kit-0.6.4/tests/op/test_run_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/test_run_train.py` & `rid-kit-0.6.4/tests/op/test_run_train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/op/utils.py` & `rid-kit-0.6.4/tests/op/utils.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/test_data.py` & `rid-kit-0.6.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/test_exploration.py` & `rid-kit-0.6.4/tests/test_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/test_init-block.py` & `rid-kit-0.6.4/tests/test_init-block.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/test_iter-block.py` & `rid-kit-0.6.4/tests/test_iter-block.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/test_label.py` & `rid-kit-0.6.4/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.3/tests/test_select.py` & `rid-kit-0.6.4/tests/test_select.py`

 * *Files identical despite different names*

