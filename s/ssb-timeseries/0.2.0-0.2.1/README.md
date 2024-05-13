# Comparing `tmp/ssb_timeseries-0.2.0.tar.gz` & `tmp/ssb_timeseries-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_timeseries-0.2.0.tar", max compression
+gzip compressed data, was "ssb_timeseries-0.2.1.tar", max compression
```

## Comparing `ssb_timeseries-0.2.0.tar` & `ssb_timeseries-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1073 2024-05-03 12:43:57.924512 ssb_timeseries-0.2.0/LICENSE
--rw-r--r--   0        0        0    10381 2024-05-03 12:43:57.924512 ssb_timeseries-0.2.0/README.md
--rw-r--r--   0        0        0     4376 2024-05-03 12:44:10.172721 ssb_timeseries-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      452 2024-05-03 12:43:57.924512 ssb_timeseries-0.2.0/src/ssb_timeseries/__init__.py
--rw-r--r--   0        0        0      739 2024-05-03 12:43:57.924512 ssb_timeseries-0.2.0/src/ssb_timeseries/__main__.py
--rw-r--r--   0        0        0     7659 2024-05-03 12:43:57.924512 ssb_timeseries-0.2.0/src/ssb_timeseries/config.py
--rw-r--r--   0        0        0    33757 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/dataset.py
--rw-r--r--   0        0        0     5774 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/dates.py
--rw-r--r--   0        0        0     9990 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/fs.py
--rw-r--r--   0        0        0      992 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/functions.py
--rw-r--r--   0        0        0    15607 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/io.py
--rw-r--r--   0        0        0     4242 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/logging.py
--rw-r--r--   0        0        0    10230 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/meta.py
--rw-r--r--   0        0        0     5667 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/properties.py
--rw-r--r--   0        0        0        0 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/py.typed
--rw-r--r--   0        0        0     5241 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/sample_data.py
--rw-r--r--   0        0        0     1203 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/sample_metadata.py
--rw-r--r--   0        0        0     1451 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/setup.py
--rw-r--r--   0        0        0      411 2024-05-03 12:43:57.928512 ssb_timeseries-0.2.0/src/ssb_timeseries/types.py
--rw-r--r--   0        0        0    11723 1970-01-01 00:00:00.000000 ssb_timeseries-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-13 13:03:04.285199 ssb_timeseries-0.2.1/LICENSE
+-rw-r--r--   0        0        0    10072 2024-05-13 13:03:04.285199 ssb_timeseries-0.2.1/README.md
+-rw-r--r--   0        0        0     4486 2024-05-13 13:03:13.921200 ssb_timeseries-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      452 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/__main__.py
+-rw-r--r--   0        0        0     7659 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/config.py
+-rw-r--r--   0        0        0    37857 2024-05-13 13:03:13.925200 ssb_timeseries-0.2.1/src/ssb_timeseries/dataset.py
+-rw-r--r--   0        0        0     8028 2024-05-13 13:03:13.925200 ssb_timeseries-0.2.1/src/ssb_timeseries/dates.py
+-rw-r--r--   0        0        0     9990 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/fs.py
+-rw-r--r--   0        0        0    16512 2024-05-13 13:03:13.925200 ssb_timeseries-0.2.1/src/ssb_timeseries/io.py
+-rw-r--r--   0        0        0     4242 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/logging.py
+-rw-r--r--   0        0        0    11842 2024-05-13 13:03:13.925200 ssb_timeseries-0.2.1/src/ssb_timeseries/meta.py
+-rw-r--r--   0        0        0     5963 2024-05-13 13:03:13.925200 ssb_timeseries-0.2.1/src/ssb_timeseries/properties.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/py.typed
+-rw-r--r--   0        0        0     5786 2024-05-13 13:03:13.925200 ssb_timeseries-0.2.1/src/ssb_timeseries/sample_data.py
+-rw-r--r--   0        0        0     1203 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/sample_metadata.py
+-rw-r--r--   0        0        0     1451 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/setup.py
+-rw-r--r--   0        0        0      411 2024-05-13 13:03:04.289199 ssb_timeseries-0.2.1/src/ssb_timeseries/types.py
+-rw-r--r--   0        0        0    11197 1970-01-01 00:00:00.000000 ssb_timeseries-0.2.1/PKG-INFO
```

### Comparing `ssb_timeseries-0.2.0/LICENSE` & `ssb_timeseries-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/README.md` & `ssb_timeseries-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,132 +14,124 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)][poetry]
 
 [pypi status]: https://pypi.org/project/ssb-timeseries/
 [documentation]: https://statisticsnorway.github.io/ssb-timeseries
 [tests]: https://github.com/statisticsnorway/ssb-timeseries/actions?workflow=Tests
-
 [sonarcov]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [sonarquality]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 [poetry]: https://python-poetry.org/
 
 ## Background
 
 Statistics Norway is building a new procuction system in the cloud.
 
 Moving towards modern architecture, development methodology and open source technologies: Python and R are replacing SAS for statistics production code. Oracle databases and ODI for ETL are being replaced by a data lake architecture relying heavily on Parquet files.
 
-Another big issue has been time series.Time series are essential to statistics production, so  the decision to phase out FAME while not having landed precisely what should replace it has left a huge gap.
+Another big issue has been time series.Time series are essential to statistics production, so the decision to phase out FAME while not having landed precisely what should replace it has left a huge gap.
 
 A complete solution will touch several areas of functionality:
 
- * The core is storage with performant read and write, search and filtering
- * Good descriptive metadata is key to findability
- * A wide selection of math and statistics libraries is key for calculations and models
- * Visualisation tools play a role both in ad hoc and routine inspection and quality control
- * Workflow integration with automation and process monitoring help keeping consistent quality
- * Data lineage and process metadata is essential for quality control
+- The core is storage with performant read and write, search and filtering
+- Good descriptive metadata is key to findability
+- A wide selection of math and statistics libraries is key for calculations and models
+- Visualisation tools play a role both in ad hoc and routine inspection and quality control
+- Workflow integration with automation and process monitoring help keeping consistent quality
+- Data lineage and process metadata is essential for quality control
 
- In Statistics Norway strict requirements for transparency and data quality are mandated by law and  commitment to international standards. The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are some times significant, they are far from extreme. This shifts the focus from performance towards process and data control.
+In Statistics Norway strict requirements for transparency and data quality are mandated by law and commitment to international standards. The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are some times significant, they are far from extreme. This shifts the focus from performance towards process and data control.
 
 This project came out of a PoC to demonstrate how the key functionality may be provided with the core technologies Python and Parquet, in alignment with architecture decisions and process model requirements. Constructed to be an abstraction between the storage layer and the statistics production code, it provides a way forward while postponing some the technical choices.
 
- * Basic functionality for read/write, calculations, time aggregation and plotting was demonstrated December 2023.
- * Persisting snapshots in alignment with the process model, simple descriptive tagging and integrations with GCS buckets was added Q1 2024.
+- Basic functionality for read/write, calculations, time aggregation and plotting was demonstrated December 2023.
+- Persisting snapshots in alignment with the process model, simple descriptive tagging and integrations with GCS buckets was added Q1 2024.
 
 ## How to get started?
 
 See notebook files and tests, `demo.ipynb` and `tests/test_*.py` for examples of usage, and what works and in some cases what does not.
 
 Note that
