# Comparing `tmp/django_tailwind_cli-2.8.1.tar.gz` & `tmp/django_tailwind_cli-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tailwind_cli-2.8.1.tar", max compression
+gzip compressed data, was "django_tailwind_cli-2.9.0.tar", max compression
```

## Comparing `django_tailwind_cli-2.8.1.tar` & `django_tailwind_cli-2.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1071 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/LICENSE
--rw-r--r--   0        0        0     3163 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/README.md
--rw-r--r--   0        0        0     3466 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/pyproject.toml
--rw-r--r--   0        0        0       78 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/__init__.py
--rw-r--r--   0        0        0      168 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/apps.py
--rw-r--r--   0        0        0        0 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/management/__init__.py
--rw-r--r--   0        0        0        0 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/management/commands/__init__.py
--rw-r--r--   0        0        0    14594 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/management/commands/tailwind.py
--rw-r--r--   0        0        0        0 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/py.typed
--rw-r--r--   0        0        0      572 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/templates/tailwind_cli/base.html
--rw-r--r--   0        0        0      263 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
--rw-r--r--   0        0        0        0 2024-01-09 14:49:43.603150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/templatetags/__init__.py
--rw-r--r--   0        0        0      483 2024-01-09 14:49:43.607150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/templatetags/tailwind_cli.py
--rw-r--r--   0        0        0     3963 2024-01-09 14:49:43.607150 django_tailwind_cli-2.8.1/src/django_tailwind_cli/utils.py
--rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 django_tailwind_cli-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/LICENSE
+-rw-r--r--   0        0        0     3163 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/README.md
+-rw-r--r--   0        0        0     3428 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/__init__.py
+-rw-r--r--   0        0        0      168 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/apps.py
+-rw-r--r--   0        0        0        0 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/management/commands/__init__.py
+-rw-r--r--   0        0        0    12850 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/management/commands/tailwind.py
+-rw-r--r--   0        0        0        0 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/py.typed
+-rw-r--r--   0        0        0      572 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/templates/tailwind_cli/base.html
+-rw-r--r--   0        0        0      263 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/templates/tailwind_cli/tailwind_css.html
+-rw-r--r--   0        0        0        0 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/templatetags/__init__.py
+-rw-r--r--   0        0        0      482 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/templatetags/tailwind_cli.py
+-rw-r--r--   0        0        0     3891 2024-03-10 20:06:04.985489 django_tailwind_cli-2.9.0/src/django_tailwind_cli/utils.py
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 django_tailwind_cli-2.9.0/PKG-INFO
```

### Comparing `django_tailwind_cli-2.8.1/LICENSE` & `django_tailwind_cli-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.8.1/README.md` & `django_tailwind_cli-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 - Necessary configuration to adapt the library to your project, when the defaults don't fit you.
 - A template tag to include the Tailwind CSS file in your project.
 - A base template for your project.
 - A sane tailwind.config.js that activates all the official plugins and includes a simple HTMX plugin.
 
 ## Requirements
 
-Python 3.8 or newer with Django >= 3.2.
+Python 3.9 or newer with Django >= 3.2.
 
 ## Documentation
 
 The documentation can be found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-cli.andrich.me/)
 
 ## Contributing
```

#### html2text {}

```diff
@@ -28,15 +28,15 @@
 - Simplest possible integration. - Management commands: - To start the Tailwind
 CLI in watch mode during development. - To build the production grade CSS file
 for your project. - To start a debug server along with the Tailwind CLI in
 watch mode in a single session. - Necessary configuration to adapt the library
 to your project, when the defaults don't fit you. - A template tag to include
 the Tailwind CSS file in your project. - A base template for your project. - A
 sane tailwind.config.js that activates all the official plugins and includes a
