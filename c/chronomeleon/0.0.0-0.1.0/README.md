# Comparing `tmp/chronomeleon-0.0.0.tar.gz` & `tmp/chronomeleon-0.1.0.tar.gz`

## Comparing `chronomeleon-0.0.0.tar` & `chronomeleon-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/README.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/domain-specific-terms.txt
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/requirements.txt
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/src/_chronomeleon_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/src/chronomeleon/__init__.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/src/chronomeleon/mymodule.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/src/chronomeleon/py.typed
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/src/chronomeleon/models/__init__.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/src/chronomeleon/models/chrono_assumption.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/.gitignore
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 chronomeleon-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/README.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/domain-specific-terms.txt
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/requirements.txt
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/_chronomeleon_version.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/chronomeleon/__init__.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/chronomeleon/mapping.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/chronomeleon/py.typed
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/chronomeleon/models/__init__.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/chronomeleon/models/chrono_assumption.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/src/chronomeleon/models/mapping_config.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 chronomeleon-0.1.0/PKG-INFO
```

### Comparing `chronomeleon-0.0.0/.pre-commit-config.yaml` & `chronomeleon-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/README.md` & `chronomeleon-0.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 ![Python Versions (officially) supported](https://img.shields.io/pypi/pyversions/chronomeleon.svg)
 ![Pypi status badge](https://img.shields.io/pypi/v/chronomeleon)
 ![Unittests status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Formatting/badge.svg)
 
-Chronomeleon is a Python package that converts date and time related objects in migration scenarios.
-It's meant to be used when migrate dates, datetimes or time slices/ranges from one system to another.
+Chronomeleon is a Python package that converts and maps date and time information from their representation in one system to another.
+It's meant to be used in data migration projects.
 
 ## Rationale
 While converting a datetime alone is possible with either Python builtin tools or libraries like `pendulum` and `arrow`,
 things become more complicated when you have to convert time slices or ranges or when the source and target system interpret dates and times differently.
 
 Think your migrating e.g., contracts from system A to system B.
 In system A might have an API, a data dump or something else from where you can read,
@@ -28,28 +28,56 @@
   * What if there was a system C, which supported microseconds but only stored the date and time in a single integer?
 * What about the end date (times)? It seems that system A uses the end date as inclusive (contract ends at the end of june), whereas system B uses it as exclusive (start of the followup contract == end of the previous contract).
 
 Chronomeleon has two purposes:
 1. It forces you to make assumptions explicit.
 2. Once the assumptions are explicit, it helps you do the conversion.
 
-The latter is no rocket science (and neither is any code in chronomeleon), but the former is crucial for a successful migration.
+The latter is no rocket science (and neither is any line of code in chronomeleon), but making assumptions explicit is crucial and that's why using it is beneficial.
+
+When you're constantly wondering why other coders seem to randomly
+* add or subtract a day, a second, a tick here and there
+* pass around naive dates and datetimes and try to convert them to UTC or other timezones with no clear reason
+
+then chronomeleon is for you.
 
 Chronomeleon makes your code more readable and makes your assumption clear.
-This allows you to spot errors in your or your team mates code and explain, why things are done the way they are.
+This allows you to spot errors in your or your teammates code more easily and explain why things are done the way they are.
 
 ## How to use it?
 Install it from pypi:
 ```bash
 pip install chronomeleon
 ```
 
 Then, in your code: Make assumptions about the source and target system explicit.
 To do so, chronomeleon provides you with so-called ChronoConfig objects.
+
+Here's an advanced example, that shows the capabilities of Chronomeleon:
 ```python
+from datetime import date, datetime, timedelta
+
+import pytz
+
+from chronomeleon import ChronoAssumption, MappingConfig, adapt_to_target
+
+config = MappingConfig( # make assumptions explicit
+    source=ChronoAssumption(
+        implicit_timezone=pytz.timezone("Europe/Berlin"),
+        resolution=timedelta(days=1),
+        is_inclusive_end=True,
+        is_gastag_aware=False,
+    ),
+    target=ChronoAssumption(resolution=timedelta(milliseconds=1), is_inclusive_end=True, is_gastag_aware=True),
+    is_end=True,
+    is_gas=True,
+)
+source_value = date(2021, 12, 31)
+result = adapt_to_target(source_value, config) # do the mapping
+assert result == datetime(2022, 1, 1, 4, 59, 59, microsecond=999000, tzinfo=pytz.utc)
 ```
 
 
 ## Setup for Local Development
 Follow the instructions from our [template repository](https://github.com/Hochfrequenz/python_template_repository?tab=readme-ov-file#how-to-use-this-repository-on-your-machine).
 tl;dr: `tox`.
```

### Comparing `chronomeleon-0.0.0/tox.ini` & `chronomeleon-0.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/dependabot.yml` & `chronomeleon-0.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/codeql-analysis.yml` & `chronomeleon-0.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/coverage.yml` & `chronomeleon-0.1.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/dependabot_automerge.yml` & `chronomeleon-0.1.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/dev_test.yml` & `chronomeleon-0.1.0/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/formatting.yml` & `chronomeleon-0.1.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/packaging_test.yml` & `chronomeleon-0.1.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/python-publish.yml` & `chronomeleon-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/pythonlint.yml` & `chronomeleon-0.1.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/.github/workflows/unittests.yml` & `chronomeleon-0.1.0/.github/workflows/unittests.yml`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     branches: [main]
   pull_request: {}
 jobs:
   pytest:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.10", "3.11", "3.12"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `chronomeleon-0.0.0/dev_requirements/requirements-packaging.txt` & `chronomeleon-0.1.0/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/src/chronomeleon/models/chrono_assumption.py` & `chronomeleon-0.1.0/src/chronomeleon/models/chrono_assumption.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 @dataclass(frozen=True, kw_only=True)
 class ChronoAssumption:
     """
     represents assumptions about how a specific system interprets a specific field that holds date or time
     """
 
-    resolution: timedelta
+    resolution: Optional[timedelta] = None
     """
+    This is only necessary to provide, if the field is an inclusive end date.
     The smallest unit of time that this field can represent.
     Typically this is something like 1 day, 1 second, 1 microsecond.
     Adding one "unit" of the resolution leads to the smallest possible increase in the field.
     If e.g. the resolution is 1 day, then the next possible value after 2024-01-01 is 2024-01-02.
     But if the resolution is 1 second, then the next possible value after 2024-01-01 00:00:00 is 2024-01-01 00:00:01.
     """
 
@@ -28,20 +29,47 @@
     In this case, the system implicitly uses a specific timezone.
     You can specific this implicit timezone here.
     If the datetimes come with a specified UTC offset, leave it None.
     You have to specify the implicit timezone as a pytz-timezone object, e.g. pytz.timezone("Europe/Berlin").
     pytz is a dependency of chronomeleon; If you install chronomeleon, you also get pytz.
     """
 
-    is_end: Optional[bool] = None
-    """
-    True if and only if the date or time is the end of a range. None if it doesn't matter.
-    """
-
     is_inclusive_end: Optional[bool] = None
     """
     Must not be None if is_end is True.
     True if and only if the end of the range is inclusive.
     If the resolution is timedelta(days=1) and is_inclusive_end is True, then the range 2024-01-01 to 2024-01-31 covers
     the entire month of January.
     If is_inclusive_end is False, then the range 2024-01-01 to 2024-02-01 covers the entire month of January.
     """
+
+    is_gastag_aware: bool = False
+    """
+    True if and only if the start of a day is 6:00 am German local time.
+    If you never heard of the "Gastag", you can ignore this parameter and let it default to False.
+    """
+
+    is_date_only: bool = False
+    """
+    True if and only if the field in the respective system is a date without a time component (datetime.date).
+    """
+
+    def get_consistency_errors(self) -> list[str]:
+        """
+        returns errors from the self-consistency check; if the returned list is empty, the object is self-consistent
+        """
+        result: list[str] = []
+        if self.is_inclusive_end and self.resolution is None:
+            result.append("if is_inclusive_end is True, then resolution must be set")
+        if self.resolution is not None and not isinstance(self.resolution, timedelta):
+            result.append(f"resolution must be a timedelta object but is {self.resolution.__class__.__name__}")
+        if self.implicit_timezone is not None and not isinstance(self.implicit_timezone, BaseTzInfo):
+            result.append(
+                f"implicit_timezone must be a pytz timezone object but is {self.implicit_timezone.__class__.__name__}"
+            )
+        return result
+
+    def is_self_consistent(self) -> bool:
+        """
+        returns True if the object is self-consistent
+        """
+        return not any(self.get_consistency_errors())
```

### Comparing `chronomeleon-0.0.0/.gitignore` & `chronomeleon-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chronomeleon-0.0.0/pyproject.toml` & `chronomeleon-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [project]
 name = "chronomeleon"
 description = "A python package to flexibly adapt start and end date(times) to your system background"
 license = { text = "MIT" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 authors = [{ name = "Hochfrequenz Unternehmensberatung GmbH", email = "info+github@hochfrequenz.de" }]
 keywords = ["date", "time", "conversion", "migration", "inclusive", "exclusive", "dateonly"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
+    # no python 3.8 and 3.9 because of missing kw_only arg to dataclass
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pytz"
 ]     # add all the dependencies here
@@ -26,15 +25,15 @@
 
 [project.urls]
 Changelog = "https://github.com/Hochfrequenz/chronomeleon/releases"
 Homepage = "https://github.com/Hochfrequenz/chronomeleon"
 
 [tool.black]
 line-length = 120
-target_version = ["py38", "py39", "py310", "py311", "py312"]
+target_version = ["py310", "py311", "py312"]
 
 [tool.isort]
 line_length = 120
 profile = "black"
 
 [tool.pylint."MESSAGES CONTROL"]
 max-line-length = 120
```

### Comparing `chronomeleon-0.0.0/PKG-INFO` & `chronomeleon-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.3
 Name: chronomeleon
-Version: 0.0.0
+Version: 0.1.0
 Summary: A python package to flexibly adapt start and end date(times) to your system background
 Project-URL: Changelog, https://github.com/Hochfrequenz/chronomeleon/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/chronomeleon
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
+License-File: LICENSE
 Keywords: conversion,date,dateonly,exclusive,inclusive,migration,time
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: pytz
 Description-Content-Type: text/markdown
 
 # Chronomeleon
 🚧 Still Work In Progress!
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 ![Python Versions (officially) supported](https://img.shields.io/pypi/pyversions/chronomeleon.svg)
 ![Pypi status badge](https://img.shields.io/pypi/v/chronomeleon)
 ![Unittests status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/chronomeleon/workflows/Formatting/badge.svg)
 
-Chronomeleon is a Python package that converts date and time related objects in migration scenarios.
-It's meant to be used when migrate dates, datetimes or time slices/ranges from one system to another.
+Chronomeleon is a Python package that converts and maps date and time information from their representation in one system to another.
+It's meant to be used in data migration projects.
 
 ## Rationale
 While converting a datetime alone is possible with either Python builtin tools or libraries like `pendulum` and `arrow`,
 things become more complicated when you have to convert time slices or ranges or when the source and target system interpret dates and times differently.
 
 Think your migrating e.g., contracts from system A to system B.
 In system A might have an API, a data dump or something else from where you can read,
@@ -53,28 +52,56 @@
   * What if there was a system C, which supported microseconds but only stored the date and time in a single integer?
 * What about the end date (times)? It seems that system A uses the end date as inclusive (contract ends at the end of june), whereas system B uses it as exclusive (start of the followup contract == end of the previous contract).
 
 Chronomeleon has two purposes:
 1. It forces you to make assumptions explicit.
 2. Once the assumptions are explicit, it helps you do the conversion.
 
-The latter is no rocket science (and neither is any code in chronomeleon), but the former is crucial for a successful migration.
+The latter is no rocket science (and neither is any line of code in chronomeleon), but making assumptions explicit is crucial and that's why using it is beneficial.
+
+When you're constantly wondering why other coders seem to randomly
+* add or subtract a day, a second, a tick here and there
+* pass around naive dates and datetimes and try to convert them to UTC or other timezones with no clear reason
+
+then chronomeleon is for you.
 
 Chronomeleon makes your code more readable and makes your assumption clear.
-This allows you to spot errors in your or your team mates code and explain, why things are done the way they are.
+This allows you to spot errors in your or your teammates code more easily and explain why things are done the way they are.
 
 ## How to use it?
 Install it from pypi:
 ```bash
 pip install chronomeleon
 ```
 
 Then, in your code: Make assumptions about the source and target system explicit.
 To do so, chronomeleon provides you with so-called ChronoConfig objects.
+
+Here's an advanced example, that shows the capabilities of Chronomeleon:
 ```python
+from datetime import date, datetime, timedelta
+
+import pytz
+
+from chronomeleon import ChronoAssumption, MappingConfig, adapt_to_target
+
+config = MappingConfig( # make assumptions explicit
+    source=ChronoAssumption(
+        implicit_timezone=pytz.timezone("Europe/Berlin"),
+        resolution=timedelta(days=1),
+        is_inclusive_end=True,
+        is_gastag_aware=False,
+    ),
+    target=ChronoAssumption(resolution=timedelta(milliseconds=1), is_inclusive_end=True, is_gastag_aware=True),
+    is_end=True,
+    is_gas=True,
+)
+source_value = date(2021, 12, 31)
+result = adapt_to_target(source_value, config) # do the mapping
+assert result == datetime(2022, 1, 1, 4, 59, 59, microsecond=999000, tzinfo=pytz.utc)
 ```
 
 
 ## Setup for Local Development
 Follow the instructions from our [template repository](https://github.com/Hochfrequenz/python_template_repository?tab=readme-ov-file#how-to-use-this-repository-on-your-machine).
 tl;dr: `tox`.
```

