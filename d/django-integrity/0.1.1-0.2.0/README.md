# Comparing `tmp/django_integrity-0.1.1.tar.gz` & `tmp/django_integrity-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_integrity-0.1.1.tar", last modified: Thu May  9 09:43:43 2024, max compression
+gzip compressed data, was "django_integrity-0.2.0.tar", last modified: Mon May 13 11:43:26 2024, max compression
```

## Comparing `django_integrity-0.1.1.tar` & `django_integrity-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.701741 django_integrity-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-09 09:43:40.000000 django_integrity-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-09 09:43:43.701741 django_integrity-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-09 09:43:40.000000 django_integrity-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-09 09:43:40.000000 django_integrity-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:43:43.701741 django_integrity-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.697741 django_integrity-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.697741 django_integrity-0.1.1/src/django_integrity/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.701741 django_integrity-0.1.1/src/django_integrity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:43:26.302113 django_integrity-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-13 11:43:23.000000 django_integrity-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-13 11:43:26.302113 django_integrity-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-13 11:43:23.000000 django_integrity-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-13 11:43:23.000000 django_integrity-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:43:26.302113 django_integrity-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:43:26.294113 django_integrity-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:43:26.298113 django_integrity-0.2.0/src/django_integrity/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 11:43:23.000000 django_integrity-0.2.0/src/django_integrity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-13 11:43:23.000000 django_integrity-0.2.0/src/django_integrity/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-13 11:43:23.000000 django_integrity-0.2.0/src/django_integrity/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:43:23.000000 django_integrity-0.2.0/src/django_integrity/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:43:26.298113 django_integrity-0.2.0/src/django_integrity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-13 11:43:26.000000 django_integrity-0.2.0/src/django_integrity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-13 11:43:26.000000 django_integrity-0.2.0/src/django_integrity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:43:26.000000 django_integrity-0.2.0/src/django_integrity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 11:43:26.000000 django_integrity-0.2.0/src/django_integrity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 11:43:26.000000 django_integrity-0.2.0/src/django_integrity.egg-info/top_level.txt
```

### Comparing `django_integrity-0.1.1/LICENSE` & `django_integrity-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_integrity-0.1.1/PKG-INFO` & `django_integrity-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: django_integrity
-Version: 0.1.1
+Version: 0.2.0
+Summary: Tools for refining Django's IntegrityError, and working with deferred database constraints.
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Kraken Technologies Limited
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -26,42 +27,61 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: repository, https://github.com/octoenergy/django-integrity
-Project-URL: changelog, https://github.com/octoenergy/django-integrity/blob/main/CHANGELOG.md
+Project-URL: repository, https://github.com/kraken-tech/django-integrity
+Project-URL: changelog, https://github.com/kraken-tech/django-integrity/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: pytest-in-tox
+Requires-Dist: dj-database-url>=2.1.0; extra == "pytest-in-tox"
+Requires-Dist: django-stubs>=5.0.0; extra == "pytest-in-tox"
+Requires-Dist: environs>=11.0.0; extra == "pytest-in-tox"
+Requires-Dist: pytest-django>=4.8.0; extra == "pytest-in-tox"
+Requires-Dist: pytest>=8.2.0; extra == "pytest-in-tox"
+Provides-Extra: release
+Requires-Dist: packaging>=24.0; extra == "release"
+Requires-Dist: rich>=13.7.1; extra == "release"
+Requires-Dist: tomli>=1.1.0; python_version < "3.11" and extra == "release"
+Requires-Dist: typer>=0.12.3; extra == "release"
+Provides-Extra: tox
+Requires-Dist: tox-uv>=1.8.2; extra == "tox"
+Requires-Dist: tox>=4.15.0; extra == "tox"
 Provides-Extra: dev
