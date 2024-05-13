# Comparing `tmp/ophyd_async-0.3a3.tar.gz` & `tmp/ophyd_async-0.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_async-0.3a3.tar", last modified: Fri May  3 13:43:33 2024, max compression
+gzip compressed data, was "ophyd_async-0.3a4.tar", last modified: Mon May 13 12:05:11 2024, max compression
```

## Comparing `ophyd_async-0.3a3.tar` & `ophyd_async-0.3a4.tar`

### file list

```diff
@@ -1,244 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.663325 ophyd_async-0.3a3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.671325 ophyd_async-0.3a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/_templates/README
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/examples/epics_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/examples/foo_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.675325 ophyd_async-0.3a3/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0003-ophyd-async-migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0004-repository-structure.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0005-respect-black-line-length.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/0006-procedural-device-definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/design-goals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/event-loop-choice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations/flyscanning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/choose-interfaces-for-devices.md
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/compound-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/make-a-simple-device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/make-a-standard-detector.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to/write-tests-for-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/bluesky_ophyd_epics_devices_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/bluesky_ophyd_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   253748 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/hardware-triggered-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/ophyd_favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    89951 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/outer-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)   128990 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/images/simple-hardware-scan.png
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/reference/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/tutorials/using-existing-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.667325 ophyd_async-0.3a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.679325 ophyd_async-0.3a3/src/ophyd_async/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.683325 ophyd_async-0.3a3/src/ophyd_async/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/sim_signal_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.683325 ophyd_async-0.3a3/src/ophyd_async/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.683325 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_aioca.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_p4p.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/_backend/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/aravis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/ad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/vimba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.687325 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/_hdffile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/mover.db
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/demo/sensor.db
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/motion/motor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/pvi/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/pvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/pvi/pvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/epics/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/signal/_epics_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/epics/signal/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/panda/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_common_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/panda/writers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/writers/_hdf_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/panda/writers/_panda_hdf_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.691325 ophyd_async-0.3a3/src/ophyd_async/planstubs/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/planstubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/src/ophyd_async/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/src/ophyd_async/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/demo/sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/src/ophyd_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 13:43:33.000000 ophyd_async-0.3a3/src/ophyd_async.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_async_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_device_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_device_save_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_flyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_standard_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/epics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.695325 ophyd_async-0.3a3/tests/epics/_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/_backend/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/epics/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_aravis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_kinetix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_pilatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_single_trigger_det.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_vimba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/areadetector/test_writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/epics/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/demo/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/demo/test_demo_ad_sim_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/epics/motion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/motion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/motion/test_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/test_pvi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/test_records.db
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/epics/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/panda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/panda/db/
--rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/db/panda.db
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_hdf_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_panda_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_panda_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_panda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/panda/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/protocols/test_protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.699325 ophyd_async-0.3a3/tests/sim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:33.703325 ophyd_async-0.3a3/tests/sim/demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/demo/test_sim_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_pattern_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_sim_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_sim_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/sim/test_streaming_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/test_flyer_with_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-03 13:43:28.000000 ophyd_async-0.3a3/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.814739 ophyd_async-0.3a4/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.774739 ophyd_async-0.3a4/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2926 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-13 12:05:11.814739 ophyd_async-0.3a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.782739 ophyd_async-0.3a4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/_templates/README
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/examples/epics_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/examples/foo_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0003-ophyd-async-migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0004-repository-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0005-respect-black-line-length.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/0006-procedural-device-definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/design-goals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/event-loop-choice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations/flyscanning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.786739 ophyd_async-0.3a4/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/choose-interfaces-for-devices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/compound-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/make-a-simple-device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/make-a-standard-detector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to/write-tests-for-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/bluesky_ophyd_epics_devices_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24931 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/bluesky_ophyd_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   253748 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/hardware-triggered-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/ophyd_favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    89951 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/outer-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)   128990 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/images/simple-hardware-scan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/reference/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/tutorials/using-existing-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:05:11.814739 ophyd_async-0.3a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.774739 ophyd_async-0.3a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.790739 ophyd_async-0.3a4/src/ophyd_async/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/mock_signal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14674 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8794 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_aioca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_p4p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/_backend/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/aravis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.794739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/ad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/pilatus_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/vimba_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/vimba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/_hdfdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/_hdffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/demo_ad_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/mover.db
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/demo/sensor.db
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/motion/motor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/pvi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/pvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/pvi/pvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.798739 ophyd_async-0.3a4/src/ophyd_async/epics/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/signal/_epics_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/epics/signal/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/panda/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_common_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/panda/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/writers/_hdf_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/panda/writers/_panda_hdf_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/planstubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/planstubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/planstubs/prepare_trigger_and_dets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/src/ophyd_async/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/demo/sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.810739 ophyd_async-0.3a4/src/ophyd_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 12:05:11.000000 ophyd_async-0.3a4/src/ophyd_async.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.802739 ophyd_async-0.3a4/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_async_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_device_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_device_save_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_mock_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_soft_signal_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_standard_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/_backend/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_aravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_kinetix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_pilatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_single_trigger_det.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_vimba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/areadetector/test_writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/demo/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/demo/test_demo_ad_sim_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/epics/motion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/motion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/motion/test_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/test_pvi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/test_records.db
+-rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/epics/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/panda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/panda/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/db/panda.db
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_hdf_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_panda_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_panda_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_panda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/panda/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.806739 ophyd_async-0.3a4/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/protocols/test_protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.810739 ophyd_async-0.3a4/tests/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:11.810739 ophyd_async-0.3a4/tests/sim/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/demo/test_sim_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_pattern_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_sim_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_sim_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/sim/test_streaming_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/test_flyer_with_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-13 12:05:08.000000 ophyd_async-0.3a4/tests/test_log.py
```

### Comparing `ophyd_async-0.3a3/.devcontainer/devcontainer.json` & `ophyd_async-0.3a4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/CONTRIBUTING.md` & `ophyd_async-0.3a4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/actions/install_requirements/action.yml` & `ophyd_async-0.3a4/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/dependabot.yml` & `ophyd_async-0.3a4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/pages/make_switcher.py` & `ophyd_async-0.3a4/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/workflows/_check.yml` & `ophyd_async-0.3a4/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/workflows/_dist.yml` & `ophyd_async-0.3a4/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/workflows/_docs.yml` & `ophyd_async-0.3a4/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/workflows/_release.yml` & `ophyd_async-0.3a4/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/workflows/_test.yml` & `ophyd_async-0.3a4/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.github/workflows/ci.yml` & `ophyd_async-0.3a4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.gitignore` & `ophyd_async-0.3a4/.gitignore`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.mailmap` & `ophyd_async-0.3a4/.mailmap`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/.pre-commit-config.yaml` & `ophyd_async-0.3a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/Dockerfile` & `ophyd_async-0.3a4/Dockerfile`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/LICENSE` & `ophyd_async-0.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/PKG-INFO` & `ophyd_async-0.3a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a3
+Version: 0.3a4
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
@@ -44,14 +44,15 @@
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pint
 Requires-Dist: bluesky>=1.13.0a3
 Requires-Dist: event-model<1.21.0
 Requires-Dist: p4p
 Requires-Dist: pyyaml
+Requires-Dist: colorlog
 Provides-Extra: ca
 Requires-Dist: aioca>=1.6; extra == "ca"
 Provides-Extra: pva
 Requires-Dist: p4p; extra == "pva"
 Provides-Extra: dev
 Requires-Dist: ophyd_async[pva]; extra == "dev"
 Requires-Dist: ophyd_async[ca]; extra == "dev"
@@ -83,15 +84,14 @@
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinxcontrib-mermaid; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
-Requires-Dist: colorlog; extra == "dev"
 
 [![CI](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml/badge.svg)](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/bluesky/ophyd-async/branch/main/graph/badge.svg)](https://codecov.io/gh/bluesky/ophyd-async)
 [![PyPI](https://img.shields.io/pypi/v/ophyd-async.svg)](https://pypi.org/project/ophyd-async)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 # ophyd-async
```

### Comparing `ophyd_async-0.3a3/README.md` & `ophyd_async-0.3a4/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/_templates/custom-class-template.rst` & `ophyd_async-0.3a4/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/_templates/custom-module-template.rst` & `ophyd_async-0.3a4/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/conf.py` & `ophyd_async-0.3a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/examples/epics_demo.py` & `ophyd_async-0.3a4/docs/examples/epics_demo.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/examples/foo_detector.py` & `ophyd_async-0.3a4/docs/examples/foo_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `ophyd_async-0.3a4/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/decisions/0003-ophyd-async-migration.rst` & `ophyd_async-0.3a4/docs/explanations/decisions/0003-ophyd-async-migration.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/decisions/0004-repository-structure.rst` & `ophyd_async-0.3a4/docs/explanations/decisions/0004-repository-structure.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/decisions/0005-respect-black-line-length.rst` & `ophyd_async-0.3a4/docs/explanations/decisions/0005-respect-black-line-length.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/decisions/0006-procedural-device-definitions.rst` & `ophyd_async-0.3a4/docs/explanations/decisions/0006-procedural-device-definitions.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/design-goals.rst` & `ophyd_async-0.3a4/docs/explanations/design-goals.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/event-loop-choice.rst` & `ophyd_async-0.3a4/docs/explanations/event-loop-choice.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/explanations/flyscanning.rst` & `ophyd_async-0.3a4/docs/explanations/flyscanning.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/how-to/choose-interfaces-for-devices.md` & `ophyd_async-0.3a4/docs/how-to/choose-interfaces-for-devices.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/how-to/compound-devices.rst` & `ophyd_async-0.3a4/docs/how-to/compound-devices.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/how-to/make-a-simple-device.rst` & `ophyd_async-0.3a4/docs/how-to/make-a-simple-device.rst`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,16 @@
    :pyobject: Sensor
 
 First some Signals are constructed and stored on the Device. Each one is passed
 its Python type, which could be:
 
 - A primitive (`str`, `int`, `float`)
 - An array (`numpy.typing.NDArray` or ``Sequence[str]``)
-- An enum (`enum.Enum`). 
+- An enum (`enum.Enum`) which **must** also extend `str`
+    - `str` and ``EnumClass(str, Enum)`` are the only valid ``datatype`` for an enumerated signal.
 
 The rest of the arguments are PV connection information, in this case the PV suffix.
 
 Finally `super().__init__() <StandardReadable>` is called with:
 
 - Possibly empty Device ``name``: will also dash-prefix its child Device names is set
 - Optional ``primary`` signal: a Signal that should be renamed to take the name
```

### Comparing `ophyd_async-0.3a3/docs/how-to/make-a-standard-detector.rst` & `ophyd_async-0.3a4/docs/how-to/make-a-standard-detector.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/how-to/write-tests-for-devices.rst` & `ophyd_async-0.3a4/docs/how-to/write-tests-for-devices.rst`

 * *Files 11% similar despite different names*

```diff
@@ -17,35 +17,37 @@
 
    # pyproject.toml
 
    [tool.pytest.ini_options]
    ...
    asyncio_mode = "auto"
 
-Sim Backend
------------
+Mock Backend
+------------
 
-Ophyd devices initialized with a sim backend behave in a similar way to mocks, without requiring you to mock out all the dependencies and internals. The `DeviceCollector` can initialize any number of devices, and their signals and sub-devices (recursively), with a sim backend.
+Ophyd devices initialized with a mock backend behave in a similar way to mocks, without requiring you to mock out all the dependencies and internals. The `DeviceCollector` can initialize any number of devices, and their signals and sub-devices (recursively), with a mock backend.
 
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
-   :pyobject: sim_sensor
+   :pyobject: mock_sensor
 
 
-Sim Utility Functions
----------------------
+Mock Utility Functions
+----------------------
 
-Sim signals behave as simply as possible, holding a sensible default value when initialized and retaining any value (in memory) to which they are set. This model breaks down in the case of read-only signals, which cannot be set because there is an expectation of some external device setting them in the real world. There is a utility function, ``set_sim_value``, to mock-set values for sim signals, including read-only ones.
+Mock signals behave as simply as possible, holding a sensible default value when initialized and retaining any value (in memory) to which they are set. This model breaks down in the case of read-only signals, which cannot be set because there is an expectation of some external device setting them in the real world. There is a utility function, ``set_mock_value``, to mock-set values for mock signals, including read-only ones.
 
 In addition this example also utilizes helper functions like ``assert_reading`` and ``assert_value`` to ensure the validity of device readings and values. For more information see: :doc:`API.core<../generated/ophyd_async.core>`
 
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
    :pyobject: test_sensor_reading_shows_value
 
 
-There is another utility function, ``set_sim_callback``, for hooking in logic when a sim value changes (e.g. because someone puts to it).
+There are several other test utility functions:
+
+Use ``callback_on_mock_put``, for hooking in logic when a mock value changes (e.g. because someone puts to it). This can be called directly, or used as a context, with the callbacks ending after exit.
 
 .. literalinclude:: ../../tests/epics/demo/test_demo.py
    :pyobject: test_mover_stopped
 
 
 Testing a Device in a Plan with the RunEngine
 ---------------------------------------------
```

### Comparing `ophyd_async-0.3a3/docs/images/bluesky_ophyd_epics_devices_logo.svg` & `ophyd_async-0.3a4/docs/images/bluesky_ophyd_epics_devices_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/images/bluesky_ophyd_logo.svg` & `ophyd_async-0.3a4/docs/images/bluesky_ophyd_logo.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/images/hardware-triggered-scan.png` & `ophyd_async-0.3a4/docs/images/hardware-triggered-scan.png`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/images/ophyd_favicon.svg` & `ophyd_async-0.3a4/docs/images/ophyd_favicon.svg`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/images/outer-scan.png` & `ophyd_async-0.3a4/docs/images/outer-scan.png`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/images/simple-hardware-scan.png` & `ophyd_async-0.3a4/docs/images/simple-hardware-scan.png`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/index.md` & `ophyd_async-0.3a4/docs/index.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/reference/api.rst` & `ophyd_async-0.3a4/docs/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/tutorials/installation.md` & `ophyd_async-0.3a4/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/docs/tutorials/using-existing-devices.rst` & `ophyd_async-0.3a4/docs/tutorials/using-existing-devices.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 - If ``set_name=True`` (the default), then call `Device.set_name` passing the
   name of the variable within the context. For example, here we call
   ``det.set_name("det")``
 - If ``connect=True`` (the default), then call `Device.connect` in parallel for
   all top level Devices, waiting for up to ``timeout`` seconds. For example,
   here we call ``asyncio.wait([det.connect(), samp.connect()])``
-- If ``sim=True`` is passed, then don't connect to PVs, but set Devices into
+- If ``mock=True`` is passed, then don't connect to PVs, but set Devices into
   simulation mode
 
 The Devices we create in this example are a "sample stage" with a couple of
 "movers" called ``x`` and ``y`` and a "sensor" called ``det`` that gives a
 different reading depending on the position of the "movers".
 
 .. note::
```

### Comparing `ophyd_async-0.3a3/pyproject.toml` & `ophyd_async-0.3a4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "numpy",
     "packaging",
     "pint",
     "bluesky>=1.13.0a3",
     "event-model<1.21.0",
     "p4p",
     "pyyaml",
+    "colorlog",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
@@ -60,15 +61,14 @@
     "sphinx-autobuild",
     "sphinxcontrib-mermaid",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
     "types-pyyaml",
-    "colorlog"
 ]
 
 [project.scripts]
 ophyd-async = "ophyd_async.__main__:main"
 
 [project.urls]
 GitHub = "https://github.com/bluesky/ophyd-async"
@@ -82,15 +82,14 @@
 write_to = "src/ophyd_async/_version.py"
 
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
     --tb=native -vv --strict-markers --doctest-modules
     --doctest-glob="*.rst" --doctest-glob="*.md" --ignore=docs/examples
-    --cov=src/ophyd_async --cov-report term --cov-report xml:cov.xml
     """
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = "error"
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 log_format = "%(asctime)s,%(msecs)03d %(levelname)s (%(threadName)s) %(message)s"
 log_date_format = "%H:%M:%S"
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/__init__.py` & `ophyd_async-0.3a4/src/ophyd_async/core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,70 +20,84 @@
     load_from_yaml,
     save_device,
     save_to_yaml,
     set_signal_values,
     walk_rw_signals,
 )
 from .flyer import HardwareTriggeredFlyable, TriggerLogic
+from .mock_signal_backend import (
+    MockSignalBackend,
+)
+from .mock_signal_utils import (
+    assert_mock_put_called_with,
+    callback_on_mock_put,
+    mock_puts_blocked,
+    reset_mock_put_calls,
+    set_mock_put_proceeds,
+    set_mock_value,
+    set_mock_values,
+)
 from .signal import (
     Signal,
     SignalR,
     SignalRW,
     SignalW,
     SignalX,
     assert_configuration,
     assert_emitted,
     assert_reading,
     assert_value,
     observe_value,
     set_and_wait_for_value,
-    set_sim_callback,
-    set_sim_put_proceeds,
-    set_sim_value,
-    soft_signal_r_and_backend,
+    soft_signal_r_and_setter,
     soft_signal_rw,
     wait_for_value,
 )
 from .signal_backend import SignalBackend
-from .sim_signal_backend import SimSignalBackend
+from .soft_signal_backend import SoftSignalBackend
 from .standard_readable import ConfigSignal, HintedSignal, StandardReadable
 from .utils import (
     DEFAULT_TIMEOUT,
     Callback,
     NotConnected,
     ReadingValueCallback,
     T,
     get_dtype,
     get_unique,
     merge_gathered_dicts,
     wait_for_connection,
 )
 
 __all__ = [
+    "assert_mock_put_called_with",
+    "callback_on_mock_put",
+    "mock_puts_blocked",
+    "set_mock_values",
+    "reset_mock_put_calls",
     "SignalBackend",
-    "SimSignalBackend",
+    "SoftSignalBackend",
     "DetectorControl",
+    "MockSignalBackend",
     "DetectorTrigger",
     "DetectorWriter",
     "StandardDetector",
     "Device",
     "DeviceCollector",
     "DeviceVector",
     "Signal",
     "SignalR",
     "SignalW",
     "SignalRW",
     "SignalX",
-    "soft_signal_r_and_backend",
+    "soft_signal_r_and_setter",
     "soft_signal_rw",
     "observe_value",
     "set_and_wait_for_value",
-    "set_sim_callback",
-    "set_sim_put_proceeds",
-    "set_sim_value",
+    "set_mock_put_proceeds",
+    "set_mock_value",
     "wait_for_value",
     "AsyncStatus",
     "DirectoryInfo",
     "DirectoryProvider",
     "NameProvider",
     "ShapeProvider",
     "StaticDirectoryProvider",
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/_providers.py` & `ophyd_async-0.3a4/src/ophyd_async/core/_providers.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/async_status.py` & `ophyd_async-0.3a4/src/ophyd_async/core/async_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         awaitable: Awaitable,
         watchers: Optional[List[Callable]] = None,
     ):
         if isinstance(awaitable, asyncio.Task):
             self.task = awaitable
         else:
             self.task = asyncio.create_task(awaitable)  # type: ignore
+
         self.task.add_done_callback(self._run_callbacks)
+
         self._callbacks = cast(List[Callback[Status]], [])
         self._watchers = watchers
 
     def __await__(self):
         return self.task.__await__()
 
     def add_callback(self, callback: Callback[Status]):
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/detector.py` & `ophyd_async-0.3a4/src/ophyd_async/core/detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/device.py` & `ophyd_async-0.3a4/src/ophyd_async/core/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Base device"""
 
 from __future__ import annotations
 
 import sys
