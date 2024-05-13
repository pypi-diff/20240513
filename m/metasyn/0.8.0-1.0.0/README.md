# Comparing `tmp/metasyn-0.8.0.tar.gz` & `tmp/metasyn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasyn-0.8.0.tar", last modified: Mon Mar 25 15:07:07 2024, max compression
+gzip compressed data, was "metasyn-1.0.0.tar", last modified: Mon May 13 15:38:36 2024, max compression
```

## Comparing `metasyn-0.8.0.tar` & `metasyn-1.0.0.tar`

### file list

```diff
@@ -1,155 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.823397 metasyn-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.795397 metasyn-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.795397 metasyn-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-25 15:07:02.000000 metasyn-0.8.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-25 15:07:02.000000 metasyn-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-25 15:07:02.000000 metasyn-0.8.0/.github/workflows/release-dockerhub.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-25 15:07:02.000000 metasyn-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-25 15:07:02.000000 metasyn-0.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-25 15:07:02.000000 metasyn-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-25 15:07:02.000000 metasyn-0.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-25 15:07:02.000000 metasyn-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-25 15:07:07.823397 metasyn-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-03-25 15:07:02.000000 metasyn-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.795397 metasyn-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.799397 metasyn-0.8.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.799397 metasyn-0.8.0/docs/source/about/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/about/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/about/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13664 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/about/metasyn_in_detail.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.799397 metasyn-0.8.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/api/metasyn.demo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/api/metasyn.distribution.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/api/metasyn.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/api/metasyn.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.799397 metasyn-0.8.0/docs/source/developer/
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/developer/GMF.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/developer/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/developer/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16665 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/developer/distributions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/developer/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/developer/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.803397 metasyn-0.8.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)    65114 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/ClassDiagram.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    24188 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/distributions.drawio
--rw-r--r--   0 runner    (1001) docker     (127)    34827 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/distributions.svg
--rw-r--r--   0 runner    (1001) docker     (127)   171099 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/example_input_output.png
--rw-r--r--   0 runner    (1001) docker     (127)   145073 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/example_input_output_concise.png
--rw-r--r--   0 runner    (1001) docker     (127)    53165 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/flow_metadata_generation.png
--rw-r--r--   0 runner    (1001) docker     (127)    59443 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/flow_metadata_generation_code.png
--rw-r--r--   0 runner    (1001) docker     (127)    56147 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/flow_synthetic_data_generation.png
--rw-r--r--   0 runner    (1001) docker     (127)    60571 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/flow_synthetic_data_generation_code.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.807397 metasyn-0.8.0/docs/source/images/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/basic-grey.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/basic_grey-med.png
--rw-r--r--   0 runner    (1001) docker     (127)    30715 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/basic_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)    32624 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/blue.png
--rw-r--r--   0 runner    (1001) docker     (127)    87159 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/blue.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/blue_med.png
--rw-r--r--   0 runner    (1001) docker     (127)   117563 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/grey.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32277 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/grey_med.png
--rw-r--r--   0 runner    (1001) docker     (127)    32854 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/metasyn.afdesign
--rw-r--r--   0 runner    (1001) docker     (127)    85618 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/soda.png
--rw-r--r--   0 runner    (1001) docker     (127)    27577 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/white.png
--rw-r--r--   0 runner    (1001) docker     (127)    74743 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/white.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/logos/white_med.png
--rw-r--r--   0 runner    (1001) docker     (127)    96271 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_basic.png
--rw-r--r--   0 runner    (1001) docker     (127)   203582 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_basic_legacy.png
--rw-r--r--   0 runner    (1001) docker     (127)   155746 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_cli.png
--rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_cli_create_meta.png
--rw-r--r--   0 runner    (1001) docker     (127)    61202 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_estimation_code.png
--rw-r--r--   0 runner    (1001) docker     (127)   123167 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_estimation_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)   147699 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_func_names.png
--rw-r--r--   0 runner    (1001) docker     (127)    62213 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_generation_code.png
--rw-r--r--   0 runner    (1001) docker     (127)   123056 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_generation_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)    64310 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_serialization_code.png
--rw-r--r--   0 runner    (1001) docker     (127)   122965 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/images/pipeline_serialization_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.811397 metasyn-0.8.0/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/exporting_metaframes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/generating_metaframes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/generating_synthetic_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/interactive_tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-25 15:07:02.000000 metasyn-0.8.0/docs/source/usage/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.811397 metasyn-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/basic_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    81698 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/demonstration.csv
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/example_config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/example_gmf_simple.json
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/example_gmf_titanic.json
--rw-r--r--   0 runner    (1001) docker     (127)   101265 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-25 15:07:02.000000 metasyn-0.8.0/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.811397 metasyn-0.8.0/metasyn/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.815397 metasyn-0.8.0/metasyn/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/demo/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/demo/demo_fruit.csv
--rw-r--r--   0 runner    (1001) docker     (127)   805421 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/demo/demo_spaceship.csv
--rw-r--r--   0 runner    (1001) docker     (127)    88611 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/demo/demo_titanic.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.815397 metasyn-0.8.0/metasyn/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.815397 metasyn-0.8.0/metasyn/distribution/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/na.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/distribution/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/metaframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)    20005 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.815397 metasyn-0.8.0/metasyn/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/schema/generative_metadata_format.json
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-03-25 15:07:02.000000 metasyn-0.8.0/metasyn/var.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.819397 metasyn-0.8.0/metasyn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 15:07:07.000000 metasyn-0.8.0/metasyn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-25 15:07:02.000000 metasyn-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 15:07:07.823397 metasyn-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.819397 metasyn-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:07:07.819397 metasyn-0.8.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/data/example_config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/data/no_data_config.toml
--rw-r--r--   0 runner    (1001) docker     (127)    60302 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/data/titanic.csv
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_faker.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_na.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_privacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-03-25 15:07:02.000000 metasyn-0.8.0/tests/test_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.428193 metasyn-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.400193 metasyn-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-13 15:38:31.000000 metasyn-1.0.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-13 15:38:31.000000 metasyn-1.0.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.404193 metasyn-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 15:38:31.000000 metasyn-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-13 15:38:31.000000 metasyn-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 15:38:31.000000 metasyn-1.0.0/.github/workflows/release-dockerhub.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-13 15:38:31.000000 metasyn-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 15:38:31.000000 metasyn-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 15:38:31.000000 metasyn-1.0.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 15:38:31.000000 metasyn-1.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 15:38:31.000000 metasyn-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-13 15:38:36.428193 metasyn-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-13 15:38:31.000000 metasyn-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.404193 metasyn-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.404193 metasyn-1.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.404193 metasyn-1.0.0/docs/source/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/about/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/about/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.404193 metasyn-1.0.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/api/developer_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/api/metaframe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/api/metasyn.demo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/api/metasyn.distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/api/metasyn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/api/varspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.404193 metasyn-1.0.0/docs/source/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/developer/GMF.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/developer/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/developer/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/developer/distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/developer/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/developer/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.412193 metasyn-1.0.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    65114 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/ClassDiagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    24188 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/distributions.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    34827 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/distributions.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   171099 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/example_input_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)   145073 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/example_input_output_concise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53165 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/flow_metadata_generation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59443 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/flow_metadata_generation_code.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56147 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/flow_synthetic_data_generation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60571 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/flow_synthetic_data_generation_code.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.416193 metasyn-1.0.0/docs/source/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    16397 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/basic-grey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/basic_grey-med.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30715 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/basic_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32624 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)    87159 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/blue.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/blue_med.png
+-rw-r--r--   0 runner    (1001) docker     (127)   117563 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/grey.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32277 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/grey_med.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32854 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/metasyn.afdesign
+-rw-r--r--   0 runner    (1001) docker     (127)    85618 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/soda.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27577 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74743 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11607 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/logos/white_med.png
+-rw-r--r--   0 runner    (1001) docker     (127)    96271 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_basic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   203582 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_basic_legacy.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155746 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_cli.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171516 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_cli_create_meta.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61202 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_estimation_code.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123167 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_estimation_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)   147699 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_func_names.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62213 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_generation_code.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123056 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_generation_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64310 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_serialization_code.png
+-rw-r--r--   0 runner    (1001) docker     (127)   122965 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/images/pipeline_serialization_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/metasyn_in_detail.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.416193 metasyn-1.0.0/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/config_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/exporting_metaframes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/generating_metaframes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/generating_synthetic_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/interactive_tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 15:38:31.000000 metasyn-1.0.0/docs/source/usage/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.416193 metasyn-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/basic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81698 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/demonstration.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/example_config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/example_gmf_simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/example_gmf_titanic.json
+-rw-r--r--   0 runner    (1001) docker     (127)   101265 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-13 15:38:31.000000 metasyn-1.0.0/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.420193 metasyn-1.0.0/metasyn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.424193 metasyn-1.0.0/metasyn/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/demo/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/demo/demo_fruit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   805421 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/demo/demo_spaceship.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    88611 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/demo/demo_titanic.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.424193 metasyn-1.0.0/metasyn/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12101 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11269 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/discrete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.424193 metasyn-1.0.0/metasyn/distribution/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/na.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/distribution/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/metaframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.424193 metasyn-1.0.0/metasyn/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/schema/generative_metadata_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/schema/plugin_registry.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-13 15:38:31.000000 metasyn-1.0.0/metasyn/varspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.428193 metasyn-1.0.0/metasyn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 15:38:36.000000 metasyn-1.0.0/metasyn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-13 15:38:31.000000 metasyn-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:38:36.428193 metasyn-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.428193 metasyn-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:36.428193 metasyn-1.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/data/example_config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/data/no_data_config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    60302 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/data/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_na.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-13 15:38:31.000000 metasyn-1.0.0/tests/test_var.py
```

### Comparing `metasyn-0.8.0/.github/workflows/python-package.yml` & `metasyn-1.0.0/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       run: |
         pydocstyle metasyn --convention=numpy --add-select=D417 --add-ignore="D102,D105"
     - name: Check types with MyPy
       run: |
         mypy metasyn
     - name: Check if documentation builds.
       run: |
-        cd docs; make html SPHINXOPTS="-W --keep-going"
+        cd docs; make html SPHINXOPTS="--keep-going"
     - name: Test with pytest
       run: |
         pytest tests
     - name: Check notebook output
       if: ${{ matrix.os != 'macos-latest' }}
       run: |
         pytest --nbval-lax examples
```

### Comparing `metasyn-0.8.0/.github/workflows/python-publish.yml` & `metasyn-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/.github/workflows/release-dockerhub.yml` & `metasyn-1.0.0/.github/workflows/release-dockerhub.yml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/.gitignore` & `metasyn-1.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -141,7 +141,8 @@
 
 #DS_Store
 .DS_Store
 .DS_Store
 docs/source/images/pipeline.afphoto~lock~
 docs/source/images/.$ClassDiagram.drawio.bkp
 docs/source/images/.$distributions.drawio.bkp
+docs/source/api/generated
```

### Comparing `metasyn-0.8.0/.readthedocs.yaml` & `metasyn-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/CITATION.cff` & `metasyn-1.0.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/LICENSE` & `metasyn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/PKG-INFO` & `metasyn-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasyn
-Version: 0.8.0
+Version: 1.0.0
 Summary: Package for creating synthetic datasets while preserving privacy.
 Author-email: Raoul Schram <r.d.schram@uu.nl>, Erik-Jan van Kesteren <e.vankesteren1@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 SoDa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,19 +70,19 @@
 Requires-Dist: sphinx_copybutton; extra == "test"
 Requires-Dist: XlsxWriter; extra == "test"
 Requires-Dist: types-tqdm; extra == "test"
 Requires-Dist: types-regex; extra == "test"
 Requires-Dist: pandas; extra == "test"
 
 <p align="center">
-  <img src="docs/source/images/logos/blue.svg" width="600px" alt="Metasyn logo"></img>
+  <img src="https://github.com/sodascience/metasyn/blob/main/docs/source/images/logos/blue.svg" width="600px" alt="Metasyn logo"></img>
   <h3 align="center">Transparent and privacy-friendly synthetic data generation</h3>
   <p align="center">
     <span>
-        <a href="https://www.repostatus.org/#wip"><img src="https://www.repostatus.org/badges/latest/wip.svg" alt="Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public."/></a>
+        <a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>
         <a href="https://pypi.org/project/metasyn"><img src="https://img.shields.io/pypi/pyversions/metasyn" alt="metasyn on pypi"></img></a>
         <a href="https://colab.research.google.com/github/sodascience/metasyn/blob/main/examples/getting_started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="open getting started on colab"></img></a>
         <a href="https://metasyn.readthedocs.io/en/latest/index.html"><img src="https://readthedocs.org/projects/metasyn/badge/?version=latest" alt="Readthedocs"></img></a>
         <a href="https://hub.docker.com/r/sodateam/metasyn"><img src="https://img.shields.io/docker/v/sodateam/metasyn?logo=docker&label=docker&color=blue" alt="Docker image version"></img></a>
         <a href="https://zenodo.org/doi/10.5281/zenodo.7696031"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7696031.svg" alt="DOI"></a>
     </span>
   </p>
@@ -113,15 +113,15 @@
 ```sh
 pip install git+https://github.com/sodascience/metasyn
 ```
 
 ## Usage
 To generate synthetic data, `metasyn` first needs to fit a `MetaFrame` to the data which can then be used to produce new synthetic rows:
 
