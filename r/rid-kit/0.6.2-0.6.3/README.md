# Comparing `tmp/rid-kit-0.6.2.tar.gz` & `tmp/rid-kit-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rid-kit-0.6.2.tar", last modified: Tue Aug 29 13:48:19 2023, max compression
+gzip compressed data, was "rid-kit-0.6.3.tar", last modified: Mon May 13 08:39:23 2024, max compression
```

## Comparing `rid-kit-0.6.2.tar` & `rid-kit-0.6.3.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.490527 rid-kit-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.466526 rid-kit-0.6.2/.eggs/
--rw-r--r--   0 runner    (1001) docker     (999)      211 2023-08-29 13:48:13.000000 rid-kit-0.6.2/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.462526 rid-kit-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.466526 rid-kit-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      230 2023-08-29 13:48:13.000000 rid-kit-0.6.2/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1002 2023-08-29 13:48:13.000000 rid-kit-0.6.2/.github/workflows/pipy_release.yml
--rw-r--r--   0 runner    (1001) docker     (999)      420 2023-08-29 13:48:13.000000 rid-kit-0.6.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (999)       94 2023-08-29 13:48:13.000000 rid-kit-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      715 2023-08-29 13:48:13.000000 rid-kit-0.6.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     7652 2023-08-29 13:48:13.000000 rid-kit-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)    10808 2023-08-29 13:48:19.490527 rid-kit-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    10482 2023-08-29 13:48:13.000000 rid-kit-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.466526 rid-kit-0.6.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.470526 rid-kit-0.6.2/docs/.eggs/
--rw-r--r--   0 runner    (1001) docker     (999)      211 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/.eggs/README.txt
--rw-r--r--   0 runner    (1001) docker     (999)      638 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (999)      804 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.470526 rid-kit-0.6.2/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (999)   567861 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/pics/mcmc_ala_1cv.png
--rw-r--r--   0 runner    (1001) docker     (999)   738823 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/pics/mcmc_ala_2cv.png
--rw-r--r--   0 runner    (1001) docker     (999)   639421 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/pics/rid_workflow.jpg
--rwxr-xr-x   0 runner    (1001) docker     (999)      146 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.470526 rid-kit-0.6.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.470526 rid-kit-0.6.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/_static/.gitkeep
--rwxr-xr-x   0 runner    (1001) docker     (999)     2693 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     1114 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     4271 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (999)     5533 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/install_dp.md
--rw-r--r--   0 runner    (1001) docker     (999)     4034 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/mcmc_configuration.md
--rw-r--r--   0 runner    (1001) docker     (999)     2582 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/prepare_files.md
--rw-r--r--   0 runner    (1001) docker     (999)    16232 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/rid_configuration.md
--rw-r--r--   0 runner    (1001) docker     (999)     4900 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/rid_download.md
--rw-r--r--   0 runner    (1001) docker     (999)    13074 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/rid_machine.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/docs/source/troubleshooting/
--rwxr-xr-x   0 runner    (1001) docker     (999)      345 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/troubleshooting/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2011 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/troubleshooting/installation.md
--rw-r--r--   0 runner    (1001) docker     (999)     1927 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/troubleshooting/minikube.md
--rw-r--r--   0 runner    (1001) docker     (999)     3288 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/troubleshooting/submit.md
--rw-r--r--   0 runner    (1001) docker     (999)    16827 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (999)    11213 2023-08-29 13:48:13.000000 rid-kit-0.6.2/docs/source/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/examples/JSON/
--rw-r--r--   0 runner    (1001) docker     (999)      396 2023-08-29 13:48:13.000000 rid-kit-0.6.2/examples/JSON/rid.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     3448 2023-08-29 13:48:13.000000 rid-kit-0.6.2/examples/install-linux-cn.sh
--rw-r--r--   0 runner    (1001) docker     (999)    49439 2023-08-29 13:48:13.000000 rid-kit-0.6.2/examples/quick-start-postgres-stable-cn.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    25032 2023-08-29 13:48:13.000000 rid-kit-0.6.2/examples/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/install/
--rw-r--r--   0 runner    (1001) docker     (999)     9005 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/DeePFE.cpp
--rw-r--r--   0 runner    (1001) docker     (999)      245 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/README.md
--rw-r--r--   0 runner    (1001) docker     (999)     3972 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/gmx_exploration.dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)     3726 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/gmx_plumed.dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)      756 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/gmx_tf.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)     4090 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/lmp_exploration_dp.dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)      300 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/tf_cpu.dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)      308 2023-08-29 13:48:13.000000 rid-kit-0.6.2/install/tf_gpu.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (999)      125 2023-08-29 13:48:13.000000 rid-kit-0.6.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/rid/
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/__about__.py
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/rid/common/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/rid/common/gromacs/
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/gromacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2181 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/gromacs/command.py
--rw-r--r--   0 runner    (1001) docker     (999)     3107 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/gromacs/gmx_constant.py
--rw-r--r--   0 runner    (1001) docker     (999)     2820 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/gromacs/mdp.py
--rw-r--r--   0 runner    (1001) docker     (999)     2335 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/gromacs/trjconv.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/rid/common/lammps/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      203 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/lammps/command.py
--rw-r--r--   0 runner    (1001) docker     (999)       77 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/lammps/lmp_constant.py
--rw-r--r--   0 runner    (1001) docker     (999)     4381 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/mol.py
--rw-r--r--   0 runner    (1001) docker     (999)     1221 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/mol_dpdata.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.474526 rid-kit-0.6.2/rid/common/plumed/
--rw-r--r--   0 runner    (1001) docker     (999)      236 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/plumed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      636 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/plumed/check_plumed.py
--rw-r--r--   0 runner    (1001) docker     (999)    12420 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/plumed/make_plumed.py
--rw-r--r--   0 runner    (1001) docker     (999)      623 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/plumed/plumed_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/common/sampler/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2844 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/sampler/command.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/common/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      825 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/common/tensorflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (999)     2452 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      686 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (999)     2353 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/download.py
--rw-r--r--   0 runner    (1001) docker     (999)     6634 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/explore.py
--rw-r--r--   0 runner    (1001) docker     (999)     1040 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/info.py
--rw-r--r--   0 runner    (1001) docker     (999)     5923 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/label.py
--rw-r--r--   0 runner    (1001) docker     (999)    16710 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/main.py
--rw-r--r--   0 runner    (1001) docker     (999)     2810 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/redim.py
--rw-r--r--   0 runner    (1001) docker     (999)     6273 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/relabel.py
--rw-r--r--   0 runner    (1001) docker     (999)     3781 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/reredim.py
--rw-r--r--   0 runner    (1001) docker     (999)     7629 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/resubmit.py
--rw-r--r--   0 runner    (1001) docker     (999)     1937 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/server.py
--rw-r--r--   0 runner    (1001) docker     (999)     8753 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/submit.py
--rw-r--r--   0 runner    (1001) docker     (999)     2565 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/entrypoint/train.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/flow/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    21137 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/flow/loop.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/main.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/mcmc/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5716 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/mcmc/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/nn/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3155 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/nn/freeze.py
--rw-r--r--   0 runner    (1001) docker     (999)    27197 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/nn/model.py
--rw-r--r--   0 runner    (1001) docker     (999)     7434 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/nn/train_net.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.478526 rid-kit-0.6.2/rid/op/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3259 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/adjust_trust_level.py
--rw-r--r--   0 runner    (1001) docker     (999)     3775 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/label_stats.py
--rw-r--r--   0 runner    (1001) docker     (999)    11437 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/mcmc_plot.py
--rw-r--r--   0 runner    (1001) docker     (999)     7762 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/mcmc_run.py
--rw-r--r--   0 runner    (1001) docker     (999)     2580 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/prep_data.py
--rw-r--r--   0 runner    (1001) docker     (999)     5499 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/prep_exploration.py
--rw-r--r--   0 runner    (1001) docker     (999)     6555 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/prep_label.py
--rw-r--r--   0 runner    (1001) docker     (999)     9938 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/prep_rid.py
--rw-r--r--   0 runner    (1001) docker     (999)     5824 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/prep_select.py
--rw-r--r--   0 runner    (1001) docker     (999)     1554 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/recorder.py
--rw-r--r--   0 runner    (1001) docker     (999)    14616 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/run_exploration.py
--rw-r--r--   0 runner    (1001) docker     (999)     9111 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/run_label.py
--rw-r--r--   0 runner    (1001) docker     (999)     4267 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/run_model_devi.py
--rw-r--r--   0 runner    (1001) docker     (999)     7907 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/run_select.py
--rw-r--r--   0 runner    (1001) docker     (999)     4855 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/op/run_train.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.482526 rid-kit-0.6.2/rid/select/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5892 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/select/cluster.py
--rw-r--r--   0 runner    (1001) docker     (999)     1443 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/select/conf_select.py
--rw-r--r--   0 runner    (1001) docker     (999)     1802 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/select/model_devi.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.482526 rid-kit-0.6.2/rid/superop/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (999)    27192 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/blocks.py
--rw-r--r--   0 runner    (1001) docker     (999)     3694 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/data.py
--rwxr-xr-x   0 runner    (1001) docker     (999)    10888 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/exploration.py
--rwxr-xr-x   0 runner    (1001) docker     (999)    11594 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/label.py
--rw-r--r--   0 runner    (1001) docker     (999)     5886 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/mcmc.py
--rwxr-xr-x   0 runner    (1001) docker     (999)    12664 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/superop/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.482526 rid-kit-0.6.2/rid/task/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11234 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/task/builder.py
--rw-r--r--   0 runner    (1001) docker     (999)     1313 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.482526 rid-kit-0.6.2/rid/template/
--rwxr-xr-x   0 runner    (1001) docker     (999)     5900 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_bohrium.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     5116 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_bohrium_k8s.json
--rw-r--r--   0 runner    (1001) docker     (999)     2620 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_bohrium_k8s_mcmc.json
--rw-r--r--   0 runner    (1001) docker     (999)     1795 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_local_k8s.json
--rw-r--r--   0 runner    (1001) docker     (999)     1864 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_slurm_k8s.json
--rw-r--r--   0 runner    (1001) docker     (999)     1549 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_slurm_k8s_mcmc.json
--rw-r--r--   0 runner    (1001) docker     (999)     2025 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_slurm_local.json
--rw-r--r--   0 runner    (1001) docker     (999)     1673 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/machine_slurm_local_mcmc.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     1999 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_gmx_custom.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     2026 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_gmx_dih.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     2031 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_gmx_dis.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     2536 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_gmx_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     1505 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_lmp_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     3013 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_lmp_gmx_dp.json
--rwxr-xr-x   0 runner    (1001) docker     (999)      465 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_mcmc_cv_dih.json
--rwxr-xr-x   0 runner    (1001) docker     (999)      696 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_mcmc_cv_dis.json
--rwxr-xr-x   0 runner    (1001) docker     (999)     1160 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/template/rid_mcmc_path.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.482526 rid-kit-0.6.2/rid/tools/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    12217 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/tools/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.482526 rid-kit-0.6.2/rid/utils/
--rw-r--r--   0 runner    (1001) docker     (999)      360 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      534 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/utils/command.py
--rw-r--r--   0 runner    (1001) docker     (999)     1449 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (999)      207 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (999)      543 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (999)     1549 2023-08-29 13:48:13.000000 rid-kit-0.6.2/rid/utils/set_config.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.486527 rid-kit-0.6.2/rid_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    10808 2023-08-29 13:48:19.000000 rid-kit-0.6.2/rid_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4975 2023-08-29 13:48:19.000000 rid-kit-0.6.2/rid_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 13:48:19.000000 rid-kit-0.6.2/rid_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       50 2023-08-29 13:48:19.000000 rid-kit-0.6.2/rid_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-08-29 13:48:19.000000 rid-kit-0.6.2/rid_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)      210 2023-08-29 13:48:19.000000 rid-kit-0.6.2/rid_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 13:48:19.490527 rid-kit-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1654 2023-08-29 13:48:15.000000 rid-kit-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.486527 rid-kit-0.6.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (999)      629 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.486527 rid-kit-0.6.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.486527 rid-kit-0.6.2/tests/data/000/
--rw-r--r--   0 runner    (1001) docker     (999)    80843 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/000/conf.gro
--rw-r--r--   0 runner    (1001) docker     (999)     7156 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/000/topol.top
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.486527 rid-kit-0.6.2/tests/data/001/
--rw-r--r--   0 runner    (1001) docker     (999)    80843 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/001/conf.gro
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/001/plumed.dat
--rw-r--r--   0 runner    (1001) docker     (999)     7156 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/001/topol.top
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/centers.out
--rw-r--r--   0 runner    (1001) docker     (999)       13 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/cls_sel.ndx
--rw-r--r--   0 runner    (1001) docker     (999)      134 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/cls_sel.out
--rw-r--r--   0 runner    (1001) docker     (999)    80843 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/conf.gro
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/conf.json
--rwxr-xr-x   0 runner    (1001) docker     (999)       53 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/cv_forces.out
--rwxr-xr-x   0 runner    (1001) docker     (999)        7 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/kappa.out
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.490527 rid-kit-0.6.2/tests/data/models/
--rw-r--r--   0 runner    (1001) docker     (999)   536959 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/models/model_000.pb
--rw-r--r--   0 runner    (1001) docker     (999)   536959 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/models/model_001.pb
--rw-r--r--   0 runner    (1001) docker     (999)   536959 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/models/model_002.pb
--rw-r--r--   0 runner    (1001) docker     (999)   536959 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/models/model_003.pb
--rwxr-xr-x   0 runner    (1001) docker     (999)     4238 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/plm.out
--rwxr-xr-x   0 runner    (1001) docker     (999)    15119 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/plm_label.out
--rw-r--r--   0 runner    (1001) docker     (999)      124 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/plumed.dat
--rwxr-xr-x   0 runner    (1001) docker     (999)     1493 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/rid.json
--rw-r--r--   0 runner    (1001) docker     (999)     7377 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/topol.top
--rw-r--r--   0 runner    (1001) docker     (999)   217160 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/data/traj_comp.xtc
--rwxr-xr-x   0 runner    (1001) docker     (999)    12799 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/mocked_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 13:48:19.490527 rid-kit-0.6.2/tests/op/
--rwxr-xr-x   0 runner    (1001) docker     (999)      113 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/context.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     1470 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_adjust_trust_l.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     2507 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_prep_data.py
--rw-r--r--   0 runner    (1001) docker     (999)     4272 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_prep_explore.py
--rw-r--r--   0 runner    (1001) docker     (999)     3863 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_prep_label.py
--rw-r--r--   0 runner    (1001) docker     (999)     1626 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_prep_rid.py
--rw-r--r--   0 runner    (1001) docker     (999)     1763 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_prep_select.py
--rwxr-xr-x   0 runner    (1001) docker     (999)      874 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (999)     1692 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_run_explore.py
--rw-r--r--   0 runner    (1001) docker     (999)     1806 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_run_label.py
--rw-r--r--   0 runner    (1001) docker     (999)     4530 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_run_select.py
--rw-r--r--   0 runner    (1001) docker     (999)     1332 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/test_run_train.py
--rw-r--r--   0 runner    (1001) docker     (999)      654 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/op/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     4405 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     6897 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/test_exploration.py
--rw-r--r--   0 runner    (1001) docker     (999)     6818 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/test_init-block.py
--rw-r--r--   0 runner    (1001) docker     (999)     7402 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/test_iter-block.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     6882 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (999)     5060 2023-08-29 13:48:13.000000 rid-kit-0.6.2/tests/test_select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.265521 rid-kit-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.229522 rid-kit-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.github/workflows/pipy_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-13 08:39:17.000000 rid-kit-0.6.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-13 08:39:17.000000 rid-kit-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-13 08:39:23.265521 rid-kit-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-13 08:39:17.000000 rid-kit-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.233522 rid-kit-0.6.3/docs/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/.eggs/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)   567861 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/pics/mcmc_ala_1cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)   738823 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/pics/mcmc_ala_2cv.png
+-rw-r--r--   0 runner    (1001) docker     (127)   639421 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/pics/rid_workflow.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/_static/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2693 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/install_dp.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/mcmc_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/prepare_files.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16232 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/rid_configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/rid_download.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/rid_machine.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.237522 rid-kit-0.6.3/docs/source/troubleshooting/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/minikube.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/troubleshooting/submit.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-05-13 08:39:17.000000 rid-kit-0.6.3/docs/source/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/examples/JSON/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/JSON/rid.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3448 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/install-linux-cn.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    49439 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/quick-start-postgres-stable-cn.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    25032 2024-05-13 08:39:17.000000 rid-kit-0.6.3/examples/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/DeePFE.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/gmx_exploration.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/gmx_plumed.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/gmx_tf.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/lmp_exploration_dp.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/tf_cpu.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 08:39:17.000000 rid-kit-0.6.3/install/tf_gpu.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 08:39:17.000000 rid-kit-0.6.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/common/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/gmx_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/mdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/gromacs/trjconv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.241522 rid-kit-0.6.3/rid/common/lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/lammps/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/lammps/lmp_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/mol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/mol_dpdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/common/plumed/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/check_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/make_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/plumed/plumed_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/common/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/sampler/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/common/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/common/tensorflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/redim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/relabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/reredim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/entrypoint/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/flow/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.245522 rid-kit-0.6.3/rid/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/mcmc/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.249522 rid-kit-0.6.3/rid/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/nn/train_net.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.249522 rid-kit-0.6.3/rid/op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/adjust_trust_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/label_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/mcmc_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/mcmc_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_rid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/prep_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_model_devi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/op/run_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.249522 rid-kit-0.6.3/rid/select/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/conf_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/select/model_devi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/superop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27192 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10888 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/exploration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11594 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/mcmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12664 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/superop/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/task/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/template/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5900 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_bohrium.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5116 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_bohrium_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_bohrium_k8s_mcmc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_local_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_k8s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_k8s_mcmc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_local.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/machine_slurm_local_mcmc.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1999 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_custom.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2026 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_dih.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2031 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_dis.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_gmx_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1505 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_lmp_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3013 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_lmp_gmx_dp.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_mcmc_cv_dih.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_mcmc_cv_dis.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1160 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/template/rid_mcmc_path.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.253522 rid-kit-0.6.3/rid/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/tools/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.257521 rid-kit-0.6.3/rid/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 08:39:17.000000 rid-kit-0.6.3/rid/utils/set_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.257521 rid-kit-0.6.3/rid_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 08:39:23.000000 rid-kit-0.6.3/rid_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:39:23.265521 rid-kit-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 08:39:19.000000 rid-kit-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.257521 rid-kit-0.6.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/000/
+-rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/000/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/000/topol.top
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/001/
+-rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/001/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/001/plumed.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/001/topol.top
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/centers.out
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/cls_sel.ndx
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/cls_sel.out
+-rw-r--r--   0 runner    (1001) docker     (127)    80843 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/conf.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/cv_forces.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)        7 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/kappa.out
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.261521 rid-kit-0.6.3/tests/data/models/
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_000.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_001.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_002.pb
+-rw-r--r--   0 runner    (1001) docker     (127)   536959 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/models/model_003.pb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4238 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/plm.out
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15119 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/plm_label.out
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/plumed.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1493 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/rid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/topol.top
+-rw-r--r--   0 runner    (1001) docker     (127)   217160 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/data/traj_comp.xtc
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12799 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/mocked_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:39:23.265521 rid-kit-0.6.3/tests/op/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      113 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1470 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_adjust_trust_l.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2507 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_rid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_prep_select.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      874 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/test_run_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/op/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4405 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6897 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_init-block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_iter-block.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6882 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-13 08:39:17.000000 rid-kit-0.6.3/tests/test_select.py
```

### Comparing `rid-kit-0.6.2/.github/workflows/pipy_release.yml` & `rid-kit-0.6.3/.github/workflows/pipy_release.yml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/.readthedocs.yaml` & `rid-kit-0.6.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/LICENSE` & `rid-kit-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/PKG-INFO` & `rid-kit-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rid-kit
-Version: 0.6.2
+Version: 0.6.3
 Summary: RiD package for enhanced sampling
 Home-page: https://github.com/deepmodeling/rid-kit
 Author: Yanze Wang, Jiahao Fan
 Author-email: yanze039@mit.edu,jiahaofan@pku.edu.cn
 License: UNKNOWN
 Keywords: enhanced sampling reinforced dynamics RiD
 Platform: UNKNOWN
