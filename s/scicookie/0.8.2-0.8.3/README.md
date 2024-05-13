# Comparing `tmp/scicookie-0.8.2.tar.gz` & `tmp/scicookie-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scicookie-0.8.2.tar", max compression
+gzip compressed data, was "scicookie-0.8.3.tar", max compression
```

## Comparing `scicookie-0.8.2.tar` & `scicookie-0.8.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     1508 2024-05-11 23:13:27.875334 scicookie-0.8.2/LICENSE
--rw-r--r--   0        0        0     4875 2024-05-11 23:13:27.875334 scicookie-0.8.2/docs/description.md
--rw-r--r--   0        0        0     2147 2024-05-11 23:14:41.674267 scicookie-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       68 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/__init__.py
--rw-r--r--   0        0        0      116 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/__main__.py
--rw-r--r--   0        0        0     4394 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/cli.py
--rw-r--r--   0        0        0     1860 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/cookiecutter.json
--rw-r--r--   0        0        0    12535 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/hooks/post_gen_project.py
--rw-r--r--   0        0        0      359 2024-05-11 23:13:27.883334 scicookie-0.8.2/src/scicookie/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      971 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/logs.py
--rw-r--r--   0        0        0     1607 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/profile.py
--rw-r--r--   0        0        0     6460 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/profiles/base.yaml
--rw-r--r--   0        0        0     1380 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/profiles/osl.yaml
--rw-r--r--   0        0        0       41 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/tools/__init__.py
--rw-r--r--   0        0        0      965 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/tools/fix_eof.py
--rw-r--r--   0        0        0     4153 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/ui.py
--rw-r--r--   0        0        0      336 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
--rw-r--r--   0        0        0     5119 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1208 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2051 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
--rw-r--r--   0        0        0     2939 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1390 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2720 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
--rw-r--r--   0        0        0     3899 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2812 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0        0        0     4404 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml
--rw-r--r--   0        0        0     3354 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.prettierignore
--rw-r--r--   0        0        0      108 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.prettierrc.yaml
--rw-r--r--   0        0        0     2229 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
--rw-r--r--   0        0        0     6004 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0        0        0     3563 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0        0        0      432 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0        0        0     1809 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-config-pyproject.toml
--rw-r--r--   0        0        0     2633 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-pyproject.toml
--rw-r--r--   0        0        0     1917 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/pyproject.toml
--rw-r--r--   0        0        0      228 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/urls-pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit/pyproject.toml
--rw-r--r--   0        0        0      557 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch/pyproject.toml
--rw-r--r--   0        0        0      681 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/Cargo.toml
--rw-r--r--   0        0        0      615 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/lib.rs
--rw-r--r--   0        0        0      347 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/pyproject.toml
--rw-r--r--   0        0        0      402 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/main.cpp
--rw-r--r--   0        0        0      830 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/meson.build
--rw-r--r--   0        0        0      296 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/pyproject.toml
--rw-r--r--   0        0        0      561 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm/pyproject.toml
--rw-r--r--   0        0        0     3602 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry/pyproject.toml
--rw-r--r--   0        0        0      281 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      632 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/main.cpp
--rw-r--r--   0        0        0      450 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/pyproject.toml
--rw-r--r--   0        0        0      497 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/setup.py
--rw-r--r--   0        0        0      321 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/CMakeLists.txt
--rw-r--r--   0        0        0      195 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/main.cpp
--rw-r--r--   0        0        0      329 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/pyproject.toml
--rw-r--r--   0        0        0      401 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools/pyproject.toml
--rw-r--r--   0        0        0      497 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools/setup.py
--rw-r--r--   0        0        0     6436 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
--rw-r--r--   0        0        0     6436 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5488 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
--rw-r--r--   0        0        0     5488 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
--rw-r--r--   0        0        0    19228 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md
--rw-r--r--   0        0        0     5593 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md
--rw-r--r--   0        0        0     1998 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
--rw-r--r--   0        0        0      300 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
--rw-r--r--   0        0        0       54 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
--rw-r--r--   0        0        0      182 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
--rw-r--r--   0        0        0       20 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
--rw-r--r--   0        0        0    14485 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
--rw-r--r--   0        0        0     1116 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
--rw-r--r--   0        0        0    72342 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
--rw-r--r--   0        0        0    20402 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
--rw-r--r--   0        0        0     3383 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
--rw-r--r--   0        0        0     1123 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
--rw-r--r--   0        0        0      967 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
--rw-r--r--   0        0        0      141 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
--rw-r--r--   0        0        0     4518 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
--rw-r--r--   0        0        0      719 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml
--rw-r--r--   0        0        0       17 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/styles.css
--rwxr-xr-x   0        0        0     5275 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
--rw-r--r--   0        0        0      374 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
--rw-r--r--   0        0        0      829 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
--rw-r--r--   0        0        0       30 2024-05-11 23:13:27.887334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
--rw-r--r--   0        0        0    16405 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
--rw-r--r--   0        0        0     6840 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
--rw-r--r--   0        0        0     1554 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
--rw-r--r--   0        0        0       61 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py
--rw-r--r--   0        0        0     1009 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml
--rw-r--r--   0        0        0      892 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt
--rw-r--r--   0        0        0      848 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
--rw-r--r--   0        0        0      546 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
--rw-r--r--   0        0        0     2151 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py
--rw-r--r--   0        0        0        0 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/py.typed
--rw-r--r--   0        0        0       19 2024-05-11 23:13:27.891334 scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
--rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 scicookie-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1508 2024-05-13 16:12:36.881837 scicookie-0.8.3/LICENSE
+-rw-r--r--   0        0        0     4875 2024-05-13 16:12:36.885837 scicookie-0.8.3/docs/description.md
+-rw-r--r--   0        0        0     2147 2024-05-13 16:13:53.381470 scicookie-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0       68 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/__main__.py
+-rw-r--r--   0        0        0     4717 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/cli.py
+-rw-r--r--   0        0        0     1860 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/cookiecutter.json
+-rw-r--r--   0        0        0    12546 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      359 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      971 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/logs.py
+-rw-r--r--   0        0        0     1607 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/profile.py
+-rw-r--r--   0        0        0     6460 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/profiles/base.yaml
+-rw-r--r--   0        0        0     1380 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/profiles/osl.yaml
+-rw-r--r--   0        0        0       41 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/tools/__init__.py
+-rw-r--r--   0        0        0      965 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/tools/fix_eof.py
+-rw-r--r--   0        0        0     4153 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/ui.py
+-rw-r--r--   0        0        0      336 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.editorconfig
+-rw-r--r--   0        0        0     5119 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1208 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2051 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml
+-rw-r--r--   0        0        0     2939 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1390 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2720 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml
+-rw-r--r--   0        0        0     3899 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2812 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0        0        0     4404 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml
+-rw-r--r--   0        0        0     3354 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.prettierignore
+-rw-r--r--   0        0        0      108 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.prettierrc.yaml
+-rw-r--r--   0        0        0     2229 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json
+-rw-r--r--   0        0        0     6004 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0        0        0     3563 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0        0        0      432 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0        0        0     1809 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-config-pyproject.toml
+-rw-r--r--   0        0        0     2633 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-pyproject.toml
+-rw-r--r--   0        0        0     1917 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/urls-pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/flit/pyproject.toml
+-rw-r--r--   0        0        0      557 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch/pyproject.toml
+-rw-r--r--   0        0        0      681 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/Cargo.toml
+-rw-r--r--   0        0        0      615 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/lib.rs
+-rw-r--r--   0        0        0      347 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/pyproject.toml
+-rw-r--r--   0        0        0      402 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/main.cpp
+-rw-r--r--   0        0        0      830 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/meson.build
+-rw-r--r--   0        0        0      296 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/pyproject.toml
+-rw-r--r--   0        0        0      561 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm/pyproject.toml
+-rw-r--r--   0        0        0     3602 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry/pyproject.toml
+-rw-r--r--   0        0        0      281 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      632 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/main.cpp
+-rw-r--r--   0        0        0      450 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      497 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/setup.py
+-rw-r--r--   0        0        0      321 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/CMakeLists.txt
+-rw-r--r--   0        0        0      195 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/main.cpp
+-rw-r--r--   0        0        0      329 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/scikit-build-core/pyproject.toml
+-rw-r--r--   0        0        0      401 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools/pyproject.toml
+-rw-r--r--   0        0        0      497 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/setuptools/setup.py
+-rw-r--r--   0        0        0     6436 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md
+-rw-r--r--   0        0        0     6436 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5488 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md
+-rw-r--r--   0        0        0     5488 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md
+-rw-r--r--   0        0        0    19228 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md
+-rw-r--r--   0        0        0     5593 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md
+-rw-r--r--   0        0        0     1998 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile
+-rw-r--r--   0        0        0      300 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/containers/compose.yaml
+-rw-r--r--   0        0        0       54 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.md
+-rw-r--r--   0        0        0      182 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/api/references.rst
+-rw-r--r--   0        0        0       20 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/changelog.md
+-rw-r--r--   0        0        0    14485 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md
+-rw-r--r--   0        0        0     1116 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb
+-rw-r--r--   0        0        0    72342 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico
+-rw-r--r--   0        0        0    20402 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png
+-rw-r--r--   0        0        0     3383 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md
+-rw-r--r--   0        0        0     1123 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md
+-rw-r--r--   0        0        0      967 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml
+-rw-r--r--   0        0        0      141 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_toc.yml
+-rw-r--r--   0        0        0     4518 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml
+-rw-r--r--   0        0        0      719 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml
+-rw-r--r--   0        0        0       17 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/styles.css
+-rwxr-xr-x   0        0        0     5275 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      374 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/index.rst
+-rw-r--r--   0        0        0      829 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat
+-rw-r--r--   0        0        0       30 2024-05-13 16:12:36.897837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/readme.md
+-rw-r--r--   0        0        0    16405 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md
+-rw-r--r--   0        0        0     6840 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md
+-rw-r--r--   0        0        0     1554 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md
+-rw-r--r--   0        0        0       61 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py
+-rw-r--r--   0        0        0     1009 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml
+-rw-r--r--   0        0        0      892 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt
+-rw-r--r--   0        0        0      848 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py
+-rw-r--r--   0        0        0     2151 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/py.typed
+-rw-r--r--   0        0        0       19 2024-05-13 16:12:36.901837 scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/{{cookiecutter.package_slug}}.py
+-rw-r--r--   0        0        0     5658 1970-01-01 00:00:00.000000 scicookie-0.8.3/PKG-INFO
```

### Comparing `scicookie-0.8.2/LICENSE` & `scicookie-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/docs/description.md` & `scicookie-0.8.3/docs/description.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/pyproject.toml` & `scicookie-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scicookie"
-version = "0.8.2"  # semantic-release
+version = "0.8.3"  # semantic-release
 description = "Cookiecutter template for a Python package"
 readme = "docs/description.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD-3-Clause"
 include = [
     {path = "src/scicookie/cookiecutter.json"},
     {path = "src/scicookie/{{cookiecutter.project_slug}}"},
```

### Comparing `scicookie-0.8.2/src/scicookie/cli.py` & `scicookie-0.8.3/src/scicookie/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """Module with CLI functions."""
 
+from __future__ import annotations
+
 import argparse
 import json
+import os
+import platform
+import sys
 
 from pathlib import Path
 from typing import Union
 
 from cookiecutter.main import cookiecutter
 
 from scicookie.logs import SciCookieErrorType, SciCookieLogs
@@ -93,17 +98,22 @@
             answers_profile[question_id] = answer
             continue
 
         for choice in answer:
             choice_id = f"use_{choice.replace('-', '_')}"
             answers_profile[choice_id] = "yes"
 
-        cookiecutter(
-            str(PACKAGE_PATH), no_input=True, extra_context=answers_profile
-        )
+    env_path_sep = ";" if platform.system() == "Windows" else ":"
+    pipx_path: list[str] = list(filter(lambda v: ".local/pipx" in v, sys.path))
+    new_path: list[str] = [*pipx_path, os.getenv("PATH", "")]
+    os.environ["PATH"] = env_path_sep.join(new_path)
+
+    cookiecutter(
+        str(PACKAGE_PATH), no_input=True, extra_context=answers_profile
+    )
 
 
 def app():
     """Run SciCookie."""
     # note: this parameter should be provided by a CLI argument
 
     parser = argparse.ArgumentParser(
```

### Comparing `scicookie-0.8.2/src/scicookie/cookiecutter.json` & `scicookie-0.8.3/src/scicookie/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/hooks/post_gen_project.py` & `scicookie-0.8.3/src/scicookie/hooks/post_gen_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 import datetime
 import os
 import shutil
 import subprocess
+import sys
 
 from pathlib import Path
 
 from scicookie.tools import fix_eof
 
 PROJECT_DIRECTORY = Path(os.path.abspath(os.path.curdir)).resolve()
```

### Comparing `scicookie-0.8.2/src/scicookie/logs.py` & `scicookie-0.8.3/src/scicookie/logs.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/profile.py` & `scicookie-0.8.3/src/scicookie/profile.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/profiles/base.yaml` & `scicookie-0.8.3/src/scicookie/profiles/base.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/profiles/osl.yaml` & `scicookie-0.8.3/src/scicookie/profiles/osl.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/tools/fix_eof.py` & `scicookie-0.8.3/src/scicookie/tools/fix_eof.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/ui.py` & `scicookie-0.8.3/src/scicookie/ui.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/documentation-report.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.gitignore` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.makim.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/.releaserc.json`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/LICENSE` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/Makefile` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-config-pyproject.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-config-pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-pyproject.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/dev-deps-pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/pyproject.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/base/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch/pyproject.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/hatch/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/Cargo.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/lib.rs` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/maturin/lib.rs`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/meson.build` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/mesonpy/meson.build`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm/pyproject.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pdm/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry/pyproject.toml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/poetry/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/main.cpp` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/build-system/pybind11/main.cpp`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CITIZEN.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_CONVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/CONTRIBUTOR_COVENANT.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/NUMFOCUS_adapted_coc.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/coc/PYTHON_ADAPTED_COC.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/containers/Dockerfile`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/example.ipynb`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/index.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs/installation.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-jupyter-book/_config.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-mkdocs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-quarto/_quarto.yml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/docs-sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/governance/numpy_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/governance/sciml_governance.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/roadmap/ignite_roadmap.md`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/conda/dev.yaml`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/virtualenvs/pyenv/requirements.txt`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__init__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/__main__.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py` & `scicookie-0.8.3/src/scicookie/{{cookiecutter.project_slug}}/{{cookiecutter.package_slug}}/cli.py`

 * *Files identical despite different names*

### Comparing `scicookie-0.8.2/PKG-INFO` & `scicookie-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scicookie
-Version: 0.8.2
+Version: 0.8.3
 Summary: Cookiecutter template for a Python package
 License: BSD-3-Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