-Requires-Dist: dj-database-url; extra == "dev"
-Requires-Dist: django-stubs; extra == "dev"
-Requires-Dist: environs; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-django; extra == "dev"
-Requires-Dist: tox; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mypy-json-report; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: rich; extra == "dev"
+Requires-Dist: dj-database-url>=2.1.0; extra == "dev"
+Requires-Dist: django>=4.2.0; extra == "dev"
+Requires-Dist: django-stubs>=5.0.0; extra == "dev"
+Requires-Dist: environs>=11.0.0; extra == "dev"
+Requires-Dist: psycopg2-binary>=2.9.9; extra == "dev"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "dev"
+Requires-Dist: pytest-django>=4.8.0; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: tox>=4.15.0; extra == "dev"
+Requires-Dist: types-psycopg2>=2.9.21.20240417; extra == "dev"
+Requires-Dist: mypy>=1.10.0; extra == "dev"
+Requires-Dist: mypy-json-report>=1.2.0; extra == "dev"
+Requires-Dist: pre-commit>=3.7.0; extra == "dev"
+Requires-Dist: packaging>=24.0; extra == "dev"
+Requires-Dist: rich>=13.7.1; extra == "dev"
 Requires-Dist: tomli>=1.1.0; python_version < "3.11" and extra == "dev"
-Requires-Dist: typer; extra == "dev"
+Requires-Dist: typer>=0.12.3; extra == "dev"
 
 # Django Integrity
 
 Django Integrity contains tools for controlling deferred constraints
 and handling `IntegrityError`s in Django projects which use PostgreSQL.
 
 ## Deferrable constraints
@@ -137,19 +157,19 @@
     Creates a user with the provided email address.
 
     Raises:
         UserAlreadyExists: If the email was not unique.
         EmailCannotBeNull: If the email was None.
         EmailMustBeLowerCase: If the email had a non-lowercase character.
     """
-    rules = {
-        conversion.Unique(model=User, fields=("email",)): UserAlreadyExists,
-        conversion.NotNull(model=User, field="email"): EmailCannotBeNull,
-        conversion.Named(name="constraint_islowercase"): EmailMustBeLowerCase,
-    }
+    rules = [
+        (conversion.Unique(model=User, fields=("email",)), UserAlreadyExists),
+        (conversion.NotNull(model=User, field="email"), EmailCannotBeNull),
+        (conversion.Named(name="constraint_islowercase"), EmailMustBeLowerCase),
+    ]
     with conversion.refine_integrity_error(rules):
         User.objects.create(email=email)
 ```
 
 ## Supported dependencies
 
 This package is tested against:
```

### Comparing `django_integrity-0.1.1/README.md` & `django_integrity-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,19 @@
     Creates a user with the provided email address.
 
     Raises:
         UserAlreadyExists: If the email was not unique.
         EmailCannotBeNull: If the email was None.
         EmailMustBeLowerCase: If the email had a non-lowercase character.
     """
-    rules = {
-        conversion.Unique(model=User, fields=("email",)): UserAlreadyExists,
-        conversion.NotNull(model=User, field="email"): EmailCannotBeNull,
-        conversion.Named(name="constraint_islowercase"): EmailMustBeLowerCase,
-    }
+    rules = [
+        (conversion.Unique(model=User, fields=("email",)), UserAlreadyExists),
+        (conversion.NotNull(model=User, field="email"), EmailCannotBeNull),
+        (conversion.Named(name="constraint_islowercase"), EmailMustBeLowerCase),
+    ]
     with conversion.refine_integrity_error(rules):
         User.objects.create(email=email)
 ```
 
 ## Supported dependencies
 
 This package is tested against:
```

### Comparing `django_integrity-0.1.1/pyproject.toml` & `django_integrity-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 where = ["src"]
 
 # Project
 # -------
 
 [project]
 name = "django_integrity"
-version = "0.1.1"
+version = "0.2.0"
+description = "Tools for refining Django's IntegrityError, and working with deferred database constraints."
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     # We cannot decide for users if they want to use psycopg2, psycopg2-binary, or
     # psycopg (i.e. psycopg3) with or without the [binary] extra. It should be part of
     # their own project dependencies anyway.
@@ -41,36 +42,63 @@
   "Typing :: Typed",
 ]
 
 
 [project.urls]
 # See https://daniel.feldroy.com/posts/2023-08-pypi-project-urls-cheatsheet for
 # additional URLs that can be included here.