```

### Comparing `rid-kit-0.6.2/README.md` & `rid-kit-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/Makefile` & `rid-kit-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/make.bat` & `rid-kit-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/pics/mcmc_ala_1cv.png` & `rid-kit-0.6.3/docs/pics/mcmc_ala_1cv.png`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/pics/mcmc_ala_2cv.png` & `rid-kit-0.6.3/docs/pics/mcmc_ala_2cv.png`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/pics/rid_workflow.jpg` & `rid-kit-0.6.3/docs/pics/rid_workflow.jpg`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/conf.py` & `rid-kit-0.6.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/index.rst` & `rid-kit-0.6.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/install.md` & `rid-kit-0.6.3/docs/source/install.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 Use the command
 ```bash
 conda create -n rid-drop python=3.9 libtensorflow_cc=2.6.2=*cuda110* tensorflow=2.6.2=*cuda110* -c conda-forge
 ```
 ```bash
 conda activate rid-drop
 conda install mdtraj nccl -c conda-forge
+conda install cudatoolkit-dev -c conda-forge
 pip install cmake cython
 pip install matplotlib parmed scikit-learn dpdata
 ```
 to get the compiled libtensorflow_cc and other necessary packages.
 After installation, activate the enviroment and set library path
 ```bash
 conda activate rid-drop