+from functools import cached_property
+from logging import LoggerAdapter, getLogger
 from typing import (
     Any,
     Coroutine,
     Dict,
     Generator,
     Iterator,
     Optional,
@@ -35,47 +37,58 @@
         self.set_name(name)
 
     @property
     def name(self) -> str:
         """Return the name of the Device"""
         return self._name
 
+    @cached_property
+    def log(self):
+        return LoggerAdapter(
+            getLogger("ophyd_async.devices"), {"ophyd_async_device_name": self.name}
+        )
+
     def children(self) -> Iterator[Tuple[str, Device]]:
         for attr_name, attr in self.__dict__.items():
             if attr_name != "parent" and isinstance(attr, Device):
                 yield attr_name, attr
 
     def set_name(self, name: str):
         """Set ``self.name=name`` and each ``self.child.name=name+"-child"``.
 
         Parameters
         ----------
         name:
             New name to set
         """
+
+        # Ensure self.log is recreated after a name change
+        if hasattr(self, "log"):
+            del self.log
+
         self._name = name
         for attr_name, child in self.children():
             child_name = f"{name}-{attr_name.rstrip('_')}" if name else ""
             child.set_name(child_name)
             child.parent = self
 
-    async def connect(self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT):
+    async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
         """Connect self and all child Devices.
 
         Contains a timeout that gets propagated to child.connect methods.
 
         Parameters
         ----------
-        sim:
-            If True then connect in simulation mode.
+        mock:
+            If True then use ``MockSignalBackend`` for all Signals
         timeout:
             Time to wait before failing with a TimeoutError.
         """
         coros = {
-            name: child_device.connect(sim, timeout=timeout)
+            name: child_device.connect(mock=mock, timeout=timeout)
             for name, child_device in self.children()
         }
         if coros:
             await wait_for_connection(**coros)
 
 
 VT = TypeVar("VT", bound=Device)
@@ -101,17 +114,17 @@
 
     Parameters
     ----------
     set_name:
         If True, call ``device.set_name(variable_name)`` on all collected
         Devices
     connect:
-        If True, call ``device.connect(sim)`` in parallel on all
+        If True, call ``device.connect(mock)`` in parallel on all
         collected Devices
-    sim:
+    mock:
         If True, connect Signals in simulation mode
     timeout:
         How long to wait for connect before logging an exception
 
     Notes
     -----
     Example usage::
@@ -125,20 +138,20 @@
 
     """
 
     def __init__(
         self,
         set_name=True,
         connect=True,
-        sim=False,
+        mock=False,
         timeout: float = 10.0,
     ):
         self._set_name = set_name
         self._connect = connect
-        self._sim = sim
+        self._mock = mock
         self._timeout = timeout
         self._names_on_enter: Set[str] = set()
         self._objects_on_exit: Dict[str, Any] = {}
 
     def _caller_locals(self):
         """Walk up until we find a stack frame that doesn't have us as self"""
         try:
@@ -164,15 +177,15 @@
         connect_coroutines: Dict[str, Coroutine] = {}
         for name, obj in self._objects_on_exit.items():
             if name not in self._names_on_enter and isinstance(obj, Device):
                 if self._set_name and not obj.name:
                     obj.set_name(name)
                 if self._connect:
                     connect_coroutines[name] = obj.connect(
-                        self._sim, timeout=self._timeout
+                        self._mock, timeout=self._timeout
                     )
 
         # Connect to all the devices
         if connect_coroutines:
             await wait_for_connection(**connect_coroutines)
 
     async def __aexit__(self, type, value, traceback):
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/device_save_loader.py` & `ophyd_async-0.3a4/src/ophyd_async/core/device_save_loader.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/flyer.py` & `ophyd_async-0.3a4/src/ophyd_async/core/flyer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/signal.py` & `ophyd_async-0.3a4/src/ophyd_async/core/signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,22 @@
     Locatable,
     Location,
     Movable,
     Reading,
     Subscribable,
 )
 
+from ophyd_async.core.mock_signal_backend import MockSignalBackend
 from ophyd_async.protocols import AsyncConfigurable, AsyncReadable, AsyncStageable
 
 from .async_status import AsyncStatus
 from .device import Device
 from .signal_backend import SignalBackend
-from .sim_signal_backend import SimSignalBackend
-from .utils import DEFAULT_TIMEOUT, Callback, ReadingValueCallback, T
-
-_sim_backends: Dict[Signal, SimSignalBackend] = {}
+from .soft_signal_backend import SoftSignalBackend
+from .utils import DEFAULT_TIMEOUT, Callback, T
 
 
 def _add_timeout(func):
     @functools.wraps(func)
     async def wrapper(self: Signal, *args, **kwargs):
         return await asyncio.wait_for(func(self, *args, **kwargs), self._timeout)
 
@@ -57,25 +56,25 @@
 
     def __init__(
         self,
         backend: SignalBackend[T],
         timeout: Optional[float] = DEFAULT_TIMEOUT,
         name: str = "",
     ) -> None:
-        super().__init__(name)
         self._timeout = timeout
-        self._init_backend = self._backend = backend
+        self._initial_backend = self._backend = backend
+        super().__init__(name)
 
-    async def connect(self, sim=False, timeout=DEFAULT_TIMEOUT):
-        if sim:
-            self._backend = SimSignalBackend(datatype=self._init_backend.datatype)
-            _sim_backends[self] = self._backend
-        else:
-            self._backend = self._init_backend
-            _sim_backends.pop(self, None)
+    async def connect(self, mock=False, timeout=DEFAULT_TIMEOUT):
+        if mock and not isinstance(self._backend, MockSignalBackend):
+            # Using a soft backend, look to the initial value
+            self._backend = MockSignalBackend(
+                initial_backend=self._initial_backend,
+            )
+        self.log.debug(f"Connecting to {self.source}")
         await self._backend.connect(timeout=timeout)
 
     @property
     def source(self) -> str:
         """Like ca://PV_PREFIX:SIGNAL, or "" if not set"""
         return self._backend.source(self.name)
 
@@ -92,30 +91,36 @@
         self._staged = False
         self._listeners: Dict[Callback, bool] = {}
         self._valid = asyncio.Event()
         self._reading: Optional[Reading] = None
         self._value: Optional[T] = None
 
         self.backend = backend
+        signal.log.debug(f"Making subscription on source {signal.source}")
         backend.set_callback(self._callback)
 
     def close(self):
         self.backend.set_callback(None)
+        self._signal.log.debug(f"Closing subscription on source {self._signal.source}")
 
     async def get_reading(self) -> Reading:
         await self._valid.wait()
         assert self._reading is not None, "Monitor not working"
         return self._reading
 
     async def get_value(self) -> T:
         await self._valid.wait()
         assert self._value is not None, "Monitor not working"
         return self._value
 
     def _callback(self, reading: Reading, value: T):
+        self._signal.log.debug(
+            f"Updated subscription: reading of source {self._signal.source} changed"
+            f"from {self._reading} to {reading}"
+        )
         self._reading = reading
         self._value = value
         self._valid.set()
         for function, want_value in self._listeners.items():
             self._notify(function, want_value)
 
     def _notify(self, function: Callback, want_value: bool):
@@ -174,15 +179,17 @@
     async def describe(self) -> Dict[str, DataKey]:
         """Return a single item dict with the descriptor in it"""
         return {self.name: await self._backend.get_datakey(self.source)}
 
     @_add_timeout
     async def get_value(self, cached: Optional[bool] = None) -> T:
         """The current value"""
-        return await self._backend_or_cache(cached).get_value()
+        value = await self._backend_or_cache(cached).get_value()
+        self.log.debug(f"get_value() on source {self.source} returned {value}")
+        return value
 
     def subscribe_value(self, function: Callback[T]):
         """Subscribe to updates in value of a device"""
         self._get_cache().subscribe(function, want_value=True)
 
     def subscribe(self, function: Callback[Dict[str, Reading]]) -> None:
         """Subscribe to updates in the reading"""
@@ -209,16 +216,23 @@
 class SignalW(Signal[T], Movable):
     """Signal that can be set"""
 
     def set(self, value: T, wait=True, timeout=USE_DEFAULT_TIMEOUT) -> AsyncStatus:
         """Set the value and return a status saying when it's done"""
         if timeout is USE_DEFAULT_TIMEOUT:
             timeout = self._timeout