-repository = "https://github.com/octoenergy/django-integrity"
-changelog = "https://github.com/octoenergy/django-integrity/blob/main/CHANGELOG.md"
+repository = "https://github.com/kraken-tech/django-integrity"
+changelog = "https://github.com/kraken-tech/django-integrity/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
+# None of these extras are recommended for normal installation.
+# We use combinations of these groups in development and testing environments.
+pytest-in-tox = [
+    # We deliberately exclude Django and Psycopg from this list because
+    # this groups is used for running the pytest tests with tox,
+    # and those packages are a part of tox's test matrix.
+    "dj-database-url>=2.1.0",
+    "django-stubs>=5.0.0",
+    "environs>=11.0.0",
+    "pytest-django>=4.8.0",
+    "pytest>=8.2.0",
+]
+release = [
+    "packaging>=24.0",
+    "rich>=13.7.1",
+    "tomli >= 1.1.0 ; python_version < '3.11'",
+    "typer>=0.12.3",
+]
+tox = [
+    "tox-uv>=1.8.2",
+    "tox>=4.15.0",
+]
 dev = [
     # Testing
-    "dj-database-url",
-    "django-stubs",
-    "environs",
-    "pytest",
-    "pytest-django",
-    "tox",
+    "dj-database-url>=2.1.0",
+    "django>=4.2.0",
+    "django-stubs>=5.0.0",
+    "environs>=11.0.0",
+    "psycopg2-binary>=2.9.9",
+    "psycopg[binary]>=3.1.18",
+    "pytest-django>=4.8.0",
+    "pytest>=8.2.0",
+    "tox>=4.15.0",
+    "types-psycopg2>=2.9.21.20240417",
 
     # Linting
-    "mypy",
-    "mypy-json-report",
-    "ruff",
+    "mypy>=1.10.0",
+    "mypy-json-report>=1.2.0",
+    "pre-commit>=3.7.0",
 
     # CLI utils
-    "rich",
+    "packaging>=24.0",
+    "rich>=13.7.1",
     "tomli >= 1.1.0 ; python_version < '3.11'",
-    "typer",
+    "typer>=0.12.3",
 ]
 
 # Ruff
 # ----
 
 [tool.ruff]
 lint.select = [
@@ -127,9 +155,11 @@
 
 # Pytest
 # ------
 
 [tool.pytest.ini_options]
 # Ensure error warnings are converted into test errors.
 filterwarnings = "error"
+# Ensure that tests fail if an xfail test unexpectedly passes.
+xfail_strict = true
 
 DJANGO_SETTINGS_MODULE = "tests.example_app.settings"
```

### Comparing `django_integrity-0.1.1/src/django_integrity/constraints.py` & `django_integrity-0.2.0/src/django_integrity/constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import contextlib
 from collections.abc import Iterator, Sequence
 
-from django import db as django_db
+from django.db import connections, models, transaction
 
 
 try:
     from psycopg import sql
 except ImportError:
-    from psycopg2 import sql
+    from psycopg2 import sql  # type: ignore[no-redef]
 
 
 # Note [Deferrable constraints]
 # -----------------------------
 # Only some types of PostgreSQL constraint can be DEFERRED, and
 # they may be deferred if they are created with the DEFERRABLE option.
 #
@@ -65,15 +65,15 @@
         using: The name of the database connection to use.
 
     Raises:
         NotInTransaction: When we try to change constraints outside of a transaction.
     """
     set_immediate(names, using=using)
     try:
-        with django_db.transaction.atomic(using=using):
+        with transaction.atomic(using=using):
             yield
     finally:
         set_deferred(names, using=using)
 
 
 def set_all_immediate(*, using: str) -> None:
     """
@@ -83,18 +83,18 @@
 
     Args:
         using: The name of the database connection to use.
 
     Raises:
         NotInTransaction: When we try to change constraints outside of a transaction.
     """
-    if django_db.transaction.get_autocommit(using):
+    if transaction.get_autocommit(using):
         raise NotInTransaction
 
-    with django_db.connections[using].cursor() as cursor:
+    with connections[using].cursor() as cursor:
         cursor.execute("SET CONSTRAINTS ALL IMMEDIATE")
 
 
 def set_immediate(names: Sequence[str], *, using: str) -> None:
     """
     Set particular constraints to IMMEDIATE for the remainder of the transaction.
 
@@ -103,25 +103,25 @@
     Args:
         names: The names of the constraints to set to IMMEDIATE.
         using: The name of the database connection to use.
 
     Raises:
         NotInTransaction: When we try to change constraints outside of a transaction.
     """
-    if django_db.transaction.get_autocommit(using):
+    if transaction.get_autocommit(using):
         raise NotInTransaction
 
     if not names:
         return
 
     query = sql.SQL("SET CONSTRAINTS {names} IMMEDIATE").format(
         names=sql.SQL(", ").join(sql.Identifier(name) for name in names)
     )
 
-    with django_db.connections[using].cursor() as cursor:
+    with connections[using].cursor() as cursor:
         cursor.execute(query)
 
 
 def set_deferred(names: Sequence[str], *, using: str) -> None:
     """
     Set particular constraints to DEFERRED for the remainder of the transaction.
 
@@ -130,25 +130,25 @@
     Args:
         names: The names of the constraints to set to DEFERRED.
         using: The name of the database connection to use.
 
     Raises:
         NotInTransaction: When we try to change constraints outside of a transaction.
     """
-    if django_db.transaction.get_autocommit(using):
+    if transaction.get_autocommit(using):
         raise NotInTransaction
 
     if not names:
         return
 
     query = sql.SQL("SET CONSTRAINTS {names} DEFERRED").format(
         names=sql.SQL(", ").join(sql.Identifier(name) for name in names)
     )
 
-    with django_db.connections[using].cursor() as cursor:
+    with connections[using].cursor() as cursor:
         cursor.execute(query)
 
 
 class NotInTransaction(Exception):
     """
     Raised when we try to change the state of constraints outside of a transaction.
 
@@ -156,15 +156,15 @@
     because the change of state would only last for the remainder of the transaction.
 
     See https://www.postgresql.org/docs/current/sql-set-constraints.html
     """
 
 
 def foreign_key_constraint_name(
-    model: type[django_db.models.Model], field_name: str, *, using: str
+    model: type[models.Model], field_name: str, *, using: str
 ) -> str:
     """
     Calculate FK constraint name for a model's field.
 
     Django's constraint names are based on the names of the tables and columns involved.
 
     Because there is a 63-character limit on constraint names in PostgreSQL,
@@ -191,15 +191,15 @@
     if remote_field is None:
         raise NotAForeignKey
 
     to_table = remote_field.model._meta.db_table
     to_field = remote_field.name
     suffix = f"_fk_{to_table}_{to_field}"
 
-    connection = django_db.connections[using]
+    connection = connections[using]
     with connection.schema_editor() as editor:
         # The _fk_constraint_name method is not part of the public API,
         # and only exists on the PostgreSQL schema editor.
         # Django-stubs does not know about this method, so we have to use a type ignore.
         constraint_name = editor._fk_constraint_name(model, field, suffix)  # type: ignore[attr-defined]
 
     return str(constraint_name).removeprefix('"').removesuffix('"')
```

### Comparing `django_integrity-0.1.1/src/django_integrity/conversion.py` & `django_integrity-0.2.0/src/django_integrity/conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from __future__ import annotations
 
 import abc
 import contextlib
 import dataclasses
 import re
-from collections.abc import Iterator, Mapping
+from collections.abc import Iterator, Sequence
 
 from django import db as django_db
 
 
 try:
     import psycopg
 except ImportError:
-    import psycopg2 as psycopg
+    import psycopg2 as psycopg  # type: ignore[no-redef]
 
 
 @contextlib.contextmanager
-def refine_integrity_error(rules: Mapping[_Rule, Exception]) -> Iterator[None]:
+def refine_integrity_error(
+    rules: Sequence[tuple[_Rule, Exception | type[Exception]]],
+) -> Iterator[None]:
     """
     Convert a generic IntegrityError into a more specific exception.
 
-    The conversion is based on a mapping of rules to exceptions.
+    The conversion is based on (rule, exception) pairs.
 
     Args:
-        rules: A mapping of rules to the exceptions we'll raise if they match.
+        rules: A sequence of rule, exception pairs.
+            If the rule matches the IntegrityError, the exception is raised.
 
     Raises:
-        An error from the rules mapping if an IntegrityError matches a rule.
+        The exception paired with the first matching rule.
         Otherwise, the original IntegrityError.
     """
     try:
         yield
     except django_db.IntegrityError as e:
-        for rule, refined_error in rules.items():
+        for rule, refined_error in rules:
             if rule.is_match(e):
                 raise refined_error from e
         raise
 
 
 class _Rule(abc.ABC):
     @abc.abstractmethod
@@ -71,23 +74,23 @@
 @dataclasses.dataclass(frozen=True)
 class Unique(_Rule):
     """
     A unique constraint defined by a model and a set of fields.
     """
 
     model: type[django_db.models.Model]
-    fields: tuple[str]
+    fields: tuple[str, ...]
 
     _pattern = re.compile(r"Key \((?P<fields>.+)\)=\(.*\) already exists.")
 
     def is_match(self, error: django_db.IntegrityError) -> bool:
         if not isinstance(error.__cause__, psycopg.errors.UniqueViolation):
             return False
 
-        match = self._pattern.match(error.__cause__.diag.message_detail)
+        match = self._pattern.match(error.__cause__.diag.message_detail or "")
         if match is None:
             return False
 
         return (
             tuple(match.group("fields").split(", ")) == self.fields
             and error.__cause__.diag.table_name == self.model._meta.db_table
         )
@@ -102,15 +105,15 @@
     trying to create a PrimaryKey rule.
     """
 
     model: type[django_db.models.Model]
 
     _pattern = re.compile(r"Key \((?P<fields>.+)\)=\(.*\) already exists.")
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         """
         Ensure the model has a primary key.
 
         There's no sense in creating a rule to match a primary key constraint
         if the model has no primary key.
 
         This helps us to justify an assert statement in is_match.
@@ -118,15 +121,15 @@
         if self.model._meta.pk is None:
             raise ModelHasNoPrimaryKey
 
     def is_match(self, error: django_db.IntegrityError) -> bool:
         if not isinstance(error.__cause__, psycopg.errors.UniqueViolation):
             return False
 
-        match = self._pattern.match(error.__cause__.diag.message_detail)
+        match = self._pattern.match(error.__cause__.diag.message_detail or "")
         if match is None:
             return False
 
         # The assert below informs Mypy that self.model._meta.pk is not None.
         # This has been enforced in __post_init__,
         # so this should never raise an error in practice.
         assert self.model._meta.pk is not None
@@ -175,15 +178,17 @@
         r"Key \((?P<field>.+)\)=\((?P<value>.+)\) is not present in table"
     )
 
     def is_match(self, error: django_db.IntegrityError) -> bool:
         if not isinstance(error.__cause__, psycopg.errors.ForeignKeyViolation):
             return False
 
