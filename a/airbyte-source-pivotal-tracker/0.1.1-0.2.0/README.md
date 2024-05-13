# Comparing `tmp/airbyte-source-pivotal-tracker-0.1.1.tar.gz` & `tmp/airbyte_source_pivotal_tracker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-pivotal-tracker-0.1.1.tar", last modified: Wed Jan 31 15:42:06 2024, max compression
+gzip compressed data, was "airbyte_source_pivotal_tracker-0.2.0.tar", max compression
```

## Comparing `airbyte-source-pivotal-tracker-0.1.1.tar` & `airbyte_source_pivotal_tracker-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.350868 airbyte-source-pivotal-tracker-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     5585 2024-01-31 15:42:06.350868 airbyte-source-pivotal-tracker-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5507 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.346868 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5585 2024-01-31 15:42:06.000000 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1463 2024-01-31 15:42:06.000000 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 15:42:06.000000 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2024-01-31 15:42:06.000000 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-01-31 15:42:06.000000 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-31 15:42:06.000000 airbyte-source-pivotal-tracker-0.1.1/airbyte_source_pivotal_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.342868 airbyte-source-pivotal-tracker-0.1.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)    13797 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1581 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     5418 2024-01-31 15:42:06.350868 airbyte-source-pivotal-tracker-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      973 2024-01-31 15:42:04.000000 airbyte-source-pivotal-tracker-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.342868 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/
--rw-r--r--   0 root         (0) root         (0)      140 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      255 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.346868 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/
--rw-r--r--   0 root         (0) root         (0)     1653 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/activity.json
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/epics.json
--rw-r--r--   0 root         (0) root         (0)       83 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/labels.json
--rw-r--r--   0 root         (0) root         (0)      978 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/project_memberships.json
--rw-r--r--   0 root         (0) root         (0)     2157 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/projects.json
--rw-r--r--   0 root         (0) root         (0)      894 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/releases.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.346868 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/shared/
--rw-r--r--   0 root         (0) root         (0)      445 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/shared/label.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/shared/person.json
--rw-r--r--   0 root         (0) root         (0)     1366 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/schemas/stories.json
--rw-r--r--   0 root         (0) root         (0)     5247 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/source.py
--rw-r--r--   0 root         (0) root         (0)      488 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/source_pivotal_tracker/spec.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.346868 airbyte-source-pivotal-tracker-0.1.1/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      881 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:42:06.346868 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/
--rw-r--r--   0 root         (0) root         (0)    48626 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/activity.json
--rw-r--r--   0 root         (0) root         (0)     2184 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/epics.json
--rw-r--r--   0 root         (0) root         (0)     1592 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/labels.json
--rw-r--r--   0 root         (0) root         (0)     4040 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/project_memberships.json
--rw-r--r--   0 root         (0) root         (0)     2174 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/projects.json
--rw-r--r--   0 root         (0) root         (0)      407 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/releases.json
--rw-r--r--   0 root         (0) root         (0)      904 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/responses/stories.json
--rw-r--r--   0 root         (0) root         (0)      860 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     3352 2024-01-31 15:33:11.000000 airbyte-source-pivotal-tracker-0.1.1/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4657 2024-05-13 09:19:34.000000 airbyte_source_pivotal_tracker-0.2.0/README.md
+-rw-r--r--   0        0        0      143 2024-05-13 09:19:34.000000 airbyte_source_pivotal_tracker-0.2.0/main.py
+-rw-r--r--   0        0        0      830 2024-05-13 09:41:05.262278 airbyte_source_pivotal_tracker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      140 2024-05-13 09:19:34.000000 airbyte_source_pivotal_tracker-0.2.0/source_pivotal_tracker/__init__.py
+-rw-r--r--   0        0        0    20335 2024-05-13 09:19:34.000000 airbyte_source_pivotal_tracker-0.2.0/source_pivotal_tracker/manifest.yaml
+-rw-r--r--   0        0        0      255 2024-05-13 09:19:34.000000 airbyte_source_pivotal_tracker-0.2.0/source_pivotal_tracker/run.py
+-rw-r--r--   0        0        0      483 2024-05-13 09:19:34.000000 airbyte_source_pivotal_tracker-0.2.0/source_pivotal_tracker/source.py
+-rw-r--r--   0        0        0     5386 1970-01-01 00:00:00.000000 airbyte_source_pivotal_tracker-0.2.0/PKG-INFO
```

### Comparing `airbyte-source-pivotal-tracker-0.1.1/PKG-INFO` & `airbyte_source_pivotal_tracker-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,126 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pivotal-tracker
-Version: 0.1.1
-Summary: Source implementation for Pivotal Tracker.
+Version: 0.2.0
+Summary: Source implementation for pivotal-tracker.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pivotal-tracker
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: responses~=0.13.3; extra == "tests"
 
 # Pivotal Tracker Source
 
-This is the repository for the Pivotal Tracker source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/pivotal-tracker).
+This is the repository for the Pivotal Tracker configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pivotal-tracker).
 
+## Local development
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+### Prerequisites
 
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/pivotal-tracker)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pivotal_tracker/spec.json` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pivotal-tracker)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pivotal-tracker test creds`
-and place them into `secrets/config.json`.
+
+### Locally running the connector
+
 
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-pivotal-tracker spec
+poetry run source-pivotal-tracker check --config secrets/config.json
+poetry run source-pivotal-tracker discover --config secrets/config.json
+poetry run source-pivotal-tracker read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-pivotal-tracker build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-pivotal-tracker:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-pivotal-tracker:dev .
+airbyte-ci connectors --name=source-pivotal-tracker build
 ```
 
+An image will be available on your host with the tag `airbyte/source-pivotal-tracker:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-pivotal-tracker:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pivotal-tracker:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pivotal-tracker:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pivotal-tracker:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-pivotal-tracker test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pivotal-tracker test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pivotal-tracker.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pivotal-tracker.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-pivotal-tracker-0.1.1/README.md` & `airbyte_source_pivotal_tracker-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,107 @@
 # Pivotal Tracker Source
 
-This is the repository for the Pivotal Tracker source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/pivotal-tracker).
+This is the repository for the Pivotal Tracker configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pivotal-tracker).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
 
-#### Minimum Python version required `= 3.7.0`
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/pivotal-tracker)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pivotal_tracker/spec.json` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pivotal-tracker)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pivotal-tracker test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
+
+
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-pivotal-tracker spec
+poetry run source-pivotal-tracker check --config secrets/config.json
+poetry run source-pivotal-tracker discover --config secrets/config.json
+poetry run source-pivotal-tracker read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
-### Locally running the connector docker image
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-pivotal-tracker build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-pivotal-tracker:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-pivotal-tracker:dev .
+airbyte-ci connectors --name=source-pivotal-tracker build
 ```
 
-#### Run
+An image will be available on your host with the tag `airbyte/source-pivotal-tracker:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-pivotal-tracker:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pivotal-tracker:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pivotal-tracker:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pivotal-tracker:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-pivotal-tracker test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
-### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pivotal-tracker test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pivotal-tracker.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pivotal-tracker.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