-        coro = self._backend.put(value, wait=wait, timeout=timeout)
-        return AsyncStatus(coro)
+
+        async def do_set():
+            self.log.debug(f"Putting value {value} to backend at source {self.source}")
+            await self._backend.put(value, wait=wait, timeout=timeout)
+            self.log.debug(
+                f"Successfully put value {value} to backend at source {self.source}"
+            )
+
+        return AsyncStatus(do_set())
 
 
 class SignalRW(SignalR[T], SignalW[T], Locatable):
     """Signal that can be both read and set"""
 
     async def locate(self) -> Location:
         location: Location = {
@@ -235,55 +249,37 @@
         """Trigger the action and return a status saying when it's done"""
         if timeout is USE_DEFAULT_TIMEOUT:
             timeout = self._timeout
         coro = self._backend.put(None, wait=wait, timeout=timeout)
         return AsyncStatus(coro)
 
 
-def set_sim_value(signal: Signal[T], value: T):
-    """Set the value of a signal that is in sim mode."""
-    _sim_backends[signal]._set_value(value)
-
-
-def set_sim_put_proceeds(signal: Signal[T], proceeds: bool):
-    """Allow or block a put with wait=True from proceeding"""
-    event = _sim_backends[signal].put_proceeds
-    if proceeds:
-        event.set()
-    else:
-        event.clear()
-
-
-def set_sim_callback(signal: Signal[T], callback: ReadingValueCallback[T]) -> None:
-    """Monitor the value of a signal that is in sim mode"""
-    return _sim_backends[signal].set_callback(callback)
-
-
 def soft_signal_rw(
     datatype: Optional[Type[T]] = None,
     initial_value: Optional[T] = None,
     name: str = "",
 ) -> SignalRW[T]:
-    """Creates a read-writable Signal with a SimSignalBackend"""
-    signal = SignalRW(SimSignalBackend(datatype, initial_value), name=name)
+    """Creates a read-writable Signal with a SoftSignalBackend"""
+    signal = SignalRW(SoftSignalBackend(datatype, initial_value), name=name)
     return signal
 
 
-def soft_signal_r_and_backend(
+def soft_signal_r_and_setter(
     datatype: Optional[Type[T]] = None,
     initial_value: Optional[T] = None,
     name: str = "",
-) -> Tuple[SignalR[T], SimSignalBackend]:
-    """Returns a tuple of a read-only Signal and its SimSignalBackend through
+) -> Tuple[SignalR[T], Callable[[T]]]:
+    """Returns a tuple of a read-only Signal and a callable through
     which the signal can be internally modified within the device. Use
     soft_signal_rw if you want a device that is externally modifiable
     """
-    backend = SimSignalBackend(datatype, initial_value)
+    backend = SoftSignalBackend(datatype, initial_value)
     signal = SignalR(backend, name=name)
-    return (signal, backend)
+
+    return (signal, backend.set_value)
 
 
 async def assert_value(signal: SignalR[T], value: Any) -> None:
     """Assert a signal's value and compare it an expected signal.
 
     Parameters
     ----------
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/signal_backend.py` & `ophyd_async-0.3a4/src/ophyd_async/core/signal_backend.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/sim_signal_backend.py` & `ophyd_async-0.3a4/src/ophyd_async/core/soft_signal_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
-import asyncio
 import inspect
 import time
 from collections import abc
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, Generic, Optional, Type, Union, cast, get_origin
+from typing import Dict, Generic, Optional, Type, Union, cast, get_origin
 
 import numpy as np
 from bluesky.protocols import DataKey, Dtype, Reading
 
 from .signal_backend import SignalBackend
 from .utils import DEFAULT_TIMEOUT, ReadingValueCallback, T, get_dtype
 
@@ -18,15 +17,15 @@
     str: "string",
     int: "integer",
     float: "number",
     bool: "boolean",
 }
 
 
-class SimConverter(Generic[T]):
+class SoftConverter(Generic[T]):
     def value(self, value: T) -> T:
         return value
 
     def write_value(self, value: T) -> T:
         return value
 
     def reading(self, value: T, timestamp: float, severity: int) -> Reading:
@@ -51,30 +50,30 @@
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         return datatype()
 
 
-class SimArrayConverter(SimConverter):
+class SoftArrayConverter(SoftConverter):
     def get_datakey(self, source: str, value) -> DataKey:
         return {"source": source, "dtype": "array", "shape": [len(value)]}
 
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         if get_origin(datatype) == abc.Sequence:
             return cast(T, [])
 
         return cast(T, datatype(shape=0))  # type: ignore
 
 
 @dataclass
-class SimEnumConverter(SimConverter):
+class SoftEnumConverter(SoftConverter):
     enum_class: Type[Enum]
 
     def write_value(self, value: Union[Enum, str]) -> Enum:
         if isinstance(value, Enum):
             return value
         else:
             return self.enum_class(value)
@@ -86,79 +85,70 @@
     def make_initial_value(self, datatype: Optional[Type[T]]) -> T:
         if datatype is None:
             return cast(T, None)
 
         return cast(T, list(datatype.__members__.values())[0])  # type: ignore
 
 
-class DisconnectedSimConverter(SimConverter):
-    def __getattribute__(self, __name: str) -> Any:
-        raise NotImplementedError("No PV has been set as connect() has not been called")
-
-
 def make_converter(datatype):
     is_array = get_dtype(datatype) is not None
     is_sequence = get_origin(datatype) == abc.Sequence
     is_enum = issubclass(datatype, Enum) if inspect.isclass(datatype) else False
 
     if is_array or is_sequence:
-        return SimArrayConverter()
+        return SoftArrayConverter()
     if is_enum:
-        return SimEnumConverter(datatype)
+        return SoftEnumConverter(datatype)
 
-    return SimConverter()
+    return SoftConverter()
 
 
-class SimSignalBackend(SignalBackend[T]):
-    """An simulated backend to a Signal, created with ``Signal.connect(sim=True)``"""
+class SoftSignalBackend(SignalBackend[T]):
+    """An backend to a soft Signal, for test signals see ``MockSignalBackend``."""
 
     _value: T
     _initial_value: Optional[T]
     _timestamp: float
     _severity: int
 
     def __init__(
         self,
         datatype: Optional[Type[T]],
         initial_value: Optional[T] = None,
     ) -> None:
         self.datatype = datatype
-        self.converter: SimConverter = DisconnectedSimConverter()
         self._initial_value = initial_value
-        self.put_proceeds = asyncio.Event()
-        self.put_proceeds.set()
-        self.callback: Optional[ReadingValueCallback[T]] = None
-
-    def source(self, name: str) -> str:
-        return f"soft://{name}"
-
-    async def connect(self, timeout: float = DEFAULT_TIMEOUT) -> None:
-        self.converter = make_converter(self.datatype)
+        self.converter: SoftConverter = make_converter(datatype)
         if self._initial_value is None:
             self._initial_value = self.converter.make_initial_value(self.datatype)
         else:
-            # convert potentially unconverted initial value passed to init method
             self._initial_value = self.converter.write_value(self._initial_value)
+
+        self.callback: Optional[ReadingValueCallback[T]] = None
         self._severity = 0
+        self.set_value(self._initial_value)
 
-        await self.put(None)
+    def source(self, name: str) -> str:
+        return f"soft://{name}"
+
+    async def connect(self, timeout: float = DEFAULT_TIMEOUT) -> None:
+        """Connection isn't required for soft signals."""
+        pass
 
     async def put(self, value: Optional[T], wait=True, timeout=None):
         write_value = (
             self.converter.write_value(value)
             if value is not None
             else self._initial_value
         )
-        self._set_value(write_value)
 
-        if wait:
-            await asyncio.wait_for(self.put_proceeds.wait(), timeout)
+        self.set_value(write_value)
 
-    def _set_value(self, value: T):
-        """Method to bypass asynchronous logic, designed to only be used in tests."""
+    def set_value(self, value: T):
+        """Method to bypass asynchronous logic."""
         self._value = value
         self._timestamp = time.monotonic()
         reading: Reading = self.converter.reading(
             self._value, self._timestamp, self._severity
         )
 
         if self.callback:
@@ -170,15 +160,15 @@
     async def get_reading(self) -> Reading:
         return self.converter.reading(self._value, self._timestamp, self._severity)
 
     async def get_value(self) -> T:
         return self.converter.value(self._value)
 
     async def get_setpoint(self) -> T:
-        """For a simulated backend, the setpoint and readback values are the same."""
+        """For a soft signal, the setpoint and readback values are the same."""
         return await self.get_value()
 
     def set_callback(self, callback: Optional[ReadingValueCallback[T]]) -> None:
         if callback:
             assert not self.callback, "Cannot set a callback when one is already set"
             reading: Reading = self.converter.reading(
                 self._value, self._timestamp, self._severity
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/standard_readable.py` & `ophyd_async-0.3a4/src/ophyd_async/core/standard_readable.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/core/utils.py` & `ophyd_async-0.3a4/src/ophyd_async/core/utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_aioca.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_aioca.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     T,
     get_dtype,
     get_unique,
     wait_for_connection,
 )
 from ophyd_async.core.utils import DEFAULT_TIMEOUT, NotConnected
 
-from .common import get_supported_enum_class
+from .common import get_supported_values
 
 dbr_to_dtype: Dict[Dbr, Dtype] = {
     dbr.DBR_STRING: "string",
     dbr.DBR_SHORT: "integer",
     dbr.DBR_FLOAT: "number",
     dbr.DBR_CHAR: "string",
     dbr.DBR_LONG: "integer",
@@ -75,28 +75,32 @@
 class CaArrayConverter(CaConverter):
     def get_datakey(self, source: str, value: AugmentedValue) -> DataKey:
         return {"source": source, "dtype": "array", "shape": [len(value)]}
 
 
 @dataclass
 class CaEnumConverter(CaConverter):
-    enum_class: Type[Enum]
+    choices: dict[str, str]
 
     def write_value(self, value: Union[Enum, str]):
         if isinstance(value, Enum):
             return value.value
         else:
             return value
 
     def value(self, value: AugmentedValue):
-        return self.enum_class(value)
+        return self.choices[value]
 
     def get_datakey(self, source: str, value: AugmentedValue) -> DataKey:
-        choices = [e.value for e in self.enum_class]
-        return {"source": source, "dtype": "string", "shape": [], "choices": choices}
+        return {
+            "source": source,
+            "dtype": "string",
+            "shape": [],
+            "choices": list(self.choices),
+        }
 
 
 class DisconnectedCaConverter(CaConverter):
     def __getattribute__(self, __name: str) -> Any:
         raise NotImplementedError("No PV has been set as connect() has not been called")
 
 
@@ -134,16 +138,16 @@
             raise TypeError(f"{pv} has {pv_choices_len} choices, can't map to bool")
         return CaConverter(dbr.DBR_SHORT, dbr.DBR_SHORT)
     elif pv_dbr == dbr.DBR_ENUM:
         # This is an Enum
         pv_choices = get_unique(
             {k: tuple(v.enums) for k, v in values.items()}, "choices"
         )
-        enum_class = get_supported_enum_class(pv, datatype, pv_choices)
-        return CaEnumConverter(dbr.DBR_STRING, None, enum_class)
+        supported_values = get_supported_values(pv, datatype, pv_choices)
+        return CaEnumConverter(dbr.DBR_STRING, None, supported_values)
     else:
         value = list(values.values())[0]
         # Done the dbr check, so enough to check one of the values
         if datatype and not isinstance(value, datatype):
             raise TypeError(
                 f"{pv} has type {type(value).__name__.replace('ca_', '')} "
                 + f"not {datatype.__name__}"
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/_backend/_p4p.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/_backend/_p4p.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     T,
     get_dtype,
     get_unique,
     wait_for_connection,
 )
 from ophyd_async.core.utils import DEFAULT_TIMEOUT, NotConnected
 
-from .common import get_supported_enum_class
+from .common import get_supported_values
 
 # https://mdavidsaver.github.io/p4p/values.html
 specifier_to_dtype: Dict[str, Dtype] = {
     "?": "integer",  # bool
     "b": "integer",  # int8
     "B": "integer",  # uint8
     "h": "integer",  # int16
@@ -105,28 +105,33 @@
         # complexities around flattening to 1-D - e.g. dimension-order.
         # Don't support this for now.
         raise TypeError("Writing to NDArray not supported")
 
 
 @dataclass
 class PvaEnumConverter(PvaConverter):
-    enum_class: Type[Enum]
+    def __init__(self, choices: dict[str, str]):
+        self.choices = tuple(choices.values())
 
     def write_value(self, value: Union[Enum, str]):
         if isinstance(value, Enum):
             return value.value
         else:
             return value
 
     def value(self, value):
-        return list(self.enum_class)[value["value"]["index"]]
+        return self.choices[value["value"]["index"]]
 
     def get_datakey(self, source: str, value) -> DataKey:
-        choices = [e.value for e in self.enum_class]
-        return {"source": source, "dtype": "string", "shape": [], "choices": choices}
+        return {
+            "source": source,
+            "dtype": "string",
+            "shape": [],
+            "choices": list(self.choices),
+        }
 
 
 class PvaEnumBoolConverter(PvaConverter):
     def value(self, value):
         return value["value"]["index"]
 
     def get_datakey(self, source: str, value) -> DataKey:
@@ -210,15 +215,15 @@
             raise TypeError(f"{pv} has {pv_choices_len} choices, can't map to bool")
         return PvaEnumBoolConverter()
     elif "NTEnum" in typeid:
         # This is an Enum
         pv_choices = get_unique(
             {k: tuple(v["value"]["choices"]) for k, v in values.items()}, "choices"
         )
-        return PvaEnumConverter(get_supported_enum_class(pv, datatype, pv_choices))
+        return PvaEnumConverter(get_supported_values(pv, datatype, pv_choices))
     elif "NTScalar" in typeid:
         if (
             datatype
             and not issubclass(typ, datatype)
             and not (
                 typ is float and datatype is int
             )  # Allow float -> int since prec can be 0
@@ -240,15 +245,14 @@
         self.datatype = datatype
         self.read_pv = read_pv
         self.write_pv = write_pv
         self.initial_values: Dict[str, Any] = {}
         self.converter: PvaConverter = DisconnectedPvaConverter()
         self.subscription: Optional[Subscription] = None
 
-    @property
     def source(self, name: str):
         return f"pva://{self.read_pv}"
 
     @property
     def ctxt(self) -> Context:
         if PvaSignalBackend._ctxt is None:
             PvaSignalBackend._ctxt = Context("pva", nt=False)
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/aravis.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/aravis.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/ad_sim_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/aravis_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/kinetix_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/pilatus_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/controllers/vimba_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/ad_base.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/ad_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     AsyncStatus,
     ShapeProvider,
     set_and_wait_for_value,
 )
 
-from ...signal.signal import epics_signal_rw
-from ..utils import ImageMode, ad_r, ad_rw
+from ...signal.signal import epics_signal_r, epics_signal_rw, epics_signal_rw_rbv
+from ..utils import ImageMode
 from ..writers.nd_plugin import NDArrayBase
 
 
 class DetectorState(str, Enum):
     """
     Default set of states of an AreaDetector driver.
     See definition in ADApp/ADSrc/ADDriver.h in https://github.com/areaDetector/ADCore
@@ -39,22 +39,24 @@
     [DetectorState.Idle, DetectorState.Aborted]
 )
 
 
 class ADBase(NDArrayBase):
     def __init__(self, prefix: str, name: str = "") -> None:
         # Define some signals
-        self.acquire = ad_rw(bool, prefix + "Acquire")
-        self.acquire_time = ad_rw(float, prefix + "AcquireTime")
-        self.num_images = ad_rw(int, prefix + "NumImages")
-        self.image_mode = ad_rw(ImageMode, prefix + "ImageMode")
-        self.array_counter = ad_rw(int, prefix + "ArrayCounter")
-        self.array_size_x = ad_r(int, prefix + "ArraySizeX")
-        self.array_size_y = ad_r(int, prefix + "ArraySizeY")
-        self.detector_state = ad_r(DetectorState, prefix + "DetectorState")
+        self.acquire = epics_signal_rw_rbv(bool, prefix + "Acquire")
+        self.acquire_time = epics_signal_rw_rbv(float, prefix + "AcquireTime")
+        self.num_images = epics_signal_rw_rbv(int, prefix + "NumImages")
+        self.image_mode = epics_signal_rw_rbv(ImageMode, prefix + "ImageMode")
+        self.array_counter = epics_signal_rw_rbv(int, prefix + "ArrayCounter")
+        self.array_size_x = epics_signal_r(int, prefix + "ArraySizeX_RBV")
+        self.array_size_y = epics_signal_r(int, prefix + "ArraySizeY_RBV")
+        self.detector_state = epics_signal_r(
+            DetectorState, prefix + "DetectorState_RBV"
+        )
         # There is no _RBV for this one
         self.wait_for_plugins = epics_signal_rw(bool, prefix + "WaitForPlugins")
         super().__init__(prefix, name=name)
 
 
 async def start_acquiring_driver_and_ensure_status(
     driver: ADBase,
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/aravis_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from typing import Callable, Dict, Literal, Optional, Tuple
 
 from ophyd_async.epics.areadetector.drivers import ADBase
-from ophyd_async.epics.areadetector.utils import ad_r, ad_rw
+from ophyd_async.epics.signal.signal import epics_signal_r, epics_signal_rw_rbv
 
 
 class AravisTriggerMode(str, Enum):
     """GigEVision GenICAM standard: on=externally triggered"""
 
     on = "On"
     off = "Off"
@@ -134,18 +134,20 @@
     """Generic Driver supporting the Manta and Mako drivers.
     Fetches deadtime prior to use in a Streaming scan.
     Requires driver firmware up to date:
     - Model_RBV must be of the form "^(Mako|Manta) (model)$"
     """
 
     def __init__(self, prefix: str, name: str = "") -> None:
-        self.trigger_mode = ad_rw(AravisTriggerMode, prefix + "TriggerMode")
-        self.trigger_source = ad_rw(str, prefix + "TriggerSource")
-        self.model = ad_r(str, prefix + "Model")
-        self.pixel_format = ad_rw(str, prefix + "PixelFormat")
+        self.trigger_mode = epics_signal_rw_rbv(
+            AravisTriggerMode, prefix + "TriggerMode"
+        )
+        self.trigger_source = epics_signal_rw_rbv(str, prefix + "TriggerSource")
+        self.model = epics_signal_r(str, prefix + "Model_RBV")
+        self.pixel_format = epics_signal_rw_rbv(str, prefix + "PixelFormat")
         self.dead_time: Optional[float] = None
         super().__init__(prefix, name=name)
 
     async def fetch_deadtime(self) -> None:
         # All known in-use version B/C have same deadtime as non-B/C
         model: str = (await self.model.get_value()).removesuffix("B").removesuffix("C")
         if model not in _deadtimes:
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/drivers/kinetix_driver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import Enum
 
-from ..utils import ad_rw
+from ophyd_async.epics.signal.signal import epics_signal_rw_rbv
+
 from .ad_base import ADBase
 
 
 class KinetixTriggerMode(str, Enum):
     internal = "Internal"
     edge = "Rising Edge"
     gate = "Exp. Gate"
@@ -14,11 +15,13 @@
     sensitivity = 1
     speed = 2
     dynamic_range = 3
 
 
 class KinetixDriver(ADBase):
     def __init__(self, prefix: str, name: str = "") -> None:
-        # self.pixel_format = ad_rw(PixelFormat, prefix + "PixelFormat")
-        self.trigger_mode = ad_rw(KinetixTriggerMode, prefix + "TriggerMode")
-        self.mode = ad_rw(KinetixReadoutMode, prefix + "ReadoutPortIdx")
+        # self.pixel_format = epics_signal_rw_rbv(PixelFormat, prefix + "PixelFormat")
+        self.trigger_mode = epics_signal_rw_rbv(
+            KinetixTriggerMode, prefix + "TriggerMode"
+        )
+        self.mode = epics_signal_rw_rbv(KinetixReadoutMode, prefix + "ReadoutPortIdx")
         super().__init__(prefix, name)
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/kinetix.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/kinetix.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/pilatus.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/pilatus.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/single_trigger_det.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/single_trigger_det.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/utils.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 from enum import Enum
-from typing import Optional, Type
+from typing import Optional
 from xml.etree import cElementTree as ET
 
-from ophyd_async.core import DEFAULT_TIMEOUT, SignalR, SignalRW, T, wait_for_value
-
-from ..signal.signal import epics_signal_r, epics_signal_rw
-
-
-def ad_rw(datatype: Type[T], prefix: str) -> SignalRW[T]:
-    return epics_signal_rw(datatype, prefix + "_RBV", prefix)
-
-
-def ad_r(datatype: Type[T], prefix: str) -> SignalR[T]:
-    return epics_signal_r(datatype, prefix + "_RBV")
+from ophyd_async.core import DEFAULT_TIMEOUT, SignalRW, T, wait_for_value
 
 
 class FileWriteMode(str, Enum):
     single = "Single"
     capture = "Capture"
     stream = "Stream"
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/vimba.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/vimba.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/_hdffile.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/_hdffile.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/hdf_writer.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/hdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_file_hdf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
-from ...signal.signal import epics_signal_rw
-from ..utils import FileWriteMode, ad_r, ad_rw
+from ...signal.signal import epics_signal_r, epics_signal_rw, epics_signal_rw_rbv
+from ..utils import FileWriteMode
 from .nd_plugin import NDPluginBase
 
 
 class Compression(str, Enum):
     none = "None"
     nbit = "N-bit"
     szip = "szip"
@@ -15,26 +15,28 @@
     lz4 = "LZ4"
     jpeg = "JPEG"
 
 
 class NDFileHDF(NDPluginBase):
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
-        self.position_mode = ad_rw(bool, prefix + "PositionMode")
-        self.compression = ad_rw(Compression, prefix + "Compression")
-        self.num_extra_dims = ad_rw(int, prefix + "NumExtraDims")
-        self.file_path = ad_rw(str, prefix + "FilePath")
-        self.file_name = ad_rw(str, prefix + "FileName")
-        self.file_path_exists = ad_r(bool, prefix + "FilePathExists")
-        self.file_template = ad_rw(str, prefix + "FileTemplate")
-        self.full_file_name = ad_r(str, prefix + "FullFileName")
-        self.file_write_mode = ad_rw(FileWriteMode, prefix + "FileWriteMode")
-        self.num_capture = ad_rw(int, prefix + "NumCapture")
-        self.num_captured = ad_r(int, prefix + "NumCaptured")
-        self.swmr_mode = ad_rw(bool, prefix + "SWMRMode")
-        self.lazy_open = ad_rw(bool, prefix + "LazyOpen")
-        self.capture = ad_rw(bool, prefix + "Capture")
+        self.position_mode = epics_signal_rw_rbv(bool, prefix + "PositionMode")
+        self.compression = epics_signal_rw_rbv(Compression, prefix + "Compression")
+        self.num_extra_dims = epics_signal_rw_rbv(int, prefix + "NumExtraDims")
+        self.file_path = epics_signal_rw_rbv(str, prefix + "FilePath")
+        self.file_name = epics_signal_rw_rbv(str, prefix + "FileName")
+        self.file_path_exists = epics_signal_r(bool, prefix + "FilePathExists_RBV")
+        self.file_template = epics_signal_rw_rbv(str, prefix + "FileTemplate")
+        self.full_file_name = epics_signal_r(str, prefix + "FullFileName_RBV")
+        self.file_write_mode = epics_signal_rw_rbv(
+            FileWriteMode, prefix + "FileWriteMode"
+        )
+        self.num_capture = epics_signal_rw_rbv(int, prefix + "NumCapture")
+        self.num_captured = epics_signal_r(int, prefix + "NumCaptured_RBV")
+        self.swmr_mode = epics_signal_rw_rbv(bool, prefix + "SWMRMode")
+        self.lazy_open = epics_signal_rw_rbv(bool, prefix + "LazyOpen")
+        self.capture = epics_signal_rw_rbv(bool, prefix + "Capture")
         self.flush_now = epics_signal_rw(bool, prefix + "FlushNow")
-        self.array_size0 = ad_r(int, prefix + "ArraySize0")
-        self.array_size1 = ad_r(int, prefix + "ArraySize1")
-        self.xml_file_name = ad_rw(str, prefix + "XMLFileName")
+        self.array_size0 = epics_signal_r(int, prefix + "ArraySize0_RBV")
+        self.array_size1 = epics_signal_r(int, prefix + "ArraySize1_RBV")
+        self.xml_file_name = epics_signal_rw_rbv(str, prefix + "XMLFileName")
         super().__init__(prefix, name)
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/areadetector/writers/nd_plugin.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/areadetector/writers/nd_plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from enum import Enum
 
 from ophyd_async.core import Device
 from ophyd_async.epics.signal import epics_signal_rw
-
-from ..utils import ad_r, ad_rw
+from ophyd_async.epics.signal.signal import epics_signal_r, epics_signal_rw_rbv
 
 
 class Callback(str, Enum):
     Enable = "Enable"
     Disable = "Disable"
 
 
 class NDArrayBase(Device):
     def __init__(self, prefix: str, name: str = "") -> None:
-        self.unique_id = ad_r(int, prefix + "UniqueId")
+        self.unique_id = epics_signal_r(int, prefix + "UniqueId_RBV")
         self.nd_attributes_file = epics_signal_rw(str, prefix + "NDAttributesFile")
-        super().__init__(name)
+        super().__init__(name=name)
 
 
 class NDPluginBase(NDArrayBase):
     def __init__(self, prefix: str, name: str = "") -> None:
-        self.nd_array_port = ad_rw(str, prefix + "NDArrayPort")
-        self.enable_callback = ad_rw(Callback, prefix + "EnableCallbacks")
-        self.nd_array_address = ad_rw(int, prefix + "NDArrayAddress")
+        self.nd_array_port = epics_signal_rw_rbv(str, prefix + "NDArrayPort")
+        self.enable_callback = epics_signal_rw_rbv(Callback, prefix + "EnableCallbacks")
+        self.nd_array_address = epics_signal_rw_rbv(int, prefix + "NDArrayAddress")
         super().__init__(prefix, name)
 
 
 class NDPluginStats(NDPluginBase):
     pass
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/demo/__init__.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/demo/demo_ad_sim_detector.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/demo/demo_ad_sim_detector.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/demo/mover.db` & `ophyd_async-0.3a4/src/ophyd_async/epics/demo/mover.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/demo/sensor.db` & `ophyd_async-0.3a4/src/ophyd_async/epics/demo/sensor.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/motion/motor.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/motion/motor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,19 @@
         super().__init__(name=name)
 
     def set_name(self, name: str):
         super().set_name(name)
         # Readback should be named the same as its parent in read()
         self.user_readback.set_name(name)
 
-    async def _move(self, new_position: float, watchers: List[Callable] = []):
+    async def _move(
+        self, new_position: float, watchers: Optional[List[Callable]] = None
+    ):
+        if watchers is None:
+            watchers = []
         self._set_success = True
         start = time.monotonic()
         old_position, units, precision = await asyncio.gather(
             self.user_setpoint.get_value(),
             self.motor_egu.get_value(),
             self.precision.get_value(),
         )
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/pvi/pvi.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/pvi/pvi.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeVar,
     Union,
     get_args,
     get_origin,
     get_type_hints,
 )
 
-from ophyd_async.core import Device, DeviceVector, SimSignalBackend
+from ophyd_async.core import Device, DeviceVector, SoftSignalBackend
 from ophyd_async.core.signal import Signal
 from ophyd_async.core.utils import DEFAULT_TIMEOUT
 from ophyd_async.epics._backend._p4p import PvaSignalBackend
 from ophyd_async.epics.signal.signal import (
     epics_signal_r,
     epics_signal_rw,
     epics_signal_w,
@@ -152,15 +152,15 @@
         is_signal = True
         signal_dtype = None
         device_cls = Signal
 
     return is_device_vector, is_signal, signal_dtype, device_cls
 
 
-def _sim_common_blocks(device: Device, stripped_type: Optional[Type] = None):
+def _mock_common_blocks(device: Device, stripped_type: Optional[Type] = None):
     device_t = stripped_type or type(device)
     sub_devices = (
         (field, field_type)
         for field, field_type in get_type_hints(device_t).items()
         if field not in ("_name", "parent")
     )
 
@@ -171,31 +171,31 @@
         assert issubclass(device_cls, Device)
 
         is_signal = issubclass(device_cls, Signal)
         signal_dtype = device_args[0] if device_args is not None else None
 
         if is_device_vector:
             if is_signal:
-                sub_device_1 = device_cls(SimSignalBackend(signal_dtype))
-                sub_device_2 = device_cls(SimSignalBackend(signal_dtype))
+                sub_device_1 = device_cls(SoftSignalBackend(signal_dtype))
+                sub_device_2 = device_cls(SoftSignalBackend(signal_dtype))
                 sub_device = DeviceVector({1: sub_device_1, 2: sub_device_2})
             else:
                 sub_device = DeviceVector({1: device_cls(), 2: device_cls()})
 
                 for sub_device_in_vector in sub_device.values():
-                    _sim_common_blocks(sub_device_in_vector, stripped_type=device_cls)
+                    _mock_common_blocks(sub_device_in_vector, stripped_type=device_cls)
 
             for value in sub_device.values():
                 value.parent = sub_device
         else:
             if is_signal:
-                sub_device = device_cls(SimSignalBackend(signal_dtype))
+                sub_device = device_cls(SoftSignalBackend(signal_dtype))
             else:
                 sub_device = getattr(device, device_name, device_cls())
-                _sim_common_blocks(sub_device, stripped_type=device_cls)
+                _mock_common_blocks(sub_device, stripped_type=device_cls)
 
         setattr(device, device_name, sub_device)
         sub_device.parent = device
 
 
 async def _get_pvi_entries(entry: PVIEntry, timeout=DEFAULT_TIMEOUT):
     if not entry.pvi_pv or not entry.pvi_pv.endswith(":PVI"):
@@ -265,24 +265,24 @@
                 _set_device_attributes(sub_entry)
 
         sub_device.parent = entry.device
         setattr(entry.device, sub_name, sub_device)
 
 
 async def fill_pvi_entries(
-    device: Device, root_pv: str, timeout=DEFAULT_TIMEOUT, sim=False
+    device: Device, root_pv: str, timeout=DEFAULT_TIMEOUT, mock=False
 ):
     """
     Fills a ``device`` with signals from a the ``root_pvi:PVI`` table.
 
     If the device names match with parent devices of ``device`` then types are used.
     """
-    if sim:
-        # set up sim signals for the common annotations
-        _sim_common_blocks(device)
+    if mock:
+        # set up mock signals for the common annotations
+        _mock_common_blocks(device)
     else:
         # check the pvi table for devices and fill the device with them
         root_entry = PVIEntry(
             pvi_pv=root_pv,
             device=device,
             common_device_type=type(device),
             sub_entries={},
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/signal/_epics_transport.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/signal/_epics_transport.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/epics/signal/signal.py` & `ophyd_async-0.3a4/src/ophyd_async/epics/signal/signal.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/log.py` & `ophyd_async-0.3a4/src/ophyd_async/log.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/__init__.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/__init__.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/_common_blocks.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/_hdf_panda.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/_hdf_panda.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,11 +38,11 @@
             writer=writer,
             config_sigs=config_sigs,
             name=name,
             writer_timeout=DEFAULT_TIMEOUT,
         )
 
     async def connect(
-        self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT
+        self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT
     ) -> None:
-        await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
-        await super().connect(sim=sim, timeout=timeout)
+        await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, mock=mock)
+        await super().connect(mock=mock, timeout=timeout)
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/_panda_controller.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/_panda_controller.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/_table.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/_trigger.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/_trigger.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/writers/_hdf_writer.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/writers/_hdf_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/panda/writers/_panda_hdf_file.py` & `ophyd_async-0.3a4/src/ophyd_async/panda/writers/_panda_hdf_file.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/planstubs/prepare_trigger_and_dets.py` & `ophyd_async-0.3a4/src/ophyd_async/planstubs/prepare_trigger_and_dets.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/protocols.py` & `ophyd_async-0.3a4/src/ophyd_async/protocols.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/sim/demo/sim_motor.py` & `ophyd_async-0.3a4/src/ophyd_async/sim/demo/sim_motor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import time
 from typing import Callable, List, Optional
 
 from bluesky.protocols import Movable, Stoppable
 
 from ophyd_async.core import StandardReadable
 from ophyd_async.core.async_status import AsyncStatus
-from ophyd_async.core.signal import soft_signal_r_and_backend, soft_signal_rw
+from ophyd_async.core.signal import soft_signal_r_and_setter, soft_signal_rw
 from ophyd_async.core.standard_readable import ConfigSignal, HintedSignal
 
 
 class SimMotor(StandardReadable, Movable, Stoppable):
     def __init__(self, name="", instant=True) -> None:
         """
         Simulated motor device
 
         args:
         - prefix: str: Signal names prefix
         - name: str: name of device
         - instant: bool: whether to move instantly, or with a delay
         """
         with self.add_children_as_readables(HintedSignal):
-            self.user_readback, self._user_readback = soft_signal_r_and_backend(
+            self.user_readback, self._user_readback_set = soft_signal_r_and_setter(
                 float, 0
             )
 
         with self.add_children_as_readables(ConfigSignal):
             self.velocity = soft_signal_rw(float, 1.0)
             self.egu = soft_signal_rw(float, "mm")
 
@@ -80,23 +80,23 @@
         async def update_position():
             while True:
                 time_elapsed = round(time.monotonic() - start, 2)
 
                 # update position based on time elapsed
                 if time_elapsed >= travel_time:
                     # successfully reached our target position
-                    await self._user_readback.put(new_position)
+                    self._user_readback_set(new_position)
                     self._set_success = True
                     break
                 else:
                     current_position = (
                         old_position + distance * time_elapsed / travel_time
                     )
 
-                await self._user_readback.put(current_position)
+                self._user_readback_set(current_position)
 
                 # notify watchers of the new position
                 for watcher in watchers:
                     watcher(
                         name=self.name,
                         current=current_position,
                         initial=old_position,
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/sim/pattern_generator.py` & `ophyd_async-0.3a4/src/ophyd_async/sim/pattern_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     ComposeStreamResourceBundle,
     StreamDatum,
     StreamRange,
     StreamResource,
 )
 
 from ophyd_async.core import DirectoryInfo, DirectoryProvider
+from ophyd_async.core.mock_signal_backend import MockSignalBackend
 from ophyd_async.core.signal import SignalR, observe_value
-from ophyd_async.core.sim_signal_backend import SimSignalBackend
 from ophyd_async.core.utils import DEFAULT_TIMEOUT
 
 # raw data path
 DATA_PATH = "/entry/data/data"
 
 # pixel sum path
 SUM_PATH = "/entry/sum"
@@ -154,16 +154,16 @@
         self.x = 0.0
         self.y = 0.0
         self.height = detector_height
         self.width = detector_width
         self.written_images_counter: int = 0
 
         # it automatically initializes to 0
-        self.signal_backend = SimSignalBackend(int)
-        self.sim_signal = SignalR(self.signal_backend)
+        self.signal_backend = MockSignalBackend(int)
+        self.mock_signal = SignalR(self.signal_backend)
         blob = np.array(
             generate_gaussian_blob(width=detector_width, height=detector_height)
             * MAX_UINT8_VALUE
         )
         self.STARTING_BLOB = blob
         self._hdf_stream_provider: Optional[HdfStreamProvider] = None
         self._handle_for_h5_file: Optional[h5py.File] = None
@@ -216,15 +216,15 @@
 
     def set_y(self, value: float) -> None:
         self.y = value
 
     async def open_file(
         self, directory: DirectoryProvider, multiplier: int = 1
     ) -> Dict[str, DataKey]:
-        await self.sim_signal.connect()
+        await self.mock_signal.connect()
 
         self.target_path = self._get_new_path(directory)
 
         self._handle_for_h5_file = h5py.File(self.target_path, "w", libver="latest")
 
         assert self._handle_for_h5_file, "not loaded the file right"
 
@@ -310,9 +310,9 @@
             self._handle_for_h5_file.close()
             print("file closed")
             self._handle_for_h5_file = None
 
     async def observe_indices_written(
         self, timeout=DEFAULT_TIMEOUT
     ) -> AsyncGenerator[int, None]:
-        async for num_captured in observe_value(self.sim_signal, timeout=timeout):
+        async for num_captured in observe_value(self.mock_signal, timeout=timeout):
             yield num_captured // self.multiplier
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_control.py` & `ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_control.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_detector_writer.py` & `ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_detector_writer.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async/sim/sim_pattern_generator.py` & `ophyd_async-0.3a4/src/ophyd_async/sim/sim_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/src/ophyd_async.egg-info/PKG-INFO` & `ophyd_async-0.3a4/src/ophyd_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-async
-Version: 0.3a3
+Version: 0.3a4
 Summary: Asynchronous Bluesky hardware abstraction code, compatible with control systems like EPICS and Tango
 Author-email: Tom Cobb <tom.cobb@diamond.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Brookhaven National Laboratory
         
         Redistribution and use in source and binary forms, with or without
@@ -44,14 +44,15 @@
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: pint
 Requires-Dist: bluesky>=1.13.0a3
 Requires-Dist: event-model<1.21.0
 Requires-Dist: p4p
 Requires-Dist: pyyaml
+Requires-Dist: colorlog
 Provides-Extra: ca
 Requires-Dist: aioca>=1.6; extra == "ca"
 Provides-Extra: pva
 Requires-Dist: p4p; extra == "pva"
 Provides-Extra: dev
 Requires-Dist: ophyd_async[pva]; extra == "dev"
 Requires-Dist: ophyd_async[ca]; extra == "dev"
@@ -83,15 +84,14 @@
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinxcontrib-mermaid; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-pyyaml; extra == "dev"
-Requires-Dist: colorlog; extra == "dev"
 
 [![CI](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml/badge.svg)](https://github.com/bluesky/ophyd-async/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/bluesky/ophyd-async/branch/main/graph/badge.svg)](https://codecov.io/gh/bluesky/ophyd-async)
 [![PyPI](https://img.shields.io/pypi/v/ophyd-async.svg)](https://pypi.org/project/ophyd-async)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 # ophyd-async
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async.egg-info/SOURCES.txt` & `ophyd_async-0.3a4/src/ophyd_async.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -75,17 +75,19 @@
 src/ophyd_async/core/__init__.py
 src/ophyd_async/core/_providers.py
 src/ophyd_async/core/async_status.py
 src/ophyd_async/core/detector.py
 src/ophyd_async/core/device.py
 src/ophyd_async/core/device_save_loader.py
 src/ophyd_async/core/flyer.py
+src/ophyd_async/core/mock_signal_backend.py
+src/ophyd_async/core/mock_signal_utils.py
 src/ophyd_async/core/signal.py
 src/ophyd_async/core/signal_backend.py
-src/ophyd_async/core/sim_signal_backend.py
+src/ophyd_async/core/soft_signal_backend.py
 src/ophyd_async/core/standard_readable.py
 src/ophyd_async/core/utils.py
 src/ophyd_async/epics/__init__.py
 src/ophyd_async/epics/_backend/__init__.py
 src/ophyd_async/epics/_backend/_aioca.py
 src/ophyd_async/epics/_backend/_p4p.py
 src/ophyd_async/epics/_backend/common.py
@@ -149,16 +151,17 @@
 tests/test_flyer_with_panda.py
 tests/test_log.py
 tests/core/test_async_status.py
 tests/core/test_device.py
 tests/core/test_device_collector.py
 tests/core/test_device_save_loader.py
 tests/core/test_flyer.py
+tests/core/test_mock_signal_backend.py
 tests/core/test_signal.py
-tests/core/test_sim.py
+tests/core/test_soft_signal_backend.py
 tests/core/test_standard_readable.py
 tests/core/test_utils.py
 tests/epics/test_pvi.py
 tests/epics/test_records.db
 tests/epics/test_signals.py
 tests/epics/_backend/test_common.py
 tests/epics/areadetector/__init__.py
```

### Comparing `ophyd_async-0.3a3/src/ophyd_async.egg-info/requires.txt` & `ophyd_async-0.3a4/src/ophyd_async.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 numpy
 packaging
 pint
 bluesky>=1.13.0a3
 event-model<1.21.0
 p4p
 pyyaml
+colorlog
 
 [ca]
 aioca>=1.6
 
 [dev]
 ophyd_async[pva]
 ophyd_async[ca]
@@ -41,11 +42,10 @@
 sphinx-autobuild
 sphinxcontrib-mermaid
 sphinx-copybutton
 sphinx-design
 tox-direct
 types-mock
 types-pyyaml
-colorlog
 
 [pva]
 p4p
```

### Comparing `ophyd_async-0.3a3/tests/conftest.py` & `ophyd_async-0.3a4/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,31 @@
         raise call.excinfo.value
 
     @pytest.hookimpl(tryfirst=True)
     def pytest_internalerror(excinfo):
         raise excinfo.value
 
 
+# Autouse fixture that will set all EPICS networking env vars to use lo interface
+# to avoid false failures caused by things like firewalls blocking EPICS traffic.
+@pytest.fixture(scope="session", autouse=True)
+def configure_epics_environment():
+    os.environ["EPICS_CAS_INTF_ADDR_LIST"] = "127.0.0.1"
+    os.environ["EPICS_CAS_BEACON_ADDR_LIST"] = "127.0.0.1"
+    os.environ["EPICS_CA_ADDR_LIST"] = "127.0.0.1"
+    os.environ["EPICS_CAS_AUTO_ADDR_LIST"] = "NO"
+    os.environ["EPICS_CA_AUTO_BEACON_ADDR_LIST"] = "NO"
+
+    os.environ["EPICS_PVAS_INTF_ADDR_LIST"] = "127.0.0.1"
+    os.environ["EPICS_PVAS_BEACON_ADDR_LIST"] = "127.0.0.1"
+    os.environ["EPICS_PVA_ADDR_LIST"] = "127.0.0.1"
+    os.environ["EPICS_PVAS_AUTO_BEACON_ADDR_LIST"] = "NO"
+    os.environ["EPICS_PVA_AUTO_ADDR_LIST"] = "NO"
+
+
 @pytest.fixture(scope="function")
 def RE(request):
     loop = asyncio.new_event_loop()
     loop.set_debug(True)
     RE = RunEngine({}, call_returns_result=True, loop=loop)
 
     def clean_event_loop():
```

### Comparing `ophyd_async-0.3a3/tests/core/test_async_status.py` & `ophyd_async-0.3a4/tests/core/test_async_status.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/core/test_device.py` & `ophyd_async-0.3a4/tests/core/test_device.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 
 
 class DummyBaseDevice(Device):
     def __init__(self) -> None:
         self.connected = False
 
-    async def connect(self, sim=False, timeout=DEFAULT_TIMEOUT):
+    async def connect(self, mock=False, timeout=DEFAULT_TIMEOUT):
         self.connected = True
 
 
 class DummyDeviceGroup(Device):
     def __init__(self, name: str) -> None:
         self.child1 = DummyBaseDevice()
         self.child2 = DummyBaseDevice()
@@ -67,15 +67,15 @@
     await parent.connect()
 
     assert parent.child1.connected
     assert parent.dict_with_children[123].connected
 
 
 async def test_device_with_device_collector():
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         parent = DummyDeviceGroup("parent")
 
     assert parent.name == "parent"
     assert parent.child1.name == "parent-child1"
     assert parent.child2.name == "parent-child2"
     assert parent.dict_with_children.name == "parent-dict_with_children"
     assert parent.dict_with_children[123].name == "parent-dict_with_children-123"
@@ -84,15 +84,15 @@
 
 
 async def test_wait_for_connection():
     class DummyDeviceWithSleep(DummyBaseDevice):
         def __init__(self, name) -> None:
             self.set_name(name)
 
-        async def connect(self, sim=False, timeout=DEFAULT_TIMEOUT):
+        async def connect(self, mock=False, timeout=DEFAULT_TIMEOUT):
             await asyncio.sleep(0.01)
             self.connected = True
 
     device1, device2 = DummyDeviceWithSleep("device1"), DummyDeviceWithSleep("device2")
 
     normal_coros = {"device1": device1.connect(), "device2": device2.connect()}
 
@@ -106,7 +106,14 @@
     normal_coroutine, failing_coroutine
 ):
     failing_coros = {"test": normal_coroutine(), "failing": failing_coroutine()}
 
     with pytest.raises(NotConnected) as e:
         await wait_for_connection(**failing_coros)
         assert traceback.extract_tb(e.__traceback__)[-1].name == "failing_coroutine"
+
+
+async def test_device_log_has_correct_name():
+    device = DummyBaseDevice()
+    assert device.log.extra["ophyd_async_device_name"] == ""
+    device.set_name("device")
+    assert device.log.extra["ophyd_async_device_name"] == "device"
```

### Comparing `ophyd_async-0.3a3/tests/core/test_device_collector.py` & `ophyd_async-0.3a4/tests/core/test_device_collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from bluesky.run_engine import RunEngine, TransitionError
 
 from ophyd_async.core import DEFAULT_TIMEOUT, Device, DeviceCollector, NotConnected
 from ophyd_async.epics.motion import motor
 
 
 class FailingDevice(Device):
-    async def connect(self, sim: bool = False, timeout=DEFAULT_TIMEOUT):
+    async def connect(self, mock: bool = False, timeout=DEFAULT_TIMEOUT):
         raise AttributeError()
 
 
 class WorkingDevice(Device):
     connected = False
 
-    async def connect(self, sim: bool = True, timeout=DEFAULT_TIMEOUT):
+    async def connect(self, mock: bool = True, timeout=DEFAULT_TIMEOUT):
         self.connected = True
-        return await super().connect(sim=True)
+        return await super().connect(mock=True)
 
     async def set(self, new_position: float): ...
 
 
 async def test_device_collector_handles_top_level_errors(caplog):
     caplog.set_level(10)
     with pytest.raises(NotConnected) as exc:
@@ -79,33 +79,33 @@
 
     request.addfinalizer(clean_event_loop)
     return RE
 
 
 def test_async_device_connector_run_engine_same_event_loop():
     async def set_up_device():
-        async with DeviceCollector(sim=True):
-            sim_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
-        return sim_motor
+        async with DeviceCollector(mock=True):
+            mock_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
+        return mock_motor
 
     loop = asyncio.new_event_loop()
     checking_loop = asyncio.new_event_loop()
 
     try:
-        sim_motor = loop.run_until_complete(set_up_device())
+        mock_motor = loop.run_until_complete(set_up_device())
         RE = RunEngine(call_returns_result=True, loop=loop)
 
         def my_plan():
-            yield from bps.mov(sim_motor, 3.14)
+            yield from bps.mov(mock_motor, 3.14)
 
         RE(my_plan())
 
         assert (
-            checking_loop.run_until_complete(sim_motor.user_setpoint.read())[
-                "sim_motor-user_setpoint"
+            checking_loop.run_until_complete(mock_motor.user_setpoint.read())[
+                "mock_motor-user_setpoint"
             ]["value"]
             == 3.14
         )
 
     finally:
         if RE.state not in ("idle", "panicked"):
             try:
@@ -117,37 +117,37 @@
         RE._th.join()
         loop.close()
         checking_loop.close()
 
 
 @pytest.mark.skip(
     reason=(
-        "SimSignalBackend currently allows a different event-"
+        "MockSignalBackend currently allows a different event-"
         "loop to set the value, unlike real signals."
     )
 )
 def test_async_device_connector_run_engine_different_event_loop():
     async def set_up_device():
-        async with DeviceCollector(sim=True):
-            sim_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
-        return sim_motor
+        async with DeviceCollector(mock=True):
+            mock_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
+        return mock_motor
 
     device_connector_loop = asyncio.new_event_loop()
     run_engine_loop = asyncio.new_event_loop()
     assert run_engine_loop is not device_connector_loop
 
-    sim_motor = device_connector_loop.run_until_complete(set_up_device())
+    mock_motor = device_connector_loop.run_until_complete(set_up_device())
 
     RE = RunEngine(loop=run_engine_loop)
 
     def my_plan():
-        yield from bps.mov(sim_motor, 3.14)
+        yield from bps.mov(mock_motor, 3.14)
 
     RE(my_plan())
 
     # The set should fail since the run engine is on a different event loop
     assert (
-        device_connector_loop.run_until_complete(sim_motor.user_setpoint.read())[
-            "sim_motor-user_setpoint"
+        device_connector_loop.run_until_complete(mock_motor.user_setpoint.read())[
+            "mock_motor-user_setpoint"
         ]["value"]
         != 3.14
     )
```

### Comparing `ophyd_async-0.3a3/tests/core/test_device_save_loader.py` & `ophyd_async-0.3a4/tests/core/test_device_save_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self.parent_sig3: SignalRW = epics_signal_rw(str, "ParentValue3")
         self.position: npt.NDArray[np.int32]
 
 
 @pytest.fixture
 async def device() -> DummyDeviceGroup:
     device = DummyDeviceGroup("parent")
-    await device.connect(sim=True)
+    await device.connect(mock=True)
     return device
 
 
 # Dummy function to check different phases save properly
 def sort_signal_by_phase(values: Dict[str, Any]) -> List[Dict[str, Any]]:
     phase_1 = {"child1.sig1": values["child1.sig1"]}
     phase_2 = {"child2.sig1": values["child2.sig1"]}
```

### Comparing `ophyd_async-0.3a3/tests/core/test_flyer.py` & `ophyd_async-0.3a4/tests/core/test_flyer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     DetectorControl,
     DetectorTrigger,
     DetectorWriter,
     HardwareTriggeredFlyable,
-    SignalRW,
-    SimSignalBackend,
     TriggerInfo,
     TriggerLogic,
 )
 from ophyd_async.core.detector import StandardDetector
 from ophyd_async.core.signal import observe_value
+from ophyd_async.epics.signal.signal import epics_signal_rw
 
 
 class TriggerState(str, Enum):
     null = "null"
     preparing = "preparing"
     starting = "starting"
     stopping = "stopping"
@@ -47,15 +46,15 @@
 
     async def stop(self):
         self.state = TriggerState.stopping
 
 
 class DummyWriter(DetectorWriter):
     def __init__(self, name: str, shape: Sequence[int]):
-        self.dummy_signal = SignalRW(backend=SimSignalBackend(int))
+        self.dummy_signal = epics_signal_rw(int, "pva://read_pv")
         self._shape = shape
         self._name = name
         self._file: Optional[ComposeStreamResourceBundle] = None
         self._last_emitted = 0
         self.index = 0
 
     async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
@@ -108,16 +107,16 @@
     async def close(self) -> None:
         self._file = None
 
 
 @pytest.fixture
 async def detector_list(RE: RunEngine) -> tuple[StandardDetector, StandardDetector]:
     writers = [DummyWriter("testa", (1, 1)), DummyWriter("testb", (1, 1))]
-    await writers[0].dummy_signal.connect(sim=True)
-    await writers[1].dummy_signal.connect(sim=True)
+    await writers[0].dummy_signal.connect(mock=True)
+    await writers[1].dummy_signal.connect(mock=True)
 
     async def dummy_arm_1(self=None, trigger=None, num=0, exposure=None):
         return writers[0].dummy_signal.set(1)
 
     async def dummy_arm_2(self=None, trigger=None, num=0, exposure=None):
         return writers[1].dummy_signal.set(1)
```

### Comparing `ophyd_async-0.3a3/tests/core/test_signal.py` & `ophyd_async-0.3a4/tests/core/test_signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,179 @@
 import asyncio
+import logging
 import re
 import time
 from unittest.mock import ANY
 
 import numpy
 import pytest
 from bluesky.protocols import Reading
 
 from ophyd_async.core import (
     ConfigSignal,
     DeviceCollector,
     HintedSignal,
-    Signal,
     SignalR,
     SignalRW,
-    SimSignalBackend,
+    SoftSignalBackend,
     StandardReadable,
     assert_configuration,
     assert_reading,
     assert_value,
     set_and_wait_for_value,
-    set_sim_put_proceeds,
-    set_sim_value,
-    soft_signal_r_and_backend,
+    set_mock_put_proceeds,
+    set_mock_value,
+    soft_signal_r_and_setter,
     soft_signal_rw,
     wait_for_value,
 )
-from ophyd_async.core.utils import DEFAULT_TIMEOUT
+from ophyd_async.core.signal import _SignalCache
 from ophyd_async.epics.signal import epics_signal_r, epics_signal_rw
 
 
-class MySignal(Signal):
-    @property
-    def source(self) -> str:
-        return "me"
+async def test_signals_equality_raises():
+    s1 = epics_signal_rw(int, "pva://pv1", name="signal")
+    s2 = epics_signal_rw(int, "pva://pv2", name="signal")
+    await s1.connect(mock=True)
+    await s2.connect(mock=True)
 
-    async def connect(self, sim=False, timeout=DEFAULT_TIMEOUT):
-        pass
-
-
-def test_signals_equality_raises():
-    sim_backend = SimSignalBackend(str)
-
-    s1 = MySignal(sim_backend)
-    s2 = MySignal(sim_backend)
     with pytest.raises(
         TypeError,
         match=re.escape(
             "Can't compare two Signals, did you mean await signal.get_value() instead?"
         ),
     ):
         s1 == s2
     with pytest.raises(
         TypeError,
-        match=re.escape("'>' not supported between instances of 'MySignal' and 'int'"),
+        match=re.escape("'>' not supported between instances of 'SignalRW' and 'int'"),
     ):
         s1 > 4
 
 
-async def test_set_sim_put_proceeds():
-    sim_signal = Signal(SimSignalBackend(str))
-    await sim_signal.connect(sim=True)
-
-    assert sim_signal._backend.put_proceeds.is_set() is True
-
-    set_sim_put_proceeds(sim_signal, False)
-    assert sim_signal._backend.put_proceeds.is_set() is False
-    set_sim_put_proceeds(sim_signal, True)
-    assert sim_signal._backend.put_proceeds.is_set() is True
-
-
 async def time_taken_by(coro) -> float:
     start = time.monotonic()
     await coro
     return time.monotonic() - start
 
 
+async def test_set_and_wait_for_value():
+    signal = epics_signal_rw(int, "pva://pv", name="signal")
+    await signal.connect(mock=True)
+    assert await signal.get_value() == 0
+    set_mock_put_proceeds(signal, False)
+
+    async def wait_and_set_proceeds():
+        await asyncio.sleep(0.1)
+        set_mock_put_proceeds(signal, True)
+        await asyncio.sleep(0.01)
+
+    async def check_set_and_wait():
+        st = await set_and_wait_for_value(signal, 1, timeout=100)
+        await st
+        await asyncio.sleep(0.01)
+
+    assert (
+        0.1
+        < await time_taken_by(
+            asyncio.gather(wait_and_set_proceeds(), check_set_and_wait())
+        )
+        < 0.15
+    )
+    assert await signal.get_value() == 1
+
+
 async def test_wait_for_value_with_value():
-    sim_signal = SignalRW(SimSignalBackend(str))
-    sim_signal.set_name("sim_signal")
-    await sim_signal.connect(sim=True)
-    set_sim_value(sim_signal, "blah")
+    signal = epics_signal_rw(str, read_pv="pva://signal", name="signal")
+    await signal.connect(mock=True)
+    await signal.set("blah")
 
     with pytest.raises(
         TimeoutError,
-        match="sim_signal didn't match 'something' in 0.1s, last value 'blah'",
+        match="signal didn't match 'something' in 0.1s, last value 'blah'",
     ):
-        await wait_for_value(sim_signal, "something", timeout=0.1)
-    assert await time_taken_by(wait_for_value(sim_signal, "blah", timeout=2)) < 0.1
+        await wait_for_value(signal, "something", timeout=0.1)
+    assert await time_taken_by(wait_for_value(signal, "blah", timeout=2)) < 0.1
     t = asyncio.create_task(
-        time_taken_by(wait_for_value(sim_signal, "something else", timeout=2))
+        time_taken_by(wait_for_value(signal, "something else", timeout=2))
     )
     await asyncio.sleep(0.2)
     assert not t.done()
-    set_sim_value(sim_signal, "something else")
+    set_mock_value(signal, "something else")
     assert 0.2 < await t < 1.0
 
 
 async def test_wait_for_value_with_funcion():
-    sim_signal = SignalRW(SimSignalBackend(float))
-    sim_signal.set_name("sim_signal")
-    await sim_signal.connect(sim=True)
-    set_sim_value(sim_signal, 45.8)
+    signal = epics_signal_rw(float, read_pv="pva://signal", name="signal")
+    await signal.connect(mock=True)
+    set_mock_value(signal, 45.8)
 
     def less_than_42(v):
         return v < 42
 
     with pytest.raises(
         TimeoutError,
-        match="sim_signal didn't match less_than_42 in 0.1s, last value 45.8",
+        match="signal didn't match less_than_42 in 0.1s, last value 45.8",
     ):
-        await wait_for_value(sim_signal, less_than_42, timeout=0.1)
+        await wait_for_value(signal, less_than_42, timeout=0.1)
     t = asyncio.create_task(
-        time_taken_by(wait_for_value(sim_signal, less_than_42, timeout=2))
+        time_taken_by(wait_for_value(signal, less_than_42, timeout=2))
     )
     await asyncio.sleep(0.2)
     assert not t.done()
-    set_sim_value(sim_signal, 41)
+    set_mock_value(signal, 41)
     assert 0.2 < await t < 1.0
-    assert (
-        await time_taken_by(wait_for_value(sim_signal, less_than_42, timeout=2)) < 0.1
-    )
-
-
-async def test_set_and_wait_for_value():
-    sim_signal = SignalRW(SimSignalBackend(int))
-    sim_signal.set_name("sim_signal")
-    await sim_signal.connect(sim=True)
-    set_sim_value(sim_signal, 0)
-    set_sim_put_proceeds(sim_signal, False)
-    st = await set_and_wait_for_value(sim_signal, 1)
-    assert not st.done
-    set_sim_put_proceeds(sim_signal, True)
-    assert await time_taken_by(st) < 0.1
+    assert await time_taken_by(wait_for_value(signal, less_than_42, timeout=2)) < 0.1
 
 
 @pytest.mark.parametrize(
     "signal_method,signal_class",
-    [(soft_signal_r_and_backend, SignalR), (soft_signal_rw, SignalRW)],
+    [(soft_signal_r_and_setter, SignalR), (soft_signal_rw, SignalRW)],
 )
 async def test_create_soft_signal(signal_method, signal_class):
     SIGNAL_NAME = "TEST-PREFIX:SIGNAL"
     INITIAL_VALUE = "INITIAL"
-    if signal_method == soft_signal_r_and_backend:
-        signal, backend = signal_method(str, INITIAL_VALUE, SIGNAL_NAME)
+    if signal_method == soft_signal_r_and_setter:
+        signal, unused_backend_set = signal_method(str, INITIAL_VALUE, SIGNAL_NAME)
     elif signal_method == soft_signal_rw:
         signal = signal_method(str, INITIAL_VALUE, SIGNAL_NAME)
-        backend = signal._backend
     assert signal.source == f"soft://{SIGNAL_NAME}"
     assert isinstance(signal, signal_class)
-    assert isinstance(signal._backend, SimSignalBackend)
+    assert isinstance(signal._backend, SoftSignalBackend)
     await signal.connect()
     assert (await signal.get_value()) == INITIAL_VALUE
-    # connecting with sim=False uses existing SimSignalBackend
-    assert signal._backend is backend
 
 
 async def test_soft_signal_numpy():
     float_signal = soft_signal_rw(numpy.float64, numpy.float64(1), "float_signal")
     int_signal = soft_signal_rw(numpy.int32, numpy.int32(1), "int_signal")
     await float_signal.connect()
     await int_signal.connect()
     assert (await float_signal.describe())["float_signal"]["dtype"] == "number"
     assert (await int_signal.describe())["int_signal"]["dtype"] == "integer"
 
 
 @pytest.fixture
-async def sim_signal():
-    sim_signal = SignalRW(SimSignalBackend(int, "test"))
-    sim_signal.set_name("sim_signal")
-    await sim_signal.connect(sim=True)
-    yield sim_signal
+async def mock_signal():
+    mock_signal = epics_signal_rw(int, "pva://mock_signal", name="mock_signal")
+    await mock_signal.connect(mock=True)
+    yield mock_signal
 
 
-async def test_assert_value(sim_signal: SignalRW):
-    set_sim_value(sim_signal, 168)
-    await assert_value(sim_signal, 168)
+async def test_assert_value(mock_signal: SignalRW):
+    set_mock_value(mock_signal, 168)
+    await assert_value(mock_signal, 168)
 
 
-async def test_assert_reaading(sim_signal: SignalRW):
-    set_sim_value(sim_signal, 888)
+async def test_assert_reaading(mock_signal: SignalRW):
+    set_mock_value(mock_signal, 888)
     dummy_reading = {
-        "sim_signal": Reading({"alarm_severity": 0, "timestamp": ANY, "value": 888})
+        "mock_signal": Reading({"alarm_severity": 0, "timestamp": ANY, "value": 888})
     }
-    await assert_reading(sim_signal, dummy_reading)
+    await assert_reading(mock_signal, dummy_reading)
 
 
 class DummyReadable(StandardReadable):
     """A demo Readable to produce read and config signal"""
 
     def __init__(self, prefix: str, name="") -> None:
         # Define some signals
@@ -197,34 +183,61 @@
             self.mode = epics_signal_rw(str, prefix + "Mode")
             self.mode2 = epics_signal_rw(str, prefix + "Mode2")
         # Set name and signals for read() and read_configuration()
         super().__init__(name=name)
 
 
 @pytest.fixture
-async def sim_readable():
-    async with DeviceCollector(sim=True):
-        sim_readable = DummyReadable("SIM:READABLE:")
-        # Signals connected here
-    assert sim_readable.name == "sim_readable"
-    yield sim_readable
+async def mock_readable():
+    async with DeviceCollector(mock=True):
+        mock_readable = DummyReadable("SIM:READABLE:", name="mock_readable")
+
+    yield mock_readable
 
 
-async def test_assert_configuration(sim_readable: DummyReadable):
-    set_sim_value(sim_readable.value, 123)
-    set_sim_value(sim_readable.mode, "super mode")
-    set_sim_value(sim_readable.mode2, "slow mode")
+async def test_assert_configuration(mock_readable: DummyReadable):
+    set_mock_value(mock_readable.value, 123)
+    set_mock_value(mock_readable.mode, "super mode")
+    set_mock_value(mock_readable.mode2, "slow mode")
     dummy_config_reading = {
-        "sim_readable-mode": (
+        "mock_readable-mode": (
             {
                 "alarm_severity": 0,
                 "timestamp": ANY,
                 "value": "super mode",
             }
         ),
-        "sim_readable-mode2": {
+        "mock_readable-mode2": {
             "alarm_severity": 0,
             "timestamp": ANY,
             "value": "slow mode",
         },
     }
-    await assert_configuration(sim_readable, dummy_config_reading)
+    await assert_configuration(mock_readable, dummy_config_reading)
+
+
+async def test_signal_connect_logs(caplog):
+    caplog.set_level(logging.DEBUG)
+    mock_signal_rw = epics_signal_rw(int, "pva://mock_signal", name="mock_signal")
+    await mock_signal_rw.connect(mock=True)
+    assert caplog.text.endswith("Connecting to mock+pva://mock_signal\n")
+
+
+async def test_signal_get_and_set_logging(caplog):
+    caplog.set_level(logging.DEBUG)
+    mock_signal_rw = epics_signal_rw(int, "pva://mock_signal", name="mock_signal")
+    await mock_signal_rw.connect(mock=True)
+    await mock_signal_rw.set(value=0)
+    assert "Putting value 0 to backend at source" in caplog.text
+    assert "Successfully put value 0 to backend at source" in caplog.text
+    await mock_signal_rw.get_value()
+    assert "get_value() on source" in caplog.text
+
+
+async def test_subscription_logs(caplog):
+    caplog.set_level(logging.DEBUG)
+    mock_signal_rw = epics_signal_rw(int, "pva://mock_signal", name="mock_signal")
+    await mock_signal_rw.connect(mock=True)
+    cache = _SignalCache(mock_signal_rw._backend, signal=mock_signal_rw)
+    assert "Making subscription" in caplog.text
+    cache.close()
+    assert "Closing subscription on source" in caplog.text
```

### Comparing `ophyd_async-0.3a3/tests/core/test_sim.py` & `ophyd_async-0.3a4/tests/core/test_soft_signal_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import Any, Callable, Sequence, Tuple, Type
 
 import numpy as np
 import numpy.typing as npt
 import pytest
 from bluesky.protocols import Reading
 
-from ophyd_async.core import Signal, SignalBackend, SimSignalBackend, T
+from ophyd_async.core import Signal, SignalBackend, T
+from ophyd_async.core.soft_signal_backend import SoftSignalBackend
 
 
 class MyEnum(str, Enum):
     a = "Aaa"
     b = "Bbb"
     c = "Ccc"
 
@@ -83,21 +84,21 @@
         (npt.NDArray[np.float64], [], [0.2], waveform_d),
         (Sequence[str], [], ["nine", "ten"], waveform_d),
         # Can't do long strings until https://github.com/epics-base/pva2pva/issues/17
         # (str, "longstr", ls1, ls2, string_d),
         # (str, "longstr2.VAL$", ls1, ls2, string_d),
     ],
 )
-async def test_backend_get_put_monitor(
+async def test_soft_signal_backend_get_put_monitor(
     datatype: Type[T],
     initial_value: T,
     put_value: T,
     descriptor: Callable[[Any], dict],
 ):
-    backend = SimSignalBackend(datatype)
+    backend = SoftSignalBackend(datatype)
 
     await backend.connect()
     q = MonitorQueue(backend)
     try:
         # Check descriptor
         source = "soft://test"
         assert dict(
@@ -110,31 +111,25 @@
         # Put to new value and check that
         await backend.put(put_value)
         await q.assert_updates(pytest.approx(put_value))
     finally:
         q.close()
 
 
-async def test_sim_backend_if_disconnected():
-    sim_backend = SimSignalBackend(npt.NDArray[np.float64])
-    with pytest.raises(NotImplementedError):
-        await sim_backend.get_value()
+async def test_soft_signal_backend_with_numpy_typing():
+    soft_backend = SoftSignalBackend(npt.NDArray[np.float64])
+    await soft_backend.connect()
 
-
-async def test_sim_backend_with_numpy_typing():
-    sim_backend = SimSignalBackend(npt.NDArray[np.float64])
-    await sim_backend.connect()
-
-    array = await sim_backend.get_value()
+    array = await soft_backend.get_value()
     assert array.shape == (0,)
 
 
-async def test_sim_backend_descriptor_fails_for_invalid_class():
+async def test_soft_signal_descriptor_fails_for_invalid_class():
     class myClass:
         def __init__(self) -> None:
             pass
 
-    sim_signal = Signal(SimSignalBackend(myClass))
-    await sim_signal.connect(sim=True)
+    soft_signal = Signal(SoftSignalBackend(myClass))
+    await soft_signal.connect()
 
     with pytest.raises(AssertionError):
-        await sim_signal._backend.get_datakey("")
+        await soft_signal._backend.get_datakey("")
```

### Comparing `ophyd_async-0.3a3/tests/core/test_standard_readable.py` & `ophyd_async-0.3a4/tests/core/test_standard_readable.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from unittest.mock import MagicMock
 
 import pytest
 from bluesky.protocols import HasHints
 
 from ophyd_async.core import ConfigSignal, HintedSignal, StandardReadable
 from ophyd_async.core.device import Device, DeviceVector
+from ophyd_async.core.mock_signal_backend import MockSignalBackend
 from ophyd_async.core.signal import SignalR
-from ophyd_async.core.sim_signal_backend import SimSignalBackend
 from ophyd_async.protocols import AsyncConfigurable, AsyncReadable, AsyncStageable
 
 
 def test_standard_readable_hints():
     sr = StandardReadable()
 
     assert sr.hints == {}
@@ -132,15 +132,15 @@
     sr.add_readables = mock
 
     with sr.add_children_as_readables():
         sr.a = MagicMock(spec=SignalR)
         sr.b = MagicMock(spec=Device)
         sr.c = 1.0
         sr.d = "abc"
-        sr.e = MagicMock(spec=SimSignalBackend)
+        sr.e = MagicMock(spec=MockSignalBackend)
 
     # Can't use assert_called_once_with() as the order of items returned from
     # internal dict comprehension is not guaranteed
     mock.assert_called_once()
     assert set(mock.call_args.args[0]) == {sr.a, sr.b}
```

### Comparing `ophyd_async-0.3a3/tests/core/test_utils.py` & `ophyd_async-0.3a4/tests/core/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+from unittest.mock import patch
+
 import pytest
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     Device,
     DeviceCollector,
-    DirectoryInfo,
+    MockSignalBackend,
     NotConnected,
     SignalRW,
-    SimSignalBackend,
-    StaticDirectoryProvider,
 )
 from ophyd_async.epics.signal import epics_signal_rw
 
 
-class ValueErrorBackend(SimSignalBackend):
+class ValueErrorBackend(MockSignalBackend):
     def __init__(self, exc_text=""):
         self.exc_text = exc_text
-        super().__init__(int, "VALUE_ERROR_SIGNAL")
+        super().__init__(datatype=int, initial_backend=None)
 
     async def connect(self, timeout: float = DEFAULT_TIMEOUT):
         raise ValueError(self.exc_text)
 
 
 class WorkingDummyChildDevice(Device):
     def __init__(self, name: str = "working_dummy_child_device") -> None:
-        self.working_signal = SignalRW(backend=SimSignalBackend(int))
+        self.working_signal = SignalRW(backend=MockSignalBackend(datatype=int))
         super().__init__(name=name)
 
 
 class TimeoutDummyChildDeviceCA(Device):
     def __init__(self, name: str = "timeout_dummy_child_device_ca") -> None:
         self.timeout_signal = epics_signal_rw(int, "ca://A_NON_EXISTENT_SIGNAL")
         super().__init__(name=name)
@@ -119,39 +119,43 @@
     # This should work since the error is a connection timeout
     with pytest.raises(NotConnected) as e:
         await dummy_device_one_working_one_timeout.connect(timeout=0.01)
 
     assert str(e.value) == str(ONE_WORKING_ONE_TIMEOUT_OUTPUT)
 
     logs = caplog.get_records("call")
-    assert len(logs) == 1
-    assert "signal ca://A_NON_EXISTENT_SIGNAL timed out" == logs[0].message
-    assert logs[0].levelname == "DEBUG"
+    assert len(logs) == 3
+    assert "signal ca://A_NON_EXISTENT_SIGNAL timed out" == logs[-1].message
+    assert logs[-1].levelname == "DEBUG"
 
 
 async def test_error_handling_value_errors(caplog):
     """Checks that NotConnected is aggregated correctly across Devices."""
 
     caplog.set_level(10)
 
     dummy_device_two_working_one_timeout_two_value_error = (
-        DummyDeviceTwoWorkingTwoTimeOutTwoValueError()
+        DummyDeviceTwoWorkingTwoTimeOutTwoValueError("dsf")
     )
 
     # This should fail since the error is a ValueError
     with pytest.raises(NotConnected) as e:
         (
             await dummy_device_two_working_one_timeout_two_value_error.connect(
                 timeout=0.01
             ),
         )
     assert str(e.value) == str(TWO_WORKING_TWO_TIMEOUT_TWO_VALUE_ERROR_OUTPUT)
 
     logs = caplog.get_records("call")
-    logs = [log for log in logs if "ophyd_async" in log.pathname]
+    logs = [
+        log
+        for log in logs
+        if "ophyd_async" in log.pathname and "signal" not in log.pathname
+    ]
     assert len(logs) == 4
 
     for i in range(0, 2):
         assert (
             "device `value_error_signal` raised unexpected exception ValueError"
             == logs[i].message
         )
@@ -164,31 +168,37 @@
     for protocol in ("pva", "ca"):
         assert f"signal {protocol}://A_NON_EXISTENT_SIGNAL timed out" in messages
 
 
 async def test_error_handling_device_collector(caplog):
     caplog.set_level(10)
     with pytest.raises(NotConnected) as e:
+        # flake8: noqa
         async with DeviceCollector(timeout=0.1):
-            # flake8: noqa
             dummy_device_two_working_one_timeout_two_value_error = (
                 DummyDeviceTwoWorkingTwoTimeOutTwoValueError()
             )
             dummy_device_one_working_one_timeout = DummyDeviceOneWorkingOneTimeout()
 
     expected_output = NotConnected(
         {
-            "dummy_device_two_working_one_timeout_two_value_error": TWO_WORKING_TWO_TIMEOUT_TWO_VALUE_ERROR_OUTPUT,
+            "dummy_device_two_working_one_timeout_two_value_error": (
+                TWO_WORKING_TWO_TIMEOUT_TWO_VALUE_ERROR_OUTPUT
+            ),
             "dummy_device_one_working_one_timeout": ONE_WORKING_ONE_TIMEOUT_OUTPUT,
         }
     )
     assert str(expected_output) == str(e.value)
 
     logs = caplog.get_records("call")
-    logs = [log for log in logs if "ophyd_async" in log.pathname]
+    logs = [
+        log
+        for log in logs
+        if "ophyd_async" in log.pathname and "signal" not in log.pathname
+    ]
     assert len(logs) == 5
     assert (
         logs[0].message
         == logs[1].message
         == "device `value_error_signal` raised unexpected exception ValueError"
     )
     assert logs[0].levelname == logs[1].levelname == "ERROR"
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_aravis.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_aravis.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from bluesky.run_engine import RunEngine
 
 from ophyd_async.core import (
     DetectorTrigger,
     DeviceCollector,
     DirectoryProvider,
     TriggerInfo,
-    set_sim_value,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.aravis import AravisDetector
 
 
 @pytest.fixture
 async def adaravis(
     RE: RunEngine,
     static_directory_provider: DirectoryProvider,
 ) -> AravisDetector:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         adaravis = AravisDetector("ADARAVIS:", static_directory_provider)
 
     return adaravis
 
 
 @pytest.mark.parametrize(
     "model,pixel_format,deadtime",
@@ -42,53 +42,53 @@
 )
 async def test_deadtime_fetched(
     model: str,
     pixel_format: str,
     deadtime: float,
     adaravis: AravisDetector,
 ):
-    set_sim_value(adaravis.drv.model, model)
-    set_sim_value(adaravis.drv.pixel_format, pixel_format)
+    set_mock_value(adaravis.drv.model, model)
+    set_mock_value(adaravis.drv.pixel_format, pixel_format)
 
     await adaravis.drv.fetch_deadtime()
     # deadtime invariant with exposure time
     assert adaravis.controller.get_deadtime(0) == deadtime
     assert adaravis.controller.get_deadtime(500) == deadtime
 
 
 async def test_unknown_model_deadtime(
     adaravis: AravisDetector,
 ):
-    set_sim_value(adaravis.drv.model, "FOO")
+    set_mock_value(adaravis.drv.model, "FOO")
 
     with pytest.raises(ValueError, match="Model FOO does not have defined deadtimes"):
         await adaravis.drv.fetch_deadtime()
 
 
 async def test_unknown_pixel_format_deadtime(
     adaravis: AravisDetector,
 ):
-    set_sim_value(adaravis.drv.model, "Manta G-235")
-    set_sim_value(adaravis.drv.pixel_format, "BAR")
+    set_mock_value(adaravis.drv.model, "Manta G-235")
+    set_mock_value(adaravis.drv.pixel_format, "BAR")
 
     with pytest.raises(
         ValueError,
         match="Model Manta G-235 does not have a defined deadtime "
         "for pixel format BAR",
     ):
         await adaravis.drv.fetch_deadtime()
 
 
 async def test_trigger_source_set_to_gpio_line(adaravis: AravisDetector):
-    set_sim_value(adaravis.drv.trigger_source, "Freerun")
+    set_mock_value(adaravis.drv.trigger_source, "Freerun")
 
     async def trigger_and_complete():
         await adaravis.controller.arm(num=1, trigger=DetectorTrigger.edge_trigger)
         # Prevent timeouts
-        set_sim_value(adaravis.drv.acquire, True)
+        set_mock_value(adaravis.drv.acquire, True)
 
     # Default TriggerSource
     assert (await adaravis.drv.trigger_source.get_value()) == "Freerun"
     adaravis.set_external_trigger_gpio(1)
     # TriggerSource not changed by setting gpio
     assert (await adaravis.drv.trigger_source.get_value()) == "Freerun"
 
@@ -123,37 +123,37 @@
 
 async def test_can_read(adaravis: AravisDetector):
     # Standard detector can be used as Readable
     assert (await adaravis.read()) == {}
 
 
 async def test_decribe_describes_writer_dataset(adaravis: AravisDetector):
-    set_sim_value(adaravis._writer.hdf.file_path_exists, True)
-    set_sim_value(adaravis._writer.hdf.capture, True)
+    set_mock_value(adaravis._writer.hdf.file_path_exists, True)
+    set_mock_value(adaravis._writer.hdf.capture, True)
 
     assert await adaravis.describe() == {}
     await adaravis.stage()
     assert await adaravis.describe() == {
         "adaravis": {
-            "source": "soft://adaravis-hdf-full_file_name",
+            "source": "mock+ca://ADARAVIS:HDF1:FullFileName_RBV",
             "shape": (0, 0),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
 
 async def test_can_collect(
     adaravis: AravisDetector, static_directory_provider: DirectoryProvider
 ):
     directory_info = static_directory_provider()
     full_file_name = directory_info.root / directory_info.resource_dir / "foo.h5"
-    set_sim_value(adaravis.hdf.full_file_name, str(full_file_name))
-    set_sim_value(adaravis._writer.hdf.file_path_exists, True)
-    set_sim_value(adaravis._writer.hdf.capture, True)
+    set_mock_value(adaravis.hdf.full_file_name, str(full_file_name))
+    set_mock_value(adaravis._writer.hdf.file_path_exists, True)
+    set_mock_value(adaravis._writer.hdf.capture, True)
     await adaravis.stage()
     docs = [(name, doc) async for name, doc in adaravis.collect_asset_docs(1)]
     assert len(docs) == 2
     assert docs[0][0] == "stream_resource"
     stream_resource = docs[0][1]
     sr_uid = stream_resource["uid"]
     assert stream_resource["data_key"] == "adaravis"
@@ -172,30 +172,30 @@
     stream_datum = docs[1][1]
     assert stream_datum["stream_resource"] == sr_uid
     assert stream_datum["seq_nums"] == {"start": 0, "stop": 0}
     assert stream_datum["indices"] == {"start": 0, "stop": 1}
 
 
 async def test_can_decribe_collect(adaravis: AravisDetector):
-    set_sim_value(adaravis._writer.hdf.file_path_exists, True)
-    set_sim_value(adaravis._writer.hdf.capture, True)
+    set_mock_value(adaravis._writer.hdf.file_path_exists, True)
+    set_mock_value(adaravis._writer.hdf.capture, True)
     assert (await adaravis.describe_collect()) == {}
     await adaravis.stage()
     assert (await adaravis.describe_collect()) == {
         "adaravis": {
-            "source": "soft://adaravis-hdf-full_file_name",
+            "source": "mock+ca://ADARAVIS:HDF1:FullFileName_RBV",
             "shape": (0, 0),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
 
 async def test_unsupported_trigger_excepts(adaravis: AravisDetector):
-    set_sim_value(adaravis.drv.model, "Manta G-125")
-    set_sim_value(adaravis.drv.pixel_format, "Mono12Packed")
+    set_mock_value(adaravis.drv.model, "Manta G-125")
+    set_mock_value(adaravis.drv.pixel_format, "Mono12Packed")
     with pytest.raises(
         ValueError,
         # str(EnumClass.value) handling changed in Python 3.11
         match=r"AravisController only supports the following trigger types: .* but",
     ):
         await adaravis.prepare(TriggerInfo(1, DetectorTrigger.variable_gate, 1, 1))
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_controllers.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_controllers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from ophyd_async.epics.areadetector.drivers import ADBase, PilatusDriver
 from ophyd_async.epics.areadetector.drivers.pilatus_driver import PilatusTriggerMode
 from ophyd_async.epics.areadetector.utils import ImageMode
 
 
 @pytest.fixture
 async def pilatus(RE) -> PilatusController:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         drv = PilatusDriver("DRIVER:")
         controller = PilatusController(drv)
 
     return controller
 
 
 @pytest.fixture
 async def ad(RE) -> ADSimController:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         drv = ADBase("DRIVER:")
         controller = ADSimController(drv)
 
     return controller
 
 
 async def test_ad_controller(RE, ad: ADSimController):
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_drivers.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_drivers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import asyncio
 
 import pytest
 
-from ophyd_async.core import DeviceCollector, set_sim_value
+from ophyd_async.core import DeviceCollector, set_mock_value
 from ophyd_async.epics.areadetector.drivers import (
     ADBase,
     DetectorState,
     start_acquiring_driver_and_ensure_status,
 )
 
 
 @pytest.fixture
 def driver(RE) -> ADBase:
-    with DeviceCollector(sim=True):
+    with DeviceCollector(mock=True):
         driver = ADBase("DRV:", name="drv")
     return driver
 
 
 async def test_start_acquiring_driver_and_ensure_status_flags_immediate_failure(
     driver: ADBase,
 ):
-    set_sim_value(driver.detector_state, DetectorState.Error)
+    set_mock_value(driver.detector_state, DetectorState.Error)
     acquiring = await start_acquiring_driver_and_ensure_status(driver, timeout=0.01)
     with pytest.raises(ValueError):
         await acquiring
 
 
 async def test_start_acquiring_driver_and_ensure_status_fails_after_some_time(
     driver: ADBase,
 ):
     """This test ensures a failing status is captured halfway through acquisition.
 
     Real world application; it takes some time to start acquiring, and during that time
     the detector gets itself into a bad state.
     """
-    set_sim_value(driver.detector_state, DetectorState.Idle)
+    set_mock_value(driver.detector_state, DetectorState.Idle)
 
     async def wait_then_fail():
         await asyncio.sleep(0)
-        set_sim_value(driver.detector_state, DetectorState.Disconnected)
+        set_mock_value(driver.detector_state, DetectorState.Disconnected)
 
     acquiring = await start_acquiring_driver_and_ensure_status(driver, timeout=0.1)
     await wait_then_fail()
 
     with pytest.raises(ValueError):
         await acquiring
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_kinetix.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_kinetix.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import pytest
 from bluesky.run_engine import RunEngine
 
 from ophyd_async.core import (
     DetectorTrigger,
     DeviceCollector,
     DirectoryProvider,
-    set_sim_value,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.kinetix import KinetixDetector
 
 
 @pytest.fixture
 async def adkinetix(
     RE: RunEngine,
     static_directory_provider: DirectoryProvider,
 ) -> KinetixDetector:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         adkinetix = KinetixDetector("KINETIX:", static_directory_provider)
 
     return adkinetix
 
 
 async def test_get_deadtime(
     adkinetix: KinetixDetector,
 ):
     # Currently Kinetix driver doesn't support getting deadtime.
     assert adkinetix._controller.get_deadtime(0) == 0.001
 
 
 async def test_trigger_modes(adkinetix: KinetixDetector):
-    set_sim_value(adkinetix.drv.trigger_mode, "Internal")
+    set_mock_value(adkinetix.drv.trigger_mode, "Internal")
 
     async def setup_trigger_mode(trig_mode: DetectorTrigger):
         await adkinetix.controller.arm(num=1, trigger=trig_mode)
         # Prevent timeouts
-        set_sim_value(adkinetix.drv.acquire, True)
+        set_mock_value(adkinetix.drv.acquire, True)
 
     # Default TriggerSource
     assert (await adkinetix.drv.trigger_mode.get_value()) == "Internal"
 
     await setup_trigger_mode(DetectorTrigger.edge_trigger)
     assert (await adkinetix.drv.trigger_mode.get_value()) == "Rising Edge"
 
@@ -58,37 +58,37 @@
 
 async def test_can_read(adkinetix: KinetixDetector):
     # Standard detector can be used as Readable
     assert (await adkinetix.read()) == {}
 
 
 async def test_decribe_describes_writer_dataset(adkinetix: KinetixDetector):
-    set_sim_value(adkinetix._writer.hdf.file_path_exists, True)
-    set_sim_value(adkinetix._writer.hdf.capture, True)
+    set_mock_value(adkinetix._writer.hdf.file_path_exists, True)
+    set_mock_value(adkinetix._writer.hdf.capture, True)
 
     assert await adkinetix.describe() == {}
     await adkinetix.stage()
     assert await adkinetix.describe() == {
         "adkinetix": {
-            "source": "soft://adkinetix-hdf-full_file_name",
+            "source": "mock+ca://KINETIX:HDF1:FullFileName_RBV",
             "shape": (0, 0),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
 
 async def test_can_collect(
     adkinetix: KinetixDetector, static_directory_provider: DirectoryProvider
 ):
     directory_info = static_directory_provider()
     full_file_name = directory_info.root / directory_info.resource_dir / "foo.h5"
-    set_sim_value(adkinetix.hdf.full_file_name, str(full_file_name))
-    set_sim_value(adkinetix._writer.hdf.file_path_exists, True)
-    set_sim_value(adkinetix._writer.hdf.capture, True)
+    set_mock_value(adkinetix.hdf.full_file_name, str(full_file_name))
+    set_mock_value(adkinetix._writer.hdf.file_path_exists, True)
+    set_mock_value(adkinetix._writer.hdf.capture, True)
     await adkinetix.stage()
     docs = [(name, doc) async for name, doc in adkinetix.collect_asset_docs(1)]
     assert len(docs) == 2
     assert docs[0][0] == "stream_resource"
     stream_resource = docs[0][1]
     sr_uid = stream_resource["uid"]
     assert stream_resource["data_key"] == "adkinetix"
@@ -107,19 +107,19 @@
     stream_datum = docs[1][1]
     assert stream_datum["stream_resource"] == sr_uid
     assert stream_datum["seq_nums"] == {"start": 0, "stop": 0}
     assert stream_datum["indices"] == {"start": 0, "stop": 1}
 
 
 async def test_can_decribe_collect(adkinetix: KinetixDetector):
-    set_sim_value(adkinetix._writer.hdf.file_path_exists, True)
-    set_sim_value(adkinetix._writer.hdf.capture, True)
+    set_mock_value(adkinetix._writer.hdf.file_path_exists, True)
+    set_mock_value(adkinetix._writer.hdf.capture, True)
     assert (await adkinetix.describe_collect()) == {}
     await adkinetix.stage()
     assert (await adkinetix.describe_collect()) == {
         "adkinetix": {
-            "source": "soft://adkinetix-hdf-full_file_name",
+            "source": "mock+ca://KINETIX:HDF1:FullFileName_RBV",
             "shape": (0, 0),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_pilatus.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_pilatus.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from bluesky.run_engine import RunEngine
 
 from ophyd_async.core import (
     DetectorTrigger,
     DeviceCollector,
     DirectoryProvider,
     TriggerInfo,
-    set_sim_value,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.drivers.pilatus_driver import PilatusTriggerMode
 from ophyd_async.epics.areadetector.pilatus import PilatusDetector
 
 
 @pytest.fixture
 async def pilatus(
     RE: RunEngine,
     static_directory_provider: DirectoryProvider,
 ) -> PilatusDetector:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         adpilatus = PilatusDetector("PILATUS:", static_directory_provider)
 
     return adpilatus
 
 
 async def test_deadtime_invariant(
     pilatus: PilatusDetector,
@@ -44,15 +44,15 @@
     pilatus: PilatusDetector,
     detector_trigger: DetectorTrigger,
     expected_trigger_mode: PilatusTriggerMode,
 ):
     async def trigger_and_complete():
         await pilatus.controller.arm(num=1, trigger=detector_trigger)
         # Prevent timeouts
-        set_sim_value(pilatus.controller._drv.acquire, True)
+        set_mock_value(pilatus.controller._drv.acquire, True)
 
     # Default TriggerMode
     assert (await pilatus.drv.trigger_mode.get_value()) == PilatusTriggerMode.internal
 
     await trigger_and_complete()
 
     # TriggerSource changes
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_scans.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_scans.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DetectorTrigger,
     DeviceCollector,
     HardwareTriggeredFlyable,
     StandardDetector,
     StaticDirectoryProvider,
     TriggerInfo,
     TriggerLogic,
-    set_sim_value,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.controllers import ADSimController
 from ophyd_async.epics.areadetector.drivers import ADBase
 from ophyd_async.epics.areadetector.writers import HDFWriter, NDFileHDF
 
 
 class DummyTriggerLogic(TriggerLogic[int]):
@@ -53,23 +53,23 @@
 
     def get_deadtime(self, exposure: float) -> float:
         return 0.002
 
 
 @pytest.fixture
 def controller(RE) -> ADSimController:
-    with DeviceCollector(sim=True):
+    with DeviceCollector(mock=True):
         drv = ADBase("DRV")
 
     return ADSimController(drv)
 
 
 @pytest.fixture
 def writer(RE, tmp_path: Path) -> HDFWriter:
-    with DeviceCollector(sim=True):
+    with DeviceCollector(mock=True):
         hdf = NDFileHDF("HDF")
 
     return HDFWriter(
         hdf,
         directory_provider=StaticDirectoryProvider(tmp_path),
         name_provider=lambda: "test",
         shape_provider=AsyncMock(),
@@ -77,28 +77,28 @@
 
 
 async def test_hdf_writer_fails_on_timeout_with_stepscan(
     RE: RunEngine,
     writer: HDFWriter,
     controller: ADSimController,
 ):
-    set_sim_value(writer.hdf.file_path_exists, True)
+    set_mock_value(writer.hdf.file_path_exists, True)
     detector: StandardDetector[Any] = StandardDetector(
         controller, writer, name="detector", writer_timeout=0.01
     )
 
     with pytest.raises(Exception) as exc:
         RE(bp.count([detector]))
 
     assert isinstance(exc.value.__cause__, asyncio.TimeoutError)
 
 
 def test_hdf_writer_fails_on_timeout_with_flyscan(RE: RunEngine, writer: HDFWriter):
     controller = DummyController()
-    set_sim_value(writer.hdf.file_path_exists, True)
+    set_mock_value(writer.hdf.file_path_exists, True)
 
     detector: StandardDetector[Optional[TriggerInfo]] = StandardDetector(
         controller, writer, writer_timeout=0.01
     )
     trigger_logic = DummyTriggerLogic()
 
     flyer = HardwareTriggeredFlyable(trigger_logic, [], name="flyer")
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_single_trigger_det.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_single_trigger_det.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import bluesky.plans as bp
 import pytest
 from bluesky import RunEngine
 
-from ophyd_async.core import DeviceCollector, set_sim_value
+from ophyd_async.core import DeviceCollector, set_mock_value
 from ophyd_async.epics.areadetector import ImageMode, SingleTriggerDet
 from ophyd_async.epics.areadetector.drivers import ADBase
 from ophyd_async.epics.areadetector.writers import NDPluginStats
 
 
 @pytest.fixture
 async def single_trigger_det():
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         stats = NDPluginStats("PREFIX:STATS")
         det = SingleTriggerDet(
             drv=ADBase("PREFIX:DRV"), stats=stats, read_uncached=[stats.unique_id]
         )
 
     assert det.name == "det"
     assert stats.name == "det-stats"
     # Set non-default values to check they are set back
-    # These are using set_sim_value to simulate the backend IOC being setup
+    # These are using set_mock_value to simulate the backend IOC being setup
     # in a particular way, rather than values being set by the Ophyd signals
-    set_sim_value(det.drv.acquire_time, 0.5)
-    set_sim_value(det.drv.array_counter, 1)
-    set_sim_value(det.drv.image_mode, ImageMode.continuous)
-    set_sim_value(stats.unique_id, 3)
+    set_mock_value(det.drv.acquire_time, 0.5)
+    set_mock_value(det.drv.array_counter, 1)
+    set_mock_value(det.drv.image_mode, ImageMode.continuous)
+    set_mock_value(stats.unique_id, 3)
     yield det
 
 
 async def test_single_trigger_det(single_trigger_det: SingleTriggerDet, RE: RunEngine):
     names = []
     docs = []
     RE.subscribe(lambda name, _: names.append(name))
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_utils.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_utils.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_vimba.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_vimba.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import pytest
 from bluesky.run_engine import RunEngine
 
 from ophyd_async.core import (
     DetectorTrigger,
     DeviceCollector,
     DirectoryProvider,
-    set_sim_value,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.vimba import VimbaDetector
 
 
 @pytest.fixture
 async def advimba(
     RE: RunEngine,
     static_directory_provider: DirectoryProvider,
 ) -> VimbaDetector:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         advimba = VimbaDetector("VIMBA:", static_directory_provider)
 
     return advimba
 
 
 async def test_get_deadtime(
     advimba: VimbaDetector,
 ):
     # Currently Vimba controller doesn't support getting deadtime.
     assert advimba._controller.get_deadtime(0) == 0.001
 
 
 async def test_arming_trig_modes(advimba: VimbaDetector):
-    set_sim_value(advimba.drv.trig_source, "Freerun")
-    set_sim_value(advimba.drv.trigger_mode, "Off")
-    set_sim_value(advimba.drv.expose_mode, "Timed")
+    set_mock_value(advimba.drv.trig_source, "Freerun")
+    set_mock_value(advimba.drv.trigger_mode, "Off")
+    set_mock_value(advimba.drv.expose_mode, "Timed")
 
     async def setup_trigger_mode(trig_mode: DetectorTrigger):
         await advimba.controller.arm(num=1, trigger=trig_mode)
         # Prevent timeouts
-        set_sim_value(advimba.drv.acquire, True)
+        set_mock_value(advimba.drv.acquire, True)
 
     # Default TriggerSource
     assert (await advimba.drv.trig_source.get_value()) == "Freerun"
     assert (await advimba.drv.trigger_mode.get_value()) == "Off"
     assert (await advimba.drv.expose_mode.get_value()) == "Timed"
 
     await setup_trigger_mode(DetectorTrigger.edge_trigger)
@@ -70,37 +70,37 @@
 
 async def test_can_read(advimba: VimbaDetector):
     # Standard detector can be used as Readable
     assert (await advimba.read()) == {}
 
 
 async def test_decribe_describes_writer_dataset(advimba: VimbaDetector):
-    set_sim_value(advimba._writer.hdf.file_path_exists, True)
-    set_sim_value(advimba._writer.hdf.capture, True)
+    set_mock_value(advimba._writer.hdf.file_path_exists, True)
+    set_mock_value(advimba._writer.hdf.capture, True)
 
     assert await advimba.describe() == {}
     await advimba.stage()
     assert await advimba.describe() == {
         "advimba": {
-            "source": "soft://advimba-hdf-full_file_name",
+            "source": "mock+ca://VIMBA:HDF1:FullFileName_RBV",
             "shape": (0, 0),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
 
 async def test_can_collect(
     advimba: VimbaDetector, static_directory_provider: DirectoryProvider
 ):
     directory_info = static_directory_provider()
     full_file_name = directory_info.root / directory_info.resource_dir / "foo.h5"
-    set_sim_value(advimba.hdf.full_file_name, str(full_file_name))
-    set_sim_value(advimba._writer.hdf.file_path_exists, True)
-    set_sim_value(advimba._writer.hdf.capture, True)
+    set_mock_value(advimba.hdf.full_file_name, str(full_file_name))
+    set_mock_value(advimba._writer.hdf.file_path_exists, True)
+    set_mock_value(advimba._writer.hdf.capture, True)
     await advimba.stage()
     docs = [(name, doc) async for name, doc in advimba.collect_asset_docs(1)]
     assert len(docs) == 2
     assert docs[0][0] == "stream_resource"
     stream_resource = docs[0][1]
     sr_uid = stream_resource["uid"]
     assert stream_resource["data_key"] == "advimba"
@@ -119,19 +119,19 @@
     stream_datum = docs[1][1]
     assert stream_datum["stream_resource"] == sr_uid
     assert stream_datum["seq_nums"] == {"start": 0, "stop": 0}
     assert stream_datum["indices"] == {"start": 0, "stop": 1}
 
 
 async def test_can_decribe_collect(advimba: VimbaDetector):
-    set_sim_value(advimba._writer.hdf.file_path_exists, True)
-    set_sim_value(advimba._writer.hdf.capture, True)
+    set_mock_value(advimba._writer.hdf.file_path_exists, True)
+    set_mock_value(advimba._writer.hdf.capture, True)
     assert (await advimba.describe_collect()) == {}
     await advimba.stage()
     assert (await advimba.describe_collect()) == {
         "advimba": {
-            "source": "soft://advimba-hdf-full_file_name",
+            "source": "mock+ca://VIMBA:HDF1:FullFileName_RBV",
             "shape": (0, 0),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
```

### Comparing `ophyd_async-0.3a3/tests/epics/areadetector/test_writers.py` & `ophyd_async-0.3a4/tests/epics/areadetector/test_writers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 
 import pytest
 
 from ophyd_async.core import (
     DeviceCollector,
     ShapeProvider,
     StaticDirectoryProvider,
-    set_sim_value,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.writers import HDFWriter, NDFileHDF
 
 
 class DummyShapeProvider(ShapeProvider):
     def __init__(self) -> None:
         pass
 
     async def __call__(self) -> Sequence[int]:
         return (10, 10)
 
 
 @pytest.fixture
 async def hdf_writer(RE) -> HDFWriter:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         hdf = NDFileHDF("HDF:")
 
     return HDFWriter(
         hdf,
         StaticDirectoryProvider("some_path", "some_prefix"),
         name_provider=lambda: "test",
         shape_provider=DummyShapeProvider(),
     )
 
 
 async def test_correct_descriptor_doc_after_open(hdf_writer: HDFWriter):
-    set_sim_value(hdf_writer.hdf.file_path_exists, True)
+    set_mock_value(hdf_writer.hdf.file_path_exists, True)
     with patch("ophyd_async.core.signal.wait_for_value", return_value=None):
         descriptor = await hdf_writer.open()
 
     assert descriptor == {
         "test": {
-            "source": "soft://hdf-full_file_name",
+            "source": "mock+ca://HDF:FullFileName_RBV",
             "shape": (10, 10),
             "dtype": "array",
             "external": "STREAM:",
         }
     }
 
     await hdf_writer.close()
```

### Comparing `ophyd_async-0.3a3/tests/epics/demo/test_demo_ad_sim_detector.py` & `ophyd_async-0.3a4/tests/epics/demo/test_demo_ad_sim_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 from bluesky.utils import new_uid
 
 from ophyd_async.core import (
     AsyncStatus,
     DeviceCollector,
     StandardDetector,
     StaticDirectoryProvider,
-    set_sim_callback,
-    set_sim_value,
+    callback_on_mock_put,
+    set_mock_value,
 )
 from ophyd_async.epics.areadetector.controllers import ADSimController
 from ophyd_async.epics.areadetector.drivers import ADBase
 from ophyd_async.epics.areadetector.utils import FileWriteMode, ImageMode
 from ophyd_async.epics.areadetector.writers import HDFWriter, NDFileHDF
 from ophyd_async.epics.demo.demo_ad_sim_detector import DemoADSimDetector
 
 
 async def make_detector(prefix: str, name: str, tmp_path: Path):
     dp = StaticDirectoryProvider(tmp_path, f"test-{new_uid()}")
 
-    async with DeviceCollector(sim=True):
-        drv = ADBase(f"{prefix}DRV:")
+    async with DeviceCollector(mock=True):
+        drv = ADBase(f"{prefix}DRV:", name="drv")
         hdf = NDFileHDF(f"{prefix}HDF:")
         det = DemoADSimDetector(
             drv, hdf, dp, config_sigs=[drv.acquire_time, drv.acquire], name=name
         )
 
-    def _set_full_file_name(_, val):
-        set_sim_value(hdf.full_file_name, str(tmp_path / val))
+    def _set_full_file_name(val, *args, **kwargs):
+        set_mock_value(hdf.full_file_name, str(tmp_path / val))
 
-    set_sim_callback(hdf.file_name, _set_full_file_name)
+    callback_on_mock_put(hdf.file_name, _set_full_file_name)
 
     return det
 
 
 def count_sim(dets: List[StandardDetector], times: int = 1):
     """Test plan to do the equivalent of bp.count for a sim detector."""
 
@@ -56,15 +56,15 @@
             )
 
         for det in dets:
             yield from bps.trigger(det, wait=False, group="wait_for_trigger")
 
         yield from bps.sleep(0.001)
         [
-            set_sim_value(
+            set_mock_value(
                 cast(HDFWriter, det.writer).hdf.num_captured, read_values[det] + 1
             )
             for det in dets
         ]
 
         yield from bps.wait(group="wait_for_trigger")
         yield from bps.create()
@@ -78,49 +78,49 @@
     yield from bps.unstage_all(*dets)
 
 
 @pytest.fixture
 async def single_detector(RE: RunEngine, tmp_path: Path) -> StandardDetector:
     detector = await make_detector(prefix="TEST:", name="test", tmp_path=tmp_path)
 
-    set_sim_value(detector._controller.driver.array_size_x, 10)
-    set_sim_value(detector._controller.driver.array_size_y, 20)
+    set_mock_value(detector._controller.driver.array_size_x, 10)
+    set_mock_value(detector._controller.driver.array_size_y, 20)
     return detector
 
 
 @pytest.fixture
 async def two_detectors(tmp_path: Path):
     deta = await make_detector(prefix="PREFIX1:", name="testa", tmp_path=tmp_path)
     detb = await make_detector(prefix="PREFIX2:", name="testb", tmp_path=tmp_path)
 
     # Simulate backend IOCs being in slightly different states
     for i, det in enumerate((deta, detb)):
         # accessing the hidden objects just for neat typing
         controller = det._controller
         writer = det._writer
 
-        set_sim_value(controller.driver.acquire_time, 0.8 + i)
-        set_sim_value(controller.driver.image_mode, ImageMode.continuous)
-        set_sim_value(writer.hdf.num_capture, 1000)
-        set_sim_value(writer.hdf.num_captured, 0)
-        set_sim_value(controller.driver.array_size_x, 1024 + i)
-        set_sim_value(controller.driver.array_size_y, 768 + i)
+        set_mock_value(controller.driver.acquire_time, 0.8 + i)
+        set_mock_value(controller.driver.image_mode, ImageMode.continuous)
+        set_mock_value(writer.hdf.num_capture, 1000)
+        set_mock_value(writer.hdf.num_captured, 0)
+        set_mock_value(controller.driver.array_size_x, 1024 + i)
+        set_mock_value(controller.driver.array_size_y, 768 + i)
     yield deta, detb
 
 
 async def test_two_detectors_step(
     two_detectors: List[StandardDetector],
     RE: RunEngine,
 ):
     names = []
     docs = []
     RE.subscribe(lambda name, _: names.append(name))
     RE.subscribe(lambda _, doc: docs.append(doc))
     [
-        set_sim_value(cast(HDFWriter, det._writer).hdf.file_path_exists, True)
+        set_mock_value(cast(HDFWriter, det._writer).hdf.file_path_exists, True)
         for det in two_detectors
     ]
 
     RE(count_sim(two_detectors, times=1))
 
     controller_a = cast(ADSimController, two_detectors[0].controller)
     writer_a = cast(HDFWriter, two_detectors[0].writer)
@@ -180,15 +180,15 @@
 async def test_detector_writes_to_file(
     RE: RunEngine, single_detector: StandardDetector, tmp_path: Path
 ):
     names = []
     docs = []
     RE.subscribe(lambda name, _: names.append(name))
     RE.subscribe(lambda _, doc: docs.append(doc))
-    set_sim_value(cast(HDFWriter, single_detector._writer).hdf.file_path_exists, True)
+    set_mock_value(cast(HDFWriter, single_detector._writer).hdf.file_path_exists, True)
 
     RE(count_sim([single_detector], times=3))
 
     assert await cast(
         HDFWriter, single_detector.writer
     ).hdf.file_path.get_value() == str(tmp_path)
 
@@ -210,20 +210,20 @@
 
 
 async def test_read_and_describe_detector(single_detector: StandardDetector):
     describe = await single_detector.describe_configuration()
     read = await single_detector.read_configuration()
     assert describe == {
         "test-drv-acquire_time": {
-            "source": "soft://test-drv-acquire_time",
+            "source": "mock+ca://TEST:DRV:AcquireTime_RBV",
             "dtype": "number",
             "shape": [],
         },
         "test-drv-acquire": {
-            "source": "soft://test-drv-acquire",
+            "source": "mock+ca://TEST:DRV:Acquire_RBV",
             "dtype": "boolean",
             "shape": [],
         },
     }
     assert read == {
         "test-drv-acquire_time": {
             "value": 0.0,
@@ -248,26 +248,26 @@
     1. the detector.controller is armed, and that starts the acquisition so that,
     2. The detector.writer.hdf.num_captured is 1
 
     Probably the best thing to do here is mock the detector.controller.driver and
     detector.writer.hdf. Then, mock out set_and_wait_for_value in
     ophyd_async.epics.DemoADSimDetector.controllers.standard_controller.ADSimController
     so that, as well as setting detector.controller.driver.acquire to True, it sets
-    detector.writer.hdf.num_captured to 1, using set_sim_value
+    detector.writer.hdf.num_captured to 1, using set_mock_value
     """
     ...
 
 
 async def test_detector_with_unnamed_or_disconnected_config_sigs(RE, tmp_path: Path):
     dp = StaticDirectoryProvider(tmp_path)
     drv = ADBase("FOO:DRV:")
 
     some_other_driver = ADBase("TEST")
 
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         hdf = NDFileHDF("FOO:HDF:")
         det = DemoADSimDetector(
             drv,
             hdf,
             dp,
             config_sigs=[some_other_driver.acquire_time, drv.acquire],
             name="foo",
```

### Comparing `ophyd_async-0.3a3/tests/epics/motion/test_motor.py` & `ophyd_async-0.3a4/tests/epics/motion/test_motor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import asyncio
 from typing import Dict
 from unittest.mock import Mock, call
 
 import pytest
 from bluesky.protocols import Reading
 
-from ophyd_async.core import DeviceCollector, set_sim_put_proceeds, set_sim_value
+from ophyd_async.core import (
+    DeviceCollector,
+    set_mock_put_proceeds,
+    set_mock_value,
+)
 from ophyd_async.epics.motion import motor
 
 # Long enough for multiple asyncio event loop cycles to run so
 # all the tasks have a chance to run
-A_BIT = 0.001
+A_BIT = 0.01
 
 
 @pytest.fixture
 async def sim_motor():
-    async with DeviceCollector(sim=True):
-        sim_motor = motor.Motor("BLxxI-MO-TABLE-01:X")
-        # Signals connected here
-
-    assert sim_motor.name == "sim_motor"
-    set_sim_value(sim_motor.motor_egu, "mm")
-    set_sim_value(sim_motor.precision, 3)
-    set_sim_value(sim_motor.velocity, 1)
+    async with DeviceCollector(mock=True):
+        sim_motor = motor.Motor("BLxxI-MO-TABLE-01:X", name="sim_motor")
+
+    set_mock_value(sim_motor.motor_egu, "mm")
+    set_mock_value(sim_motor.precision, 3)
+    set_mock_value(sim_motor.velocity, 1)
     yield sim_motor
 
 
 async def test_motor_moving_well(sim_motor: motor.Motor) -> None:
-    set_sim_put_proceeds(sim_motor.user_setpoint, False)
+    set_mock_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(0.55)
     watcher = Mock()
     s.watch(watcher)
     done = Mock()
     s.add_callback(done)
     await asyncio.sleep(A_BIT)
     assert watcher.call_count == 1
@@ -44,56 +46,56 @@
         precision=3,
         time_elapsed=pytest.approx(0.0, abs=0.05),
     )
     watcher.reset_mock()
     assert 0.55 == await sim_motor.user_setpoint.get_value()
     assert not s.done
     await asyncio.sleep(0.1)
-    set_sim_value(sim_motor.user_readback, 0.1)
+    set_mock_value(sim_motor.user_readback, 0.1)
     assert watcher.call_count == 1
     assert watcher.call_args == call(
         name="sim_motor",
         current=0.1,
         initial=0.0,
         target=0.55,
         unit="mm",
         precision=3,
         time_elapsed=pytest.approx(0.1, abs=0.05),
     )
-    set_sim_put_proceeds(sim_motor.user_setpoint, True)
+    set_mock_put_proceeds(sim_motor.user_setpoint, True)
     await asyncio.sleep(A_BIT)
     assert s.done
     done.assert_called_once_with(s)
 
 
 async def test_motor_moving_stopped(sim_motor: motor.Motor):
-    set_sim_put_proceeds(sim_motor.user_setpoint, False)
+    set_mock_put_proceeds(sim_motor.user_setpoint, False)
     s = sim_motor.set(1.5)
     s.add_callback(Mock())
     await asyncio.sleep(0.2)
     assert not s.done
     await sim_motor.stop()
-    set_sim_put_proceeds(sim_motor.user_setpoint, True)
+    set_mock_put_proceeds(sim_motor.user_setpoint, True)
     await asyncio.sleep(A_BIT)
     assert s.done
     assert s.success is False
 
 
 async def test_read_motor(sim_motor: motor.Motor):
-    sim_motor.stage()
+    await sim_motor.stage()
     assert (await sim_motor.read())["sim_motor"]["value"] == 0.0
     assert (await sim_motor.read_configuration())["sim_motor-velocity"]["value"] == 1
     assert (await sim_motor.describe_configuration())["sim_motor-motor_egu"][
         "shape"
     ] == []
-    set_sim_value(sim_motor.user_readback, 0.5)
+    set_mock_value(sim_motor.user_readback, 0.5)
     assert (await sim_motor.read())["sim_motor"]["value"] == 0.5
-    sim_motor.unstage()
+    await sim_motor.unstage()
     # Check we can still read and describe when not staged
-    set_sim_value(sim_motor.user_readback, 0.1)
+    set_mock_value(sim_motor.user_readback, 0.1)
     assert (await sim_motor.read())["sim_motor"]["value"] == 0.1
     assert await sim_motor.describe()
 
 
 async def test_set_velocity(sim_motor: motor.Motor) -> None:
     v = sim_motor.velocity
     q: asyncio.Queue[Dict[str, Reading]] = asyncio.Queue()
```

### Comparing `ophyd_async-0.3a3/tests/epics/test_pvi.py` & `ophyd_async-0.3a4/tests/epics/test_pvi.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,25 +41,27 @@
 
     class TestDevice(Block3, Device):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             super().__init__(name)
 
         async def connect(
-            self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT
+            self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT
         ) -> None:
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
 
-            await super().connect(sim)
+            await super().connect(mock=mock)
 
     yield TestDevice
 
 
-async def test_fill_pvi_entries_sim_mode(pvi_test_device_t):
-    async with DeviceCollector(sim=True):
+async def test_fill_pvi_entries_mock_mode(pvi_test_device_t):
+    async with DeviceCollector(mock=True):
         test_device = pvi_test_device_t("PREFIX:")
 
     # device vectors are typed
     assert isinstance(test_device.device_vector[1], Block2)
     assert isinstance(test_device.device_vector[2], Block2)
 
     # elements of device vectors are typed recursively
@@ -103,19 +105,21 @@
     class TestDevice(Block3, Device):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             super().__init__(name)
             create_children_from_annotations(self)
 
         async def connect(
-            self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT
+            self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT
         ) -> None:
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
 
-            await super().connect(sim)
+            await super().connect(mock=mock)
 
     yield TestDevice
 
 
 async def test_device_create_children_from_annotations(
     pvi_test_device_create_children_from_annotations_t,
 ):
@@ -130,13 +134,13 @@
     assert isinstance(block_2_device, Block2)
     assert isinstance(block_1_device, Block1)
     assert isinstance(top_block_1_device, Block1)
     assert not hasattr(device, "signal_x")
     assert not hasattr(device, "signal_rw")
     assert not hasattr(top_block_1_device, "signal_rw")
 
-    await device.connect(sim=True)
+    await device.connect(mock=True)
 
     # The memory addresses have not changed
     assert device.device is block_2_device
     assert device.device.device is block_1_device
     assert device.signal_device is top_block_1_device
```

### Comparing `ophyd_async-0.3a3/tests/epics/test_records.db` & `ophyd_async-0.3a4/tests/epics/test_records.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/epics/test_signals.py` & `ophyd_async-0.3a4/tests/epics/test_signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,24 @@
             RECORDS,
         ],
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         universal_newlines=True,
     )
+
+    start_time = time.monotonic()
+    while "iocRun: All initialization complete" not in (
+        process.stdout.readline().strip()
+    ):
+        if time.monotonic() - start_time > 10:
+            raise TimeoutError("IOC did not start in time")
+
     yield IOC(process, protocol)
+
     # close backend caches before the event loop
     purge_channel_caches()
     try:
         print(process.communicate("exit")[0])
     except ValueError:
         # Someone else already called communicate
         pass
@@ -198,14 +207,15 @@
 @pytest.mark.parametrize(
     "datatype, suffix, initial_value, put_value, descriptor",
     [
         (int, "int", 42, 43, integer_d),
         (float, "float", 3.141, 43.5, number_d),
         (str, "str", "hello", "goodbye", string_d),
         (MyEnum, "enum", MyEnum.b, MyEnum.c, enum_d),
+        (str, "enum", "Bbb", "Ccc", enum_d),
         (npt.NDArray[np.int8], "int8a", [-128, 127], [-8, 3, 44], waveform_d),
         (npt.NDArray[np.uint8], "uint8a", [0, 255], [218], waveform_d),
         (npt.NDArray[np.int16], "int16a", [-32768, 32767], [-855], waveform_d),
         (npt.NDArray[np.uint16], "uint16a", [0, 65535], [5666], waveform_d),
         (npt.NDArray[np.int32], "int32a", [-2147483648, 2147483647], [-2], waveform_d),
         (npt.NDArray[np.uint32], "uint32a", [0, 4294967295], [1022233], waveform_d),
         (npt.NDArray[np.int64], "int64a", [-2147483649, 2147483648], [-3], waveform_d),
@@ -334,15 +344,15 @@
                 "<enum 'BadEnum'>, which has ('Aaa', 'B', 'Ccc')"
             ),
         ),
         (int, "str", "has type str not int"),
         (str, "float", "has type float not str"),
         (str, "stra", "has type [str] not str"),
         (int, "uint8a", "has type [uint8] not int"),
-        (float, "enum", "has type Enum not float"),
+        (float, "enum", "is type Enum but doesn't inherit from String"),
         (npt.NDArray[np.int32], "float64a", "has type [float64] not [int32]"),
     ],
 )
 async def test_backend_wrong_type_errors(ioc: IOC, typ, suff, error):
     with pytest.raises(
         TypeError, match=re.escape(f"{PV_PREFIX}:{ioc.protocol}:{suff} {error}")
     ):