-        detail_match = self._detail_pattern.match(error.__cause__.diag.message_detail)
+        detail_match = self._detail_pattern.match(
+            error.__cause__.diag.message_detail or ""
+        )
         if detail_match is None:
             return False
 
         return (
             detail_match.group("field") == self.field
             and error.__cause__.diag.table_name == self.model._meta.db_table
         )
```

### Comparing `django_integrity-0.1.1/src/django_integrity.egg-info/PKG-INFO` & `django_integrity-0.2.0/src/django_integrity.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: django_integrity
-Version: 0.1.1
+Version: 0.2.0
+Summary: Tools for refining Django's IntegrityError, and working with deferred database constraints.
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Kraken Technologies Limited
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -26,42 +27,61 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Project-URL: repository, https://github.com/octoenergy/django-integrity
-Project-URL: changelog, https://github.com/octoenergy/django-integrity/blob/main/CHANGELOG.md
+Project-URL: repository, https://github.com/kraken-tech/django-integrity
+Project-URL: changelog, https://github.com/kraken-tech/django-integrity/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: pytest-in-tox
+Requires-Dist: dj-database-url>=2.1.0; extra == "pytest-in-tox"
+Requires-Dist: django-stubs>=5.0.0; extra == "pytest-in-tox"
+Requires-Dist: environs>=11.0.0; extra == "pytest-in-tox"
+Requires-Dist: pytest-django>=4.8.0; extra == "pytest-in-tox"
+Requires-Dist: pytest>=8.2.0; extra == "pytest-in-tox"
+Provides-Extra: release
+Requires-Dist: packaging>=24.0; extra == "release"
+Requires-Dist: rich>=13.7.1; extra == "release"
+Requires-Dist: tomli>=1.1.0; python_version < "3.11" and extra == "release"
+Requires-Dist: typer>=0.12.3; extra == "release"
+Provides-Extra: tox
+Requires-Dist: tox-uv>=1.8.2; extra == "tox"
+Requires-Dist: tox>=4.15.0; extra == "tox"
 Provides-Extra: dev