```

### Comparing `rid-kit-0.6.2/docs/source/install_dp.md` & `rid-kit-0.6.3/docs/source/install_dp.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 > If you want to set environments by hand, please follow settings of this section. 
 >
 > You can also set computation environment of rid through docker, just run "docker pull pkufjhdocker/rid-kit:latest" to get the docker image we built. Or build the image through the dockerfile in rid-kit/install directory.
 
 ### Install tensorflow's C++ interface and other necessary packages
 We recommend using conda to manage the python enviroment. 
 Use the command
-```
+```bash
 conda create -n rid-dp python=3.9 libtensorflow_cc=2.6.2=*cuda110* tensorflow=2.6.2=*cuda110* nccl mdtraj numpy scikit-learn cmake dpdata cython -c conda-forge
 ```
 to get the compiled libtensorflow_cc and other necessary packages.
+Install the cudatoolkit which manage the nvcc and other commands.
+```bash
+conda install cudatoolkit-dev -c conda-forge
+```
 After installation, activate the enviroment and set library path
 ```bash
 conda activate rid-dp
 export LIBRARY_PATH=${CONDA_PREFIX}/lib:$LIBRARY_PATH
 export LD_LIBRARY_PATH=${CONDA_PREFIX}/lib:$LD_LIBRARY_PATH
 ```
```