@@ -531,7 +541,31 @@
     assert read._backend.read_pv == "Read"
 
     write = epics_signal_w(int, "Write")
     assert write._backend.write_pv == "Write"
 
     execute = epics_signal_x("Execute")
     assert execute._backend.write_pv == "Execute"
+
+
+async def test_str_enum_returns_enum(ioc: IOC):
+    await ioc.make_backend(MyEnum, "enum")
+    pv_name = f"{ioc.protocol}://{PV_PREFIX}:{ioc.protocol}:enum"
+
+    sig = epics_signal_rw(MyEnum, pv_name)
+    await sig.connect()
+    val = await sig.get_value()
+    assert repr(val) == "<MyEnum.b: 'Bbb'>"
+    assert val is MyEnum.b
+    assert val == "Bbb"
+
+
+async def test_str_returns_enum(ioc: IOC):
+    await ioc.make_backend(str, "enum")
+    pv_name = f"{ioc.protocol}://{PV_PREFIX}:{ioc.protocol}:enum"
+
+    sig = epics_signal_rw(str, pv_name)
+    await sig.connect()
+    val = await sig.get_value()
+    assert val == MyEnum.b
+    assert val == "Bbb"
+    assert val is not MyEnum.b
```

### Comparing `ophyd_async-0.3a3/tests/panda/db/panda.db` & `ophyd_async-0.3a4/tests/panda/db/panda.db`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/panda/test_hdf_panda.py` & `ophyd_async-0.3a4/tests/panda/test_hdf_panda.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,163 +1,130 @@
-import asyncio
-from typing import Dict, Optional
+from typing import Dict
 
 import pytest
 from bluesky import plan_stubs as bps
 from bluesky.run_engine import RunEngine
 
-from ophyd_async.core import StaticDirectoryProvider, set_sim_value
-from ophyd_async.core.async_status import AsyncStatus
-from ophyd_async.core.detector import DetectorControl, DetectorTrigger
+from ophyd_async.core import StaticDirectoryProvider, set_mock_value
 from ophyd_async.core.device import Device
 from ophyd_async.core.flyer import HardwareTriggeredFlyable
-from ophyd_async.core.signal import SignalR, assert_emitted, wait_for_value
-from ophyd_async.core.sim_signal_backend import SimSignalBackend
-from ophyd_async.core.utils import DEFAULT_TIMEOUT
-from ophyd_async.panda import HDFPanda, PcapBlock
+from ophyd_async.core.mock_signal_utils import callback_on_mock_put
+from ophyd_async.core.signal import SignalR, assert_emitted
+from ophyd_async.epics.signal.signal import epics_signal_r
+from ophyd_async.panda import HDFPanda
 from ophyd_async.panda._trigger import StaticSeqTableTriggerLogic
 from ophyd_async.panda.writers._hdf_writer import Capture
 from ophyd_async.planstubs.prepare_trigger_and_dets import (
     prepare_static_seq_table_flyer_and_detectors_with_same_trigger,
 )
 
 
-class MockPandaPcapController(DetectorControl):
-    def __init__(self, pcap: PcapBlock) -> None:
-        self.pcap = pcap
-
-    def get_deadtime(self, exposure: float) -> float:
-        return 0.000000008
-
-    async def arm(
-        self,
-        num: int,
-        trigger: DetectorTrigger = DetectorTrigger.constant_gate,
-        exposure: Optional[float] = None,
-        timeout=DEFAULT_TIMEOUT,
-    ) -> AsyncStatus:
-        assert trigger in (
-            DetectorTrigger.constant_gate,
-            trigger == DetectorTrigger.variable_gate,
-        ), (
-            f"Receieved trigger {trigger}. Only constant_gate and "
-            "variable_gate triggering is supported on the PandA"
-        )
-        await self.pcap.arm.set(True, wait=True, timeout=timeout)
-        await wait_for_value(self.pcap.active, True, timeout=timeout)
-        await asyncio.sleep(0.2)
-        await self.pcap.arm.set(False, wait=False, timeout=timeout)
-        return AsyncStatus(wait_for_value(self.pcap.active, False, timeout=None))
-
-    async def disarm(self, timeout=DEFAULT_TIMEOUT) -> AsyncStatus:
-        await self.pcap.arm.set(False, wait=True, timeout=timeout)
-        await wait_for_value(self.pcap.active, False, timeout=timeout)
-        await asyncio.sleep(0.2)
-        set_sim_value(self.pcap.active, True)
-        return AsyncStatus(wait_for_value(self.pcap.active, False, timeout=None))
-
-
 @pytest.fixture
-async def sim_hdf_panda(tmp_path):
+async def mock_hdf_panda(tmp_path):
     class CaptureBlock(Device):
         test_capture: SignalR
 
     directory_provider = StaticDirectoryProvider(str(tmp_path), filename_prefix="test")
-    sim_hdf_panda = HDFPanda(
+    mock_hdf_panda = HDFPanda(
         "HDFPANDA:", directory_provider=directory_provider, name="panda"
     )
-    sim_hdf_panda._controller = MockPandaPcapController(sim_hdf_panda.pcap)
     block_a = CaptureBlock(name="block_a")
     block_b = CaptureBlock(name="block_b")
-    block_a.test_capture = SignalR(backend=SimSignalBackend(Capture))
-    block_b.test_capture = SignalR(backend=SimSignalBackend(Capture))
+    block_a.test_capture = epics_signal_r(
+        Capture, "pva://test_capture_a", name="test_capture_a"
+    )
+    block_b.test_capture = epics_signal_r(
+        Capture, "pva://test_capture_b", name="test_capture_b"
+    )
 
-    setattr(sim_hdf_panda, "block_a", block_a)
-    setattr(sim_hdf_panda, "block_b", block_b)
-    await sim_hdf_panda.connect(sim=True)
-    set_sim_value(block_a.test_capture, Capture.Min)
-    set_sim_value(block_b.test_capture, Capture.Diff)
+    setattr(mock_hdf_panda, "block_a", block_a)
+    setattr(mock_hdf_panda, "block_b", block_b)
+    await mock_hdf_panda.connect(mock=True)
 
-    yield sim_hdf_panda
+    def link_function(value, **kwargs):
+        set_mock_value(mock_hdf_panda.pcap.active, value)
 
+    callback_on_mock_put(mock_hdf_panda.pcap.arm, link_function)
+    set_mock_value(block_a.test_capture, Capture.Min)
+    set_mock_value(block_b.test_capture, Capture.Diff)
 
-async def test_hdf_panda_passes_blocks_to_controller(sim_hdf_panda: HDFPanda):
-    assert hasattr(sim_hdf_panda.controller, "pcap")
-    assert sim_hdf_panda.controller.pcap is sim_hdf_panda.pcap
+    yield mock_hdf_panda
+
+
+async def test_hdf_panda_passes_blocks_to_controller(mock_hdf_panda: HDFPanda):
+    assert hasattr(mock_hdf_panda.controller, "pcap")
+    assert mock_hdf_panda.controller.pcap is mock_hdf_panda.pcap
 
 
 async def test_hdf_panda_hardware_triggered_flyable(
     RE: RunEngine,
-    sim_hdf_panda,
+    mock_hdf_panda,
 ):
     docs = {}
 
     def append_and_print(name, doc):
         if name not in docs:
             docs[name] = []
         docs[name] += [doc]
 
     RE.subscribe(append_and_print)
 
     shutter_time = 0.004
     exposure = 1
 
-    trigger_logic = StaticSeqTableTriggerLogic(sim_hdf_panda.seq[1])
+    trigger_logic = StaticSeqTableTriggerLogic(mock_hdf_panda.seq[1])
     flyer = HardwareTriggeredFlyable(trigger_logic, [], name="flyer")
 
     def flying_plan():
-        yield from bps.stage_all(sim_hdf_panda, flyer)
+        yield from bps.stage_all(mock_hdf_panda, flyer)
 
         yield from prepare_static_seq_table_flyer_and_detectors_with_same_trigger(
             flyer,
-            [sim_hdf_panda],
+            [mock_hdf_panda],
             num=1,
             width=exposure,
-            deadtime=sim_hdf_panda.controller.get_deadtime(1),
+            deadtime=mock_hdf_panda.controller.get_deadtime(1),
             shutter_time=shutter_time,
         )
-        # sim_hdf_panda.controller.disarm.assert_called_once  # type: ignore
+        # mock_hdf_panda.controller.disarm.assert_called_once  # type: ignore
 
         yield from bps.open_run()
-        yield from bps.declare_stream(sim_hdf_panda, name="main_stream", collect=True)
+        yield from bps.declare_stream(mock_hdf_panda, name="main_stream", collect=True)
 
-        set_sim_value(flyer.trigger_logic.seq.active, 1)
+        set_mock_value(flyer.trigger_logic.seq.active, 1)
 
         yield from bps.kickoff(flyer, wait=True)
-        yield from bps.kickoff(sim_hdf_panda)
+        yield from bps.kickoff(mock_hdf_panda)
 
         yield from bps.complete(flyer, wait=False, group="complete")
-        yield from bps.complete(sim_hdf_panda, wait=False, group="complete")
+        yield from bps.complete(mock_hdf_panda, wait=False, group="complete")
 
         # Manually incremenet the index as if a frame was taken
-        set_sim_value(
-            sim_hdf_panda.data.num_captured,
-            sim_hdf_panda.data.num_captured._backend._value + 1,
-        )
-
-        set_sim_value(flyer.trigger_logic.seq.active, 0)
+        set_mock_value(mock_hdf_panda.data.num_captured, 1)
+        set_mock_value(flyer.trigger_logic.seq.active, 0)
 
         done = False
         while not done:
             try:
                 yield from bps.wait(group="complete", timeout=0.5)
             except TimeoutError:
                 pass
             else:
                 done = True
             yield from bps.collect(
-                sim_hdf_panda,
+                mock_hdf_panda,
                 return_payload=False,
                 name="main_stream",
             )
         yield from bps.wait(group="complete")
         yield from bps.close_run()
 
-        yield from bps.unstage_all(flyer, sim_hdf_panda)
-        # assert sim_hdf_panda.controller.disarm.called  # type: ignore
+        yield from bps.unstage_all(flyer, mock_hdf_panda)
+        yield from bps.wait_for([lambda: mock_hdf_panda.controller.disarm()])
+        # assert mock_hdf_panda.controller.disarm.called  # type: ignore
 
     # fly scan
     RE(flying_plan())
 
     assert_emitted(
         docs, start=1, descriptor=1, stream_resource=2, stream_datum=2, stop=1
     )
@@ -167,15 +134,15 @@
     assert data_key_names == [
         "panda-block_a-test-Min",
         "panda-block_b-test-Diff",
     ]
     for data_key_name in data_key_names:
         assert (
             docs["descriptor"][0]["data_keys"][data_key_name]["source"]
-            == "soft://panda-data-hdf_directory"
+            == "mock+soft://panda-data-hdf_directory"
         )
 
     # test stream resources
     for block_letter, stream_resource, data_key_name in zip(
         ("a", "b"), docs["stream_resource"], data_key_names
     ):
         assert stream_resource["data_key"] == data_key_name
```