-Requires-Dist: dj-database-url; extra == "dev"
-Requires-Dist: django-stubs; extra == "dev"
-Requires-Dist: environs; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-django; extra == "dev"
-Requires-Dist: tox; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mypy-json-report; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: rich; extra == "dev"
+Requires-Dist: dj-database-url>=2.1.0; extra == "dev"
+Requires-Dist: django>=4.2.0; extra == "dev"
+Requires-Dist: django-stubs>=5.0.0; extra == "dev"
+Requires-Dist: environs>=11.0.0; extra == "dev"
+Requires-Dist: psycopg2-binary>=2.9.9; extra == "dev"
+Requires-Dist: psycopg[binary]>=3.1.18; extra == "dev"
+Requires-Dist: pytest-django>=4.8.0; extra == "dev"
+Requires-Dist: pytest>=8.2.0; extra == "dev"
+Requires-Dist: tox>=4.15.0; extra == "dev"
+Requires-Dist: types-psycopg2>=2.9.21.20240417; extra == "dev"
+Requires-Dist: mypy>=1.10.0; extra == "dev"
+Requires-Dist: mypy-json-report>=1.2.0; extra == "dev"
+Requires-Dist: pre-commit>=3.7.0; extra == "dev"
+Requires-Dist: packaging>=24.0; extra == "dev"
+Requires-Dist: rich>=13.7.1; extra == "dev"
 Requires-Dist: tomli>=1.1.0; python_version < "3.11" and extra == "dev"