### Comparing `rid-kit-0.6.2/docs/source/mcmc_configuration.md` & `rid-kit-0.6.3/docs/source/mcmc_configuration.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/prepare_files.md` & `rid-kit-0.6.3/docs/source/prepare_files.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/rid_configuration.md` & `rid-kit-0.6.3/docs/source/rid_configuration.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/rid_download.md` & `rid-kit-0.6.3/docs/source/rid_download.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/rid_machine.md` & `rid-kit-0.6.3/docs/source/rid_machine.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/troubleshooting/installation.md` & `rid-kit-0.6.3/docs/source/troubleshooting/installation.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/troubleshooting/minikube.md` & `rid-kit-0.6.3/docs/source/troubleshooting/minikube.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/troubleshooting/submit.md` & `rid-kit-0.6.3/docs/source/troubleshooting/submit.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/tutorial.ipynb` & `rid-kit-0.6.3/docs/source/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/docs/source/tutorial.md` & `rid-kit-0.6.3/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/examples/install-linux-cn.sh` & `rid-kit-0.6.3/examples/install-linux-cn.sh`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/examples/quick-start-postgres-stable-cn.yaml` & `rid-kit-0.6.3/examples/quick-start-postgres-stable-cn.yaml`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/examples/tutorial.ipynb` & `rid-kit-0.6.3/examples/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/install/DeePFE.cpp` & `rid-kit-0.6.3/install/DeePFE.cpp`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/install/gmx_exploration.dockerfile` & `rid-kit-0.6.3/install/gmx_exploration.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/install/gmx_plumed.dockerfile` & `rid-kit-0.6.3/install/gmx_plumed.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/install/gmx_tf.Dockerfile` & `rid-kit-0.6.3/install/gmx_tf.Dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/install/lmp_exploration_dp.dockerfile` & `rid-kit-0.6.3/install/lmp_exploration_dp.dockerfile`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/gromacs/command.py` & `rid-kit-0.6.3/rid/common/gromacs/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/gromacs/gmx_constant.py` & `rid-kit-0.6.3/rid/common/gromacs/gmx_constant.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/gromacs/mdp.py` & `rid-kit-0.6.3/rid/common/gromacs/mdp.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/gromacs/trjconv.py` & `rid-kit-0.6.3/rid/common/gromacs/trjconv.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/mol.py` & `rid-kit-0.6.3/rid/common/mol.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,14 +43,51 @@
             dihedral_angle[residue.index+1] = {}
             if residue.index in phi_found_indices:
                 dihedral_angle[residue.index+1]["phi"] = phi_info[residue.index+1]
             if residue.index in psi_found_indices:
                 dihedral_angle[residue.index+1]["psi"] = psi_info[residue.index+1]
     return dihedral_angle
 