### Comparing `ophyd_async-0.3a3/tests/panda/test_panda_connect.py` & `ophyd_async-0.3a4/tests/panda/test_panda_connect.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,41 +46,43 @@
 
     class Panda(CommonPandaBlocksNoData):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             create_children_from_annotations(self)
             super().__init__(name)
 
-        async def connect(self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT):
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
-            await super().connect(sim, timeout)
+        async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
+            await super().connect(mock=mock, timeout=timeout)
 
     yield Panda
 
 
 @pytest.fixture
-async def sim_panda(panda_t):
-    async with DeviceCollector(sim=True):
-        sim_panda = panda_t("PANDAQSRV:", "sim_panda")
+async def mock_panda(panda_t):
+    async with DeviceCollector(mock=True):
+        mock_panda = panda_t("PANDAQSRV:", "mock_panda")
 
-    assert sim_panda.name == "sim_panda"
-    yield sim_panda
+    assert mock_panda.name == "mock_panda"
+    yield mock_panda
 
 
-def test_panda_names_correct(sim_panda):
-    assert sim_panda.seq[1].name == "sim_panda-seq-1"
-    assert sim_panda.pulse[1].name == "sim_panda-pulse-1"
+def test_panda_names_correct(mock_panda):
+    assert mock_panda.seq[1].name == "mock_panda-seq-1"
+    assert mock_panda.pulse[1].name == "mock_panda-pulse-1"
 
 
 def test_panda_name_set(panda_t):
     panda = panda_t(":", "panda")
     assert panda.name == "panda"
 
 