-Requires-Dist: typer; extra == "dev"
+Requires-Dist: typer>=0.12.3; extra == "dev"
 
 # Django Integrity
 
 Django Integrity contains tools for controlling deferred constraints
 and handling `IntegrityError`s in Django projects which use PostgreSQL.
 
 ## Deferrable constraints
@@ -137,19 +157,19 @@
     Creates a user with the provided email address.
 
     Raises:
         UserAlreadyExists: If the email was not unique.
         EmailCannotBeNull: If the email was None.
         EmailMustBeLowerCase: If the email had a non-lowercase character.
     """
-    rules = {
-        conversion.Unique(model=User, fields=("email",)): UserAlreadyExists,
-        conversion.NotNull(model=User, field="email"): EmailCannotBeNull,
-        conversion.Named(name="constraint_islowercase"): EmailMustBeLowerCase,
-    }
+    rules = [
+        (conversion.Unique(model=User, fields=("email",)), UserAlreadyExists),
+        (conversion.NotNull(model=User, field="email"), EmailCannotBeNull),
+        (conversion.Named(name="constraint_islowercase"), EmailMustBeLowerCase),
+    ]
     with conversion.refine_integrity_error(rules):
         User.objects.create(email=email)
 ```
 
 ## Supported dependencies
 
 This package is tested against:
```