+def get_dihedral_value_from_resid(file_path: str, selected_resid: List[int])-> Dict:
+    if len(selected_resid) == 0:
+        return {}
+    # Load the .gro file
+    traj = md.load(file_path)
+    
+    atom_list = []
+    atom_indices = [atom.index for atom in traj.topology.atoms 
+                    if ((atom.residue.index) in selected_resid or (atom.residue.index + 1) in selected_resid
+                        or (atom.residue.index - 1) in selected_resid)]
+    atom_list.extend(atom_indices)
+    traj = traj.atom_slice(atom_list)
+    # Compute the phi and psi angles for all residues
+    phi_indices, phi_angles = md.compute_phi(traj)
+    psi_indices, psi_angles = md.compute_psi(traj)
+    
+    cv_info = get_dihedral_from_resid(file_path, selected_resid)
+    
+    # Extract the angles from the lists
+    psi_angles = psi_angles[0]
+    phi_angles = phi_angles[0]
+
+    # Create the correspondence dictionary
+    selected_dihedral_value = {}
+    psi_counter = 0
+    phi_counter = 0
+
+    for key, value in cv_info.items():
+        selected_dihedral_value[key] = {}
+        if 'psi' in value:
+            selected_dihedral_value[key]['psi'] = psi_angles[psi_counter]
+            psi_counter += 1
+        if 'phi' in value:
+            selected_dihedral_value[key]['phi'] = phi_angles[phi_counter]
+            phi_counter += 1
+    
+    return selected_dihedral_value
 
 def get_dihedral_from_resid(file_path: str, selected_resid: List[int]) -> Dict:
     if len(selected_resid) == 0:
         return {}
     traj = md.load(file_path)
     top = traj.topology
     psi_found_indices, psi_atom_indices = _atom_sequence(top, PSI_ATOMS)