-simple HTMX plugin. ## Requirements Python 3.8 or newer with Django >= 3.2. ##
+simple HTMX plugin. ## Requirements Python 3.9 or newer with Django >= 3.2. ##
 Documentation The documentation can be found at [https://django-tailwind-
 cli.andrich.me/](https://django-tailwind-cli.andrich.me/) ## Contributing If
 you want to contribute to this project, checkout the [development guide](https:
 //django-tailwind-cli.andrich.me/development/) for details to get your dev
 environment up and running. ## License This software is licensed under [MIT
 license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/
 LICENSE).
```

### Comparing `django_tailwind_cli-2.8.1/pyproject.toml` & `django_tailwind_cli-2.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 [tool.poetry]
 name = "django-tailwind-cli"
-version = "2.8.1"
+version = "2.9.0"
 description = "Django and Tailwind integration based on the prebuilt Tailwind CSS CLI."
 authors = ["Oliver Andrich <oliver@andrich.me>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://django-tailwind-cli.andrich.me/"
 repository = "https://github.com/oliverandrich/django-tailwind-cli"
 documentation = "https://django-tailwind-cli.andrich.me/"
 keywords = ["django", "tailwind", "css"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries",
   "Topic :: Utilities",
   "Environment :: Web Environment",
   "Framework :: Django :: 3.2",
-  "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
 ]
 packages = [{ include = "django_tailwind_cli", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+python = "^3.9"
 django = ">=3.2"
-certifi = "^2023.7.22"
+certifi = ">=2023.7.22,<2025.0.0"
 django-extensions = { version = "^3.2.1", optional = true }
 werkzeug = { version = "^3.0.0", optional = true }
+django-typer = "^1.0.3"
 
 [tool.poetry.extras]
 "django-extensions" = ["django-extensions", "werkzeug"]
 
 [tool.poetry.group.dev.dependencies]
-django-types = ">=0.17,<0.20"
 mkdocs-material = "^9.3.1"
 coverage = { extras = ["toml"], version = "^7.3.2" }
-pytest = "^7.4.2"
+pytest = ">=7.4.2,<9.0.0"
 pytest-django = "^4.5.2"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.12.0"
-tox = "^4.11.4"
+django-types = "^0.19.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Black
 [tool.black]
-target-version = ["py38"]
-line-length = 100
+target-version = ["py39"]
+line-length = 120
 skip-string-normalization = true
 exclude = '''
 /(
     \.git
   | \.tox
   | \.venv
   | _build
@@ -68,66 +66,45 @@
   | dist
   | ^.*\b(migrations)\b.*$
 )/
 '''
 
 # Pyright
 [tool.pyright]
-pythonVersion = "3.8"
+venvPath = "."
+venv = ".venv"
 typeCheckingMode = "strict"
-venvPath = ".venv"
-venv = "."
+ignore = ["./tests/**/*"]
 
 # Ruff
 [tool.ruff]
-target-version = "py38"
-line-length = 100
+target-version = "py39"
+line-length = 120
 select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DJ",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
+  "A",   # flake8-builtins
+  "ARG", # flake8-unused-arguments
+  "B",   # flake8-bugbear
+  "C4",  # flake8-comprehensions
+  "DJ",  # flake8-django
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "FBT", # flake8-boolean-trap
+  "N",   # pep8-naming
+  "Q",   # flake8-quotes
+  "TID", # flake8-tidy-imports
+  "W",   # pycodestyle
+  "YTT", # flake8-2020
 ]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
-  # Ignore checks for possible passwords
-  "S105",
-  "S106",
-  "S107",
   # Ignore complexity
   "C901",
-  "PLR0911",
-  "PLR0912",
-  "PLR0913",
-  "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
   # Don't touch unused variables
   "F841",
 ]
```

### Comparing `django_tailwind_cli-2.8.1/src/django_tailwind_cli/templates/tailwind_cli/base.html` & `django_tailwind_cli-2.9.0/src/django_tailwind_cli/templates/tailwind_cli/base.html`

 * *Files identical despite different names*

### Comparing `django_tailwind_cli-2.8.1/src/django_tailwind_cli/utils.py` & `django_tailwind_cli-2.9.0/src/django_tailwind_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 import os
 import platform
 from pathlib import Path
 from typing import Tuple, Union
 
 from django.conf import settings
 
-x: int = 1
-
 
 class Config:
     """Configuration for the Tailwind CSS CLI."""
 
     @property
     def tailwind_version(self) -> str:
-        return getattr(settings, "TAILWIND_CLI_VERSION", "3.4.0")
+        return getattr(settings, "TAILWIND_CLI_VERSION", "3.4.1")
 
     @property
     def cli_path(self) -> Union[Path, None]:
         p = getattr(settings, "TAILWIND_CLI_PATH", "~/.local/bin/")
         if p is None:
             return p
         return Path(p).expanduser()
@@ -76,20 +74,15 @@
             f"v{self.tailwind_version}/tailwindcss-{system}-{machine}{extension}"
         )
 
     def get_full_cli_path(self) -> Path:
         """Get path to the Tailwind CSS CLI."""
 
         # If Tailwind CSS CLI path points to an existing executable use is.
-        if (
-            self.cli_path
-            and self.cli_path.exists()
-            and self.cli_path.is_file()
-            and os.access(self.cli_path, os.X_OK)
-        ):
+        if self.cli_path and self.cli_path.exists() and self.cli_path.is_file() and os.access(self.cli_path, os.X_OK):
             return self.cli_path
 
         # Otherwise try to calculate the full cli path as usual.
         system, machine = self.get_system_and_machine()
         extension = ".exe" if system == "windows" else ""
         executable_name = f"tailwindcss-{system}-{machine}-{self.tailwind_version}{extension}"
         if self.cli_path is None:
```

### Comparing `django_tailwind_cli-2.8.1/PKG-INFO` & `django_tailwind_cli-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: django-tailwind-cli
-Version: 2.8.1
+Version: 2.9.0
 Summary: Django and Tailwind integration based on the prebuilt Tailwind CSS CLI.
 Home-page: https://django-tailwind-cli.andrich.me/
 License: MIT
 Keywords: django,tailwind,css
 Author: Oliver Andrich
 Author-email: oliver@andrich.me
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Provides-Extra: django-extensions
-Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
+Requires-Dist: certifi (>=2023.7.22,<2025.0.0)
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-extensions (>=3.2.1,<4.0.0) ; extra == "django-extensions"
+Requires-Dist: django-typer (>=1.0.3,<2.0.0)
 Requires-Dist: werkzeug (>=3.0.0,<4.0.0) ; extra == "django-extensions"
 Project-URL: Documentation, https://django-tailwind-cli.andrich.me/
 Project-URL: Repository, https://github.com/oliverandrich/django-tailwind-cli
 Description-Content-Type: text/markdown
 
 # django-tailwind-cli
 
@@ -101,15 +100,15 @@
 - Necessary configuration to adapt the library to your project, when the defaults don't fit you.
 - A template tag to include the Tailwind CSS file in your project.
 - A base template for your project.
 - A sane tailwind.config.js that activates all the official plugins and includes a simple HTMX plugin.
 
 ## Requirements
 
-Python 3.8 or newer with Django >= 3.2.
+Python 3.9 or newer with Django >= 3.2.
 
 ## Documentation
 
 The documentation can be found at [https://django-tailwind-cli.andrich.me/](https://django-tailwind-cli.andrich.me/)
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,63 +1,62 @@
-Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.8.1 Summary: Django
+Metadata-Version: 2.1 Name: django-tailwind-cli Version: 2.9.0 Summary: Django
 and Tailwind integration based on the prebuilt Tailwind CSS CLI. Home-page:
 https://django-tailwind-cli.andrich.me/ License: MIT Keywords:
 django,tailwind,css Author: Oliver Andrich Author-email: oliver@andrich.me
-Requires-Python: >=3.8.1,<4.0.0 Classifier: Development Status :: 5 -
-Production/Stable Classifier: Environment :: Web Environment Classifier:
-Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.1 Classifier:
-Framework :: Django :: 4.2 Classifier: Framework :: Django :: 5.0 Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8 Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Utilities Provides-Extra: django-
-extensions Requires-Dist: certifi (>=2023.7.22,<2024.0.0) Requires-Dist: django
-(>=3.2) Requires-Dist: django-extensions (>=3.2.1,<4.0.0) ; extra == "django-
-extensions" Requires-Dist: werkzeug (>=3.0.0,<4.0.0) ; extra == "django-
-extensions" Project-URL: Documentation, https://django-tailwind-cli.andrich.me/
-Project-URL: Repository, https://github.com/oliverandrich/django-tailwind-cli
-Description-Content-Type: text/markdown # django-tailwind-cli ![GitHub Workflow
-Status](https://img.shields.io/github/actions/workflow/status/oliverandrich/
-django-tailwind-cli/test.yml?style=flat-square) [![PyPI](https://
-img.shields.io/pypi/v/django-tailwind-cli.svg?style=flat-square)](https://
-pypi.org/project/django-tailwind-cli/) [![Code style: black](https://
-img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://
-github.com/psf/black) ![GitHub](https://img.shields.io/github/license/
-oliverandrich/django-tailwind-cli?style=flat-square) [![Poetry](https://
-img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json&style=flat-
-square)](https://python-poetry.org/) This library provides an integration of
-[Tailwind CSS](https://tailwindcss.com) for Django that is using on the
-precompiled versions of the [Tailwind CSS CLI](https://tailwindcss.com/blog/
-standalone-cli). The goal of this library is to provided the simplest possible
-Tailwind integration for your Django project. It took its inspiration from the
-[Tailwind integration for Phoenix](https://github.com/phoenixframework/
-tailwind) which completely skips the neccesity of a node installation. ##
-Installation 1. Install the library. ```shell python -m pip install django-
-tailwind-cli ``` 2. Add `django_tailwind_cli` to `INSTALLED_APPS` in
-`settings.py`. ```python INSTALLED_APPS = [ # other Django apps
-"django_tailwind_cli", ] ``` 3. Configure the `STATICFILES_DIRS` parameter in
-your `settings.py` if not already configured. ```python STATICFILES_DIRS =
+Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Environment :: Web Environment Classifier: Framework ::
+Django :: 3.2 Classifier: Framework :: Django :: 4.2 Classifier: Framework ::
+Django :: 5.0 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Utilities Provides-Extra: django-extensions
+Requires-Dist: certifi (>=2023.7.22,<2025.0.0) Requires-Dist: django (>=3.2)
+Requires-Dist: django-extensions (>=3.2.1,<4.0.0) ; extra == "django-
+extensions" Requires-Dist: django-typer (>=1.0.3,<2.0.0) Requires-Dist:
+werkzeug (>=3.0.0,<4.0.0) ; extra == "django-extensions" Project-URL:
+Documentation, https://django-tailwind-cli.andrich.me/ Project-URL: Repository,
+https://github.com/oliverandrich/django-tailwind-cli Description-Content-Type:
+text/markdown # django-tailwind-cli ![GitHub Workflow Status](https://
+img.shields.io/github/actions/workflow/status/oliverandrich/django-tailwind-
+cli/test.yml?style=flat-square) [![PyPI](https://img.shields.io/pypi/v/django-
+tailwind-cli.svg?style=flat-square)](https://pypi.org/project/django-tailwind-
+cli/) [![Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg?style=flat-square)](https://github.com/psf/black) ![GitHub](https://
+img.shields.io/github/license/oliverandrich/django-tailwind-cli?style=flat-
+square) [![Poetry](https://img.shields.io/endpoint?url=https://python-
+poetry.org/badge/v0.json&style=flat-square)](https://python-poetry.org/) This
+library provides an integration of [Tailwind CSS](https://tailwindcss.com) for
+Django that is using on the precompiled versions of the [Tailwind CSS CLI]
+(https://tailwindcss.com/blog/standalone-cli). The goal of this library is to
+provided the simplest possible Tailwind integration for your Django project. It
+took its inspiration from the [Tailwind integration for Phoenix](https://
+github.com/phoenixframework/tailwind) which completely skips the neccesity of a
+node installation. ## Installation 1. Install the library. ```shell python -
+m pip install django-tailwind-cli ``` 2. Add `django_tailwind_cli` to
+`INSTALLED_APPS` in `settings.py`. ```python INSTALLED_APPS = [ # other Django
+apps "django_tailwind_cli", ] ``` 3. Configure the `STATICFILES_DIRS` parameter
+in your `settings.py` if not already configured. ```python STATICFILES_DIRS =
 [BASE_DIR / "assets"] ``` 4. Add template code. ```htmldjango {% load
 tailwind_cli %} ...
 ... {% tailwind_css %} ...
 ``` 5. Start the debug server. ```shell python manage.py tailwind runserver ```
 Enjoy! Checkout the detailed [installation guide](https://django-tailwind-
 cli.andrich.me/installation/) if you want to activate browser reload or the
 `runserver_plus` management command known from `django-extensions`. ## Features
 - Simplest possible integration. - Management commands: - To start the Tailwind
 CLI in watch mode during development. - To build the production grade CSS file
 for your project. - To start a debug server along with the Tailwind CLI in
 watch mode in a single session. - Necessary configuration to adapt the library
 to your project, when the defaults don't fit you. - A template tag to include
 the Tailwind CSS file in your project. - A base template for your project. - A
 sane tailwind.config.js that activates all the official plugins and includes a
-simple HTMX plugin. ## Requirements Python 3.8 or newer with Django >= 3.2. ##
+simple HTMX plugin. ## Requirements Python 3.9 or newer with Django >= 3.2. ##
 Documentation The documentation can be found at [https://django-tailwind-
 cli.andrich.me/](https://django-tailwind-cli.andrich.me/) ## Contributing If
 you want to contribute to this project, checkout the [development guide](https:
 //django-tailwind-cli.andrich.me/development/) for details to get your dev
 environment up and running. ## License This software is licensed under [MIT
 license](https://github.com/oliverandrich/django-tailwind-cli/blob/main/
 LICENSE).
```