-async def test_panda_children_connected(sim_panda):
+async def test_panda_children_connected(mock_panda):
     # try to set and retrieve from simulated values...
     table = SeqTable(
         repeats=np.array([1, 1, 1, 32]).astype(np.uint16),
         trigger=(
             SeqTrigger.POSA_GT,
             SeqTrigger.POSA_LT,
             SeqTrigger.IMMEDIATE,
@@ -98,19 +100,19 @@
         outa2=np.array([1, 0, 0, 1]).astype(np.bool_),
         outb2=np.array([0, 0, 1, 1]).astype(np.bool_),
         outc2=np.array([0, 1, 1, 0]).astype(np.bool_),
         outd2=np.array([1, 1, 0, 1]).astype(np.bool_),
         oute2=np.array([1, 0, 1, 0]).astype(np.bool_),
         outf2=np.array([1, 0, 0, 0]).astype(np.bool_),
     )
-    await sim_panda.pulse[1].delay.set(20.0)
-    await sim_panda.seq[1].table.set(table)
+    await mock_panda.pulse[1].delay.set(20.0)
+    await mock_panda.seq[1].table.set(table)
 
-    readback_pulse = await sim_panda.pulse[1].delay.get_value()
-    readback_seq = await sim_panda.seq[1].table.get_value()
+    readback_pulse = await mock_panda.pulse[1].delay.get_value()
+    readback_seq = await mock_panda.seq[1].table.get_value()
 
     assert readback_pulse == 20.0
     assert readback_seq == table
 
 
 async def test_panda_with_missing_blocks(panda_pva, panda_t):
     panda = panda_t("PANDAQSRVI:")
```

### Comparing `ophyd_async-0.3a3/tests/panda/test_panda_controller.py` & `ophyd_async-0.3a4/tests/panda/test_panda_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,44 +7,45 @@
 from ophyd_async.core import DEFAULT_TIMEOUT, DetectorTrigger, Device, DeviceCollector
 from ophyd_async.epics.pvi import fill_pvi_entries
 from ophyd_async.epics.signal import epics_signal_rw
 from ophyd_async.panda import CommonPandaBlocks, PandaPcapController
 
 
 @pytest.fixture
-async def sim_panda():
+async def mock_panda():
     class Panda(CommonPandaBlocks):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             super().__init__(name)
 
-        async def connect(self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT):
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
-            await super().connect(sim, timeout)
-
-    async with DeviceCollector(sim=True):
-        sim_panda = Panda("PANDACONTROLLER:", "sim_panda")
-        sim_panda.phase_1_signal_units = epics_signal_rw(int, "")
-    assert sim_panda.name == "sim_panda"
-    yield sim_panda
+        async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
+            await super().connect(mock=mock, timeout=timeout)
+
+    async with DeviceCollector(mock=True):
+        mock_panda = Panda("PANDACONTROLLER:", name="mock_panda")
+        mock_panda.phase_1_signal_units = epics_signal_rw(int, "")
+    yield mock_panda
 
 
 async def test_panda_controller_not_filled_blocks():
     class PcapBlock(Device):
         pass  # Not filled
 
     pandaController = PandaPcapController(pcap=PcapBlock())
     with patch("ophyd_async.panda._panda_controller.wait_for_value", return_value=None):
         with pytest.raises(AttributeError) as exc:
             await pandaController.arm(num=1, trigger=DetectorTrigger.constant_gate)
     assert ("'PcapBlock' object has no attribute 'arm'") in str(exc.value)
 
 
-async def test_panda_controller_arm_disarm(sim_panda):
-    pandaController = PandaPcapController(sim_panda.pcap)
+async def test_panda_controller_arm_disarm(mock_panda):
+    pandaController = PandaPcapController(mock_panda.pcap)
     with patch("ophyd_async.panda._panda_controller.wait_for_value", return_value=None):
         await pandaController.arm(num=1, trigger=DetectorTrigger.constant_gate)
     await pandaController.disarm()
 
 
 async def test_panda_controller_wrong_trigger():
     pandaController = PandaPcapController(None)
```

### Comparing `ophyd_async-0.3a3/tests/panda/test_panda_utils.py` & `ophyd_async-0.3a4/tests/panda/test_panda_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 from ophyd_async.epics.signal import epics_signal_rw
 from ophyd_async.panda import CommonPandaBlocks, TimeUnits
 from ophyd_async.panda._common_blocks import DataBlock
 from ophyd_async.panda._utils import phase_sorter
 
 
 @pytest.fixture
-async def sim_panda():
+async def mock_panda():
     class Panda(CommonPandaBlocks):
         data: DataBlock
 
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             super().__init__(name)
 
-        async def connect(self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT):
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
-            await super().connect(sim, timeout)
-
-    async with DeviceCollector(sim=True):
-        sim_panda = Panda("PANDA")
-        sim_panda.phase_1_signal_units = epics_signal_rw(int, "")
-    assert sim_panda.name == "sim_panda"
-    yield sim_panda
+        async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
+            await super().connect(mock=mock, timeout=timeout)
+
+    async with DeviceCollector(mock=True):
+        mock_panda = Panda("PANDA")
+        mock_panda.phase_1_signal_units = epics_signal_rw(int, "")
+    assert mock_panda.name == "mock_panda"
+    yield mock_panda
 
 
 @patch("ophyd_async.core.device_save_loader.save_to_yaml")
-async def test_save_panda(mock_save_to_yaml, sim_panda, RE: RunEngine):
-    RE(save_device(sim_panda, "path", sorter=phase_sorter))
+async def test_save_panda(mock_save_to_yaml, mock_panda, RE: RunEngine):
+    RE(save_device(mock_panda, "path", sorter=phase_sorter))
     mock_save_to_yaml.assert_called_once()
     assert mock_save_to_yaml.call_args[0] == (
         [
             {
                 "phase_1_signal_units": 0,
                 "seq.1.prescale_units": TimeUnits("min"),
                 "seq.2.prescale_units": TimeUnits("min"),
```

### Comparing `ophyd_async-0.3a3/tests/panda/test_table.py` & `ophyd_async-0.3a4/tests/panda/test_table.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/panda/test_trigger.py` & `ophyd_async-0.3a4/tests/panda/test_trigger.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 @pytest.fixture
 async def panda():
     class Panda(CommonPandaBlocks):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             super().__init__(name)
 
-        async def connect(self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT):
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
-            await super().connect(sim, timeout)
+        async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
+            await super().connect(mock=mock, timeout=timeout)
 
-    async with DeviceCollector(sim=True):
-        sim_panda = Panda("PANDAQSRV:", "sim_panda")
+    async with DeviceCollector(mock=True):
+        mock_panda = Panda("PANDAQSRV:", "mock_panda")
 
-    assert sim_panda.name == "sim_panda"
-    yield sim_panda
+    assert mock_panda.name == "mock_panda"
+    yield mock_panda
 
 
-def test_trigger_logic_has_given_methods(panda):
+async def test_trigger_logic_has_given_methods(panda):
     trigger_logic = StaticSeqTableTriggerLogic(panda.seq[1])
     assert hasattr(trigger_logic, "prepare")
     assert hasattr(trigger_logic, "kickoff")
     assert hasattr(trigger_logic, "complete")
     assert hasattr(trigger_logic, "stop")
```

### Comparing `ophyd_async-0.3a3/tests/sim/demo/test_sim_motor.py` & `ophyd_async-0.3a4/tests/sim/demo/test_sim_motor.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/sim/test_pattern_generator.py` & `ophyd_async-0.3a4/tests/sim/test_pattern_generator.py`

 * *Files identical despite different names*

### Comparing `ophyd_async-0.3a3/tests/sim/test_sim_detector.py` & `ophyd_async-0.3a4/tests/sim/test_sim_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ophyd_async.core.device import DeviceCollector
 from ophyd_async.epics.motion import motor
 from ophyd_async.sim.sim_pattern_generator import SimPatternDetector
 
 
 @pytest.fixture
 async def sim_motor():
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         sim_motor = motor.Motor("test")
     return sim_motor
 
 
 async def test_sim_pattern_detector_initialization(
     sim_pattern_detector: SimPatternDetector,
 ):
```

### Comparing `ophyd_async-0.3a3/tests/sim/test_sim_writer.py` & `ophyd_async-0.3a4/tests/sim/test_sim_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ophyd_async.core.device import DeviceCollector
 from ophyd_async.sim import PatternGenerator
 from ophyd_async.sim.sim_pattern_detector_writer import SimPatternDetectorWriter
 
 
 @pytest.fixture
 async def writer(tmp_path) -> SimPatternDetectorWriter:
-    async with DeviceCollector(sim=True):
+    async with DeviceCollector(mock=True):
         driver = PatternGenerator()
     directory = StaticDirectoryProvider(tmp_path)
 
     return SimPatternDetectorWriter(driver, directory)
 
 
 async def test_correct_descriptor_doc_after_open(writer: SimPatternDetectorWriter):
```

### Comparing `ophyd_async-0.3a3/tests/sim/test_streaming_plan.py` & `ophyd_async-0.3a4/tests/sim/test_streaming_plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         names.append(name)
         docs.append(doc)
 
     RE.subscribe(append_and_print)
 
     RE(bp.count([sim_pattern_detector], num=1))
 
-    print(names)
     # NOTE - double resource because double stream
     assert names == [
         "start",
         "descriptor",
         "stream_resource",
         "stream_resource",
         "stream_datum",
```

### Comparing `ophyd_async-0.3a3/tests/test_flyer_with_panda.py` & `ophyd_async-0.3a4/tests/test_flyer_with_panda.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 from event_model import ComposeStreamResourceBundle, compose_stream_resource
 
 from ophyd_async.core import (
     DEFAULT_TIMEOUT,
     DetectorControl,
     DetectorWriter,
     HardwareTriggeredFlyable,
-    SignalRW,
-    SimSignalBackend,
+    observe_value,
+    set_mock_value,
 )
 from ophyd_async.core.detector import StandardDetector
 from ophyd_async.core.device import DeviceCollector
-from ophyd_async.core.signal import observe_value, set_sim_value
 from ophyd_async.epics.pvi.pvi import fill_pvi_entries
+from ophyd_async.epics.signal.signal import epics_signal_rw
 from ophyd_async.panda import CommonPandaBlocks
 from ophyd_async.panda._trigger import StaticSeqTableTriggerLogic
 from ophyd_async.planstubs import (
     prepare_static_seq_table_flyer_and_detectors_with_same_trigger,
 )
 
 
 class DummyWriter(DetectorWriter):
     def __init__(self, name: str, shape: Sequence[int]):
-        self.dummy_signal = SignalRW(backend=SimSignalBackend(int))
+        self.dummy_signal = epics_signal_rw(int, "pva://read_pv")
         self._shape = shape
         self._name = name
         self._file: Optional[ComposeStreamResourceBundle] = None
         self._last_emitted = 0
         self.index = 0
 
     async def open(self, multiplier: int = 1) -> Dict[str, DataKey]:
@@ -86,16 +86,16 @@
     async def close(self) -> None:
         self._file = None
 
 
 @pytest.fixture
 async def detector_list(RE: RunEngine) -> tuple[StandardDetector, StandardDetector]:
     writers = [DummyWriter("testa", (1, 1)), DummyWriter("testb", (1, 1))]
-    await writers[0].dummy_signal.connect(sim=True)
-    await writers[1].dummy_signal.connect(sim=True)
+    await writers[0].dummy_signal.connect(mock=True)
+    await writers[1].dummy_signal.connect(mock=True)
 
     async def dummy_arm_1(self=None, trigger=None, num=0, exposure=None):
         return writers[0].dummy_signal.set(1)
 
     async def dummy_arm_2(self=None, trigger=None, num=0, exposure=None):
         return writers[1].dummy_signal.set(1)
 
@@ -117,23 +117,25 @@
 @pytest.fixture
 async def panda():
     class Panda(CommonPandaBlocks):
         def __init__(self, prefix: str, name: str = ""):
             self._prefix = prefix
             super().__init__(name)
 
-        async def connect(self, sim: bool = False, timeout: float = DEFAULT_TIMEOUT):
-            await fill_pvi_entries(self, self._prefix + "PVI", timeout=timeout, sim=sim)
-            await super().connect(sim, timeout)
+        async def connect(self, mock: bool = False, timeout: float = DEFAULT_TIMEOUT):
+            await fill_pvi_entries(
+                self, self._prefix + "PVI", timeout=timeout, mock=mock
+            )
+            await super().connect(mock, timeout)
 
-    async with DeviceCollector(sim=True):
-        sim_panda = Panda("PANDAQSRV:", "sim_panda")
+    async with DeviceCollector(mock=True):
+        mock_panda = Panda("PANDAQSRV:", "mock_panda")
 
-    assert sim_panda.name == "sim_panda"
-    yield sim_panda
+    assert mock_panda.name == "mock_panda"
+    yield mock_panda
 
 
 async def test_hardware_triggered_flyable_with_static_seq_table_logic(
     RE: RunEngine,
     detector_list: tuple[StandardDetector],
     panda,
 ):
@@ -176,29 +178,29 @@
 
         for detector in detector_list:
             detector.controller.disarm.assert_called_once  # type: ignore
 
         yield from bps.open_run()
         yield from bps.declare_stream(*detector_list, name="main_stream", collect=True)
 
-        set_sim_value(flyer.trigger_logic.seq.active, 1)
+        set_mock_value(flyer.trigger_logic.seq.active, 1)
 
         yield from bps.kickoff(flyer, wait=True)
         for detector in detector_list:
             yield from bps.kickoff(detector)
 
         yield from bps.complete(flyer, wait=False, group="complete")
         for detector in detector_list:
             yield from bps.complete(detector, wait=False, group="complete")
 
         # Manually incremenet the index as if a frame was taken
         for detector in detector_list:
             detector.writer.index += 1
 
-        set_sim_value(flyer.trigger_logic.seq.active, 0)
+        set_mock_value(flyer.trigger_logic.seq.active, 0)
 
         done = False
         while not done:
             try:
                 yield from bps.wait(group="complete", timeout=0.5)
             except TimeoutError:
                 pass
```

### Comparing `ophyd_async-0.3a3/tests/test_log.py` & `ophyd_async-0.3a4/tests/test_log.py`

 * *Files identical despite different names*