```

### Comparing `rid-kit-0.6.2/rid/common/mol_dpdata.py` & `rid-kit-0.6.3/rid/common/mol_dpdata.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/plumed/check_plumed.py` & `rid-kit-0.6.3/rid/common/plumed/check_plumed.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/plumed/make_plumed.py` & `rid-kit-0.6.3/rid/common/plumed/make_plumed.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/plumed/plumed_constant.py` & `rid-kit-0.6.3/rid/common/plumed/plumed_constant.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/sampler/command.py` & `rid-kit-0.6.3/rid/common/sampler/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/common/tensorflow/graph.py` & `rid-kit-0.6.3/rid/common/tensorflow/graph.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/constants.py` & `rid-kit-0.6.3/rid/constants.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/cli.py` & `rid-kit-0.6.3/rid/entrypoint/cli.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/download.py` & `rid-kit-0.6.3/rid/entrypoint/download.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/explore.py` & `rid-kit-0.6.3/rid/entrypoint/explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/info.py` & `rid-kit-0.6.3/rid/entrypoint/info.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/label.py` & `rid-kit-0.6.3/rid/entrypoint/label.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from rid import SRC_ROOT
 upload_packages.append(SRC_ROOT)
 
 from rid.utils import normalize_resources
 from rid.superop.label import Label
 from rid.op.prep_label import PrepLabel, CheckLabelInputs
 from rid.op.run_label import RunLabel
+from rid.op.label_stats import LabelStats
 from rid.constants import label_task_pattern
 
 def label_rid(
         confs: Union[str, List[str]],
         topology: Optional[str],
         rid_config: str,
         machine_config: str,
@@ -43,14 +44,15 @@
         normalized_resources[resource_type] = normalize_resources(resources[resource_type])
 
     label_op = Label(
         "label",
         CheckLabelInputs,
         PrepLabel,
         RunLabel,
+        LabelStats,
         prep_config = normalized_resources[tasks["prep_label_config"]],
         run_config = normalized_resources[tasks["run_label_config"]],
         retry_times=1)
 
     if isinstance(confs, str):
         confs_artifact = upload_artifact(Path(confs), archive=None)
     elif isinstance(confs, List):
@@ -140,34 +142,47 @@
         forcefield_artifact = upload_artifact(Path(forcefield), archive=None)
         
     if topology is None:
         top_artifact = None
     else:
         top_artifact = upload_artifact(Path(topology), archive=None)
 
-    conf_tags = []
+    conf_tags = {}
     for index in range(len(confs)):
-        conf_tags.append({Path(confs[index]).name:label_task_pattern.format(index)})
+        conf_tags[Path(confs[index]).name] = label_task_pattern.format(index)
         
+    if isinstance(confs, str):
+        conf_tags_path = os.path.join(Path(confs).parent.absolute(), "conf.json")
+        with open(conf_tags_path, "w") as f:
+            json.dump(conf_tags,f)
+    elif isinstance(confs, List):
+        conf_tags_path = os.path.join(Path(confs[0]).parent.absolute(), "conf.json")
+        with open(conf_tags_path,"w") as f:
+            json.dump(conf_tags,f)
+    else:
+        raise RuntimeError("Invalid type of `confs`.")
+    
+    conf_tags_artifact = upload_artifact(Path(conf_tags_path), archive=None)
+    
     rid_steps = Step("rid-label",
             label_op,
             artifacts={
                 "topology": top_artifact,
                 "models": models_artifact,
                 "forcefield": forcefield_artifact,
                 "inputfile": inputfile_artifact,
                 "confs": confs_artifact,
                 "at": None,
                 "index_file": index_file_artifact,
                 "dp_files": dp_files_artifact,
-                "cv_file": cv_file_artifact
+                "cv_file": cv_file_artifact,
+                "conf_tags": conf_tags_artifact
             },
             parameters={
                 "label_config": label_config,
                 "cv_config": cv_config,
-                "conf_tags": conf_tags,
                 "block_tag" : "000"
             },
         )
     wf = Workflow("rid-labeling", pod_gc_strategy="OnPodSuccess", parallelism=50, id = workflow_id_defined)
     wf.add(rid_steps)
     wf.submit()
```

### Comparing `rid-kit-0.6.2/rid/entrypoint/main.py` & `rid-kit-0.6.3/rid/entrypoint/main.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/redim.py` & `rid-kit-0.6.3/rid/entrypoint/redim.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/relabel.py` & `rid-kit-0.6.3/rid/entrypoint/relabel.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/reredim.py` & `rid-kit-0.6.3/rid/entrypoint/reredim.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/resubmit.py` & `rid-kit-0.6.3/rid/entrypoint/resubmit.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/server.py` & `rid-kit-0.6.3/rid/entrypoint/server.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/submit.py` & `rid-kit-0.6.3/rid/entrypoint/submit.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/entrypoint/train.py` & `rid-kit-0.6.3/rid/entrypoint/train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/flow/loop.py` & `rid-kit-0.6.3/rid/flow/loop.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/mcmc/walker.py` & `rid-kit-0.6.3/rid/mcmc/walker.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/nn/freeze.py` & `rid-kit-0.6.3/rid/nn/freeze.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/nn/model.py` & `rid-kit-0.6.3/rid/nn/model.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/nn/train_net.py` & `rid-kit-0.6.3/rid/nn/train_net.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/adjust_trust_level.py` & `rid-kit-0.6.3/rid/op/adjust_trust_level.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/label_stats.py` & `rid-kit-0.6.3/rid/op/label_stats.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/mcmc_plot.py` & `rid-kit-0.6.3/rid/op/mcmc_plot.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/mcmc_run.py` & `rid-kit-0.6.3/rid/op/mcmc_run.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/prep_data.py` & `rid-kit-0.6.3/rid/op/prep_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/prep_exploration.py` & `rid-kit-0.6.3/rid/op/prep_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/prep_label.py` & `rid-kit-0.6.3/rid/op/prep_label.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 selected_resid = op_in["cv_config"]["selected_resid"]
             elif "selected_atomid" in op_in["cv_config"]:
                 selected_atomid = op_in["cv_config"]["selected_atomid"]
             cv_file = op_in["cv_file"]
         
         #print("what is cv", cv_file)
         if op_in["label_config"]["method"] == "restrained":
-            at = 0.0
+            at = None
             if op_in["at"] is not None:
                 at = load_txt(op_in["at"])
             gmx_task_builder = RestrainedMDTaskBuilder(
                 conf = op_in["conf"],
                 topology = op_in["topology"],
                 label_config = op_in["label_config"],
                 cv_file = cv_file,
```

### Comparing `rid-kit-0.6.2/rid/op/prep_rid.py` & `rid-kit-0.6.3/rid/op/prep_rid.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/prep_select.py` & `rid-kit-0.6.3/rid/op/prep_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/recorder.py` & `rid-kit-0.6.3/rid/op/recorder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/run_exploration.py` & `rid-kit-0.6.3/rid/op/run_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/run_label.py` & `rid-kit-0.6.3/rid/op/run_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/run_model_devi.py` & `rid-kit-0.6.3/rid/op/run_model_devi.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/run_select.py` & `rid-kit-0.6.3/rid/op/run_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/op/run_train.py` & `rid-kit-0.6.3/rid/op/run_train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/select/cluster.py` & `rid-kit-0.6.3/rid/select/cluster.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/select/conf_select.py` & `rid-kit-0.6.3/rid/select/conf_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/select/model_devi.py` & `rid-kit-0.6.3/rid/select/model_devi.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/superop/blocks.py` & `rid-kit-0.6.3/rid/superop/blocks.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/superop/data.py` & `rid-kit-0.6.3/rid/superop/data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/superop/exploration.py` & `rid-kit-0.6.3/rid/superop/exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/superop/label.py` & `rid-kit-0.6.3/rid/superop/label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/superop/mcmc.py` & `rid-kit-0.6.3/rid/superop/mcmc.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/superop/selector.py` & `rid-kit-0.6.3/rid/superop/selector.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/task/builder.py` & `rid-kit-0.6.3/rid/task/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         lmp_conf_name,
         gmx_top_name,
         lmp_input_name,
         gmx_mdp_name, 
         plumed_input_name,
     )
 from rid.utils import read_txt
-from rid.common.mol import get_distance_from_atomid
+from rid.common.mol import get_distance_from_atomid,get_dihedral_value_from_resid
 from rid.common.gromacs import make_md_mdp_string
 from rid.common.plumed import make_deepfe_plumed, make_restraint_plumed, make_constraint_plumed, get_cv_name,make_distance_list_from_file
 
 
 class TaskBuilder(ABC):
 
     @abstractmethod
@@ -284,19 +284,28 @@
         kappa: Union[int, float, Sequence, np.ndarray] = 0.5,
         at: Union[int, float, Sequence, np.ndarray] = 1.0,
         stride: int = 100,
         output: str = "plm.out",
         mode: str = "torsion"
     ):
     plumed_task_files = {}