-![Example input and output](docs/source/images/example_input_output_concise.png)
+![Example input and output](https://github.com/sodascience/metasyn/blob/main/docs/source/images/example_input_output_concise.png)
 
 In Python code this happens as follows:
 
 ```python
 import polars as pl
 from metasyn import MetaFrame, demo_file
 
@@ -155,27 +155,15 @@
 ## Where to go next
 
 - As a next step to learn more about generating synthetic data with metasyn we recommend to check out the [user guide](https://metasyn.readthedocs.io/en/latest/usage/usage.html).
 - For even more privacy, have a look at our [disclosure control plugin](https://github.com/sodascience/metasyn-disclosure-control).
 - To learn more about how `metasyn` works, go to detailed overview in our [documentation](https://metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). 
 - Want to create programs that build on metasyn? Take a look at our versioned [Docker containers](https://hub.docker.com/r/sodateam/metasyn) and our [CLI](https://metasyn.readthedocs.io/en/latest/usage/cli.html).
 
-
-
 ## Contributing
-Metasyn is an open-source project, and we welcome contributions from the community.
-
-To contribute to the codebase, follow these steps:
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-More information on contributing can be found in the [contributing](https://metasyn.readthedocs.io/en/latest/developer/contributing.html) section of the documentation.
-
+Metasyn is an open-source project, and we welcome contributions from the community, from bug reports & feature requests to code contributions. Read our [contributing guidelines](.github/CONTRIBUTING.md) for more information and to get started!
 
 ## Contact
 **Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)](https://odissei-data.nl/nl/soda/) team.
-Do you have questions, suggestions, or remarks on the technical implementation? File an issue in the issue tracker or feel free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://github.com/qubixes).
+Do you have questions, suggestions, or remarks on the technical implementation? Create an issue in the [issue tracker](https://github.com/sodascience/metasyn/issues) or feel free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://github.com/qubixes).
 
 <img src="docs/source/images/logos/soda.png" alt="SoDa logo" width="250px"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metasyn Version: 0.8.0 Summary: Package for
+Metadata-Version: 2.1 Name: metasyn Version: 1.0.0 Summary: Package for
 creating synthetic datasets while preserving privacy. Author-email: Raoul
 Schram
 uu.nl>, Erik-Jan van Kesteren
 uu.nl> License: MIT License Copyright (c) 2024 SoDa Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -40,17 +40,17 @@
 sphinxcontrib-napoleon; extra == "test" Requires-Dist: sphinx-autodoc-
 typehints; extra == "test" Requires-Dist: sphinx_inline_tabs; extra == "test"
 Requires-Dist: sphinx_copybutton; extra == "test" Requires-Dist: XlsxWriter;
 extra == "test" Requires-Dist: types-tqdm; extra == "test" Requires-Dist:
 types-regex; extra == "test" Requires-Dist: pandas; extra == "test"
                                 [Metasyn logo]
      ******** TTrraannssppaarreenntt aanndd pprriivvaaccyy--ffrriieennddllyy ssyynntthheettiicc ddaattaa ggeenneerraattiioonn ********
-_[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _W_I_P_ _â___ _I_n_i_t_i_a_l_ _d_e_v_e_l_o_p_m_e_n_t_ _i_s_ _i_n_ _p_r_o_g_r_e_s_s_,_ _b_u_t_ _t_h_e_r_e_ _h_a_s_ _n_o_t
- _y_e_t_ _b_e_e_n_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _r_e_l_e_a_s_e_ _s_u_i_t_a_b_l_e_ _f_o_r_ _t_h_e_ _p_u_b_l_i_c_._]_[_m_e_t_a_s_y_n_ _o_n_ _p_y_p_i_]
-    _[_o_p_e_n_ _g_e_t_t_i_n_g_ _s_t_a_r_t_e_d_ _o_n_ _c_o_l_a_b_]_[_R_e_a_d_t_h_e_d_o_c_s_]_[_D_o_c_k_e_r_ _i_m_a_g_e_ _v_e_r_s_i_o_n_]_[_D_O_I_]
+_[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
+ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_m_e_t_a_s_y_n_ _o_n_ _p_y_p_i_]_[_o_p_e_n_ _g_e_t_t_i_n_g_ _s_t_a_r_t_e_d_ _o_n_ _c_o_l_a_b_]
+                   _[_R_e_a_d_t_h_e_d_o_c_s_]_[_D_o_c_k_e_r_ _i_m_a_g_e_ _v_e_r_s_i_o_n_]_[_D_O_I_]
 
 __Generate synthetic tabular data__ in a transparent, understandable, and
 privacy-friendly way. Metasyn makes it possible for owners of sensitive data to
 create test data, do open science, improve code reproducibility, encourage data
 reuse, and enhance accessibility of their datasets, without worrying about
 leaking private information. With metasyn you can __fit__ a model to an
 existing dataframe, __export__ it to a transparent and auditable `.json` file,
@@ -83,44 +83,42 @@
 metasyn.readthedocs.io/en/latest/developer/contributing.html) directly to the
 project. ## Installation Metasyn can be installed directly from PyPI using the
 following command in the terminal: ```sh pip install metasyn ``` The latest
 (possibly unstable) development version can be installed directly from GitHub
 like so: ```sh pip install git+https://github.com/sodascience/metasyn ``` ##
 Usage To generate synthetic data, `metasyn` first needs to fit a `MetaFrame` to
 the data which can then be used to produce new synthetic rows: ![Example input
-and output](docs/source/images/example_input_output_concise.png) In Python code
-this happens as follows: ```python import polars as pl from metasyn import
-MetaFrame, demo_file # Get the csv file path for built-in demo dataset csv_path
-= demo_file("fruit") # Create a polars dataframe from the csv file. # It is
-important to ensure the data types are correct # when creating your dataframe,
-especially categorical data! df = pl.read_csv(csv_path, dtypes={ "fruits":
-pl.Categorical, "cars": pl.Categorical }) # Create a MetaFrame from the
-DataFrame. mf = MetaFrame.fit_dataframe(df) # Generate a new DataFrame with 5
-rows from the MetaFrame. df_synth = mf.synthesize(5) # This DataFrame can be
-exported to csv, parquet, excel and more. df_synth.write_csv("output.csv") ```
-To explore more options and try this out online, take a look at our interactive
-tutorial: [![](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/sodascience/metasyn/blob/main/
-examples/getting_started.ipynb) For more information on how to create
-dataframes with polars, refer to the [Polars documentation](https://pola.rs/).
-Metasyn also works with pandas dataframes! ## Where to go next - As a next step
-to learn more about generating synthetic data with metasyn we recommend to
-check out the [user guide](https://metasyn.readthedocs.io/en/latest/usage/
-usage.html). - For even more privacy, have a look at our [disclosure control
-plugin](https://github.com/sodascience/metasyn-disclosure-control). - To learn
-more about how `metasyn` works, go to detailed overview in our [documentation]
-(https://metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). - Want
-to create programs that build on metasyn? Take a look at our versioned [Docker
+and output](https://github.com/sodascience/metasyn/blob/main/docs/source/
+images/example_input_output_concise.png) In Python code this happens as
+follows: ```python import polars as pl from metasyn import MetaFrame, demo_file
+# Get the csv file path for built-in demo dataset csv_path = demo_file("fruit")
+# Create a polars dataframe from the csv file. # It is important to ensure the
+data types are correct # when creating your dataframe, especially categorical
+data! df = pl.read_csv(csv_path, dtypes={ "fruits": pl.Categorical, "cars":
+pl.Categorical }) # Create a MetaFrame from the DataFrame. mf =
+MetaFrame.fit_dataframe(df) # Generate a new DataFrame with 5 rows from the
+MetaFrame. df_synth = mf.synthesize(5) # This DataFrame can be exported to csv,
+parquet, excel and more. df_synth.write_csv("output.csv") ``` To explore more
+options and try this out online, take a look at our interactive tutorial: [![]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/sodascience/metasyn/blob/main/examples/
+getting_started.ipynb) For more information on how to create dataframes with
+polars, refer to the [Polars documentation](https://pola.rs/). Metasyn also
+works with pandas dataframes! ## Where to go next - As a next step to learn
+more about generating synthetic data with metasyn we recommend to check out the
+[user guide](https://metasyn.readthedocs.io/en/latest/usage/usage.html). - For
+even more privacy, have a look at our [disclosure control plugin](https://
+github.com/sodascience/metasyn-disclosure-control). - To learn more about how
+`metasyn` works, go to detailed overview in our [documentation](https://
+metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). - Want to
+create programs that build on metasyn? Take a look at our versioned [Docker
 containers](https://hub.docker.com/r/sodateam/metasyn) and our [CLI](https://
 metasyn.readthedocs.io/en/latest/usage/cli.html). ## Contributing Metasyn is an
-open-source project, and we welcome contributions from the community. To
-contribute to the codebase, follow these steps: 1. Fork the Project 2. Create
-your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
-changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
-push origin feature/AmazingFeature`) 5. Open a Pull Request More information on
-contributing can be found in the [contributing](https://metasyn.readthedocs.io/
-en/latest/developer/contributing.html) section of the documentation. ## Contact
-**Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)](https://
-odissei-data.nl/nl/soda/) team. Do you have questions, suggestions, or remarks
-on the technical implementation? File an issue in the issue tracker or feel
-free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or
-[Raoul Schram](https://github.com/qubixes).[SoDa logo]
+open-source project, and we welcome contributions from the community, from bug
+reports & feature requests to code contributions. Read our [contributing
+guidelines](.github/CONTRIBUTING.md) for more information and to get started!
+## Contact **Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)]
+(https://odissei-data.nl/nl/soda/) team. Do you have questions, suggestions, or
+remarks on the technical implementation? Create an issue in the [issue tracker]
+(https://github.com/sodascience/metasyn/issues) or feel free to contact [Erik-
+Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://
+github.com/qubixes).[SoDa logo]
```

### Comparing `metasyn-0.8.0/README.md` & `metasyn-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
-  <img src="docs/source/images/logos/blue.svg" width="600px" alt="Metasyn logo"></img>
+  <img src="https://github.com/sodascience/metasyn/blob/main/docs/source/images/logos/blue.svg" width="600px" alt="Metasyn logo"></img>
   <h3 align="center">Transparent and privacy-friendly synthetic data generation</h3>
   <p align="center">
     <span>
-        <a href="https://www.repostatus.org/#wip"><img src="https://www.repostatus.org/badges/latest/wip.svg" alt="Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public."/></a>
+        <a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>
         <a href="https://pypi.org/project/metasyn"><img src="https://img.shields.io/pypi/pyversions/metasyn" alt="metasyn on pypi"></img></a>
         <a href="https://colab.research.google.com/github/sodascience/metasyn/blob/main/examples/getting_started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="open getting started on colab"></img></a>
         <a href="https://metasyn.readthedocs.io/en/latest/index.html"><img src="https://readthedocs.org/projects/metasyn/badge/?version=latest" alt="Readthedocs"></img></a>
         <a href="https://hub.docker.com/r/sodateam/metasyn"><img src="https://img.shields.io/docker/v/sodateam/metasyn?logo=docker&label=docker&color=blue" alt="Docker image version"></img></a>
         <a href="https://zenodo.org/doi/10.5281/zenodo.7696031"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7696031.svg" alt="DOI"></a>
     </span>
   </p>
@@ -38,15 +38,15 @@
 ```sh
 pip install git+https://github.com/sodascience/metasyn
 ```
 
 ## Usage
 To generate synthetic data, `metasyn` first needs to fit a `MetaFrame` to the data which can then be used to produce new synthetic rows:
 
-![Example input and output](docs/source/images/example_input_output_concise.png)
+![Example input and output](https://github.com/sodascience/metasyn/blob/main/docs/source/images/example_input_output_concise.png)
 
 In Python code this happens as follows:
 
 ```python
 import polars as pl
 from metasyn import MetaFrame, demo_file
 
@@ -80,27 +80,15 @@
 ## Where to go next
 
 - As a next step to learn more about generating synthetic data with metasyn we recommend to check out the [user guide](https://metasyn.readthedocs.io/en/latest/usage/usage.html).
 - For even more privacy, have a look at our [disclosure control plugin](https://github.com/sodascience/metasyn-disclosure-control).
 - To learn more about how `metasyn` works, go to detailed overview in our [documentation](https://metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). 
 - Want to create programs that build on metasyn? Take a look at our versioned [Docker containers](https://hub.docker.com/r/sodateam/metasyn) and our [CLI](https://metasyn.readthedocs.io/en/latest/usage/cli.html).
 
-
-
 ## Contributing
-Metasyn is an open-source project, and we welcome contributions from the community.
-
-To contribute to the codebase, follow these steps:
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-More information on contributing can be found in the [contributing](https://metasyn.readthedocs.io/en/latest/developer/contributing.html) section of the documentation.
-
+Metasyn is an open-source project, and we welcome contributions from the community, from bug reports & feature requests to code contributions. Read our [contributing guidelines](.github/CONTRIBUTING.md) for more information and to get started!
 
 ## Contact
 **Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)](https://odissei-data.nl/nl/soda/) team.
-Do you have questions, suggestions, or remarks on the technical implementation? File an issue in the issue tracker or feel free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://github.com/qubixes).
+Do you have questions, suggestions, or remarks on the technical implementation? Create an issue in the [issue tracker](https://github.com/sodascience/metasyn/issues) or feel free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://github.com/qubixes).
 
 <img src="docs/source/images/logos/soda.png" alt="SoDa logo" width="250px"/>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                                 [Metasyn logo]
      ******** TTrraannssppaarreenntt aanndd pprriivvaaccyy--ffrriieennddllyy ssyynntthheettiicc ddaattaa ggeenneerraattiioonn ********
-_[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _W_I_P_ _â___ _I_n_i_t_i_a_l_ _d_e_v_e_l_o_p_m_e_n_t_ _i_s_ _i_n_ _p_r_o_g_r_e_s_s_,_ _b_u_t_ _t_h_e_r_e_ _h_a_s_ _n_o_t
- _y_e_t_ _b_e_e_n_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _r_e_l_e_a_s_e_ _s_u_i_t_a_b_l_e_ _f_o_r_ _t_h_e_ _p_u_b_l_i_c_._]_[_m_e_t_a_s_y_n_ _o_n_ _p_y_p_i_]
-    _[_o_p_e_n_ _g_e_t_t_i_n_g_ _s_t_a_r_t_e_d_ _o_n_ _c_o_l_a_b_]_[_R_e_a_d_t_h_e_d_o_c_s_]_[_D_o_c_k_e_r_ _i_m_a_g_e_ _v_e_r_s_i_o_n_]_[_D_O_I_]
+_[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
+ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_m_e_t_a_s_y_n_ _o_n_ _p_y_p_i_]_[_o_p_e_n_ _g_e_t_t_i_n_g_ _s_t_a_r_t_e_d_ _o_n_ _c_o_l_a_b_]
+                   _[_R_e_a_d_t_h_e_d_o_c_s_]_[_D_o_c_k_e_r_ _i_m_a_g_e_ _v_e_r_s_i_o_n_]_[_D_O_I_]
 
 __Generate synthetic tabular data__ in a transparent, understandable, and
 privacy-friendly way. Metasyn makes it possible for owners of sensitive data to
 create test data, do open science, improve code reproducibility, encourage data
 reuse, and enhance accessibility of their datasets, without worrying about
 leaking private information. With metasyn you can __fit__ a model to an
 existing dataframe, __export__ it to a transparent and auditable `.json` file,
@@ -39,44 +39,42 @@
 metasyn.readthedocs.io/en/latest/developer/contributing.html) directly to the
 project. ## Installation Metasyn can be installed directly from PyPI using the
 following command in the terminal: ```sh pip install metasyn ``` The latest
 (possibly unstable) development version can be installed directly from GitHub
 like so: ```sh pip install git+https://github.com/sodascience/metasyn ``` ##
 Usage To generate synthetic data, `metasyn` first needs to fit a `MetaFrame` to
 the data which can then be used to produce new synthetic rows: ![Example input
-and output](docs/source/images/example_input_output_concise.png) In Python code
-this happens as follows: ```python import polars as pl from metasyn import
-MetaFrame, demo_file # Get the csv file path for built-in demo dataset csv_path
-= demo_file("fruit") # Create a polars dataframe from the csv file. # It is
-important to ensure the data types are correct # when creating your dataframe,
-especially categorical data! df = pl.read_csv(csv_path, dtypes={ "fruits":
-pl.Categorical, "cars": pl.Categorical }) # Create a MetaFrame from the
-DataFrame. mf = MetaFrame.fit_dataframe(df) # Generate a new DataFrame with 5
-rows from the MetaFrame. df_synth = mf.synthesize(5) # This DataFrame can be
-exported to csv, parquet, excel and more. df_synth.write_csv("output.csv") ```
-To explore more options and try this out online, take a look at our interactive
-tutorial: [![](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/sodascience/metasyn/blob/main/
-examples/getting_started.ipynb) For more information on how to create
-dataframes with polars, refer to the [Polars documentation](https://pola.rs/).
-Metasyn also works with pandas dataframes! ## Where to go next - As a next step
-to learn more about generating synthetic data with metasyn we recommend to
-check out the [user guide](https://metasyn.readthedocs.io/en/latest/usage/
-usage.html). - For even more privacy, have a look at our [disclosure control
-plugin](https://github.com/sodascience/metasyn-disclosure-control). - To learn
-more about how `metasyn` works, go to detailed overview in our [documentation]
-(https://metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). - Want
-to create programs that build on metasyn? Take a look at our versioned [Docker
+and output](https://github.com/sodascience/metasyn/blob/main/docs/source/
+images/example_input_output_concise.png) In Python code this happens as
+follows: ```python import polars as pl from metasyn import MetaFrame, demo_file
+# Get the csv file path for built-in demo dataset csv_path = demo_file("fruit")
+# Create a polars dataframe from the csv file. # It is important to ensure the
+data types are correct # when creating your dataframe, especially categorical
+data! df = pl.read_csv(csv_path, dtypes={ "fruits": pl.Categorical, "cars":
+pl.Categorical }) # Create a MetaFrame from the DataFrame. mf =
+MetaFrame.fit_dataframe(df) # Generate a new DataFrame with 5 rows from the
+MetaFrame. df_synth = mf.synthesize(5) # This DataFrame can be exported to csv,
+parquet, excel and more. df_synth.write_csv("output.csv") ``` To explore more
+options and try this out online, take a look at our interactive tutorial: [![]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/sodascience/metasyn/blob/main/examples/
+getting_started.ipynb) For more information on how to create dataframes with
+polars, refer to the [Polars documentation](https://pola.rs/). Metasyn also
+works with pandas dataframes! ## Where to go next - As a next step to learn
+more about generating synthetic data with metasyn we recommend to check out the
+[user guide](https://metasyn.readthedocs.io/en/latest/usage/usage.html). - For
+even more privacy, have a look at our [disclosure control plugin](https://
+github.com/sodascience/metasyn-disclosure-control). - To learn more about how
+`metasyn` works, go to detailed overview in our [documentation](https://
+metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). - Want to
+create programs that build on metasyn? Take a look at our versioned [Docker
 containers](https://hub.docker.com/r/sodateam/metasyn) and our [CLI](https://
 metasyn.readthedocs.io/en/latest/usage/cli.html). ## Contributing Metasyn is an
-open-source project, and we welcome contributions from the community. To
-contribute to the codebase, follow these steps: 1. Fork the Project 2. Create
-your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
-changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
-push origin feature/AmazingFeature`) 5. Open a Pull Request More information on
-contributing can be found in the [contributing](https://metasyn.readthedocs.io/
-en/latest/developer/contributing.html) section of the documentation. ## Contact
-**Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)](https://
-odissei-data.nl/nl/soda/) team. Do you have questions, suggestions, or remarks
-on the technical implementation? File an issue in the issue tracker or feel
-free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or
-[Raoul Schram](https://github.com/qubixes).[SoDa logo]
+open-source project, and we welcome contributions from the community, from bug
+reports & feature requests to code contributions. Read our [contributing
+guidelines](.github/CONTRIBUTING.md) for more information and to get started!
+## Contact **Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)]
+(https://odissei-data.nl/nl/soda/) team. Do you have questions, suggestions, or
+remarks on the technical implementation? Create an issue in the [issue tracker]
+(https://github.com/sodascience/metasyn/issues) or feel free to contact [Erik-
+Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://
+github.com/qubixes).[SoDa logo]
```

### Comparing `metasyn-0.8.0/docs/Makefile` & `metasyn-1.0.0/docs/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -8,13 +8,17 @@
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
-.PHONY: help Makefile
+.PHONY: help Makefile clean
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+
+clean:
+	rm -r $(BUILDDIR) $(SOURCEDIR)/api/generated
```

### Comparing `metasyn-0.8.0/docs/make.bat` & `metasyn-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/about/contact.rst` & `metasyn-1.0.0/docs/source/about/contact.rst`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/about/license.rst` & `metasyn-1.0.0/docs/source/about/license.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Metasyn is released under the MIT License.
 
 .. code-block:: text
 
    MIT License
 
-   Copyright (c) 2023 SoDa
+   Copyright (c) 2024 SoDa
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
```

### Comparing `metasyn-0.8.0/docs/source/about/metasyn_in_detail.rst` & `metasyn-1.0.0/docs/source/metasyn_in_detail.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Detailed overview of metasyn
-==============================
+How does metasyn work?
+======================
 
 ``Metasyn`` is a python package for generating synthetic data with a focus on maintaining privacy. It is aimed at owners of sensitive datasets such as public organisations, research groups, and individual researchers who want to improve the accessibility, reproducibility and reusability of their data. The goal of ``metasyn`` is to make it easy for data owners to share the structure and approximation of the content of their data with others with fewer privacy concerns.
 
 With this goal in mind, ``metasyn`` restricts itself to the `'synthetically-augmented plausible' <https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/onsmethodologyworkingpaperseriesnumber16syntheticdatapilot>`__ category of synthetic data, as categorized by the Office for National Statistics (ONS).
 
 .. admonition:: ONS criteria for a Synthetically-augmented plausible dataset:
    
@@ -154,15 +154,15 @@
 After a ``MetaFrame`` object is created, ``metasyn`` allows it to be stored in a human- and machine-readable ``.json`` file. This file contains all the (statistical) metadata as input for the generation step.
 Exported :obj:`MetaFrames <metasyn.metaframe.MetaFrame>` follow the  :doc:`/developer/GMF`, a standard designed to be easy to read and understand. 
 This allows for manual and automatic editing, as well as sharing.
 
 .. raw:: html
 
    <details> 
-   <summary> An example of an exported MetaFrame: </summary>
+   <summary> An example of an exported MetaFrame [click to expand]: </summary>
 
 .. code-block:: json
 
     {
         "n_rows": 5,
         "n_columns": 5,
         "provenance": {
```

### Comparing `metasyn-0.8.0/docs/source/api/metasyn.rst` & `metasyn-1.0.0/docs/source/api/developer_reference.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-API Reference
-=============
+Developer Reference
+===================
 
-.. automodule:: metasyn
+This section is intended for those that want to contribute to the metasyn package, or simply want a deeper understanding of how it works. It contains the classes, functions and modules that are not in the rest of the reference API. These are mostly elements that are not directly used by users, but are important for developers of the metasyn package to understand the architecture.
+
+DistSpec
+^^^^^^^^
+
+.. autoclass:: metasyn.varspec.DistributionSpec
    :members:
    :undoc-members:
    :show-inheritance:
 
-Subpackages
------------
-
-.. toctree::
-   :maxdepth: 1
-
-   metasyn.distribution
-   metasyn.schema
-   metasyn.demo
-
-Submodules
-----------
+metasyn.config module
+^^^^^^^^^^^^^^^^^^^^^
 
-metasyn.metaframe module
-^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. automodule:: metasyn.metaframe
+.. automodule:: metasyn.config
    :members:
    :undoc-members:
    :show-inheritance:
 
+
 metasyn.provider module
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. automodule:: metasyn.provider
    :members:
    :undoc-members:
    :show-inheritance:
@@ -62,7 +55,24 @@
 metasyn.privacy module
 ^^^^^^^^^^^^^^^^^^^^^^
 
 .. automodule:: metasyn.privacy
    :members:
    :undoc-members:
    :show-inheritance:
+
+metasyn.util module
+^^^^^^^^^^^^^^^^^^^
+
+.. automodule:: metasyn.util
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+
+metasyn.distribution.base module
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. automodule:: metasyn.distribution.base
+   :members:
+   :show-inheritance:
+   :private-members:
```

### Comparing `metasyn-0.8.0/docs/source/conf.py` & `metasyn-1.0.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
 project = 'metasyn'
 copyright = '2024, SODA Team'
 author = 'SODA Team'
 
 
 # The full version, including alpha/beta/rc tags
-release = '0.8.0'
+release = '1.0.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ['sphinx.ext.napoleon', "sphinx.ext.autodoc", "sphinx_autodoc_typehints",
-              'sphinx_rtd_theme', "sphinx_inline_tabs", "sphinx_copybutton"]
+              'sphinx_rtd_theme', "sphinx_inline_tabs", "sphinx_copybutton", "sphinx.ext.autosummary"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
```

### Comparing `metasyn-0.8.0/docs/source/developer/GMF.rst` & `metasyn-1.0.0/docs/source/developer/GMF.rst`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/developer/contributing.rst` & `metasyn-1.0.0/docs/source/developer/contributing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,9 +58,12 @@
 To do so, first install Tox to your environment following the `Tox installation guide <https://tox.wiki/en/4.11.3/installation.html>`_. Then simply run the ``tox`` on the ``metasyn`` root directory to run all the tests. If you want to run a specific test, you can do so by specifying a (list of) test environment(s), e.g. ``tox -e ruff`` or ``tox -e ruff,pylint,pydocstyle,mypy,sphinx,pytest,nbval``. The available test environments can be found in the `pyproject.toml <https://github.com/sodascience/metasyn/blob/main/pyproject.toml>`_ file, under the ``[tool.tox]`` section.
 
 
 
 
 Maintaining the package
 -----------------------
-Our GitHub Wiki contains a guide on how to maintain the package. You can find it `here <https://github.com/sodascience/metasyn/wiki/Maintainers-guide>`_.
+Our GitHub Wiki contains a guide on how to maintain the package. You can find it `here <https://github.com/sodascience/metasyn/wiki>`_.
 
+Code of Conduct
+---------------
+We expect all contributors to adhere to the Code of Conduct found on our `Github page <https://github.com/sodascience/metasyn/blob/main/.github/CODE_OF_CONDUCT.md>`_.
```

### Comparing `metasyn-0.8.0/docs/source/developer/distributions.rst` & `metasyn-1.0.0/docs/source/developer/distributions.rst`

 * *Files 12% similar despite different names*

```diff
@@ -124,40 +124,20 @@
 .. warning:: 
     
     This mixin class has a default implementation that will work for many distributions, but it may not be appropriate for all. Be sure to check the implementation before using it. 
 
 
 Other modules
 ~~~~~~~~~~~~~
-The rest of the modules in the :mod:`~metasyn.distribution` subpackage contain the classes used to represent different types of distributions.
-
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| Module                                   | Description                                                                                                                                                       |
-+==========================================+===================================================================================================================================================================+
-| :mod:`~metasyn.distribution.categorical` | Implements categorical distributions                                                                                                                              |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.constant`    | Implements constant distributions                                                                                                                                 |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.continuous`  | Implements continuous distributions                                                                                                                               |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.datetime`    | ``time``, ``date`` and ``datetime`` distributions.                                                                                                                |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.discrete`    | Implements discrete distributions.                                                                                                                                |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.faker`       | Implements distributions that are based on the `Faker <https://faker.readthedocs.io/en/master/>`_ package.                                                        |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.na`          | Implements a distribution which generates *only* NA values.                                                                                                       |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
-| :mod:`~metasyn.distribution.regex`       | Implements distributions that are based on regular expressions. It implements the open source `regexmodel <https://github.com/sodascience/regexmodel>`_ package.  |
-+------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
+The rest of the modules in the :mod:`~metasyn.distribution` subpackage contain the classes used to represent different types of distributions. A comprehensive overview of these modules, along with the distributions they implement, can be found on the API reference's :doc:`/api/metasyn.distribution` page.
 
 
 Creating a new distribution
 ---------------------------
-The first step to creating a new distribution is to inherit from a distribution class. This can be a base class (e.g. :class:`~metasyn.distribution.base.BaseDistribution`, :class:`~metasyn.distribution.base.ScipyDistribution`), or an existing distribution.```
+The first step to creating a new distribution is to inherit from a distribution class. This can be a base class (e.g. :class:`~metasyn.distribution.base.BaseDistribution`, :class:`~metasyn.distribution.base.ScipyDistribution`), or an existing distribution.
 
 The next step is to set the attributes of the distribution using the :func:`~metasyn.distribution.base.metadist` decorator. Refer to :class:`~metasyn.distribution.base.BaseDistribution` for an overview of these attributes.
 
 .. admonition:: Important
 
     In is posible to have different variations of the same distribution, for various data types. As is the case with the ``core.uniform`` distributions in ``metasyn``. 
 
@@ -166,15 +146,15 @@
 Finally the distribution has to be added to a provider list, so that it can be used by ``metasyn`` for fitting.
 
 For example, let's say we want to create a new distribution for unique continuous variables, to be a part of the core ``metasyn`` distribution provider. We could implement the distribution as follows:
 
 .. code-block:: python
 
     @metadist(implements="core.new_distribution", var_type="continuous", unique=True, version="1.0")
-    class NewDistribution(BaseDistribution, UniqueDistributionMixin):
+    class NewDistribution(UniqueDistributionMixin, BaseDistribution):
         """New custom distribution."""
 
         def __init__(self, lower=0, upper=1):
             self.lower = lower
             self.upper = upper
 
         @classmethod
```

### Comparing `metasyn-0.8.0/docs/source/developer/overview.rst` & `metasyn-1.0.0/docs/source/faq.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,71 @@
-Overview
-========
+FAQ
+===
 
-This page aims to introduce the main classes and modules of the ``metasyn`` package. It is intended to be a high-level overview of the package's structure and functionality. For a thorough overview, please refer to the :doc:`API reference </api/metasyn>`. Clicking on a class or module name will automatically take you to its API reference section.
+Here, we've compiled answers to commonly asked questions about ``metasyn`` and its development. If you have any other questions, need further assistance, or want to discuss something related to metasyn, don't hesitate to contact us directly. You can find our contact details on the :doc:`contact page </about/contact>`. We're more than happy to assist you and provide any additional information you may need.
 
-.. warning:: 
-    This page is intended for developers and advanced users. If you are new to ``metasyn``, please refer to the :doc:`/usage/usage` first. 
+**Can I use pandas DataFrames with metasyn?**
+-----------------------------------------------
+Yes, you can use pandas DataFrames with metasyn. However, please note that ``metasyn`` internally utilizes polars for consistent typing and handling of non-existing data. Although supplying pandas DataFrames is supported, there may be conversion issues, particularly in certain edge cases. To ensure optimal functionality, we recommend creating polars DataFrames. The synthetic datasets generated by ``metasyn`` are always in the form of polars DataFrames. If needed, you can easily convert them back to pandas DataFrames using the `df_pandas = df_polars.to_pandas()` method.
 
 
-MetaFrame class
----------------
+**What is a MetaFrame?**
+-------------------------
+A MetaFrame is a fitted model that describes the aggregate structure and characteristics of a dataset. It functions like (statistical) metadata for the dataset, providing information about the dataset without revealing the actual data itself. When ``metasyn`` is fed a dataset (as DataFrame), it generates this MetaFrame to capture certain key aspects of the data.
 
-The :class:`~metasyn.MetaFrame` class is a core component of the ``metasyn`` package. It represents a metadata frame, which is a structure that holds statistical metadata about a dataset. The data contained in a :obj:`~metasyn.MetaFrame` is in line with the :doc:`/developer/GMF`.
+Key elements encapsulated in a MetaFrame include variable names, their data types, the proportion of missing values, and the parameters of the distributions that these variables follow in the dataset. This information is sufficient to understand the overall structure and attributes of the data, without divulging the exact data points.
 
-Essentially, a :obj:`~metasyn.MetaFrame` is a collection of :obj:`~metasyn.MetaVar` objects, each representing a column in a dataset. It contains methods that allow for the following:
+When a MetaFrame is created from an input dataset, it can be exported for auditing or manual editing. 
 
-- **Fitting to a DataFrame**: The :meth:`~metasyn.MetaFrame.fit_dataframe` method allows for fitting a Polars DataFrame to create a :obj:`~metasyn.MetaFrame` object. This method takes several parameters including the DataFrame, column specifications, distribution providers, privacy level, and a progress bar flag.
-- **Exporting and importing**: The :meth:`~metasyn.MetaFrame.export` method serializes and exports the :obj:`~metasyn.MetaFrame` to a JSON file, following the GMF format. The :meth:`~metasyn.MetaFrame.from_json` method reads a :obj:`~metasyn.MetaFrame` from a JSON file.
-- **Synthesizing to a DataFrame**: The :meth:`~metasyn.MetaFrame.synthesize` method creates a synthetic Polars DataFrame based on the :obj:`~metasyn.MetaFrame`.
+In the ``metasyn`` workflow, once you have a MetaFrame, ``metasyn`` can generate synthetic data that aligns with the MetaFrame. This synthetic data shares the structural and distributional characteristics (as defined in the MetaFrame) with the original data but does not contain any actual data points from the original dataset, thus preserving privacy.
 
+The process of generating synthetic data solely from the MetaFrame ensures that this synthetic data is separate and independent from the original sensitive source data, thereby reducing privacy concerns while sharing or distributing this synthetic data.
 
-MetaVar class
--------------
 
-The :class:`~metasyn.MetaVar` represents a metadata variable, and is a structure that holds all metadata needed to generate a synthetic column for it. This is the variable level building block for the MetaFrame. It contains the methods to convert a polars `Series` into a variable with an appropriate distribution. The :obj:`~metasyn.MetaVar` class is to the :obj:`~metasyn.MetaFrame` what a polars `Series` is to a `DataFrame`.
 
-A :obj:`~metasyn.MetaVar` contains information on the variable type (``var_type``), the series from which the variable is created (``series``), the name of the variable (``name``), the distribution from which random values are drawn (``distribution``), the proportion of the series that are missing/NA (``prop_missing``), the type of the original values (``dtype``), and a user-provided description of the variable (``description``). 
+**I encountered the warning: "Variable PassengerId seems unique, but not set to be unique." What should I do?**
+-----------------------------------------------------------------------------------------------------------------
+This warning occurs when ``metasyn`` detects a column, that seems to have unique values in the real dataset but isn't specified to be unique in the fitting of the :obj:`MetaFrame<metasyn.metaframe.MetaFrame>`. To address this, you can use the `spec` parameter to create a specification dictionary and indicate that the column should have unique values. Here's an example of how to do this (in this example ``PassengerId`` is the column with unique values):
 
-This class is considered a passthrough class used by the :obj:`~metasyn.MetaFrame` class, and is not intended to be used directly by the user. It contains the following functionality:
+.. code-block:: python
 
-- **Fitting distributions**: The :meth:`~metasyn.MetaVar.fit` method fits distributions to the data. Here you can set the distribution, privacy package and uniqueness for the variable.
-- **Drawing values and series**: The :meth:`~metasyn.MetaVar.draw` method draws a random item for the variable in whatever type is required. The :meth:`~metasyn.MetaVar.draw_series` method draws a new synthetic series from the metadata. For this to work, the variable has to be fitted.
-- **Converting to and from a dictionary**: The :meth:`~metasyn.MetaVar.to_dict` method creates a dictionary from the variable. The :meth:`~metasyn.MetaVar.from_dict` method restores a variable from a dictionary.
+   from metasyn import VarSpec
 
+   # Create a specification dictionary, and specify the column as unique:
+   var_specs = [
+      VarSpec("PassengerId", unique=True)
+   ]
 
-Subpackages
------------
-There are currently three subpackages in the ``metasyn`` package. These are the :mod:`~metasyn.distribution`, :mod:`~metasyn.schema`, and :mod:`~metasyn.demo` packages.
+   # Call the fit_dataframe() function, passing in the `var_spec` dictionary as the `spec` argument
+   mf = MetaFrame.fit_dataframe(df, var_specs=var_specs)
 
-* the :mod:`~metasyn.distribution` subpackage contains (submodules with) the classes that are used to fit distributions to the data and draw random values from them. More information on distributions and how to implement them can be found in the :doc:`/developer/distributions` documentation page.
-* The :mod:`~metasyn.schema` package simply contains the JSON-schema used to validate metadata, and ensure that it is in line with the :doc:`/developer/GMF`.
-* The :mod:`~metasyn.demo` package is meant for demo and tutorial purposes. It contains only two functions, :meth:`~metasyn.demo.create_titanic_demo`, which can be used to create a demo dataset based on the `Titanic dataset <https://github.com/datasciencedojo/datasets/blob/master/titanic.csv>`_, and :meth:`~metasyn.demo.demo_file`, which retrieves the filepath to this demo dataset allowing users to quickly access it. 
+More information on how to use the optional parameters in the :meth:`metasyn.MetaFrame.fit_dataframe() <metasyn.metaframe.MetaFrame.fit_dataframe>` function can be found in :doc:`/usage/generating_metaframes` under :ref:`optionalparams`.
 
-:meth:`~metasyn.demo.demo_file` is imported automatically as part of the main ``metasyn`` package, as such it can be accessed through :meth:`metasyn.demo_file`, as opposed to :meth:`metasyn.demo.demo_file`. 
+**I found a bug/issue, where can I report it?**
+-----------------------------------------------
+If you encounter any bugs or have identified an issue with metasyn, we encourage you to report it on our `GitHub issue tracker <https://github.com/sodascience/metasyn/issues>`_. This allows us to track and address the problem efficiently. Alternatively, you can find out how to contact us through the details provided in our :doc:`contact page </about/contact>`.
 
-Submodules
-----------
-The ``metasyn`` package is organized into several submodules, each focusing on different aspects of synthetic data generation and privacy. Here's an overview of some key submodules:
+**I would like to contribute to the project, how do I get started?**
+---------------------------------------------------------------------
+That's fantastic! We welcome and appreciate contributions from the community. To get started with contributing to metasyn, please refer to our detailed guide in the :doc:`/developer/developer` section. It contains all the information you need to start contributing.
+
+
+**Why did you change the name from MetaSynth to metasyn?**
+----------------------------------------------------------
+
+The project was originally named MetaSynth. However, as we progressed, we discovered that there was already an existing and established audio synthesis software under the same `name <https://uisoftware.com/metasynth/>`_. To avoid potential confusion between these two unrelated projects, we have decided to change the name of our project to **metasyn**. This new name still reflects the package's core goal, of metadata-driven data synthesis. We have also changed the styling of the name to be all lowercase to align with how the package is used in code (e.g. ```import metasyn```).
+
+It is important to note that despite the name change, ``metasyn`` as a project and the package's functionality remain the same.
+
+
+**What is the classification of metasyn's synthetic datasets?**
+------------------------------------------------------------------
+Metasyn's synthetically generated datasets are classified as `Synthetically-Augmented Plausible datasets <https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/onsmethodologyworkingpaperseriesnumber16syntheticdatapilot>`__, as categorized by the Office for National Statistics (ONS).
+
+.. epigraph:: ONS criteria for a Synthetically-augmented plausible dataset:
+   
+   * Preserve the format and record-level plausibility as detailed previously and replicate marginal (univariate) distributions where possible.
+   * Constructed based on the real dataset, values are generated based on observed distributions (with added fuzziness and smoothing) but no attempt made to preserve relationships.
+   * Missing value codes and their frequency is to be preserved.
+   * Disclosure control evaluation is necessary case by case, special care to be taken with names and so on.
+   * To be used for extended code testing, minimal analytical value, non-negligible disclosure risk.
 
-* The :mod:`metasyn.var` module contains the :class:`~metasyn.var.MetaVar` class and its methods, as described above.
-* The :mod:`metasyn.metaframe` module contains the :class:`~metasyn.metaframe.MetaFrame` class and its methods, as described above. 
-* The :mod:`metasyn.provider` module contains the :class:`~metasyn.provider.BaseDistributionProvider` class, which encapsulates a set of distributions, the :class:`~metasyn.provider.BuiltinDistributionProvider` class, which includes the builtin distributions and the :class:`~metasyn.provider.DistributionProviderList` class to allow for multiple distribution providers.
-* The :mod:`metasyn.testutils` module provides testing utilities for plugins. It includes functions for checking distributions and distribution providers.
-* The :mod:`metasyn.validation` module contains tools for validating distribution outputs and GMF file formats.
-* The :mod:`metasyn.privacy` module contains the basis for implementing privacy features. A system to incorporate privacy features such as differential privacy or other forms of disclosure control is still being implemented.
-* The :mod:`metasyn.util` module contains utility classes :class:`~metasyn.util.DistributionSpec` and :class:`~metasyn.util.VarConfig`.
-* The :mod:`metasyn.config` module contains the :class:`~metasyn.config.MetaConfig` class that can read .toml configuration files.
```

### Comparing `metasyn-0.8.0/docs/source/developer/plugins.rst` & `metasyn-1.0.0/docs/source/developer/plugins.rst`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/ClassDiagram.drawio` & `metasyn-1.0.0/docs/source/images/ClassDiagram.drawio`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/distributions.drawio` & `metasyn-1.0.0/docs/source/images/distributions.drawio`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/distributions.svg` & `metasyn-1.0.0/docs/source/images/distributions.svg`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/example_input_output.png` & `metasyn-1.0.0/docs/source/images/example_input_output.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/example_input_output_concise.png` & `metasyn-1.0.0/docs/source/images/example_input_output_concise.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/flow_metadata_generation.png` & `metasyn-1.0.0/docs/source/images/flow_metadata_generation.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/flow_metadata_generation_code.png` & `metasyn-1.0.0/docs/source/images/flow_metadata_generation_code.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/flow_synthetic_data_generation.png` & `metasyn-1.0.0/docs/source/images/flow_synthetic_data_generation.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/flow_synthetic_data_generation_code.png` & `metasyn-1.0.0/docs/source/images/flow_synthetic_data_generation_code.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/basic-grey.svg` & `metasyn-1.0.0/docs/source/images/logos/basic-grey.svg`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/basic_grey-med.png` & `metasyn-1.0.0/docs/source/images/logos/basic_grey-med.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/basic_grey.png` & `metasyn-1.0.0/docs/source/images/logos/basic_grey.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/blue.png` & `metasyn-1.0.0/docs/source/images/logos/blue.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/blue.svg` & `metasyn-1.0.0/docs/source/images/logos/blue.svg`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/blue_med.png` & `metasyn-1.0.0/docs/source/images/logos/blue_med.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/grey.png` & `metasyn-1.0.0/docs/source/images/logos/grey.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/grey.svg` & `metasyn-1.0.0/docs/source/images/logos/grey.svg`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/grey_med.png` & `metasyn-1.0.0/docs/source/images/logos/grey_med.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/metasyn.afdesign` & `metasyn-1.0.0/docs/source/images/logos/metasyn.afdesign`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/soda.png` & `metasyn-1.0.0/docs/source/images/logos/soda.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/white.png` & `metasyn-1.0.0/docs/source/images/logos/white.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/white.svg` & `metasyn-1.0.0/docs/source/images/logos/white.svg`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/logos/white_med.png` & `metasyn-1.0.0/docs/source/images/logos/white_med.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_basic.png` & `metasyn-1.0.0/docs/source/images/pipeline_basic.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_basic_legacy.png` & `metasyn-1.0.0/docs/source/images/pipeline_basic_legacy.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_cli.png` & `metasyn-1.0.0/docs/source/images/pipeline_cli.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_cli_create_meta.png` & `metasyn-1.0.0/docs/source/images/pipeline_cli_create_meta.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_estimation_code.png` & `metasyn-1.0.0/docs/source/images/pipeline_estimation_code.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_estimation_simple.png` & `metasyn-1.0.0/docs/source/images/pipeline_estimation_simple.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_func_names.png` & `metasyn-1.0.0/docs/source/images/pipeline_func_names.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_generation_code.png` & `metasyn-1.0.0/docs/source/images/pipeline_generation_code.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_generation_simple.png` & `metasyn-1.0.0/docs/source/images/pipeline_generation_simple.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_serialization_code.png` & `metasyn-1.0.0/docs/source/images/pipeline_serialization_code.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/images/pipeline_serialization_simple.png` & `metasyn-1.0.0/docs/source/images/pipeline_serialization_simple.png`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/index.rst` & `metasyn-1.0.0/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -63,25 +63,29 @@
 Documentation Outline
 ---------------------
 
 .. toctree::
    :hidden:
    :maxdepth: 2
 
-   about/about
+   metasyn_in_detail
    usage/usage
    developer/developer
    api/metasyn
    faq
+   about/about
+
 
 This documentation is designed to help you easily navigate and find the information you need. It is organized into the following four sections:
 
-:doc:`/about/about`
-^^^^^^^^^^^^^^^^^^^
-The :doc:`About Section </about/about>` provides an overview of metasyn's purpose and functionality, contact information, and licensing details.
+
+:doc:`metasyn_in_detail`
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+The :doc:`/metasyn_in_detail` section provides an overview of metasyn's purpose and functionality.
 
 :doc:`/usage/usage`
 ^^^^^^^^^^^^^^^^^^^
 The :doc:`/usage/usage` contains detailed, step-by-step instructions, as well as best practices for using the package. If you're new to metasyn, we recommend you start here!
 
 :doc:`/api/metasyn`
 ^^^^^^^^^^^^^^^^^^^^^
@@ -91,15 +95,17 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 The :doc:`/developer/developer` provides resources for those interested in contributing to metasyn's development. This section includes guidance on how to build upon the existing ``metasyn`` codebase, add new modules, functions, or even integrate other packages.
 
 :doc:`/faq`
 ^^^^^^^^^^^^^^^^^^^
 The :doc:`/faq` contains commonly asked questions and answers about metasyn. 
 
+:doc:`/about/about`
+^^^^^^^^^^^^^^^^^^^
+The :doc:`About Section </about/about>` provides contact information, and licensing details.
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
-
```

### Comparing `metasyn-0.8.0/docs/source/usage/cli.rst` & `metasyn-1.0.0/docs/source/usage/cli.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 At any point, you can also use the help command to get more information about the CLI and its subcommands:
 
 .. code-block:: console
 
    metasyn --help
 
 
+.. admonition:: When should I (not) use the CLI
+
+   The CLI is mostly feature complete from creating synthetic data from ``.csv files``, but there are some limitations. The main limitation is that it needs to read the
+   csv file, for which it tries to use sensible default settings. However, this can result in errors. If you encounter errors, might want to either preprocess your data
+   so that it can be read with the default settings, or use the python API instead.
+   
+   Another limitation is that you cannot specify which columns should be categorical.
+
 Accessing the CLI
 -----------------
 If you have installed the main ``metasyn`` package, the CLI should be available automatically. You can find instructions on how to install ``metasyn`` in the :doc:`installation` section of the documentation.
 
 Alternatively, the CLI can be accessed through a Docker container, allowing you to run ``metasyn`` in an isolated environment without installing the package on your system. This can be useful, for example, when trying out ``metasyn`` without affecting your existing Python environment.
 
 Here's how you can use Docker to access Metasyn's CLI:
@@ -46,35 +54,35 @@
 
          docker run -v $(pwd):/wd sodateam/metasyn --help
 
 
 The ``metasyn`` CLI should now be up and running within the Docker container and ready for use!
 
 .. note:: 
-   You can also specify which ``metasyn`` version to use in docker, by adding a tag to the docker image. For example, to use version 0.6, you can use the following command:
+   You can also specify which ``metasyn`` version to use in docker, by adding a tag to the docker image. For example, to use version 1.0, you can use the following command:
 
    .. tab:: Installing a specific version
       
       .. code-block:: console
 
-         docker pull sodateam/metasyn:v0.6
+         docker pull sodateam/metasyn:v1.0
 
    .. tab:: Using a command on a specific version
 
       .. tab:: Windows
 
          .. code-block:: console
 
-            docker run -v %cd%:/wd sodateam/metasyn:v0.6 --help
+            docker run -v %cd%:/wd sodateam/metasyn:v1.0 --help
 
       .. tab:: Unix or MacOS:
 
          .. code-block:: console
 
-            docker run -v $(pwd):/wd sodateam/metasyn:v0.6 --help
+            docker run -v $(pwd):/wd sodateam/metasyn:v1.0 --help
 
 
 Creating Generative Metadata
 ----------------------------
 The ``create-meta`` subcommand combines the :doc:`estimation </usage/generating_metaframes>` and :doc:`serialization </usage/exporting_metaframes>` steps in the pipeline into one, this allows you to generate generative metadata for a tabular dataset (in CSV format), and store it in a GMF (Generative Metadata Format) file.
 
 .. image:: /images/pipeline_cli_create_meta.png
@@ -118,53 +126,38 @@
 
       .. code-block:: console
 
          docker run -v $(pwd):/wd sodateam/metasyn create-meta wd/my_dataset.csv wd/my_gmf.json
 
 The ``create-meta`` command also takes one optional argument:
 
-* ``--config [config-file]``: The filepath and name of a configuration file that specifies distribution behavior. For example, if we want to set a column to be unique or to have a specific distribution, we can do so by specifying it in the configuration file.
-
-.. note::
-
-   The configuration file must be in the `.toml` format. For more information on the format, please refer to the `TOML documentation <https://toml.io/en/>`_.
-
-   An example of a configuration file that specifies the ``PassengerId`` column to be unique and the ``Fare`` column to have a log-normal distribution is as follows:
-
-   .. code-block:: toml
-
-      [[var]]
-      name = "PassengerId"
-      distribution = {unique = true}  # Notice lower capitalization for .toml files.
+* ``--config [config-file]``: The filepath and name of a .toml configuration file that specifies distribution behavior. For example, if we want to set a column to be unique or to have a specific distribution, we can do so by specifying it in the configuration file. Information on how to use these files can be found in the :doc:`/usage/config_files` section.
 
+.. admonition:: Generating a GMF file without a dataset
 
-      [[var]]
-      name = "Fare"
-      distribution = {implements = "core.log_normal"}
+   It is also possible to create a GMF file (and to generate synthetic data from there) without every inputting a dataset. Adding columns not present in the input dataset is also possible using the same method.
 
-It is also possible to create a GMF file without any input CSV. For this to work, you need to supply a configuration
-file that fully specifies all wanted columns. You will need to tell ``metasyn`` in the configuration file that the
-column is ``data_free``. It is also required to set the number of rows under the `general` section, for example:
+   This can be done by supplying a configuration file that fully specifies the columns that should be generated. For each to be generated column, you need also need to set the `data_free` parameter to `true`.
 
-   .. code-block:: toml
-
-      n_rows = 100
+   It is also required to set the number of rows under the `general` section.
+   
+   For example, to create a GMF file that can be used to generate 100 rows of synthetic data with a single column `PassengerId`, that is unique and has a discrete distribution, you can use the following configuration file:
 
+      .. code-block:: toml
 
-      [[var]]
+         n_rows = 100
 
-      name = "PassengerId"
-      data_free = true
-      prop_missing = 0.0
-      description = "ID of the unfortunate passenger."
-      var_type = "discrete"
-      distribution = {implements = "core.unique_key", unique = true, parameters = {consecutive = 1, low = 0}}
+         [[var]]
 
-The example will generate a GMF file that can be used to generate new synthetic data with the ``synthesize``
-subcommand described below.
+         name = "PassengerId"
+         data_free = true
+         prop_missing = 0.0
+         description = "ID of the unfortunate passenger."
+         var_type = "discrete"
+         distribution = {implements = "core.unique_key", unique = true, parameters = {consecutive = true, low = 0}}
 
 
 Generating Synthetic Data
 -------------------------
 The ``synthesize`` subcommand combines the :doc:`deserialization </usage/exporting_metaframes>` and :doc:`generation </usage/generating_synthetic_data>` steps in the pipeline into one, and allows you to generate a synthetic dataset from a previously exported MetaFrame (stored as GMF file). 
 
 .. image:: /images/pipeline_cli.png
@@ -218,14 +211,16 @@
 - ``-p`` or ``--preview``: To preview the first six rows of synthesized data. This can be extremely useful for quick data validation without saving it to a file.
 
 .. note::
 
    The ``output`` is required unless ``--preview`` is used.
 
 
+
+
 Creating Validation schemas
 ---------------------------
 
 The ``schema`` subcommand generates a schema that describes the expected format of the GMF files. These can be used to validate GMF files before importing and loading them into a :obj:`MetaFrame<metasyn.metaframe.MetaFrame>`.
 
 .. code-block:: console
    
@@ -239,11 +234,7 @@
 
 To retrieve a list of all available plugins, you can use the ``--list`` or ``-l`` argument. This displays the available plugins:
 
 .. code-block:: console
    
    metasyn schema --list
 
-
-
-
-
```

### Comparing `metasyn-0.8.0/docs/source/usage/exporting_metaframes.rst` & `metasyn-1.0.0/docs/source/usage/exporting_metaframes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,124 +9,152 @@
 
 .. image:: /images/pipeline_serialization_simple.png
    :alt: MetaFrame Serialization Flow
    :align: center
 
 Exporting a MetaFrame
 ----------------------
-MetaFrames can be serialized and exported to a GMF file by calling the :meth:`metasyn.metaframe.MetaFrame.to_json` method on a :obj:`MetaFrames<metasyn.metaframe.MetaFrame>`. 
+MetaFrames can be serialized and exported to a GMF file by calling the :meth:`metasyn.metaframe.MetaFrame.to_json` method on a :obj:`MetaFrame<metasyn.metaframe.MetaFrame>`. 
 
 The following code exports a generated :obj:`MetaFrame<metasyn.metaframe.MetaFrame>` object named ``mf`` to a GMF file named ``exported_metaframe``.
 
 .. code-block:: python
 
    mf.to_json("exported_metaframe.json")
 
 .. raw:: html
 
    <details> 
-   <summary> An example of a MetaFrame that has been exported to a GMF file: </summary>
+   <summary> <em><b>An example of a MetaFrame that has been exported to a GMF file: </em></b></summary>
 
 .. code-block:: json
     
     {
         "n_rows": 5,
         "n_columns": 5,
         "provenance": {
             "created by": {
                 "name": "metasyn",
-                "version": "0.4.0"
+                "version": "0.8.1"
             },
-            "creation time": "2023-08-07T12:14:06.232957"
+            "creation time": "2024-04-29T12:07:36.646884"
         },
         "vars": [
             {
                 "name": "ID",
                 "type": "discrete",
                 "dtype": "Int64",
                 "prop_missing": 0.0,
                 "distribution": {
                     "implements": "core.unique_key",
+                    "version": "1.0",
                     "provenance": "builtin",
                     "class_name": "UniqueKeyDistribution",
+                    "unique": true,
                     "parameters": {
-                        "low": 1,
-                        "consecutive": 1
+                        "lower": 1,
+                        "consecutive": true
                     }
+                },
+                "creation_method": {
+                    "created_by": "metasyn",
+                    "unique": true
                 }
             },
             {
                 "name": "fruits",
                 "type": "categorical",
-                "dtype": "Categorical",
+                "dtype": "Categorical(ordering='physical')",
                 "prop_missing": 0.0,
                 "distribution": {
                     "implements": "core.multinoulli",
+                    "version": "1.0",
                     "provenance": "builtin",
                     "class_name": "MultinoulliDistribution",
+                    "unique": false,
                     "parameters": {
                         "labels": [
                             "apple",
                             "banana"
                         ],
                         "probs": [
                             0.4,
                             0.6
                         ]
                     }
+                },
+                "creation_method": {
+                    "created_by": "metasyn"
                 }
             },
             {
                 "name": "B",
                 "type": "discrete",
                 "dtype": "Int64",
                 "prop_missing": 0.0,
                 "distribution": {
-                    "implements": "core.poisson",
+                    "implements": "core.uniform",
+                    "version": "1.0",
                     "provenance": "builtin",
-                    "class_name": "PoissonDistribution",
+                    "class_name": "DiscreteUniformDistribution",
+                    "unique": false,
                     "parameters": {
-                        "mu": 3.0
+                        "lower": 1,
+                        "upper": 6
                     }
+                },
+                "creation_method": {
+                    "created_by": "metasyn",
+                    "unique": false
                 }
             },
             {
                 "name": "cars",
                 "type": "categorical",
-                "dtype": "Categorical",
+                "dtype": "Categorical(ordering='physical')",
                 "prop_missing": 0.0,
                 "distribution": {
                     "implements": "core.multinoulli",
+                    "version": "1.0",
                     "provenance": "builtin",
                     "class_name": "MultinoulliDistribution",
+                    "unique": false,
                     "parameters": {
                         "labels": [
                             "audi",
                             "beetle"
                         ],
                         "probs": [
                             0.2,
                             0.8
                         ]
                     }
+                },
+                "creation_method": {
+                    "created_by": "metasyn"
                 }
             },
             {
                 "name": "optional",
                 "type": "discrete",
                 "dtype": "Int64",
                 "prop_missing": 0.2,
                 "distribution": {
-                    "implements": "core.discrete_uniform",
+                    "implements": "core.uniform",
+                    "version": "1.0",
                     "provenance": "builtin",
                     "class_name": "DiscreteUniformDistribution",
+                    "unique": false,
                     "parameters": {
-                        "low": -30,
-                        "high": 301
+                        "lower": -30,
+                        "upper": 301
                     }
+                },
+                "creation_method": {
+                    "created_by": "metasyn"
                 }
             }
         ]
     }
 
 
 .. raw:: html
@@ -300,12 +328,12 @@
    * - 5
      - orange
      - 5
      - audi
      - 51
 
 
-As you can see, it is very easy to modify the metadata to change how data is synthesized. Similarly to this example, any other aspect of the MetaFrame can be edited, including the variable names, the variable types, the data types, the percentage of missing values, and the distribution attributes. 
+As you can see, you can modify the metadata to change how data is synthesized. Similarly to this example, any other aspect of the MetaFrame can be edited, including the variable names, the variable types, the data types, the percentage of missing values, and the distribution attributes. 
 
 .. warning:: 
-    Be extra careful when manually editing GMF files as errors in names, values, or formatting can cause problems. 
+    Be extra careful when manually editing GMF files as errors in names, values, or formatting can cause problems. In this case, metasyn will most likely produce JSON validation errors.
```

### Comparing `metasyn-0.8.0/docs/source/usage/extensions.rst` & `metasyn-1.0.0/docs/source/usage/extensions.rst`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/usage/generating_metaframes.rst` & `metasyn-1.0.0/docs/source/usage/generating_metaframes.rst`

 * *Files 11% similar despite different names*

```diff
@@ -6,43 +6,53 @@
 .. image:: /images/pipeline_estimation_simple.png
    :alt: MetaFrame Generation Flow
    :align: center
 
 
 .. admonition:: Want to learn more?
     
-   This page focuses on using ``metasyn`` to generate MetaFrames. If you're interested in learning more about how MetaFrames are generated behind the scenes and the assumptions involved, see the :doc:`/about/metasyn_in_detail` page for details.
+   This page focuses on using ``metasyn`` to generate MetaFrames. If you're interested in learning more about how MetaFrames are generated behind the scenes and the assumptions involved, see the :doc:`/metasyn_in_detail` page for details.
 
-.. admonition:: Command-line Interface
+Preparing the Dataset
+---------------------
 
-    It is also possible to generate a MetaFrame, based on a given GMF file, using the ``metasyn`` command-line interface. For instructions on how to do so, see the :doc:`/usage/cli` page.
-   
-Basics
-------
+Before we can pass a dataset into metasyn, we need to convert it to a `Polars <https://pola.rs>`__ DataFrame. In doing so, we can indicate which columns contain categorical values. We can also tell Polars to find columns that may contain dates or timestamps. Metasyn later uses this information to generate categorical or date-like values where appropriate. For more information on how to use Polars, check out the `Polars documentation <https://docs.pola.rs/>`__.
+
+For example, if we want to load a dataset named 'dataset.csv' into a Polars DataFrame, set the columns ``Color`` and ``Fruit`` to be categorical and parse dates in the DataFrame. We can use the following code:
+
+.. code:: python
+
+   # Create a Polars DataFrame
+   df = pl.read_csv(
+       source="dataset.csv",
+       dtypes={"Color": pl.Categorical, "Fruit": pl.Categorical},
+       try_parse_dates=True,
+   )
+
+.. admonition:: Note on Pandas and Polars DataFrames
 
-Metasyn can generate metadata from any given dataset (provided as Polars or Pandas DataFrame),
-using the :meth:`metasyn.MetaFrame.fit_dataframe(df) <metasyn.metaframe.MetaFrame.fit_dataframe>` classmethod.
+    Internally, ``metasyn`` uses Polars (instead of Pandas) mainly because typing and the handling of non-existing data is more consistent. It is possible to supply a Pandas DataFrame instead of a Polars DataFrame to the ``MetaFrame.fit_dataframe`` method. However, this uses the automatic Polars conversion functionality, which for some edge cases results in problems. Therefore, we recommend users to create Polars DataFrames. The resulting synthetic dataset is always a Polars DataFrame, but this can be easily converted back to a Pandas DataFrame by using ``df_pandas = df_polars.to_pandas()``.
+
+Generating a MetaFrame
+----------------------
+With the DataFrame in place, we can now generate a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` object using the :meth:`metasyn.MetaFrame.fit_dataframe(df) <metasyn.metaframe.MetaFrame.fit_dataframe>` class method, passing in a DataFrame as a parameter.
 
 .. image:: /images/pipeline_estimation_code.png
    :alt: MetaFrame Generation With Code Snippet
    :align: center
 
-This function requires a :obj:`DataFrame` to be specified as parameter. The following code returns
-a :obj:`MetaFrame<metasyn.metaframe.MetaFrame>` object named :obj:`mf`, based on a DataFrame named :obj:`df`.
+The following code returns a :obj:`MetaFrame<metasyn.metaframe.MetaFrame>` object named :obj:`mf`, based on a DataFrame named :obj:`df`.
 
 .. code-block:: python
     
-   mf = metasyn.MetaFrame.from_dataframe(df)
-
-.. admonition:: Note on Pandas and Polars DataFrames
+   mf = metasyn.MetaFrame.fit_dataframe(df)
 
-    Internally, ``metasyn`` uses Polars (instead of Pandas) mainly because typing and the handling of non-existing data is more consistent. It is possible to supply a Pandas DataFrame instead of a Polars DataFrame to the ``MetaFrame.from_dataframe`` method. However, this uses the automatic Polars conversion functionality, which for some edge cases results in problems. Therefore, we recommend users to create Polars DataFrames. The resulting synthetic dataset is always a Polars DataFrame, but this can be easily converted back to a Pandas DataFrame by using ``df_pandas = df_polars.to_pandas()``.
 
 
-It is possible to print the (statistical metadata contained in the) :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` to the console/output log. This can simply be done by calling the Python built-in `print` function on a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>`:
+It is possible to print the statistical metadata contained in the :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` to the console/output log. This can simply be done by calling the Python built-in `print` function on a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>`:
 
 .. code-block:: python
 
     print(mf)
 
 
 .. _OptionalParams:
@@ -71,15 +81,15 @@
     
     - ``unique``: Declare whether the column in the synthetic dataset should contain unique values. By default no column is set to unique.
     
     .. admonition:: Detection of unique variables
 
         When generating a MetaFrame, ``metasyn`` will automatically analyze the columns of the input DataFrame to detect ones that contain only unique values.
         If such a column is found, and it has not manually been set to unique in the ``var_specs`` list, the user will be notified with the following warning:
-        ``Warning: Variable [column_name] seems unique, but not set to be unique. Set the variable to be either unique or not unique to remove this warning``
+        ``Variable '[variable name]' was detected to be unique, but has not explicitly been set to unique. To generate only unique values for column 'PassengerId', set unique to True. To dismiss this warning, set unique to False."``
         
         It is safe to ignore this warning - however, be aware that without setting the column as unique, ``metasyn`` may generate duplicate values for that column when synthesizing data.
         
         To remove the warning and ensure the values in the synthesized column are unique, set the column to be unique (``unique = True``) in the ``var_specs`` list.    
     
     - ``description``: Includes a description for each column in the DataFrame.
 
@@ -120,16 +130,23 @@
         ]
 
         mf = MetaFrame.fit_dataframe(df, var_specs=var_specs)
 
    
 dist_providers
 ^^^^^^^^^^^^^^^^
-**dist_providers** allows you to specify distribution providers (as strings or actual provider objects) to use when fitting distributions to the column data.
 
+The parameter **dist_providers** determines which plug-ins should be loaded and in which order. By default all plug-ins will be loaded and available for fitting, which
+is what most users will probably want. It can be helpful for reproducibility to specify which providers were used. The distributions that are available through the `metasyn`
+package itself (without installing any plug-ins) is called "builtin".
    
 privacy
 ^^^^^^^^^
 **privacy** allows you to set the global privacy level for synthetic data generation. If it's not provided, the function defaults it to ``None``.
 
 .. warning::
     Privacy features (such as differential privacy or other forms of disclosure control) are currently under active development. More information on currently available extensions can be found in the :doc:`/usage/extensions` section.
+
+
+Config Files 
+^^^^^^^^^^^^
+It is also possible specify variable specifications, distribution providers and privacy levels through a .toml config file. This is mostly intended for working with the :doc:`/usage/cli`, but can also be used in the Python API. Information on how to use config files can be found in the :doc:`/usage/config_files` section.
```

### Comparing `metasyn-0.8.0/docs/source/usage/generating_synthetic_data.rst` & `metasyn-1.0.0/docs/source/usage/generating_synthetic_data.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,30 @@
 The generated synthetic data, emulates the original data's format and plausibility at the individual record
 level and attempts to reproduce marginal (univariate) distributions where possible.
 Generated values are based on the observed distributions.
 The frequency of missing values is also maintained in the synthetically-augmented dataset.
 
 The generated data does **not** preserve any relationships between variables.
 
-.. warning:: 
+.. admonition:: Prerequisite
 
    Before synthetic data can be generated, a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` object must be :doc:`created </usage/generating_metaframes>` or :doc:`loaded </usage/exporting_metaframes>`.
 
-To generate a synthetic dataset, simply call the :meth:`MetaFrame.synthesize(n) <metasyn.metaframe.MetaFrame.synthesize>` method on a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` object. This method takes an integer parameter `n` which represents the number of rows of data that should be generated.
+To generate a synthetic dataset, simply call the :meth:`MetaFrame.synthesize(n) <metasyn.metaframe.MetaFrame.synthesize>` method on a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` object. This method takes a parameter `n` which represents the number of rows of data that should be generated. By default (when `n` is not provided), metasyn tries to generate as many rows as in the original dataset.
 
 .. image:: /images/pipeline_generation_code.png
    :alt: Synthetic Data Generation With Code Snippet
    :align: center
 
 The following code generates 5 rows of data based on a :obj:`MetaFrame <metasyn.metaframe.MetaFrame>` named ``mf``.
 
 .. code-block:: python
    
    mf.synthesize(5)
 
 Upon succesful execution of the :meth:`MetaFrame.synthesize(n)<metasyn.metaframe.MetaFrame.synthesize>` method, a `Polars DataFrame <https://pola-rs.github.io/polars/py-polars/html/reference/dataframe/index.html>`_ will be returned.
+
+
+
+.. admonition:: Command-Line Interface
+
+   Though we generally recommend using the Python API for using metasyn, you can also generate synthetic data using the CLI. Instructions for doing so can be found in the :doc:`CLI documentation </usage/cli>`.
```

### Comparing `metasyn-0.8.0/docs/source/usage/installation.rst` & `metasyn-1.0.0/docs/source/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/docs/source/usage/interactive_tutorials.rst` & `metasyn-1.0.0/docs/source/usage/interactive_tutorials.rst`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/examples/basic_example.py` & `metasyn-1.0.0/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/examples/demonstration.csv` & `metasyn-1.0.0/examples/demonstration.csv`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/examples/example_config.toml` & `metasyn-1.0.0/examples/example_config.toml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/examples/example_gmf_simple.json` & `metasyn-1.0.0/examples/example_gmf_simple.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9347800925925926%*

 * *Differences: {"'provenance'": "{'created by': {'version': '0.8.1.dev0+ge481025.d20240325'}, 'creation time': "*

 * *                 "'2024-03-25T17:06:53.455575'}",*

 * * "'vars'": "{0: {'creation_method': OrderedDict([('created_by', 'metasyn'), ('unique', True)])}, "*

 * *           '1: {\'dtype\': "Categorical(ordering=\'physical\')", \'creation_method\': '*

 * *           "OrderedDict([('created_by', 'metasyn')])}, 2: {'distribution': {'implements': "*

 * *           "'core.uniform', 'class_name': 'DiscreteUniformDistribution', 'unique': Fa […]*

```diff
@@ -1,36 +1,43 @@
 {
     "n_columns": 5,
     "n_rows": 5,
     "provenance": {
         "created by": {
             "name": "metasyn",
-            "version": "0.6.1.dev45+g6cfcb6d.d20240131"
+            "version": "0.8.1.dev0+ge481025.d20240325"
         },
-        "creation time": "2024-01-31T11:52:33.761957"
+        "creation time": "2024-03-25T17:06:53.455575"
     },
     "vars": [
         {
+            "creation_method": {
+                "created_by": "metasyn",
+                "unique": true
+            },
             "distribution": {
                 "class_name": "UniqueKeyDistribution",
                 "implements": "core.unique_key",
                 "parameters": {
-                    "consecutive": 1,
+                    "consecutive": true,
                     "lower": 1
                 },
                 "provenance": "builtin",
                 "unique": true,
                 "version": "1.0"
             },
             "dtype": "Int64",
             "name": "ID",
             "prop_missing": 0.0,
             "type": "discrete"
         },
         {
+            "creation_method": {
+                "created_by": "metasyn"
+            },
             "distribution": {
                 "class_name": "MultinoulliDistribution",
                 "implements": "core.multinoulli",
                 "parameters": {
                     "labels": [
                         "apple",
                         "banana"
@@ -40,37 +47,44 @@
                         0.6
                     ]
                 },
                 "provenance": "builtin",
                 "unique": false,
                 "version": "1.0"
             },
-            "dtype": "Categorical",
+            "dtype": "Categorical(ordering='physical')",
             "name": "fruits",
             "prop_missing": 0.0,
             "type": "categorical"
         },
         {
+            "creation_method": {
+                "created_by": "metasyn",
+                "unique": false
+            },
             "distribution": {
-                "class_name": "UniqueKeyDistribution",
-                "implements": "core.unique_key",
+                "class_name": "DiscreteUniformDistribution",
+                "implements": "core.uniform",
                 "parameters": {
-                    "consecutive": 0,
-                    "lower": 1
+                    "lower": 1,
+                    "upper": 6
                 },
                 "provenance": "builtin",
-                "unique": true,
+                "unique": false,
                 "version": "1.0"
             },
             "dtype": "Int64",
             "name": "B",
             "prop_missing": 0.0,
             "type": "discrete"
         },
         {
+            "creation_method": {
+                "created_by": "metasyn"
+            },
             "distribution": {
                 "class_name": "MultinoulliDistribution",
                 "implements": "core.multinoulli",
                 "parameters": {
                     "labels": [
                         "audi",
                         "beetle"
@@ -80,36 +94,29 @@
                         0.8
                     ]
                 },
                 "provenance": "builtin",
                 "unique": false,
                 "version": "1.0"
             },
-            "dtype": "Categorical",
+            "dtype": "Categorical(ordering='physical')",
             "name": "cars",
             "prop_missing": 0.0,
             "type": "categorical"
         },
         {
+            "creation_method": {
+                "created_by": "metasyn"
+            },
             "distribution": {
-                "class_name": "MultinoulliDistribution",
-                "implements": "core.multinoulli",
+                "class_name": "DiscreteUniformDistribution",
+                "implements": "core.uniform",
                 "parameters": {
-                    "labels": [
-                        -30,
-                        2,
-                        28,
-                        300
-                    ],
-                    "probs": [
-                        0.25,
-                        0.25,
-                        0.25,
-                        0.25
-                    ]
+                    "lower": -30,
+                    "upper": 301
                 },
                 "provenance": "builtin",
                 "unique": false,
                 "version": "1.0"
             },
             "dtype": "Int64",
             "name": "optional",
```

### Comparing `metasyn-0.8.0/examples/example_gmf_titanic.json` & `metasyn-1.0.0/examples/example_gmf_titanic.json`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/examples/getting_started.ipynb` & `metasyn-1.0.0/examples/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/examples/utils.py` & `metasyn-1.0.0/examples/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-import pandas as pd
+import random
+from pathlib import Path
+
 import numpy as np
-from metasyn.distribution.datetime import UniformDateTimeDistribution, UniformTimeDistribution
-from metasyn.distribution.datetime import UniformDateDistribution
+import pandas as pd
 import wget
-from pathlib import Path
-import random
+
+from metasyn.distribution.datetime import (
+    UniformDateDistribution,
+    UniformDateTimeDistribution,
+    UniformTimeDistribution,
+)
 
 
 def get_demonstration_fp():
     demonstration_fp = Path("demonstration.csv")
     titanic_fp = Path("titanic.csv")
     if demonstration_fp.is_file():
         return demonstration_fp
```

### Comparing `metasyn-0.8.0/metasyn/__init__.py` & `metasyn-1.0.0/metasyn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 """
 
 from importlib.metadata import version
 
 from metasyn.demo.dataset import demo_dataframe, demo_file
 from metasyn.distribution.base import metadist
 from metasyn.metaframe import MetaFrame
-from metasyn.util import VarSpec
 from metasyn.var import MetaVar
+from metasyn.varspec import VarSpec
 
 __all__ = ["MetaVar", "MetaFrame", "demo_file", "demo_dataframe", "metadist", "VarSpec"]
 __version__ = version("metasyn")
```

### Comparing `metasyn-0.8.0/metasyn/__main__.py` & `metasyn-1.0.0/metasyn/__main__.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/config.py` & `metasyn-1.0.0/metasyn/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib  # type: ignore  # noqa
 
 from metasyn.privacy import BasePrivacy, BasicPrivacy, get_privacy
 from metasyn.provider import DistributionProviderList
-from metasyn.util import VarSpec
+from metasyn.varspec import VarSpec
 
 
 class MetaConfig():
     """Configuration class for creating MetaFrames.
 
     This class is used to create, manipulate, and retrieve configurations for
     individual variables in a MetaFrame. It also provides methods for loading
@@ -59,15 +59,15 @@
 
     @property
     def privacy(self) -> BasePrivacy:
         """Return default privacy for generating the metaframe."""
         return self._privacy
 
     @privacy.setter
-    def privacy(self, privacy):
+    def privacy(self, privacy: Optional[Union[dict, BasePrivacy]]):
         if privacy is None:
             self._privacy: BasePrivacy = BasicPrivacy()
         elif isinstance(privacy, dict):
             self._privacy = get_privacy(**privacy)
         else:
             self._privacy = privacy
 
@@ -93,16 +93,29 @@
             Path to the file containing the configuration.
 
         Returns
         -------
         meta_config:
             A fully initialized MetaConfig instance.
         """
-        with open(config_fp, "rb") as handle:
-            config_dict = tomllib.load(handle)
+        try:
+            with open(config_fp, "rb") as handle:
+                config_dict = tomllib.load(handle)
+        except FileNotFoundError as fnf_error:
+            raise FileNotFoundError(f"It appears '{config_fp}' is not a valid filepath."
+                                    f" Please provide a path to a .toml file to load a MetaConfig"
+                                    f" from.") from fnf_error
+        except ValueError as value_error:
+            if Path(config_fp).suffix == ".toml":
+                raise ValueError(f"It appears '{Path(config_fp).name}' is a"
+                                 f" '{Path(config_fp).suffix}' file."
+                                 f" To load a MetaConfig, "
+                                 f"provide it as a .toml file.") from value_error
+            raise ValueError(f"An error occured while parsing the configuration file \n"
+                             f"('{Path(config_fp).name}').") from value_error
         var_list = config_dict.pop("var", [])
         n_rows = config_dict.pop("n_rows", None)
         dist_providers = config_dict.pop("dist_providers", ["builtin"])
         privacy = config_dict.pop("privacy", {"name": "none", "parameters": {}})
         if len(config_dict) > 0:
             raise ValueError(f"Error parsing configuration file '{config_fp}'."
                              f" Unknown keys detected: '{list(config_dict)}'")
```

### Comparing `metasyn-0.8.0/metasyn/demo/dataset.py` & `metasyn-1.0.0/metasyn/demo/dataset.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/demo/demo_spaceship.csv` & `metasyn-1.0.0/metasyn/demo/demo_spaceship.csv`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/demo/demo_titanic.csv` & `metasyn-1.0.0/metasyn/demo/demo_titanic.csv`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/distribution/__init__.py` & `metasyn-1.0.0/metasyn/distribution/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 a series of values, and for generating synthetic data based on the fitted
 distribution. Each distribution class also provides a way to calculate the
 information criterion, used for selecting the best distribution for
 a given set of values.
 """  # pylint: disable=invalid-name
 
 from metasyn.distribution.categorical import MultinoulliDistribution
-from metasyn.distribution.constant import (
-    ConstantDistribution,
-    DateConstantDistribution,
-    DateTimeConstantDistribution,
-    DiscreteConstantDistribution,
-    StringConstantDistribution,
-    TimeConstantDistribution,
-)
 from metasyn.distribution.continuous import (
+    ConstantDistribution,
     ExponentialDistribution,
     LogNormalDistribution,
     NormalDistribution,
     TruncatedNormalDistribution,
     UniformDistribution,
 )
 from metasyn.distribution.datetime import (
+    DateConstantDistribution,
+    DateTimeConstantDistribution,
     DateTimeUniformDistribution,
     DateUniformDistribution,
+    TimeConstantDistribution,
     TimeUniformDistribution,
 )
 from metasyn.distribution.discrete import (
+    DiscreteConstantDistribution,
     DiscreteNormalDistribution,
     DiscreteTruncatedNormalDistribution,
     DiscreteUniformDistribution,
     PoissonDistribution,
     UniqueKeyDistribution,
 )
-from metasyn.distribution.faker import (
+from metasyn.distribution.na import NADistribution
+from metasyn.distribution.string import (
     FakerDistribution,
     FreeTextDistribution,
+    RegexDistribution,
+    StringConstantDistribution,
     UniqueFakerDistribution,
+    UniqueRegexDistribution,
 )
-from metasyn.distribution.na import NADistribution
-from metasyn.distribution.regex import RegexDistribution, UniqueRegexDistribution
 
 __all__ = [
     "MultinoulliDistribution",
     "ExponentialDistribution",
     "LogNormalDistribution",
     "NormalDistribution",
     "TruncatedNormalDistribution",
```

### Comparing `metasyn-0.8.0/metasyn/distribution/base.py` & `metasyn-1.0.0/metasyn/distribution/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Optional, Union
 
 import numpy as np
 import polars as pl
+from numpy import Inf
 from numpy import typing as npt
 
 
 class BaseDistribution(ABC):
     """Abstract base class to define a distribution.
 
     All distributions should be derived from this class, and should implement
@@ -36,19 +37,25 @@
     :meth:`~_param_dict`,
     :meth:`~_param_schema`,
     :meth:`~default_distribution`
     and ``__init__``.
     """
 
     implements: str = "unknown"
+    """The identifier for the implemented distribution"""
     var_type: str = "unknown"
+    """The variable type of the distribution"""
     provenance: str = "builtin"
+    """Which plugin provides the distribution or builtin"""
     privacy: str = "none"
+    """The type of privacy it implements"""
     unique: bool = False
+    """Whether the distribution creates only unique values"""
     version: str = "1.0"
+    """Version of the implemented distribution"""
 
     @classmethod
     def fit(cls, series: Union[pl.Series, npt.NDArray],
             *args, **kwargs) -> BaseDistribution:
         """Fit the distribution to the series.
 
         Parameters
@@ -227,15 +234,37 @@
             cls.var_type = var_type
         if unique is not None:
             cls.unique = unique
         if privacy is not None:
             cls.privacy = privacy
         if version is not None:
             cls.version = version
+        if cls.__doc__ is None:
+            return cls
+        cls.__doc__ = cls.__doc__.rstrip(" ")
+        if not cls.__doc__.endswith("\n"):
+            cls.__doc__ += "\n"
+        cls.__doc__ += f"""
+    Attributes
+    ----------
+    implements:
+        {cls.implements}
+    unique:
+        {cls.unique}
+    version:
+        {cls.version}
+    var_type:
+        {cls.var_type}
+    privacy:
+        {cls.privacy}
+    provenance:
+        {cls.provenance}
+    """
         return cls
+
     return _wrap
 
 
 class ScipyDistribution(BaseDistribution):
     """Base class for numerical distributions using Scipy.
 
     This base class makes it easy to implement new numerical
@@ -310,16 +339,53 @@
 
     def draw_reset(self):
         self.key_set = set()
 
     def draw(self) -> object:
         n_retry = 0
         while n_retry < 1e5:
-            new_val = super().draw()
+            new_val = super().draw()  # type: ignore
             if new_val not in self.key_set:
                 self.key_set.add(new_val)
                 return new_val
             n_retry += 1
         raise ValueError(f"Failed to draw unique string after {n_retry} tries.")
 
     def information_criterion(self, values):
         return 9999999
+
+
+
+class BaseConstantDistribution(BaseDistribution):
+    """Base class for constant distribution.
+
+    This base class makes it easy to implement new constant distributions
+    for different variable types.
+    """
+
+    def __init__(self, value) -> None:
+        self.value = value
+
+    @property
+    def n_par(self) -> int:
+        """int: Number of parameters for distribution."""
+        return 0
+
+    @classmethod
+    def _fit(cls, values: pl.Series) -> BaseDistribution:
+        # if unique, just get that value
+        if values.n_unique() == 1:
+            return cls(values.unique()[0])
+
+        # otherwise get most common value
+        val = values.value_counts(sort=True)[0,0]
+        return cls(val)
+
+    def _param_dict(self):
+        return {"value": self.value}
+
+    def draw(self):
+        return self.value
+
+    def information_criterion(self, values):
+        vals = self._to_series(values)
+        return -Inf if vals.n_unique() < 2 else Inf
```

### Comparing `metasyn-0.8.0/metasyn/distribution/categorical.py` & `metasyn-1.0.0/metasyn/distribution/categorical.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 import polars as pl
 
 from metasyn.distribution.base import BaseDistribution, metadist
 
 
 @metadist(implements="core.multinoulli", var_type=["categorical", "discrete", "string"])
 class MultinoulliDistribution(BaseDistribution):
-    """Categorical distribution that stores category labels and probabilities.
+    """Categorical distribution using labels and probabilities.
 
     This class represents a multinoulli (categorical) distribution.
     It is used in cases where there are multiple potential outcomes,
     each with a specified probability. The class stores the labels for each
     category and their corresponding probabilities.
 
     Parameters
     ----------
     labels : list of str
         The labels for each category in the distribution, representing
         the possible outcomes.
     probs : list of int
         The probabilities or frequencies of each category. These will be
         normalized internally.
+
+    Examples
+    --------
+    >>> MultinoulliDistribution(labels=["a", "b", "b"], probs=[0.1, 0.3, 0.6])
+    >>> MultinoulliDistribution(labels=[1, 3, 6], probs=[0.3, 0.4, 0.3])
     """
 
     def __init__(
         self,
         labels: Union[npt.NDArray[Union[np.str_, np.int_]], list[Union[str, int]]],
         probs: Union[npt.NDArray[np.float_], list[float]]
     ):
```

### Comparing `metasyn-0.8.0/metasyn/distribution/continuous.py` & `metasyn-1.0.0/metasyn/distribution/continuous.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Module implementing continuous (floating point) distributions."""
 
 import numpy as np
 from scipy.optimize import minimize
 from scipy.stats import expon, lognorm, norm, truncnorm, uniform
 from scipy.stats._continuous_distns import FitDataError
 
-from metasyn.distribution.base import ScipyDistribution, metadist
+from metasyn.distribution.base import (
+    BaseConstantDistribution,
+    BaseDistribution,
+    ScipyDistribution,
+    metadist,
+)
 
 
 @metadist(implements="core.uniform", var_type="continuous")
 class UniformDistribution(ScipyDistribution):
     """Uniform distribution for floating point type.
 
     This class implements the uniform distribution between a minimum
@@ -17,14 +22,18 @@
 
     Parameters
     ----------
     lower: float
         Lower bound for uniform distribution.
     upper: float
         Upper bound for uniform distribution.
+
+    Examples
+    --------
+    >>> UniformDistribution(lower=-3.0, upper=10.0)
     """
 
     dist_class = uniform
 
     def __init__(self, lower: float, upper: float):
         self.par = {"lower": lower, "upper": upper}
         self.dist = uniform(loc=self.lower, scale=max(self.upper-self.lower, 1e-8))
@@ -60,17 +69,20 @@
     This class implements the normal/gaussian distribution and takes
     the average and standard deviation as initialization input.
 
     Parameters
     ----------
     mean: float
         Mean of the normal distribution.
-
     sd: float
         Standard deviation of the normal distribution.
+
+    Examples
+    --------
+    >>> NormalDistribution(mean=1.3, sd=4.5)
     """
 
     implements = "core.normal"
     dist_class = norm
 
     def __init__(self, mean: float, sd: float):
         self.par = {"mean": mean, "sd": sd}
@@ -96,14 +108,18 @@
 
     Parameters
     ----------
     mean: float
         Controls the mean of the distribution.
     sd: float
         Controls the width of the distribution.
+
+    Examples
+    --------
+    >>> LogNormalDistribution(mean=-2.0, sd=4.5)
     """
 
     dist_class = lognorm
 
     def __init__(self, mean: float, sd: float):  # pylint: disable=invalid-name
         self.par = {"mean": mean, "sd": sd}
         self.dist = lognorm(s=max(sd, 1e-8), scale=np.exp(mean))
@@ -130,22 +146,26 @@
 
 @metadist(implements="core.truncated_normal", var_type="continuous")
 class TruncatedNormalDistribution(ScipyDistribution):
     """Truncated normal distribution for floating point type.
 
     Parameters
     ----------
-    lower: float
+    lower:
         Lower bound of the truncated normal distribution.
-    upper: float
+    upper:
         Upper bound of the truncated normal distribution.
-    mean: float
+    mean:
         Mean of the non-truncated normal distribution.
-    sd: float
+    sd:
         Standard deviation of the non-truncated normal distribution.
+
+    Examples
+    --------
+    >>> TruncatedNormalDistribution(lower=1.0, upper=3.5, mean=2.3, sd=5)
     """
 
     dist_class = truncnorm
 
     def __init__(self, lower: float, upper: float,
                  mean: float, sd: float):
         self.par = {"lower": lower, "upper": upper,
@@ -192,16 +212,20 @@
     """Exponential distribution for floating point type.
 
     This class implements the exponential distribution with the rate as its
     single parameter.
 
     Parameters
     ----------
-    rate: float
+    rate:
         Rate of the exponential distribution. This is equal to 1/mean of the distribution.
+
+    Examples
+    --------
+    >>> ExponentialDistribution(rate=2.4)
     """
 
     dist_class = expon
 
     def __init__(self, rate: float):
         self.par = {"rate": rate}
         self.dist = expon(loc=0, scale=1/max(rate, 1e-8))
@@ -218,7 +242,36 @@
         return cls(1.0)
 
     @classmethod
     def _param_schema(cls):
         return {
             "rate": {"type": "number"}
         }
+
+
+
+@metadist(implements="core.constant", var_type="continuous")
+class ConstantDistribution(BaseConstantDistribution):
+    """Constant distribution for floating point type.
+
+    This class implements the constant distribution, so that it draws always
+    the same value.
+
+    Parameters
+    ----------
+    value: float
+        Value that will be returned when drawn.
+
+    Examples
+    --------
+    >>> ConstantDistribution(2.45)
+    """
+
+    @classmethod
+    def default_distribution(cls) -> BaseDistribution:
+        return cls(0.0)
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "value": {"type": "number"}
+        }
```

### Comparing `metasyn-0.8.0/metasyn/distribution/datetime.py` & `metasyn-1.0.0/metasyn/distribution/discrete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,190 +1,251 @@
-"""Module implementing distributions for date and time types."""
+"""Module implementing discrete distributions."""
 
-import datetime as dt
-from abc import abstractmethod
-from random import random
-from typing import Any, Dict
+from typing import Set
 
 import numpy as np
+from scipy.stats import poisson, randint
 
-from metasyn.distribution.base import BaseDistribution, metadist
+from metasyn.distribution.base import (
+    BaseConstantDistribution,
+    BaseDistribution,
+    ScipyDistribution,
+    metadist,
+)
+from metasyn.distribution.continuous import NormalDistribution, TruncatedNormalDistribution
+
+
+@metadist(implements="core.uniform", var_type="discrete")
+class DiscreteUniformDistribution(ScipyDistribution):
+    """Uniform discrete distribution.
 
-
-def convert_numpy_datetime(time_obj: np.datetime64) -> dt.datetime:
-    """Convert numpy datetime to python stdlib datetime.
+    It differs from the floating point uniform distribution by
+    being a discrete distribution instead.
 
     Parameters
     ----------
-    time_obj:
-        datetime to be converted.
-
-    Returns
-    -------
-    datetime.datetime:
-        Converted datetime.
+    lower: int
+        Lower bound (inclusive) of the uniform distribution.
+    upper: int
+        Upper bound (exclusive) of the uniform distribution.
+
+    Examples
+    --------
+    >>> DiscreteUniformDistribution(lower=3, upper=20)
     """
-    unix_epoch = np.datetime64(0, 's')
-    one_second = np.timedelta64(1, 's')
-    seconds_since_epoch = (time_obj - unix_epoch) / one_second
-    return dt.datetime.utcfromtimestamp(float(seconds_since_epoch))
 
+    dist_class = randint
 
-class BaseUniformDistribution(BaseDistribution):
-    """Base class for all time/date/datetime uniform distributions."""
+    def __init__(self, lower: int, upper: int):
+        self.par = {"lower": lower, "upper": upper}
+        self.dist = self.dist_class(low=lower, high=upper)
 
-    precision_possibilities = ["microseconds", "seconds", "minutes", "hours", "days"]
-
-    def __init__(self, lower: Any, upper: Any, precision: str = "microseconds"):
-        if isinstance(lower, str):
-            lower = self.fromisoformat(lower)
-        elif isinstance(lower, np.datetime64):
-            lower = convert_numpy_datetime(lower)
-        if isinstance(upper, str):
-            upper = self.fromisoformat(upper)
-        elif isinstance(upper, np.datetime64):
-            upper = convert_numpy_datetime(upper)
-        self.precision = precision
-        self.lower = self.round(lower)
-        self.upper = self.round(upper)
+    def _information_criterion(self, values):
+        return np.log(len(values))*self.n_par - 2*np.sum(self.dist.logpmf(values))
 
     @classmethod
     def _fit(cls, values):
-        return cls(values.min(), values.max(), cls._get_precision(values))
+        param = {"lower": values.min(), "upper": values.max()+1}
+        return cls(**param)
 
     @classmethod
-    def _get_precision(cls, values):
-        cur_precision = 0
-        for precision in cls.precision_possibilities[:-1]:
-            if not np.all([getattr(d, precision[:-1]) == 0 for d in values]):
-                break
-            cur_precision += 1
-        return cls.precision_possibilities[cur_precision]
-
-    def round(self, time_obj: Any) -> Any:
-        """Round down any time object with the precision.
-
-        Parameters
-        ----------
-        time_obj:
-            Object to round down.
-
-        Return
-        ------
-        obj:
-            Time/date/datetime object rounded down to the measured precision.
-        """
-        for prec in self.precision_possibilities:
-            if prec == self.precision:
-                break
-            time_obj = time_obj.replace(**{prec[:-1]: 0})
-        try:
-            time_obj = time_obj.replace(nanosecond=0)
-        except TypeError:
-            pass
-        return time_obj
-
-    def draw(self) -> dt.datetime:
-        delta = self.upper-self.lower + self.minimum_delta
-        new_time = random()*delta + self.lower
-        return self.round(new_time)
-
-    @abstractmethod
-    def fromisoformat(self, dt_obj: str):
-        """Convert string to iso format."""
-
-    @property
-    def minimum_delta(self) -> dt.timedelta:
-        """Get the minimum time delta."""
-        return dt.timedelta(**{self.precision: 1})
-
-    def information_criterion(self, values):
-        return 0.0
+    def default_distribution(cls):
+        return cls(0, 10)
 
-    def _param_dict(self):
+    @classmethod
+    def _param_schema(cls):
         return {
-            "lower": self.lower.isoformat(),
-            "upper": self.upper.isoformat(),
-            "precision": self.precision,
+            "lower": {"type": "integer"},
+            "upper": {"type": "integer"},
         }
 
+@metadist(implements="core.normal", var_type="discrete")
+class DiscreteNormalDistribution(NormalDistribution):
+    """Normal discrete distribution.
+
+    This class implements the normal/gaussian distribution and takes
+    the average and standard deviation as initialization input.
+
+    Parameters
+    ----------
+    mean: float
+        Mean of the normal distribution.
+
+    sd: float
+        Standard deviation of the normal distribution.
+
+    Examples
+    --------
+    >>> DiscreteNormalDistribution(mean=2.4, sd=1.2)
+    """
+
+    def draw(self):
+        return int(super().draw())
+
+@metadist(implements="core.truncated_normal", var_type="discrete")
+class DiscreteTruncatedNormalDistribution(TruncatedNormalDistribution):
+    """Truncated normal discrete distribution.
+
+    Parameters
+    ----------
+    lower: float
+        Lower bound of the truncated normal distribution.
+    upper: float
+        Upper bound of the truncated normal distribution.
+    mean: float
+        Mean of the non-truncated normal distribution.
+    sd: float
+        Standard deviation of the non-truncated normal distribution.
+
+    Examples
+    --------
+    >>> DiscreteTruncatedNormalDistribution(lower=1.2, upper=4.5, mean=2.3, sd=4.5)
+    """
+
+    def draw(self):
+        return int(super().draw())
+
+
+@metadist(implements="core.poisson", var_type="discrete")
+class PoissonDistribution(ScipyDistribution):
+    """Poisson distribution.
+
+    Parameters
+    ----------
+    rate:
+        Rate (mean) of the poisson distribution.
+
+    Examples
+    --------
+    >>> PoissonDistribution(rate=3.5)
+    """
+
+    dist_class = poisson
 
-@metadist(implements="core.uniform", var_type="datetime")
-class DateTimeUniformDistribution(BaseUniformDistribution):
-    """Uniform DateTime distribution."""
+    def __init__(self, rate: float):
+        self.par = {"rate": rate}
+        self.dist = self.dist_class(mu=rate)
 
-    def fromisoformat(self, dt_obj: str) -> dt.datetime:
-        return dt.datetime.fromisoformat(dt_obj)
+    def _information_criterion(self, values):
+        return np.log(len(values))*self.n_par - 2*np.sum(self.dist.logpmf(values))
+
+    @classmethod
+    def _fit(cls, values):
+        return cls(values.mean())
 
     @classmethod
     def default_distribution(cls):
-        return cls("2022-07-15T10:39:36", "2022-08-15T10:39:36", precision="seconds")
+        return cls(0.5)
 
     @classmethod
     def _param_schema(cls):
         return {
-            "lower": {"type": "string"},
-            "upper": {"type": "string"},
-            "precision": {"type": "string"},
+            "rate": {"type": "number"},
         }
 
 
-@metadist(implements="core.uniform", var_type="time")
-class TimeUniformDistribution(BaseUniformDistribution):
-    """Uniform time distribution."""
+@metadist(implements="core.unique_key", var_type="discrete", unique=True)
+class UniqueKeyDistribution(ScipyDistribution):
+    """Unique key distribution for identifiers.
 
-    def fromisoformat(self, dt_obj: str) -> dt.time:
-        return dt.time.fromisoformat(dt_obj)
+    Discrete distribution that ensures the uniqueness of the drawn values.
+
+    Parameters
+    ----------
+    lower:
+        Minimum value for the keys.
+    consecutive:
+        True if keys are consecutive and increasing, False otherwise.
+
+    Examples
+    --------
+    >>> UniqueKeyDistribution(lower=0, consecutive=True)
+    """
+
+    def __init__(self, lower: int, consecutive: bool):
+        self.par = {"lower": lower, "consecutive": consecutive}
+        self.last_key = lower - 1
+        self.key_set: Set[int] = set()
 
     @classmethod
-    def default_distribution(cls):
-        return cls("10:39:36", "18:39:36", precision="seconds")
+    def _fit(cls, values):
+        lower = values.min()
+        high = values.max() + 1
+        if len(values) == high-lower and np.all(values.to_numpy() == np.arange(lower, high)):
+            return cls(lower, True)
+        return cls(lower, False)
+
+    def draw_reset(self):
+        self.last_key = self.lower - 1
+        self.key_set = set()
 
     def draw(self):
-        dt_lower = dt.datetime.combine(dt.datetime.today(), self.lower)
-        dt_upper = dt.datetime.combine(dt.datetime.today(), self.upper)
-        delta = dt_upper-dt_lower + self.minimum_delta
-        return self.round((random()*delta + dt_lower).time())
+        if self.consecutive == 1:
+            self.last_key += 1
+            return self.last_key
+
+        while True:
+            random_number = np.random.randint(self.lower, self.lower+2*len(self.key_set)+2)
+            if random_number not in self.key_set:
+                self.key_set.add(random_number)
+                return random_number
+
+    def _information_criterion(self, values):
+        if values.min() < self.lower:
+            return 2*np.log(len(values))+999*len(values)
+
+        # If the values are not unique the fit is extremely bad.
+        if len(set(values)) != len(values):
+            return 2*np.log(len(values))+999*len(values)
+
+        lower = values.min()
+        high = values.max()+1
+
+        if self.consecutive == 1:
+            # Check if the values are truly consecutive
+            if len(values) == high-lower and np.all(values.to_numpy() == np.arange(lower, high)):
+                return 2*np.log(len(values))
+            return 2*np.log(len(values))+999*len(values)
+
+        n_choice = high - lower
+
+        # Probabilities go up like 1/n, 1/(n-1), 1/(n-2), ..., 1/2, 1
+        return (3*np.log(len(values))
+                - 2*np.sum(np.log(1/np.arange(n_choice, n_choice-len(values), -1))))
+
+    @classmethod
+    def default_distribution(cls):
+        return cls(0, False)
 
     @classmethod
     def _param_schema(cls):
         return {
-            "lower": {"type": "string"},
-            "upper": {"type": "string"},
-            "precision": {"type": "string"},
+            "lower": {"type": "integer"},
+            "consecutive": {"type": "boolean"},
         }
 
+@metadist(implements="core.constant", var_type="discrete")
+class DiscreteConstantDistribution(BaseConstantDistribution):
+    """Constant discrete distribution.
 
-@metadist(implements="core.uniform", var_type="date")
-class DateUniformDistribution(BaseUniformDistribution):
-    """Uniform date distribution."""
-
-    precision_possibilities = ["days"]
-
-    def __init__(self, lower: Any, upper: Any):
-        super().__init__(lower, upper, precision="days")
-
-    def fromisoformat(self, dt_obj: str) -> dt.date:
-        return dt.date.fromisoformat(dt_obj)
-
-    def round(self, time_obj):
-        return time_obj
+    This class implements the constant distribution, so that it draws always
+    the same value.
 
-    def _param_dict(self) -> Dict:
-        date_dict = BaseUniformDistribution._param_dict(self)
-        del date_dict["precision"]
-        return date_dict
+    Parameters
+    ----------
+    value: int
+        Value that will be returned when drawn.
 
-    @classmethod
-    def default_distribution(cls):
-        return cls("1903-07-15", "1940-07-16")
+    Examples
+    --------
+    >>> DiscreteConstantDistribution(213456)
+    """
 
     @classmethod
-    def _fit(cls, values):
-        return cls(values.min(), values.max())
+    def default_distribution(cls) -> BaseDistribution:
+        return cls(0)
 
     @classmethod
     def _param_schema(cls):
         return {
-            "lower": {"type": "string"},
-            "upper": {"type": "string"},
+            "value": {"type": "integer"}
         }
```

### Comparing `metasyn-0.8.0/metasyn/distribution/na.py` & `metasyn-1.0.0/metasyn/distribution/na.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/metaframe.py` & `metasyn-1.0.0/metasyn/metaframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 import numpy as np
 import polars as pl
 from tqdm import tqdm
 
 from metasyn.config import MetaConfig
 from metasyn.privacy import BasePrivacy
-from metasyn.util import VarSpec
 from metasyn.validation import validate_gmf_dict
 from metasyn.var import MetaVar
+from metasyn.varspec import VarSpec
 
 
 class MetaFrame():
     """Container for statistical metadata describing a dataset.
 
     This class is used to fit a MetaFrame to a Polars DataFrame, serialize and
     export the MetaFrame to a file, read a MetaFrame from a file, and create
@@ -109,14 +109,16 @@
             meta_config = MetaConfig(var_specs, dist_providers, privacy)
         if dist_providers is not None:
             meta_config.dist_providers = dist_providers  # type: ignore
         if privacy is not None:
             meta_config.privacy = privacy  # type: ignore
 
         if df is not None and not isinstance(df, pl.DataFrame):
+            if isinstance(df, (str, pathlib.Path)):
+                raise ValueError("Please provide a DataFrame as input, not a string or path.")
             df = pl.DataFrame(df)
         all_vars = []
         columns = df.columns if df is not None else []
         if df is not None:
             for col_name in tqdm(columns, disable=not progress_bar):
                 var_spec = meta_config.get(col_name)
                 var = MetaVar.fit(
```

### Comparing `metasyn-0.8.0/metasyn/privacy.py` & `metasyn-1.0.0/metasyn/privacy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Module with privacy classes to be used for creating GMF files."""
-
 from abc import ABC, abstractmethod
 from typing import Optional, Type, Union
 
 try:
     from importlib_metadata import entry_points
 except ImportError:
     from importlib.metadata import entry_points  # type: ignore
 
 from metasyn.distribution.base import BaseDistribution
+from metasyn.util import get_registry
 
 
 class BasePrivacy(ABC):
     """Abstract base class for privacy levels.
 
     This class serves as a blueprint for privacy classes. Derived classes
     should at least set the class variable `name` and implement the `to_dict`
@@ -85,11 +85,23 @@
     KeyError
         If the name of the privacy type cannot be found.
     """
     parameters = parameters if parameters is not None else {}
     for entry in entry_points(group="metasyn.privacy"):
         if name == entry.name:
             return entry.load()(**parameters)
+
+    # Handle case where the plugin is not installed or is misspelled.
+    registry = get_registry()
+    available_plugins = {key: val for key, val in registry.items() if name in val["privacy"]}
+    if len(available_plugins) > 0:
+        avail = "\n".join(f"{key}: {val['url']}" for key, val in available_plugins.items())
+        raise ImportError(f"No plugin is installed that provides '{name}' privacy. "
+                          f"Available plugins that provide '{name}' privacy:\n\n{avail}")
     privacy_names = [entry.name for entry in entry_points(group="metasyn.privacy")]
-    raise KeyError(f"Unknown privacy type with name '{name}'. "
-                    "Ensure that you have installed the privacy package."
-                    f"Available privacy names: {privacy_names}.")
+    avail = "\n".join(f"<{key}> provides: {val['privacy']}\n\t{val['url']}"
+                      for key, val in registry.items() if len(val['privacy']) > 0)
+    raise ImportError(f"Unknown privacy type with name '{name}'. "
+                       "Ensure that you have installed the correct privacy package"
+                       " (and not misspelled it).\n"
+                      f"Installed privacy types: {privacy_names}.\n\n"
+                      f"List of plugins that provide privacy:\n\n{avail}\n")
```

### Comparing `metasyn-0.8.0/metasyn/provider.py` & `metasyn-1.0.0/metasyn/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,54 +16,55 @@
     from importlib.metadata import EntryPoint, entry_points  # type: ignore
 
 import numpy as np
 import polars as pl
 
 from metasyn.distribution.base import BaseDistribution
 from metasyn.distribution.categorical import MultinoulliDistribution
-from metasyn.distribution.constant import (
-    ConstantDistribution,
-    DateConstantDistribution,
-    DateTimeConstantDistribution,
-    DiscreteConstantDistribution,
-    StringConstantDistribution,
-    TimeConstantDistribution,
-)
 from metasyn.distribution.continuous import (
+    ConstantDistribution,
     ExponentialDistribution,
     LogNormalDistribution,
     NormalDistribution,
     TruncatedNormalDistribution,
     UniformDistribution,
 )
 from metasyn.distribution.datetime import (
+    DateConstantDistribution,
+    DateTimeConstantDistribution,
     DateTimeUniformDistribution,
     DateUniformDistribution,
+    TimeConstantDistribution,
     TimeUniformDistribution,
 )
 from metasyn.distribution.discrete import (
+    DiscreteConstantDistribution,
     DiscreteNormalDistribution,
     DiscreteTruncatedNormalDistribution,
     DiscreteUniformDistribution,
     PoissonDistribution,
     UniqueKeyDistribution,
 )
-from metasyn.distribution.faker import (
+from metasyn.distribution.na import NADistribution
+from metasyn.distribution.string import (
     FakerDistribution,
     FreeTextDistribution,
+    RegexDistribution,
+    StringConstantDistribution,
     UniqueFakerDistribution,
+    UniqueRegexDistribution,
 )
-from metasyn.distribution.na import NADistribution
-from metasyn.distribution.regex import RegexDistribution, UniqueRegexDistribution
 from metasyn.privacy import BasePrivacy, BasicPrivacy
-from metasyn.util import DistributionSpec
+from metasyn.util import get_registry
+from metasyn.varspec import DistributionSpec
 
 if TYPE_CHECKING:
     from metasyn.config import VarSpec, VarSpecAccess
 
+
 class BaseDistributionProvider(ABC):
     """Base class for all distribution providers.
 
     A distribution provider is a class that provides a set of distributions
     that can be used by metasyn to generate synthetic data.
     This class acts as a base class for creating specific distribution
     providers. It also contains a list of the available distributions and
@@ -280,19 +281,23 @@
         dist_bic = [d.information_criterion(series) for d in dist_instances]
         if unique is None:
             dist_list_unq = self.get_distributions(privacy, var_type, unique=True)
             if len(dist_list_unq) > 0:
                 dist_inst_unq = [d.fit(series, **privacy.fit_kwargs) for d in dist_list_unq]
                 dist_bic_unq = [d.information_criterion(series) for d in dist_inst_unq]
                 if np.min(dist_bic_unq) < np.min(dist_bic):
-                    warnings.simplefilter("always")
                     warnings.warn(
-                        f"\nVariable {series.name} seems unique, but not set to be unique.\n"
-                        "Set the variable to be either unique or not unique to remove this "
-                         "warning.\n")
+                        f"\nVariable '{series.name}' was detected to be unique, but has not"
+                        f" explicitly been set to unique.\n"
+                        f"To generate only unique values for column '{series.name}', "
+                        f"set unique to True.\n"
+                        f"To dismiss this warning, set unique to False.",
+                        UserWarning
+                    )
+
         return dist_instances[np.argmin(dist_bic)]
 
     def find_distribution(self,  # pylint: disable=too-many-branches
                           dist_name: str,
                           var_type: str,
                           privacy: Optional[BasePrivacy] = BasicPrivacy(),
                           unique: bool = False,
@@ -320,29 +325,40 @@
             A distribution and the arguments to create an instance.
         """
         if NADistribution.matches_name(dist_name):
             return NADistribution
 
         versions_found = []
         for dist_class in self.get_distributions(
-            privacy, var_type=var_type, unique=unique) + [NADistribution]:
+                privacy, var_type=var_type, unique=unique) + [NADistribution]:
             if dist_class.matches_name(dist_name):
                 if version is None or version == dist_class.version:
                     return dist_class
                 versions_found.append(dist_class)
 
         # Look for distribution in legacy
         warnings.simplefilter("always")
         legacy_distribs = [
             dist_class
             for dist_class in self.get_distributions(privacy, use_legacy=True,
                                                      var_type=var_type, unique=unique)
             if dist_class.matches_name(dist_name)]
 
-        if len(legacy_distribs+versions_found) == 0:
+        if len(legacy_distribs + versions_found) == 0:
+            registry = get_registry()
+            available = {}
+            for plugin, meta in registry.items():
+                if dist_name in meta["distributions"]:
+                    available[plugin] = meta["url"]
+            if len(available) > 0:
+                avail_str = "\n".join("{plugin}: {url}" for plugin, url in available.items())
+                raise ValueError(f"You are trying to use a distribution named '{dist_name}', \n"
+                                 f"but it is not installed.\n"
+                                 f"\n"
+                                 f"{dist_name} is available from:\n\n{avail_str}\n")
             raise ValueError(f"Cannot find distribution with name '{dist_name}'.")
 
         if len(versions_found) == 0:
             warnings.warn("Distribution with name '{dist_name}' is deprecated and "
                           "will be removed in the future.")
 
         # Find exact matches in legacy distributions
@@ -350,33 +366,33 @@
         if version is not None and version in legacy_versions:
             warnings.warn("Version ({version}) of distribution with name '{dist_name}'"
                           " is deprecated and will be removed in the future.")
             return legacy_distribs[legacy_versions.index(version)]
 
         # If version is None, take the latest version.
         if version is None:
-            scores = [int(dist.version.split(".")[0])*100 + int(dist.version.split(".")[1])
+            scores = [int(dist.version.split(".")[0]) * 100 + int(dist.version.split(".")[1])
                       for dist in legacy_distribs]
             i_min = np.argmax(scores)
             return legacy_distribs[i_min]
 
         # Find the distribution with the same major revision, and closest minor revision.
         major_version = int(version.split(".")[0])
         minor_version = int(version.split(".")[1])
         all_dist = versions_found + legacy_distribs
         all_versions = [[int(x) for x in dist.version.split(".")] for dist in all_dist]
-        score = [int(ver[0] == major_version)*1000000 - (ver[1]-minor_version)**2
+        score = [int(ver[0] == major_version) * 1000000 - (ver[1] - minor_version) ** 2
                  for ver in all_versions]
         i_max = np.argmax(score)
 
         # Wrong major revision.
         if score[i_max] < 500000:
             raise ValueError(
                 f"Cannot find compatible version for distribution '{dist_name}', available: "
-                f"{legacy_versions+versions_found}")
+                f"{legacy_versions + versions_found}")
 
         warnings.warn("Version mismatch ({version}) versus ({all_dist[i_max].version}))")
         return all_dist[i_max]
 
     def _fit_distribution(self, series: pl.Series,
                           dist_spec: DistributionSpec,
                           var_type: str,
@@ -482,18 +498,18 @@
     }
 
 
 def _get_all_provider_list() -> list[BaseDistributionProvider]:
     return [p.load()() for p in _get_all_providers().values()]
 
 
-def get_distribution_provider(
-        provider: Union[str, type[BaseDistributionProvider],
-                        BaseDistributionProvider] = "builtin"
-        ) -> BaseDistributionProvider:
+def get_distribution_provider(provider: Union[str, type[
+                                        BaseDistributionProvider],
+                                        BaseDistributionProvider] = "builtin"
+                              ) -> BaseDistributionProvider:
     """Get a distribution tree.
 
     Parameters
     ----------
     provider:
         Name, class or class type of the provider to be used.
     kwargs:
@@ -509,8 +525,13 @@
     if isinstance(provider, type):
         return provider()
 
     all_providers = _get_all_providers()
     try:
         return all_providers[provider].load()()
     except KeyError as exc:
-        raise ValueError(f"Cannot find distribution provider with name '{provider}'.") from exc
+        registry = get_registry()
+        if provider not in registry:
+            raise ValueError(f"Cannot find distribution provider with name '{provider}'.") from exc
+        raise ValueError(f"Distribution provider '{provider}' is not installed.\n"
+                         f"See {registry['provider']['url']} for installation instructions."
+                         ) from exc
```

### Comparing `metasyn-0.8.0/metasyn/schema/generative_metadata_format.json` & `metasyn-1.0.0/metasyn/schema/generative_metadata_format.json`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/testutils.py` & `metasyn-1.0.0/metasyn/testutils.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/util.py` & `metasyn-1.0.0/metasyn/varspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-"""Utility module for metasyn.
-
-This module provides utility classes that are used across metasyn,
-including classes for specifying distributions and storing variable
-specifications.
-"""
+"""Module for distribution and variable specifications."""
 from __future__ import annotations
 
+# from metasyn.util import VarSpec
 from dataclasses import dataclass, field
 from typing import Any, Optional, Union
 
 from metasyn.distribution.base import BaseDistribution
 from metasyn.privacy import BasePrivacy, BasicPrivacy, get_privacy
```

### Comparing `metasyn-0.8.0/metasyn/validation.py` & `metasyn-1.0.0/metasyn/validation.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/metasyn/var.py` & `metasyn-1.0.0/metasyn/var.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import polars as pl
 
 from metasyn.distribution.base import BaseDistribution
 from metasyn.privacy import BasePrivacy, BasicPrivacy
 from metasyn.provider import BaseDistributionProvider, DistributionProviderList
-from metasyn.util import DistributionSpec
+from metasyn.varspec import DistributionSpec
 
 
 class MetaVar():
     """Metadata variable describing a column in a MetaFrame.
 
     MetaVar is a structure that holds all metadata needed to generate a
     synthetic column for it. This is the variable level building block for the
```

### Comparing `metasyn-0.8.0/metasyn.egg-info/PKG-INFO` & `metasyn-1.0.0/metasyn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasyn
-Version: 0.8.0
+Version: 1.0.0
 Summary: Package for creating synthetic datasets while preserving privacy.
 Author-email: Raoul Schram <r.d.schram@uu.nl>, Erik-Jan van Kesteren <e.vankesteren1@uu.nl>
 License: MIT License
         
         Copyright (c) 2024 SoDa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,19 +70,19 @@
 Requires-Dist: sphinx_copybutton; extra == "test"
 Requires-Dist: XlsxWriter; extra == "test"
 Requires-Dist: types-tqdm; extra == "test"
 Requires-Dist: types-regex; extra == "test"
 Requires-Dist: pandas; extra == "test"
 
 <p align="center">
-  <img src="docs/source/images/logos/blue.svg" width="600px" alt="Metasyn logo"></img>
+  <img src="https://github.com/sodascience/metasyn/blob/main/docs/source/images/logos/blue.svg" width="600px" alt="Metasyn logo"></img>
   <h3 align="center">Transparent and privacy-friendly synthetic data generation</h3>
   <p align="center">
     <span>
-        <a href="https://www.repostatus.org/#wip"><img src="https://www.repostatus.org/badges/latest/wip.svg" alt="Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public."/></a>
+        <a href="https://www.repostatus.org/#active"><img src="https://www.repostatus.org/badges/latest/active.svg" alt="Project Status: Active – The project has reached a stable, usable state and is being actively developed." /></a>
         <a href="https://pypi.org/project/metasyn"><img src="https://img.shields.io/pypi/pyversions/metasyn" alt="metasyn on pypi"></img></a>
         <a href="https://colab.research.google.com/github/sodascience/metasyn/blob/main/examples/getting_started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="open getting started on colab"></img></a>
         <a href="https://metasyn.readthedocs.io/en/latest/index.html"><img src="https://readthedocs.org/projects/metasyn/badge/?version=latest" alt="Readthedocs"></img></a>
         <a href="https://hub.docker.com/r/sodateam/metasyn"><img src="https://img.shields.io/docker/v/sodateam/metasyn?logo=docker&label=docker&color=blue" alt="Docker image version"></img></a>
         <a href="https://zenodo.org/doi/10.5281/zenodo.7696031"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7696031.svg" alt="DOI"></a>
     </span>
   </p>
@@ -113,15 +113,15 @@
 ```sh
 pip install git+https://github.com/sodascience/metasyn
 ```
 
 ## Usage
 To generate synthetic data, `metasyn` first needs to fit a `MetaFrame` to the data which can then be used to produce new synthetic rows:
 
-![Example input and output](docs/source/images/example_input_output_concise.png)
+![Example input and output](https://github.com/sodascience/metasyn/blob/main/docs/source/images/example_input_output_concise.png)
 
 In Python code this happens as follows:
 
 ```python
 import polars as pl
 from metasyn import MetaFrame, demo_file
 
@@ -155,27 +155,15 @@
 ## Where to go next
 
 - As a next step to learn more about generating synthetic data with metasyn we recommend to check out the [user guide](https://metasyn.readthedocs.io/en/latest/usage/usage.html).
 - For even more privacy, have a look at our [disclosure control plugin](https://github.com/sodascience/metasyn-disclosure-control).
 - To learn more about how `metasyn` works, go to detailed overview in our [documentation](https://metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). 
 - Want to create programs that build on metasyn? Take a look at our versioned [Docker containers](https://hub.docker.com/r/sodateam/metasyn) and our [CLI](https://metasyn.readthedocs.io/en/latest/usage/cli.html).
 
-
-
 ## Contributing
-Metasyn is an open-source project, and we welcome contributions from the community.
-
-To contribute to the codebase, follow these steps:
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-More information on contributing can be found in the [contributing](https://metasyn.readthedocs.io/en/latest/developer/contributing.html) section of the documentation.
-
+Metasyn is an open-source project, and we welcome contributions from the community, from bug reports & feature requests to code contributions. Read our [contributing guidelines](.github/CONTRIBUTING.md) for more information and to get started!
 
 ## Contact
 **Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)](https://odissei-data.nl/nl/soda/) team.
-Do you have questions, suggestions, or remarks on the technical implementation? File an issue in the issue tracker or feel free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://github.com/qubixes).
+Do you have questions, suggestions, or remarks on the technical implementation? Create an issue in the [issue tracker](https://github.com/sodascience/metasyn/issues) or feel free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://github.com/qubixes).
 
 <img src="docs/source/images/logos/soda.png" alt="SoDa logo" width="250px"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metasyn Version: 0.8.0 Summary: Package for
+Metadata-Version: 2.1 Name: metasyn Version: 1.0.0 Summary: Package for
 creating synthetic datasets while preserving privacy. Author-email: Raoul
 Schram
 uu.nl>, Erik-Jan van Kesteren
 uu.nl> License: MIT License Copyright (c) 2024 SoDa Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -40,17 +40,17 @@
 sphinxcontrib-napoleon; extra == "test" Requires-Dist: sphinx-autodoc-
 typehints; extra == "test" Requires-Dist: sphinx_inline_tabs; extra == "test"
 Requires-Dist: sphinx_copybutton; extra == "test" Requires-Dist: XlsxWriter;
 extra == "test" Requires-Dist: types-tqdm; extra == "test" Requires-Dist:
 types-regex; extra == "test" Requires-Dist: pandas; extra == "test"
                                 [Metasyn logo]
      ******** TTrraannssppaarreenntt aanndd pprriivvaaccyy--ffrriieennddllyy ssyynntthheettiicc ddaattaa ggeenneerraattiioonn ********
-_[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _W_I_P_ _â___ _I_n_i_t_i_a_l_ _d_e_v_e_l_o_p_m_e_n_t_ _i_s_ _i_n_ _p_r_o_g_r_e_s_s_,_ _b_u_t_ _t_h_e_r_e_ _h_a_s_ _n_o_t
- _y_e_t_ _b_e_e_n_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _r_e_l_e_a_s_e_ _s_u_i_t_a_b_l_e_ _f_o_r_ _t_h_e_ _p_u_b_l_i_c_._]_[_m_e_t_a_s_y_n_ _o_n_ _p_y_p_i_]
-    _[_o_p_e_n_ _g_e_t_t_i_n_g_ _s_t_a_r_t_e_d_ _o_n_ _c_o_l_a_b_]_[_R_e_a_d_t_h_e_d_o_c_s_]_[_D_o_c_k_e_r_ _i_m_a_g_e_ _v_e_r_s_i_o_n_]_[_D_O_I_]
+_[_P_r_o_j_e_c_t_ _S_t_a_t_u_s_:_ _A_c_t_i_v_e_ _â___ _T_h_e_ _p_r_o_j_e_c_t_ _h_a_s_ _r_e_a_c_h_e_d_ _a_ _s_t_a_b_l_e_,_ _u_s_a_b_l_e_ _s_t_a_t_e_ _a_n_d
+ _i_s_ _b_e_i_n_g_ _a_c_t_i_v_e_l_y_ _d_e_v_e_l_o_p_e_d_._]_[_m_e_t_a_s_y_n_ _o_n_ _p_y_p_i_]_[_o_p_e_n_ _g_e_t_t_i_n_g_ _s_t_a_r_t_e_d_ _o_n_ _c_o_l_a_b_]
+                   _[_R_e_a_d_t_h_e_d_o_c_s_]_[_D_o_c_k_e_r_ _i_m_a_g_e_ _v_e_r_s_i_o_n_]_[_D_O_I_]
 
 __Generate synthetic tabular data__ in a transparent, understandable, and
 privacy-friendly way. Metasyn makes it possible for owners of sensitive data to
 create test data, do open science, improve code reproducibility, encourage data
 reuse, and enhance accessibility of their datasets, without worrying about
 leaking private information. With metasyn you can __fit__ a model to an
 existing dataframe, __export__ it to a transparent and auditable `.json` file,
@@ -83,44 +83,42 @@
 metasyn.readthedocs.io/en/latest/developer/contributing.html) directly to the
 project. ## Installation Metasyn can be installed directly from PyPI using the
 following command in the terminal: ```sh pip install metasyn ``` The latest
 (possibly unstable) development version can be installed directly from GitHub
 like so: ```sh pip install git+https://github.com/sodascience/metasyn ``` ##
 Usage To generate synthetic data, `metasyn` first needs to fit a `MetaFrame` to
 the data which can then be used to produce new synthetic rows: ![Example input
-and output](docs/source/images/example_input_output_concise.png) In Python code
-this happens as follows: ```python import polars as pl from metasyn import
-MetaFrame, demo_file # Get the csv file path for built-in demo dataset csv_path
-= demo_file("fruit") # Create a polars dataframe from the csv file. # It is
-important to ensure the data types are correct # when creating your dataframe,
-especially categorical data! df = pl.read_csv(csv_path, dtypes={ "fruits":
-pl.Categorical, "cars": pl.Categorical }) # Create a MetaFrame from the
-DataFrame. mf = MetaFrame.fit_dataframe(df) # Generate a new DataFrame with 5
-rows from the MetaFrame. df_synth = mf.synthesize(5) # This DataFrame can be
-exported to csv, parquet, excel and more. df_synth.write_csv("output.csv") ```
-To explore more options and try this out online, take a look at our interactive
-tutorial: [![](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/sodascience/metasyn/blob/main/
-examples/getting_started.ipynb) For more information on how to create
-dataframes with polars, refer to the [Polars documentation](https://pola.rs/).
-Metasyn also works with pandas dataframes! ## Where to go next - As a next step
-to learn more about generating synthetic data with metasyn we recommend to
-check out the [user guide](https://metasyn.readthedocs.io/en/latest/usage/
-usage.html). - For even more privacy, have a look at our [disclosure control
-plugin](https://github.com/sodascience/metasyn-disclosure-control). - To learn
-more about how `metasyn` works, go to detailed overview in our [documentation]
-(https://metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). - Want
-to create programs that build on metasyn? Take a look at our versioned [Docker
+and output](https://github.com/sodascience/metasyn/blob/main/docs/source/
+images/example_input_output_concise.png) In Python code this happens as
+follows: ```python import polars as pl from metasyn import MetaFrame, demo_file
+# Get the csv file path for built-in demo dataset csv_path = demo_file("fruit")
+# Create a polars dataframe from the csv file. # It is important to ensure the
+data types are correct # when creating your dataframe, especially categorical
+data! df = pl.read_csv(csv_path, dtypes={ "fruits": pl.Categorical, "cars":
+pl.Categorical }) # Create a MetaFrame from the DataFrame. mf =
+MetaFrame.fit_dataframe(df) # Generate a new DataFrame with 5 rows from the
+MetaFrame. df_synth = mf.synthesize(5) # This DataFrame can be exported to csv,
+parquet, excel and more. df_synth.write_csv("output.csv") ``` To explore more
+options and try this out online, take a look at our interactive tutorial: [![]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/sodascience/metasyn/blob/main/examples/
+getting_started.ipynb) For more information on how to create dataframes with
+polars, refer to the [Polars documentation](https://pola.rs/). Metasyn also
+works with pandas dataframes! ## Where to go next - As a next step to learn
+more about generating synthetic data with metasyn we recommend to check out the
+[user guide](https://metasyn.readthedocs.io/en/latest/usage/usage.html). - For
+even more privacy, have a look at our [disclosure control plugin](https://
+github.com/sodascience/metasyn-disclosure-control). - To learn more about how
+`metasyn` works, go to detailed overview in our [documentation](https://
+metasyn.readthedocs.io/en/latest/about/metasyn_in_detail.html). - Want to
+create programs that build on metasyn? Take a look at our versioned [Docker
 containers](https://hub.docker.com/r/sodateam/metasyn) and our [CLI](https://
 metasyn.readthedocs.io/en/latest/usage/cli.html). ## Contributing Metasyn is an
-open-source project, and we welcome contributions from the community. To
-contribute to the codebase, follow these steps: 1. Fork the Project 2. Create
-your Feature Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your
-changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git
-push origin feature/AmazingFeature`) 5. Open a Pull Request More information on
-contributing can be found in the [contributing](https://metasyn.readthedocs.io/
-en/latest/developer/contributing.html) section of the documentation. ## Contact
-**Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)](https://
-odissei-data.nl/nl/soda/) team. Do you have questions, suggestions, or remarks
-on the technical implementation? File an issue in the issue tracker or feel
-free to contact [Erik-Jan van Kesteren](https://github.com/vankesteren) or
-[Raoul Schram](https://github.com/qubixes).[SoDa logo]
+open-source project, and we welcome contributions from the community, from bug
+reports & feature requests to code contributions. Read our [contributing
+guidelines](.github/CONTRIBUTING.md) for more information and to get started!
+## Contact **Metasyn** is a project by the [ODISSEI Social Data Science (SoDa)]
+(https://odissei-data.nl/nl/soda/) team. Do you have questions, suggestions, or
+remarks on the technical implementation? Create an issue in the [issue tracker]
+(https://github.com/sodascience/metasyn/issues) or feel free to contact [Erik-
+Jan van Kesteren](https://github.com/vankesteren) or [Raoul Schram](https://
+github.com/qubixes).[SoDa logo]
```

### Comparing `metasyn-0.8.0/metasyn.egg-info/SOURCES.txt` & `metasyn-1.0.0/metasyn.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 .gitignore
 .readthedocs.yaml
 CITATION.cff
 Dockerfile
 LICENSE
 README.md
 pyproject.toml
+.github/CODE_OF_CONDUCT.md
+.github/CONTRIBUTING.md
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 .github/workflows/release-dockerhub.yml
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/faq.rst
 docs/source/index.rst
+docs/source/metasyn_in_detail.rst
 docs/source/about/about.rst
 docs/source/about/contact.rst
 docs/source/about/license.rst
-docs/source/about/metasyn_in_detail.rst
+docs/source/api/developer_reference.rst
+docs/source/api/metaframe.rst
 docs/source/api/metasyn.demo.rst
 docs/source/api/metasyn.distribution.rst
 docs/source/api/metasyn.rst
-docs/source/api/metasyn.schema.rst
+docs/source/api/varspec.rst
 docs/source/developer/GMF.rst
 docs/source/developer/contributing.rst
 docs/source/developer/developer.rst
 docs/source/developer/distributions.rst
 docs/source/developer/overview.rst
 docs/source/developer/plugins.rst
 docs/source/images/ClassDiagram.drawio
@@ -59,14 +63,15 @@
 docs/source/images/logos/grey_med.png
 docs/source/images/logos/metasyn.afdesign
 docs/source/images/logos/soda.png
 docs/source/images/logos/white.png
 docs/source/images/logos/white.svg
 docs/source/images/logos/white_med.png
 docs/source/usage/cli.rst
+docs/source/usage/config_files.rst
 docs/source/usage/exporting_metaframes.rst
 docs/source/usage/extensions.rst
 docs/source/usage/generating_metaframes.rst
 docs/source/usage/generating_synthetic_data.rst
 docs/source/usage/installation.rst
 docs/source/usage/interactive_tutorials.rst
 docs/source/usage/quick_start.rst
@@ -86,38 +91,38 @@
 metasyn/privacy.py
 metasyn/provider.py
 metasyn/py.typed
 metasyn/testutils.py
 metasyn/util.py
 metasyn/validation.py
 metasyn/var.py
+metasyn/varspec.py
 metasyn.egg-info/PKG-INFO
 metasyn.egg-info/SOURCES.txt
 metasyn.egg-info/dependency_links.txt
 metasyn.egg-info/entry_points.txt
 metasyn.egg-info/requires.txt
 metasyn.egg-info/top_level.txt
 metasyn/demo/__init__.py
 metasyn/demo/dataset.py
 metasyn/demo/demo_fruit.csv
 metasyn/demo/demo_spaceship.csv
 metasyn/demo/demo_titanic.csv
 metasyn/distribution/__init__.py
 metasyn/distribution/base.py
 metasyn/distribution/categorical.py
-metasyn/distribution/constant.py
 metasyn/distribution/continuous.py
 metasyn/distribution/datetime.py
 metasyn/distribution/discrete.py
-metasyn/distribution/faker.py
 metasyn/distribution/na.py
-metasyn/distribution/regex.py
+metasyn/distribution/string.py
 metasyn/distribution/legacy/__init__.py
 metasyn/schema/__init__.py
 metasyn/schema/generative_metadata_format.json
+metasyn/schema/plugin_registry.toml
 tests/test_builtin.py
 tests/test_cli.py
 tests/test_config.py
 tests/test_continuous.py
 tests/test_dataset.py
 tests/test_datetime.py
 tests/test_demo.py
```

### Comparing `metasyn-0.8.0/pyproject.toml` & `metasyn-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/data/example_config.toml` & `metasyn-1.0.0/tests/data/example_config.toml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/data/no_data_config.toml` & `metasyn-1.0.0/tests/data/no_data_config.toml`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/data/titanic.csv` & `metasyn-1.0.0/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_builtin.py` & `metasyn-1.0.0/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_cli.py` & `metasyn-1.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_config.py` & `metasyn-1.0.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pytest
 from pytest import mark
 
 from metasyn.config import MetaConfig, VarSpecAccess
 from metasyn.distribution import UniformDistribution
 from metasyn.privacy import BasePrivacy
-from metasyn.util import DistributionSpec, VarSpec
+from metasyn.varspec import DistributionSpec, VarSpec
 
 
 @mark.parametrize(
     "input,error",
     [
         ("uniform", False),
         (None, False),
```

### Comparing `metasyn-0.8.0/tests/test_continuous.py` & `metasyn-1.0.0/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_dataset.py` & `metasyn-1.0.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_datetime.py` & `metasyn-1.0.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_demo.py` & `metasyn-1.0.0/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_discrete.py` & `metasyn-1.0.0/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_distribution.py` & `metasyn-1.0.0/tests/test_distribution.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from pytest import mark, raises
 
 from metasyn.distribution.categorical import MultinoulliDistribution
 from metasyn.distribution.continuous import NormalDistribution, UniformDistribution
 from metasyn.distribution.discrete import DiscreteNormalDistribution, DiscreteUniformDistribution
-from metasyn.distribution.faker import FakerDistribution
-from metasyn.distribution.regex import RegexDistribution, UniqueRegexDistribution
+from metasyn.distribution.string import (
+    FakerDistribution,
+    RegexDistribution,
+    UniqueRegexDistribution,
+)
 from metasyn.provider import DistributionProviderList
 
 
 @mark.parametrize(
     "dist_str,var_type,is_unique,dist",
     [
         ("multinoulli", "string", False, MultinoulliDistribution),
```

### Comparing `metasyn-0.8.0/tests/test_faker.py` & `metasyn-1.0.0/tests/test_faker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import polars as pl
 from pytest import mark
 
-from metasyn.distribution.faker import FakerDistribution, FreeTextDistribution
+from metasyn.distribution.string import FakerDistribution, FreeTextDistribution
 
 
 @mark.parametrize("series_type", [pd.Series, pl.Series])
 def test_faker(series_type):
     var = FakerDistribution.fit(series_type([1, 2, 3]))
     assert isinstance(var.to_dict(), dict)
     assert isinstance(var.draw(), str)
```

### Comparing `metasyn-0.8.0/tests/test_provider.py` & `metasyn-1.0.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `metasyn-0.8.0/tests/test_var.py` & `metasyn-1.0.0/tests/test_var.py`

 * *Files identical despite different names*