- * The library is constructed to be platform independent, but top priority is making it work in  a Linux environment.
-* Install by way of `poetry add ssb_timeseries`.
-* The library should work out of the box with default settings. Note that the defaults are for local testing, ie not be suitable for the production setting.
-* To apply custom settings: The environment variable TIMESERIES_CONFIG should point to a JSON file with configurations.
-* The command `poetry run timeseries-config <...>` can be run from a terminal in order to shift between defauls.
- * Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the Jupyter environment (or the equivalent running elsewhere.
-* The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`.
-* With the environment variable set and the configuration in place `poetry run pytest` should succeed.
 
+- The library is constructed to be platform independent, but top priority is making it work in a Linux environment.
+- Install by way of `poetry add ssb_timeseries`.
+- The library should work out of the box with default settings. Note that the defaults are for local testing, ie not be suitable for the production setting.
+- To apply custom settings: The environment variable TIMESERIES_CONFIG should point to a JSON file with configurations.
+- The command `poetry run timeseries-config <...>` can be run from a terminal in order to shift between defauls.
+- Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the Jupyter environment (or the equivalent running elsewhere.
+- The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`.
+- With the environment variable set and the configuration in place `poetry run pytest` should succeed.
 
 While the library is in a workable state and should work both locally and in JupyterLab, it is still in an exploratory phase. There is a risk that fundamental choices are reversed and breaking changes introduced.
 
 With that disclaimer, feel free to explore and experiment, and do not be shy about asking questions or giving feedback. At this stage, feedback is all important.
 
 Assuming you have Python working with a standard SSB setup for git and poetry etc, the following should get you going:
 
-``` bash
+```bash
 # Get the poc package
 git clone https://github.com/statisticsnorway/arkitektur-poc-tidsserier.git
 
 # Run inside a poetry controlled venv:
 poetry shell
 ## Create default config
 poetry run timeseries-config home
 # Run the tests to check that everything is OK:
 poetry run pytest
 # A couple of the test cases *are expected* fail when running for the first time in a new location.
 # They should create the structures they need and should succeed in subsequent runs.
 ```
-~~ No longer needed:~~
-~~ Create and set a location for data and log files. This could be anywhere, but separated from the code is preferrable.~~
-~~ mkdir series~~
-~~ export TIMESERIES_ROOT=${PWD}/series ~~
-~~ export LOG_LOCATION=${PWD}/series ~~
-
 
 ## Functionality overview
 
 The core of the library is the Dataset class. This is essentially a wrapper around a DataFrame (for now Pandas, later probably Polars) in the .data attribute.
 
-The .data attribute should comply to conventions implied by the underlying *information model*. These will start out as pure conventions and subject to evalutation. At a later stage they are likely to be enforced by Parquet schemas. Failing to obey them will cause some methods to fail.
+The .data attribute should comply to conventions implied by the underlying _information model_. These will start out as pure conventions and subject to evalutation. At a later stage they are likely to be enforced by Parquet schemas. Failing to obey them will cause some methods to fail.
 
-The Dataset.io attribute connects the dataset to a helper class that takes care of reading and writing data. This structure abstracts away the IO mechanics, so that the user do not need to know about the "physical" details, only the *information model meaning* of the choices made.
+The Dataset.io attribute connects the dataset to a helper class that takes care of reading and writing data. This structure abstracts away the IO mechanics, so that the user do not need to know about the "physical" details, only the _information model meaning_ of the choices made.
 
- * Read and write for both versioned and unversioned data types.
- * Search for sets by name, regex and (planned for later) metadata.
- * Basic filtering of sets (selecting series within a selected set).
- * Basic linear algebra: Datasets can be added, subtracted, multiplied and divided with each other and dataframes, matrices, vectors (untested) and scalars according to normal rules.
- * Basic plotting: Dataset.plot() as shorthand for Dataset.data.plot(<and sensible defaults>).
- * Basic time aggregation:
- `Dataset.groupby(<frequency>, 'sum'|'mean'|'auto')`
- *
-
-
- ## The information model
-
- ### TLDR
-
- * **Types** are defined by
-  * **Versioning** defines how updated versions of the truth are represented: NONE overwrites a single version, NAMED or AS_OF maintaines new "logical" versions identified by name or date.
-  * **Temporality** describes the "real world" valid_at or valid_from - valid_to datetime of the data. It will translate into columns, datetime or period indexes of Dataset.data.
-  * Value type (only scalars for now) of Dataset.data "cells".
-* **Datasets** can consists of multiple series. (Later: possible extension with sets of sets.)
-* All series in a set must be of the same type.
-* **Series** are value columns in Datasets.data, rows identified by date(s) or index corresponding temporality.
-* The combination `<Dataset.name>.<Series.name>` will serve as a globally unique series identifier.
-* `<Dataset.name>` identifies a "directory", hence must be unique. (Caveat: Directories per type creates room for error.)
-* `<Series.name>` (.data column name) must be unique within the set.
-* Series names *should* be related to (preferrably constructed from) codes or meta data in such a way that they can be mapped to "tags" via a format mask (and if needed a translation table).
+- Read and write for both versioned and unversioned data types.
+- Search for sets by name, regex and (planned for later) metadata.
+- Basic filtering of sets (selecting series within a selected set).
+- Basic linear algebra: Datasets can be added, subtracted, multiplied and divided with each other and dataframes, matrices, vectors (untested) and scalars according to normal rules.
+- Basic plotting: Dataset.plot() as shorthand for Dataset.data.plot(<and sensible defaults>).
+- Basic time aggregation:
+  `Dataset.groupby(<frequency>, 'sum'|'mean'|'auto')`
+
+## The information model
+
+### TLDR
+
+- **Types** are defined by
+- **Versioning** defines how updated versions of the truth are represented: NONE overwrites a single version, NAMED or AS_OF maintaines new "logical" versions identified by name or date.
+- **Temporality** describes the "real world" valid_at or valid_from - valid_to datetime of the data. It will translate into columns, datetime or period indexes of Dataset.data.
+- Value type (only scalars for now) of Dataset.data "cells".
+- **Datasets** can consists of multiple series. (Later: possible extension with sets of sets.)
+- All series in a set must be of the same type.
+- **Series** are value columns in Datasets.data, rows identified by date(s) or index corresponding temporality.
+- The combination `<Dataset.name>.<Series.name>` will serve as a globally unique series identifier.
+- `<Dataset.name>` identifies a "directory", hence must be unique. (Caveat: Directories per type creates room for error.)
+- `<Series.name>` (.data column name) must be unique within the set.
+- Series names _should_ be related to (preferrably constructed from) codes or meta data in such a way that they can be mapped to "tags" via a format mask (and if needed a translation table).
 
-Yes, that *was* the short version. The long version is still pending production.
+Yes, that _was_ the short version. The long version is still pending production.
 
 To be continued ...
 
-### How to contribute
+### Other sources of documentation:
 
-More information about this will come later, but contributions are welcome. If you want to contribute, just let us know.
+- https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3581313026/Statistikkproduksjon
+- https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3595665419/Lagring+av+tidsserier
 
-### Other sources of documentation:
+## API-documentation
 
-* https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3581313026/Statistikkproduksjon
-* https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3595665419/Lagring+av+tidsserier
+The [documentation] is published on GitHub Pages. Se the Reference page for
+API-documentation.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `ssb_timeseries-0.2.0/pyproject.toml` & `ssb_timeseries-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 [tool.poetry]
 name = "ssb-timeseries"
-version = "0.2.0"
+version = "0.2.1"
 description = "SSB Timeseries"
 authors = ["Bernhard Ryeng <bernhard.ryeng@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-timeseries"
 repository = "https://github.com/statisticsnorway/ssb-timeseries"
 documentation = "https://statisticsnorway.github.io/ssb-timeseries"
 classifiers = ["Development Status :: 4 - Beta"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-timeseries/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.13"
+python = ">=3.10,<4.0"
 dapla-toolbelt = ">=1.3.2"
-pandas = "^2.1.1"
-pytest = "^7.4.3"
-ssb-klass-python = "^0.0.7"
-pyarrow = "^14.0.0"
-google-cloud-logging = "^3.8.0"
-pytz = "^2023.3.post1"
-polars = "^0.19.18"
-duckdb = "^0.10.0"
-bigtree = "^0.17.0"
-click = "^8.1.7"
-typing-extensions = "^4.11.0"
+pandas = ">=2.1.1"
+ssb-klass-python = ">=0.0.7"
+pyarrow = ">=14.0.0"
+bigtree = ">=0.17.0"
+typing-extensions = ">=4.11.0"
+python-dateutil = ">=2.9.0.post0"
+numpy = ">=1.26.4"
 
 [tool.poetry.group.dev.dependencies]
 pygments = ">=2.10.0"
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
 furo = ">=2021.11.12"
@@ -42,14 +38,16 @@
 sphinx = ">=6.2.1"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-autodoc-typehints = ">=1.24.0"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = { extras = ["colors"], version = ">=0.15.10" }
 myst-parser = { version = ">=0.16.1" }
+deptry = ">=0.16.1"
+click = ">=8.1.7"
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 
 [tool.poetry.scripts]
 ssb-timeseries = "ssb_timeseries.__main__:main"
 timeseries-config = "ssb_timeseries.config:main"
@@ -69,14 +67,15 @@
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_context = true
+disallow_any_generics = false
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
 target-version = "py310"  # Minimum Python version supported
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
@@ -137,10 +136,13 @@
     "D100",    # docstrings are overkill for test functions
     "D101",
     "D102",
     "D103",
     "S101",    # asserts are encouraged in pytest
 ]
 
+[tool.deptry.per_rule_ignores]
+DEP001 = ["ssb_timeseries", "nox", "nox_poetry"]  # packages available by default
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/__main__.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/__main__.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/config.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/config.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/dataset.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# mypy: disable-error-code="assignment"
+# mypy: disable-error-code="assignment,attr-defined"
 # ruff: noqa: RUF013
 from copy import deepcopy
 from datetime import datetime
 from typing import Any
 from typing import no_type_check
 
 import numpy as np
-import pandas as pd  # type: ignore[import-untyped]
+import pandas as pd
 from typing_extensions import Self
 
 from ssb_timeseries import io
 from ssb_timeseries import properties
 from ssb_timeseries.dates import date_utc  # type: ignore[attr-defined]
 from ssb_timeseries.dates import utc_iso  # type: ignore[attr-defined]
 from ssb_timeseries.logging import ts_logger
+from ssb_timeseries.meta import Taxonomy
 from ssb_timeseries.types import F
+from ssb_timeseries.types import PathStr
 
 
 class Dataset:
     """Datasets are the core unit of analysis for workflow and data storage.
 
     A dataset is a logical collection of data and metadata stemming from the same process origin. Series in a dataset must be
     """
@@ -55,21 +57,24 @@
         self.name: str = name
         if data_type:  # self.exists():
             self.data_type = data_type
         else:
             # TODO: if the datatype is not provided, search by name,
             # throw error if a) no set is found or b) multiple sets are found
             # ... till then, just continue
-            self.data_type = data_type
-
-        # TODO: for versioned series, return latest if no as_of_tz is provided
+            look_for_it = search(name)
+            if isinstance(look_for_it, Dataset):
+                self.data_type = look_for_it.data_type
+            else:
+                raise ValueError(
+                    f"Dataset {name} not found. Specify data_type to initialise a new set."
+                )
+                # TODO: for versioned series, return latest if no as_of_tz is provided
         self.as_of_utc = date_utc(as_of_tz)
 
-        # self.series: dict = kwargs.get("series", {})
-
         self.io = io.FileSystem(
             set_name=self.name, set_type=self.data_type, as_of_utc=self.as_of_utc
         )
 
         # metadata: defaults overwritten by stored overwritten by kwargs
         default_tags = {
             "name": name,
@@ -139,17 +144,14 @@
             if name_pattern:
                 for s in self.tags["series"]:
                     name_parts = s.split("_")
                     # [self.tags['series'][s][attribute] = value for attribute,  value in zip(name_pattern, name_parts)]
                     for attribute, value in zip(name_pattern, name_parts, strict=False):
                         self.tags["series"][s][attribute] = value
 
-                    ts_logger.debug(
-                        f"DATASET {self.name}: series {s} {self.tags['series'][s]} "
-                    )
                     # [self.tags.series[k] = for k, a in zip(self.numeric_columns(), name_pattern]
 
         self.product: str = kwargs.get("product", "")
         self.process_stage: str = kwargs.get("process_stage", "")
         self.sharing: dict[str, str] = kwargs.get("sharing", {})
 
     def copy(self, new_name: str, **kwargs: Any) -> Self:
@@ -285,18 +287,15 @@
         else:
             raise ValueError("Must provide either tags or kwargs.")
         # should handle different datatypes for "item" :
         # name, int index, List of name or index
         # if value not in self.series[item][attribute]:
         #    self.series[attribute].append(value)
 
-    def search(self, pattern: str = "*") -> list[str]:
-        """Search for datasets by name matching pattern."""
-        return self.io.search(pattern=pattern)
-
+    @no_type_check
     def filter(
         self,
         pattern: str = "",
         tags: dict[Any, Any] = None,
         regex: str = "",
         output: str = "dataset",
         new_name: str = "",
@@ -326,17 +325,15 @@
 
         if pattern:
             df = self.data.filter(like=pattern).copy(deep=True)
             matching_series = df.columns
 
         if tags:
             series_tags = self.series_tags()
-            ts_logger.debug(
-                f"DATASET.filter()\ntags to find:\n\t{tags}\ntags in series:\n\t{series_tags}"
-            )
+            # ts_logger.debug(f"DATASET.filter()\ntags to find:\n\t{tags}\ntags in series:\n\t{series_tags}")
             matching_series = [
                 name
                 for name, s_tags in series_tags.items()
                 if all(s_tags[k] in v for k, v in tags.items())
             ]
             ts_logger.debug(f"DATASET.filter(tags) matched series:\n{matching_series} ")
             df = self.data[matching_series].copy(deep=True)
@@ -357,54 +354,62 @@
                 out = self.copy(new_name=new_name, data=df, **kwargs)
                 matching_series_tags = {
                     k: v for k, v in out.tags["series"].items() if k in matching_series
                 }
                 out.tags["series"] = matching_series_tags
         return out
 
+    @no_type_check
     def __getitem__(
         self, criteria: str | dict[str, str] = "", **kwargs: Any
     ) -> Self | None:
         """Access Dataset.data.columns via Dataset[ list[column_names] | pattern | tags].
 
         Arguments:
-            criteria: (str | dict) Either a string pattern or a dict of tags.
+            criteria:  Either a string pattern or a dict of tags.
             kwargs: If criteria is empty, this is passed to filter().
 
         Returns:
             Self | None
+
+        Raises:
+            TypeError: If filter() returns another type than Dataset.
         """
         # pattern: str = "", regex: str = "", tags: dict = {}):
         # Dataset[...] should return a Dataset object (?) with only the requested items (columns).
         # but should not mutate the original object, ie "self",
         # so that if x is a Dataset and x[a] a columnwise subset of x
         # x[a] *= 100 should update x[a] "inside" the original x, without "setting" x to z[a]
         # that later references to x should return the entire x, not only x[a].
         # Is this possible, or do we need to return a copy?
         # (Then the original x is not affected by updates to x[a])?
         # Or, is there a trick using dataframe views?
         # --->
         if criteria and isinstance(criteria, str):
-            return self.filter(pattern=criteria)
+            result = self.filter(pattern=criteria)
         elif criteria and isinstance(criteria, dict):
-            return self.filter(tags=criteria)
+            result = self.filter(tags=criteria)
         elif kwargs:
             ts_logger.debug(f"DATASET.__getitem__(:\n\t{kwargs} ")
-            return self.filter(**kwargs)
+            result = self.filter(**kwargs)
         else:
             return None
+        if isinstance(result, Dataset):
+            return result
+        else:
+            raise TypeError("Dataset.filter() did not return a Dataset type.")
 
     def plot(self, *args: Any, **kwargs: Any) -> Any:
         """Plot dataset data.
 
         Convenience wrapper around Dataframe.plot() with sensible defaults.
         """
-        xlabels = self.datetime_columns()[0]
+        xlabels = self.datetime_columns()
         ts_logger.debug(f"Dataset.plot({args!r}, {kwargs!r}) x-labels {xlabels}")
-        return self.data.plot(
+        return self.data.plot(  # type: ignore[call-overload]
             xlabels,
             *args,
             legend=len(self.data.columns) < 9,
             title=self.name,
             figsize=(12, 4),
             **kwargs,
         )
@@ -448,36 +453,41 @@
         ts_logger.warning(f"DATASET {self.name}: datetime columns: {datetime_columns}.")
 
         # works for datetime_columns = "valid_at", untested for others
         # TODO: add support for ["valid_from", "valid_to"]
         period_index = pd.PeriodIndex(self.data[datetime_columns[0]], freq=freq)
         ts_logger.debug(f"DATASET {self.name}: period index\n{period_index}.")
 
+        # Fix for case when **kwargs contains numeric_only
+        if "numeric_only" in kwargs:
+            kwargs.pop("numeric_only")
+        numeric_only_value = True
+
         match func:
             case "mean":
-                out = self.data.groupby(period_index).mean(
-                    *args, numeric_only=True, **kwargs
+                out = self.data.groupby(period_index).mean(  # type: ignore[misc]
+                    *args, numeric_only=numeric_only_value, **kwargs
                 )
             case "sum":
-                out = self.data.groupby(period_index).sum(
-                    *args, numeric_only=True, **kwargs
+                out = self.data.groupby(period_index).sum(  # type: ignore[misc]
+                    *args, numeric_only=numeric_only_value, **kwargs
                 )
             case "auto":
                 # TODO: QA on exact logic / use "real" metadata
                 # in particular, how to check meta data and blend d1 and df2 values as appropriate
                 # (this implementation is just to show how it can be done)
                 # QUESTION: do we need a default for "other" series / what should it be?
-                df1 = self.data.groupby(period_index).mean(
-                    *args, numeric_only=True, **kwargs
+                df1 = self.data.groupby(period_index).mean(  # type: ignore[misc]
+                    *args, numeric_only=numeric_only_value, **kwargs
                 )
                 ts_logger.debug(f"groupby\n{df1}.")
 
                 df2 = (
                     self.data.groupby(period_index)
-                    .sum(*args, numeric_only=True, **kwargs)
+                    .sum(*args, numeric_only=numeric_only_value, **kwargs)  # type: ignore[misc]
                     .filter(regex="mendgde|volum|vekt")
                 )
                 ts_logger.warning(f"groupby\n{df2}.")
 
                 df1[df2.columns] = df2[df2.columns]
 
                 out = df1
@@ -771,16 +781,74 @@
                 "data_type": str(self.data_type),
                 "as_of_utc": self.as_of_utc,
                 "series": str(self.series),
                 "data": self.data.size,
             }
         )
 
-    # unfinished business
+    def aggregate(
+        self,
+        attribute: str,
+        taxonomy: Taxonomy | int | PathStr,
+        aggregate_type: str | list[str] = "sum",
+    ) -> Self:
+        """Aggregate dataset by taxonomy.
 
+        Args:
+            attribute: The attribute to aggregate by.
+            taxonomy (Taxonomy | int | PathStr): The values for `attribute`. A taxonomy object as returned by Taxonomy(klass_id_or_path), or the id or path to retrieve one.
+            aggregate_type (str | list[str]): Optional function name (or list) of the function names to apply (mean | count | sum | ...). Defaults to `sum`.
+
+        Returns:
+            Self: A dataset object with the aggregated data.
+            If the taxonomy object has hierarchical structure, aggregate series are calculated for parent nodes at all levels.
+            If the taxonomy is a flat list, only a single 'total' aggregate series is calculated.
+
+        Raises:
+            NotImplementedError: If the aggregation method is not implemented yet. --> TODO!
+        """
+        if isinstance(taxonomy, Taxonomy):
+            pass
+        else:
+            taxonomy = Taxonomy(taxonomy)
+
+        # TODO: alter to handle list of functions, eg ["mean", "10 percentile", "25 percentile", "median", "75 percentile", "90 percentile"]
+        if isinstance(aggregate_type, str):
+            match aggregate_type.lower():
+                case "mean" | "average":
+                    raise NotImplementedError(
+                        "Aggregation method 'mean' is not implemented yet."
+                    )
+                case "percentile":
+                    raise NotImplementedError(
+                        "Aggregation method 'percentile' is not implemented yet."
+                    )
+                case "count":
+                    raise NotImplementedError(
+                        "Aggregation method 'count' is not implemented yet."
+                    )
+                case "sum" | _:
+                    df = self.data.copy().drop(columns=self.numeric_columns())
+                    for node in taxonomy.parent_nodes():
+                        leaf_node_subset = self.filter(
+                            tags={attribute: taxonomy.leaf_nodes()}, output="df"
+                        ).drop(columns=self.datetime_columns())
+                        df[node.name] = leaf_node_subset.sum(axis=1)
+                        ts_logger.debug(
+                            f"DATASET.aggregate(): For node '{node.name}', column {aggregate_type} for input df:\n{leaf_node_subset}\nreturned:\n{df}"
+                        )
+                        new_col_name = node.name
+                        df = df.rename(columns={node: new_col_name})
+        else:
+            raise NotImplementedError(
+                "Multiple aggregation methods is planned, but not yet implemented."
+            )
+        return self.copy(f"{self.name}.{aggregate_type}", data=df)
+
+    # unfinished business
     # mypy: disable-error-code="no-untyped-def"
     @no_type_check
     def reindex(
         self,
         index_type: str = "dt",
         freq: str = "",
         *args,  # noqa: ANN002
@@ -790,7 +858,26 @@
             case "dt" | "datetime":
                 self.data = self.data.set_index(self.datetime_columns(), *args)
             case "p" | "period":
                 p = pd.PeriodIndex(self.data[self.datetime_columns], freq=freq)
                 self.data.reindex(p)
             case _:
                 self.data = self.data.set_index(self.datetime_columns(), *args)
+
+
+def search(
+    pattern: str = "*", as_of_tz: datetime = None
+) -> list[io.SearchResult] | Dataset | list[None]:
+    """Search for datasets by name matching pattern."""
+    found = io.find_datasets(pattern=pattern)
+    ts_logger.debug(f"DATASET.search returned:\n{found} ")
+
+    if len(found) == 1:
+        # raise NotImplementedError("TODO: extract name and type from result.")
+        return Dataset(
+            name=found[0].name,
+            data_type=properties.seriestype_from_str(found[0].type_directory),
+            as_of_tz=as_of_tz,
+        )
+    else:
+        # elif len(found) > 1:
+        return found
```

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/fs.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/fs.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/io.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 See `config` module docs for details.
 """
 
 import glob
 import os
 import re
 from datetime import datetime
+from typing import NamedTuple
 
 import pandas
 
 from ssb_timeseries import config
 from ssb_timeseries import fs
 from ssb_timeseries import properties
 from ssb_timeseries.dates import Interval
@@ -34,14 +35,21 @@
 # mypy: disable-error-code="type-var, arg-type, type-arg, return-value, attr-defined, union-attr, operator, assignment,import-untyped, "
 
 
 TIMESERIES_CONFIG: str = os.environ.get("TIMESERIES_CONFIG")
 CONFIG = config.Config(configuration_file=TIMESERIES_CONFIG)
 
 
+class SearchResult(NamedTuple):
+    """Result item for search."""
+
+    name: str
+    type_directory: str
+
+
 class FileSystem:
     """A filesystem abstraction for Dataset IO."""
 
     def __init__(
         self,
         set_name: str,
         set_type: properties.SeriesType,
@@ -392,33 +400,36 @@
                     meta_publish_path,
                     self.sharing_directory(bucket=s["path"], team=s["team"]),
                 )
                 ts_logger.warning(
                     f"DATASET {self.set_name}: sharing with {s['team']}, snapshot copied to {s['path']}."
                 )
 
-    def search(self, pattern: str | PathStr = "") -> list[str | PathStr]:
+    @classmethod
+    def search(
+        cls, pattern: str | PathStr = "", as_of: datetime | None = None
+    ) -> list[SearchResult]:
         """Search for files in under timeseries root."""
         if pattern:
             pattern = f"*{pattern}*"
         else:
             pattern = "*"
 
         search_str = os.path.join(CONFIG.timeseries_root, "*", pattern)
         dirs = glob.glob(search_str)
-        ts_logger.warning(f"DATASET.IO.SEARCH: {search_str} dirs{dirs}")
+        ts_logger.debug(f"DATASET.IO.SEARCH: {search_str} dirs{dirs}")
         search_results = [
             d.replace(CONFIG.timeseries_root, "root").split(os.path.sep) for d in dirs
         ]
-        ts_logger.warning(f"DATASET.IO.SEARCH: search_results{search_results}")
+        ts_logger.debug(f"DATASET.IO.SEARCH: search_results{search_results}")
 
-        return [f[2] for f in search_results]
+        return [SearchResult(f[2], f[1]) for f in search_results]
 
     @classmethod
-    def dir(self, *args: str, **kwargs: bool) -> str:
+    def dir(cls, *args: str, **kwargs: bool) -> str:
         """Check that target directory is under BUCKET. If so, create it if it does not exist."""
         ts_logger.debug(f"{args}:")
         path = os.path.join(*args)
         ts_root = str(CONFIG.bucket)
 
         # hidden feature: also for kwarg 'force' == True
         if ts_root in path or kwargs.get("force", False):
@@ -426,11 +437,32 @@
         else:
             raise DatasetIoException(
                 f"Directory {path} must be below {ts_root} in file tree."
             )
         return path
 
 
+def find_datasets(
+    pattern: str | PathStr = "", as_of: datetime | None = None
+) -> list[SearchResult]:
+    # ) -> list[str | PathStr]:
+    """Search for files in under timeseries root."""
+    if pattern:
+        pattern = f"*{pattern}*"
+    else:
+        pattern = "*"
+
+    search_str = os.path.join(CONFIG.timeseries_root, "*", pattern)
+    dirs = glob.glob(search_str)
+    ts_logger.debug(f"DATASET.IO.SEARCH: {search_str} dirs{dirs}")
+    search_results = [
+        d.replace(CONFIG.timeseries_root, "root").split(os.path.sep) for d in dirs
+    ]
+    ts_logger.debug(f"DATASET.IO.SEARCH: search_results{search_results}")
+
+    return [SearchResult(f[2], f[1]) for f in search_results]
+
+
 class DatasetIoException(Exception):
     """Exception for dataset io errors."""
 
     pass
```

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/logging.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/logging.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/meta.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/meta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Placeholder utility covering meta data functionality used by timeseries.
 
 Ideally, this functionality should live elsewhere, in ssb-python-klass and other meta data libraries. Likely subject to refactoring later.
 """
 
+import io
+
 import bigtree
+import bigtree.node
+import bigtree.tree
 import pandas as pd
 from klass import get_classification
 from typing_extensions import Self
 
 from ssb_timeseries import fs
 from ssb_timeseries import properties
 from ssb_timeseries.logging import ts_logger
@@ -68,15 +72,15 @@
         """Create Taxonomy object from KLASS id or file name.
 
         Key attributs: .entities holds the list of values and .structure puts the entitiees in a tree.
         """
         self.definition = {"name": root_name}
         if isinstance(id_or_path, int):
             # TO DO: handle versions of KLASS
-            klass = get_classification(id_or_path).get_codes().data
+            klass = get_classification(str(id_or_path)).get_codes().data
             self.entities = add_root_node(
                 klass, {"code": "0", "parentCode": None, "name": root_name}
             )
             if substitute:
                 for key, value in substitute.items():
                     self.entities["code"] = self.entities["code"].str.replace(
                         key, value
@@ -112,53 +116,84 @@
             trees_equal = True
 
         fields_to_compare = ["code", "parentCode", "name"]
         s_entities = self.entities[fields_to_compare].reset_index(drop=True)
         o_entities = other.entities[fields_to_compare].reset_index(drop=True)
 
         ts_logger.debug(
-            f"comparing:\n{s_entities.to_string()}\n...and:\n{s_entities.to_string()}"
+            f"comparing:\n{s_entities.to_string()}\n...and:\n{o_entities.to_string()}"
+        )
+        ts_logger.debug(
+            f".info:\n{_df_info_as_string(s_entities)}\n...and:\n{_df_info_as_string(o_entities)}"
         )
-        ts_logger.debug(f".info:\n{s_entities.info()}\n...and:\n{s_entities.info()}")
         entities_equal = all(s_entities == o_entities)
 
         return trees_equal and entities_equal
 
+    def __minus__(self, other: Self) -> bigtree.tree:  # type: ignore
+        """Return the tree difference between the two taxonomy (tree) structures."""
+        return bigtree.get_tree_diff(self.structure, other.structure)
+
+    def __getitem__(self, key: str) -> bigtree.node:  # type: ignore
+        """Get tree node by name (KLASS code)."""
+        return bigtree.find_name(self.structure.root, key)
+
+    def subtree(self, key: str) -> bigtree.tree:  # type: ignore
+        """Get subtree of node identified by name (KLASS code)."""
+        the_node = bigtree.find_name(self.structure, key)
+        return bigtree.get_subtree(the_node)
+
     def print_tree(self, *args, **kwargs) -> str:  # noqa: ANN002, ANN003
         """Return a string with the tree structure.
 
         Implementation is ugly! It would be preferable not to print the tree to std out.
         ... but this works.
         """
         import io
         from contextlib import redirect_stdout
 
         with io.StringIO() as buf, redirect_stdout(buf):
             bigtree.print_tree(self.structure, *args, **kwargs)
             output = buf.getvalue()
         return output
 
+    def all_nodes(self) -> list[bigtree.node]:  # type: ignore
+        """Return all nodes in the taxonomy."""
+        return [n for n in self.structure.root.descendants]
+
+    def leaf_nodes(self) -> list[bigtree.node]:  # type: ignore
+        """Return all leaf nodes in the taxonomy."""
+        return [n for n in self.structure.root.leaves]
+
+    def parent_nodes(self) -> list[bigtree.node]:  # type: ignore
+        """Return all non-leaf nodes in the taxonomy."""
+        return [
+            n
+            for n in self.structure.root.descendants
+            if n not in self.structure.root.leaves
+        ]
+
     def save(self, path: PathStr) -> None:
         """Save taxonomy to json file.
 
         The file can be read using Taxonomy(<path to file>).
         """
         # TODO: make this work with timeseries.fs
         self.entities.to_json(path_or_buf=path)
 
 
-def add_root_node(df: pd.DataFrame, root_node: dict) -> pd.DataFrame:
+def add_root_node(df: pd.DataFrame, root_node: dict[str, str | None]) -> pd.DataFrame:
     """Prepend root node row to taxonomy dataframe."""
-    new_row = dict((c, None) for c in df.columns)
-    for k in root_node.keys():
+    new_row = {c: None for c in df.columns}
+    for k in root_node:
         new_row[k] = root_node[k]
     df.rename(columns={"name": "fullName"})
     df["parentCode"] = df["parentCode"].fillna(value=root_node["code"])
-    df.loc[-1] = root_node
-    df.index = df.index + 1
+    root_df = pd.DataFrame(root_node, index=[0])
+    df = pd.concat([root_df, df], ignore_index=True)
     df.sort_index(inplace=True)
     return df
 
 
 # A different apporach for tagging sets and series was considered.
 # DatasetTags and SeriesTags classes are currently not used, but kept as the decision may be revisited.
 
@@ -271,7 +306,14 @@
 
         return result
     """
 
     def __repr__(self) -> str:
         """Return initialization for a copy of the series tag object: SeriesTags(name={self.name}, versioning={self.versioning}, temporality={self.temporality}, tags={self.tags})."""
         return f"SeriesTags(name={self.name}, versioning={self.versioning}, temporality={self.temporality}, tags={self.tags})"
+
+
+def _df_info_as_string(df: pd.DataFrame) -> str:
+    """Returns the content of df.info() as a string."""
+    with io.StringIO() as buffer:
+        df.info(buf=buffer)
+        return buffer.getvalue()
```

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/properties.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,40 +47,32 @@
         return self.name
 
 
 class Versioning(SuperEnum):
     """Versioning refers to how revisions of data are identified (named)."""
 
     NONE = 0
-    # ("NONE", "Version control only. Versions are not accessible through API.")
+    """Version control only. Versions are not accessible through API."""
     AS_OF = 1
-    # (
-    #     "AS_OF",
-    #     "Version identified by dates allows date arithemetic ('equals' | 'greater than'  | 'smaller than' | 'between').",
-    # )
+    """Version identified by dates allows date arithemetic ('equals' | 'greater than'  | 'smaller than' | 'between')."""
     NAMES = 2
-    # (
-    #     "NAMES",
-    #     "Consider adding support for: Versions identified by free text names.",
-    # )
+    """Consider adding support for: Versions identified by free text names."""
     SEMANTIC = 3
-    # (
-    #     "SEMANTIC",
-    #     "Consider adding support for: Versions identified by numbers on form X.Y.Z, ie. Major.Minor.Patch.",
-    # )
+    """Consider adding support for: Versions identified by numbers on form X.Y.Z, ie. Major.Minor.Patch."""
 
 
 class Temporality(SuperEnum):
     """Temporality describes the time dimensionality of each data point; notably duration or lack thereof."""
 
     NONE = 0
-    AT = 1  # (1, "Single points in time expressed with 'valid_at' dates.")
-    FROM_TO = (
-        2  # (2, "Duration from-to expressed with 'valid_from' and 'valid_to' dates.")
-    )
+    """No temporal dimension."""
+    AT = 1
+    """Single point in time expressed with 'valid_at' date."""
+    FROM_TO = 2
+    """Duration from-to expressed with 'valid_from' and 'valid_to' dates."""
 
 
 class SeriesType:
     """SeriesTypes are defined by combinations of attributes that have technical implications for time series datasets.
 
     Notable examples are Versioning and Temporality, but a few more may be added later.
     """
@@ -129,18 +121,14 @@
         return cls(versioning=Versioning.AS_OF, temporality=Temporality.FROM_TO)
 
     @classmethod
     def estimate(cls) -> Self:
         """Same as SeriesType.as_of_at(): Shorthand for SeriesType(versioning=Versioning.AS_OF, temporality=Temporality.AT)."""
         return cls.as_of_at()
 
-    # def describe(self) -> str:
-    #     """Helper for testing/logging; returns '<versioning>\n<temporality>'. Do not use in production code."""
-    #     return f"{self.versioning[1]}\n{self.temporality[1]}"
-
     @classmethod
     def permutations(cls) -> list[str]:
         """Helper; returns ['<versioning>_<temporality>', ...] ."""
         return ["_".join(c) for c in product(Versioning.keys(), Temporality.keys())]
 
     def __str__(self) -> str:
         """Helper; returns '<versioning>_<temporality>'."""
@@ -154,7 +142,26 @@
         """Equality test."""
         return repr(self) == repr(other)
 
 
 def estimate_types() -> list[str]:
     """Helper; returns list of SeriesTypes for which Versioning is not NONE."""
     return ["_".join(c) for c in product(["AS_OF"], Temporality.keys())]
+
+
+def seriestype_from_str(dir_name: str) -> SeriesType:
+    """Helper; returns SeriesType from directory name."""
+    match dir_name.lower():
+        case "none_at":
+            return SeriesType.none_at()
+        case "simple":
+            return SeriesType.simple()
+        case "from_to":
+            return SeriesType.from_to()
+        case "as_of_at":
+            return SeriesType.as_of_at()
+        case "as_of_from_to":
+            return SeriesType.as_of_from_to()
+        case "estimate":
+            return SeriesType.estimate()
+        case _:
+            raise ValueError(f"Invalid dir_name: {dir_name}")
```

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/sample_data.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/sample_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         "ME": "months",
         "MS": "months",
         "D": "days",
         "H": "hours",
         "T": "minutes",
         "S": "seconds",
     }
-    valid_to = valid_from + pd.DateOffset(**{freq_lookup[freq]: interval})
+    valid_to = valid_from + pd.DateOffset(**{freq_lookup[freq]: interval})  # type: ignore
 
     # BUGFIX: If *lists receives strings, permutations will be over chars by chars
     # Kombiner listene til en enkelt liste av lister
     # list = list(lists)
 
     # name_parts = series_names(*lists)
     # Generer alle mulige kombinasjoner av listene med separator
@@ -126,16 +126,20 @@
     #     separator.join(combination) for combination in itertools.product(*name_parts)
     # ]
     series = series_names(*lists, separator=separator)
 
     # Opprett DataFrame med tilfeldige tall
     rows = len(valid_at)
     cols = len(series)
+    some_numbers = random_numbers(
+        rows, cols, midpoint=midpoint, variance=variance, decimals=decimals
+    )
     df = pd.DataFrame(
-        (midpoint + variance * np.random.randn(rows, cols)).round(decimals),
+        # (midpoint + variance * np.random.randn(rows, cols)).round(decimals),
+        some_numbers,
         columns=series,
         dtype="float32[pyarrow]",
     )
 
     # Legg til "Dates" som den første kolonnen i "df"
     match temporality:
         case "AT":
@@ -143,7 +147,20 @@
             df.set_index("valid_at")
         case "FROM_TO":
             df.insert(0, "valid_to", valid_to)
             df.insert(0, "valid_from", valid_from)
             df.set_index(["valid_from", "valid_to"])
 
     return df
+
+
+def random_numbers(
+    rows: int,
+    cols: int,
+    decimals: int = 0,
+    midpoint: int | float = 100,
+    variance: int | float = 10,
+) -> np.ndarray:
+    """Generate sample dataframe of specified dimensions."""
+    generator = np.random.default_rng(42)
+    random_matrix = generator.standard_normal(size=(rows, cols))
+    return midpoint + variance * random_matrix.round(decimals)
```

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/sample_metadata.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/src/ssb_timeseries/setup.py` & `ssb_timeseries-0.2.1/src/ssb_timeseries/setup.py`

 * *Files identical despite different names*

### Comparing `ssb_timeseries-0.2.0/PKG-INFO` & `ssb_timeseries-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: ssb-timeseries
-Version: 0.2.0
+Version: 0.2.1
 Summary: SSB Timeseries
 Home-page: https://github.com/statisticsnorway/ssb-timeseries
 License: MIT
 Author: Bernhard Ryeng
 Author-email: bernhard.ryeng@ssb.no
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bigtree (>=0.17.0,<0.18.0)
-Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: bigtree (>=0.17.0)
 Requires-Dist: dapla-toolbelt (>=1.3.2)
-Requires-Dist: duckdb (>=0.10.0,<0.11.0)
-Requires-Dist: google-cloud-logging (>=3.8.0,<4.0.0)
-Requires-Dist: pandas (>=2.1.1,<3.0.0)
-Requires-Dist: polars (>=0.19.18,<0.20.0)
-Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
-Requires-Dist: pytest (>=7.4.3,<8.0.0)
-Requires-Dist: pytz (>=2023.3.post1,<2024.0)
-Requires-Dist: ssb-klass-python (>=0.0.7,<0.0.8)
-Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
+Requires-Dist: numpy (>=1.26.4)
+Requires-Dist: pandas (>=2.1.1)
+Requires-Dist: pyarrow (>=14.0.0)
+Requires-Dist: python-dateutil (>=2.9.0.post0)
+Requires-Dist: ssb-klass-python (>=0.0.7)
+Requires-Dist: typing-extensions (>=4.11.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/ssb-timeseries/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/ssb-timeseries
 Project-URL: Repository, https://github.com/statisticsnorway/ssb-timeseries
 Description-Content-Type: text/markdown
 
 # SSB Timeseries
 
@@ -46,132 +42,124 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)][poetry]
 
 [pypi status]: https://pypi.org/project/ssb-timeseries/
 [documentation]: https://statisticsnorway.github.io/ssb-timeseries
 [tests]: https://github.com/statisticsnorway/ssb-timeseries/actions?workflow=Tests
-
 [sonarcov]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [sonarquality]: https://sonarcloud.io/summary/overall?id=statisticsnorway_ssb-timeseries
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 [poetry]: https://python-poetry.org/
 
 ## Background
 
 Statistics Norway is building a new procuction system in the cloud.
 
 Moving towards modern architecture, development methodology and open source technologies: Python and R are replacing SAS for statistics production code. Oracle databases and ODI for ETL are being replaced by a data lake architecture relying heavily on Parquet files.
 
-Another big issue has been time series.Time series are essential to statistics production, so  the decision to phase out FAME while not having landed precisely what should replace it has left a huge gap.
+Another big issue has been time series.Time series are essential to statistics production, so the decision to phase out FAME while not having landed precisely what should replace it has left a huge gap.
 
 A complete solution will touch several areas of functionality:
 
- * The core is storage with performant read and write, search and filtering
- * Good descriptive metadata is key to findability
- * A wide selection of math and statistics libraries is key for calculations and models
- * Visualisation tools play a role both in ad hoc and routine inspection and quality control
- * Workflow integration with automation and process monitoring help keeping consistent quality
- * Data lineage and process metadata is essential for quality control
+- The core is storage with performant read and write, search and filtering
+- Good descriptive metadata is key to findability
+- A wide selection of math and statistics libraries is key for calculations and models
+- Visualisation tools play a role both in ad hoc and routine inspection and quality control
+- Workflow integration with automation and process monitoring help keeping consistent quality
+- Data lineage and process metadata is essential for quality control
 
- In Statistics Norway strict requirements for transparency and data quality are mandated by law and  commitment to international standards. The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are some times significant, they are far from extreme. This shifts the focus from performance towards process and data control.
+In Statistics Norway strict requirements for transparency and data quality are mandated by law and commitment to international standards. The data itself has a wide variety, but time resolution and publishing frequencies are typically low. While volumes are some times significant, they are far from extreme. This shifts the focus from performance towards process and data control.
 
 This project came out of a PoC to demonstrate how the key functionality may be provided with the core technologies Python and Parquet, in alignment with architecture decisions and process model requirements. Constructed to be an abstraction between the storage layer and the statistics production code, it provides a way forward while postponing some the technical choices.
 
- * Basic functionality for read/write, calculations, time aggregation and plotting was demonstrated December 2023.
- * Persisting snapshots in alignment with the process model, simple descriptive tagging and integrations with GCS buckets was added Q1 2024.
+- Basic functionality for read/write, calculations, time aggregation and plotting was demonstrated December 2023.
+- Persisting snapshots in alignment with the process model, simple descriptive tagging and integrations with GCS buckets was added Q1 2024.
 
 ## How to get started?
 
 See notebook files and tests, `demo.ipynb` and `tests/test_*.py` for examples of usage, and what works and in some cases what does not.
 
 Note that
- * The library is constructed to be platform independent, but top priority is making it work in  a Linux environment.
-* Install by way of `poetry add ssb_timeseries`.
-* The library should work out of the box with default settings. Note that the defaults are for local testing, ie not be suitable for the production setting.
-* To apply custom settings: The environment variable TIMESERIES_CONFIG should point to a JSON file with configurations.
-* The command `poetry run timeseries-config <...>` can be run from a terminal in order to shift between defauls.
- * Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the Jupyter environment (or the equivalent running elsewhere.
-* The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`.
-* With the environment variable set and the configuration in place `poetry run pytest` should succeed.
 
+- The library is constructed to be platform independent, but top priority is making it work in a Linux environment.
+- Install by way of `poetry add ssb_timeseries`.
+- The library should work out of the box with default settings. Note that the defaults are for local testing, ie not be suitable for the production setting.
+- To apply custom settings: The environment variable TIMESERIES_CONFIG should point to a JSON file with configurations.
+- The command `poetry run timeseries-config <...>` can be run from a terminal in order to shift between defauls.
+- Run `poetry run timeseries-config home` to create the environment variable and a file with default configurations in the home directory, ie `/home/jovyan` in the Jupyter environment (or the equivalent running elsewhere.
+- The similar `poetry run timeseries-config gcs` will put configurations and logs in the home directory and time series data in a shared bucket `gs://ssb-prod-dapla-felles-data-delt/poc-tidsserier`.
+- With the environment variable set and the configuration in place `poetry run pytest` should succeed.
 
 While the library is in a workable state and should work both locally and in JupyterLab, it is still in an exploratory phase. There is a risk that fundamental choices are reversed and breaking changes introduced.
 
 With that disclaimer, feel free to explore and experiment, and do not be shy about asking questions or giving feedback. At this stage, feedback is all important.
 
 Assuming you have Python working with a standard SSB setup for git and poetry etc, the following should get you going:
 
-``` bash
+```bash
 # Get the poc package
 git clone https://github.com/statisticsnorway/arkitektur-poc-tidsserier.git
 
 # Run inside a poetry controlled venv:
 poetry shell
 ## Create default config
 poetry run timeseries-config home
 # Run the tests to check that everything is OK:
 poetry run pytest
 # A couple of the test cases *are expected* fail when running for the first time in a new location.
 # They should create the structures they need and should succeed in subsequent runs.
 ```
-~~ No longer needed:~~
-~~ Create and set a location for data and log files. This could be anywhere, but separated from the code is preferrable.~~
-~~ mkdir series~~
-~~ export TIMESERIES_ROOT=${PWD}/series ~~
-~~ export LOG_LOCATION=${PWD}/series ~~
-
 
 ## Functionality overview
 
 The core of the library is the Dataset class. This is essentially a wrapper around a DataFrame (for now Pandas, later probably Polars) in the .data attribute.
 
-The .data attribute should comply to conventions implied by the underlying *information model*. These will start out as pure conventions and subject to evalutation. At a later stage they are likely to be enforced by Parquet schemas. Failing to obey them will cause some methods to fail.
+The .data attribute should comply to conventions implied by the underlying _information model_. These will start out as pure conventions and subject to evalutation. At a later stage they are likely to be enforced by Parquet schemas. Failing to obey them will cause some methods to fail.
 
-The Dataset.io attribute connects the dataset to a helper class that takes care of reading and writing data. This structure abstracts away the IO mechanics, so that the user do not need to know about the "physical" details, only the *information model meaning* of the choices made.
+The Dataset.io attribute connects the dataset to a helper class that takes care of reading and writing data. This structure abstracts away the IO mechanics, so that the user do not need to know about the "physical" details, only the _information model meaning_ of the choices made.
 
- * Read and write for both versioned and unversioned data types.
- * Search for sets by name, regex and (planned for later) metadata.
- * Basic filtering of sets (selecting series within a selected set).
- * Basic linear algebra: Datasets can be added, subtracted, multiplied and divided with each other and dataframes, matrices, vectors (untested) and scalars according to normal rules.
- * Basic plotting: Dataset.plot() as shorthand for Dataset.data.plot(<and sensible defaults>).
- * Basic time aggregation:
- `Dataset.groupby(<frequency>, 'sum'|'mean'|'auto')`
- *
-
-
- ## The information model
-
- ### TLDR
-
- * **Types** are defined by
-  * **Versioning** defines how updated versions of the truth are represented: NONE overwrites a single version, NAMED or AS_OF maintaines new "logical" versions identified by name or date.
-  * **Temporality** describes the "real world" valid_at or valid_from - valid_to datetime of the data. It will translate into columns, datetime or period indexes of Dataset.data.
-  * Value type (only scalars for now) of Dataset.data "cells".
-* **Datasets** can consists of multiple series. (Later: possible extension with sets of sets.)
-* All series in a set must be of the same type.
-* **Series** are value columns in Datasets.data, rows identified by date(s) or index corresponding temporality.
-* The combination `<Dataset.name>.<Series.name>` will serve as a globally unique series identifier.
-* `<Dataset.name>` identifies a "directory", hence must be unique. (Caveat: Directories per type creates room for error.)
-* `<Series.name>` (.data column name) must be unique within the set.
-* Series names *should* be related to (preferrably constructed from) codes or meta data in such a way that they can be mapped to "tags" via a format mask (and if needed a translation table).
+- Read and write for both versioned and unversioned data types.
+- Search for sets by name, regex and (planned for later) metadata.
+- Basic filtering of sets (selecting series within a selected set).
+- Basic linear algebra: Datasets can be added, subtracted, multiplied and divided with each other and dataframes, matrices, vectors (untested) and scalars according to normal rules.
+- Basic plotting: Dataset.plot() as shorthand for Dataset.data.plot(<and sensible defaults>).
+- Basic time aggregation:
+  `Dataset.groupby(<frequency>, 'sum'|'mean'|'auto')`
+
+## The information model
+
+### TLDR
+
+- **Types** are defined by
+- **Versioning** defines how updated versions of the truth are represented: NONE overwrites a single version, NAMED or AS_OF maintaines new "logical" versions identified by name or date.
+- **Temporality** describes the "real world" valid_at or valid_from - valid_to datetime of the data. It will translate into columns, datetime or period indexes of Dataset.data.
+- Value type (only scalars for now) of Dataset.data "cells".
+- **Datasets** can consists of multiple series. (Later: possible extension with sets of sets.)
+- All series in a set must be of the same type.
+- **Series** are value columns in Datasets.data, rows identified by date(s) or index corresponding temporality.
+- The combination `<Dataset.name>.<Series.name>` will serve as a globally unique series identifier.
+- `<Dataset.name>` identifies a "directory", hence must be unique. (Caveat: Directories per type creates room for error.)
+- `<Series.name>` (.data column name) must be unique within the set.
+- Series names _should_ be related to (preferrably constructed from) codes or meta data in such a way that they can be mapped to "tags" via a format mask (and if needed a translation table).
 
-Yes, that *was* the short version. The long version is still pending production.
+Yes, that _was_ the short version. The long version is still pending production.
 
 To be continued ...
 
-### How to contribute
+### Other sources of documentation:
 
-More information about this will come later, but contributions are welcome. If you want to contribute, just let us know.
+- https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3581313026/Statistikkproduksjon
+- https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3595665419/Lagring+av+tidsserier
 
-### Other sources of documentation:
+## API-documentation
 
-* https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3581313026/Statistikkproduksjon
-* https://statistics-norway.atlassian.net/wiki/spaces/Arkitektur/pages/3595665419/Lagring+av+tidsserier
+The [documentation] is published on GitHub Pages. Se the Reference page for
+API-documentation.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