-    if selected_atomid is not None:
-        at = []
-        cv_info = get_distance_from_atomid(conf, selected_atomid)
-        for dis_id in range(len(selected_atomid)):
-            at.append(cv_info["%s %s"%(selected_atomid[dis_id][0],selected_atomid[dis_id][1])])
+    if at is None:
+        if selected_atomid is not None:
+            at = []
+            cv_info = get_distance_from_atomid(conf, selected_atomid)
+            for dis_id in range(len(selected_atomid)):
+                at.append(cv_info["%s %s"%(selected_atomid[dis_id][0],selected_atomid[dis_id][1])])
+        if selected_resid is not None:
+            at = []
+            cv_value = get_dihedral_value_from_resid(conf, selected_resid)
+            for key in sorted(cv_value.keys()):
+                if 'phi' in cv_value[key]:
+                    at.append(cv_value[key]['phi'])
+                if 'psi' in cv_value[key]:
+                    at.append(cv_value[key]['psi'])
     plm_content = make_restraint_plumed(
         conf=conf, cv_file=cv_file, selected_resid=selected_resid,selected_atomid = selected_atomid,
         kappa=kappa, at=at, stride=stride,
         output=output, mode=mode
     )
     plumed_task_files[plumed_input_name] = (plm_content, "w")
     return plumed_task_files
```

### Comparing `rid-kit-0.6.2/rid/task/task.py` & `rid-kit-0.6.3/rid/task/task.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_bohrium.json` & `rid-kit-0.6.3/rid/template/machine_bohrium.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_bohrium_k8s.json` & `rid-kit-0.6.3/rid/template/machine_bohrium_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_bohrium_k8s_mcmc.json` & `rid-kit-0.6.3/rid/template/machine_bohrium_k8s_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_local_k8s.json` & `rid-kit-0.6.3/rid/template/machine_local_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_slurm_k8s.json` & `rid-kit-0.6.3/rid/template/machine_slurm_k8s.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_slurm_k8s_mcmc.json` & `rid-kit-0.6.3/rid/template/machine_slurm_k8s_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_slurm_local.json` & `rid-kit-0.6.3/rid/template/machine_slurm_local.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/machine_slurm_local_mcmc.json` & `rid-kit-0.6.3/rid/template/machine_slurm_local_mcmc.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_gmx_custom.json` & `rid-kit-0.6.3/rid/template/rid_gmx_custom.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_gmx_dih.json` & `rid-kit-0.6.3/rid/template/rid_gmx_dih.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_gmx_dis.json` & `rid-kit-0.6.3/rid/template/rid_gmx_dis.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_gmx_dp.json` & `rid-kit-0.6.3/rid/template/rid_gmx_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_lmp_dp.json` & `rid-kit-0.6.3/rid/template/rid_lmp_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_lmp_gmx_dp.json` & `rid-kit-0.6.3/rid/template/rid_lmp_gmx_dp.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_mcmc_cv_dis.json` & `rid-kit-0.6.3/rid/template/rid_mcmc_cv_dis.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/template/rid_mcmc_path.json` & `rid-kit-0.6.3/rid/template/rid_mcmc_path.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/tools/estimator.py` & `rid-kit-0.6.3/rid/tools/estimator.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/utils/command.py` & `rid-kit-0.6.3/rid/utils/command.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/utils/files.py` & `rid-kit-0.6.3/rid/utils/files.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/utils/path.py` & `rid-kit-0.6.3/rid/utils/path.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid/utils/set_config.py` & `rid-kit-0.6.3/rid/utils/set_config.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/rid_kit.egg-info/PKG-INFO` & `rid-kit-0.6.3/rid_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rid-kit
-Version: 0.6.2
+Version: 0.6.3
 Summary: RiD package for enhanced sampling
 Home-page: https://github.com/deepmodeling/rid-kit
 Author: Yanze Wang, Jiahao Fan
 Author-email: yanze039@mit.edu,jiahaofan@pku.edu.cn
 License: UNKNOWN
 Keywords: enhanced sampling reinforced dynamics RiD
 Platform: UNKNOWN
```

### Comparing `rid-kit-0.6.2/rid_kit.egg-info/SOURCES.txt` & `rid-kit-0.6.3/rid_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/setup.py` & `rid-kit-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 readme_file = Path(__file__).parent / "README.md"
 readme = readme_file.read_text(encoding="utf-8")
 
 setuptools.setup(
     name='rid-kit',
     author="Yanze Wang, Jiahao Fan",
     author_email="yanze039@mit.edu,jiahaofan@pku.edu.cn",
-    version='0.6.2',
+    version='0.6.3',
     description="RiD package for enhanced sampling",
     setup_requires=['setuptools_scm'],
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/deepmodeling/rid-kit",
     python_requires=">=3.6",
     packages=[
```

### Comparing `rid-kit-0.6.2/tests/context.py` & `rid-kit-0.6.3/tests/context.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/000/conf.gro` & `rid-kit-0.6.3/tests/data/000/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/000/topol.top` & `rid-kit-0.6.3/tests/data/000/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/001/conf.gro` & `rid-kit-0.6.3/tests/data/001/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/001/topol.top` & `rid-kit-0.6.3/tests/data/001/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/conf.gro` & `rid-kit-0.6.3/tests/data/conf.gro`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/models/model_000.pb` & `rid-kit-0.6.3/tests/data/models/model_000.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/models/model_001.pb` & `rid-kit-0.6.3/tests/data/models/model_001.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/models/model_002.pb` & `rid-kit-0.6.3/tests/data/models/model_002.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/models/model_003.pb` & `rid-kit-0.6.3/tests/data/models/model_003.pb`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/plm.out` & `rid-kit-0.6.3/tests/data/plm.out`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/plm_label.out` & `rid-kit-0.6.3/tests/data/plm_label.out`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/rid.json` & `rid-kit-0.6.3/tests/data/rid.json`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/topol.top` & `rid-kit-0.6.3/tests/data/topol.top`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/data/traj_comp.xtc` & `rid-kit-0.6.3/tests/data/traj_comp.xtc`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/mocked_ops.py` & `rid-kit-0.6.3/tests/mocked_ops.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_adjust_trust_l.py` & `rid-kit-0.6.3/tests/op/test_adjust_trust_l.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_prep_data.py` & `rid-kit-0.6.3/tests/op/test_prep_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_prep_explore.py` & `rid-kit-0.6.3/tests/op/test_prep_explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_prep_label.py` & `rid-kit-0.6.3/tests/op/test_prep_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_prep_rid.py` & `rid-kit-0.6.3/tests/op/test_prep_rid.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_prep_select.py` & `rid-kit-0.6.3/tests/op/test_prep_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_recorder.py` & `rid-kit-0.6.3/tests/op/test_recorder.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_run_explore.py` & `rid-kit-0.6.3/tests/op/test_run_explore.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_run_label.py` & `rid-kit-0.6.3/tests/op/test_run_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_run_select.py` & `rid-kit-0.6.3/tests/op/test_run_select.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/test_run_train.py` & `rid-kit-0.6.3/tests/op/test_run_train.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/op/utils.py` & `rid-kit-0.6.3/tests/op/utils.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/test_data.py` & `rid-kit-0.6.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/test_exploration.py` & `rid-kit-0.6.3/tests/test_exploration.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/test_init-block.py` & `rid-kit-0.6.3/tests/test_init-block.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/test_iter-block.py` & `rid-kit-0.6.3/tests/test_iter-block.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/test_label.py` & `rid-kit-0.6.3/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `rid-kit-0.6.2/tests/test_select.py` & `rid-kit-0.6.3/tests/test_select.py`

 * *Files identical despite different names*

