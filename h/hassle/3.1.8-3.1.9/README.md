# Comparing `tmp/hassle-3.1.8.tar.gz` & `tmp/hassle-3.1.9.tar.gz`

## Comparing `hassle-3.1.8.tar` & `hassle-3.1.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/__init__.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/hassle_cli.py
--rw-r--r--   0        0        0    19939 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/models.py
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/py.typed
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/utilities.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/templates/.gitignore.txt
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/templates/license.txt
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/templates/pyproject.toml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-3.1.8/src/hassle/templates/vscode_settings.json
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hassle-3.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-3.1.8/LICENSE.txt
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 hassle-3.1.8/README.md
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 hassle-3.1.8/pyproject.toml
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 hassle-3.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7655 2020-02-02 00:00:00.000000 hassle-3.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/__init__.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/hassle_cli.py
+-rw-r--r--   0        0        0    19382 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/models.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/py.typed
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/utilities.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/templates/.gitignore.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/templates/README.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/templates/license.txt
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/templates/pyproject.toml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 hassle-3.1.9/src/hassle/templates/vscode_settings.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hassle-3.1.9/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hassle-3.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 hassle-3.1.9/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 hassle-3.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 hassle-3.1.9/PKG-INFO
```

### Comparing `hassle-3.1.8/src/hassle/models.py` & `hassle-3.1.9/src/hassle/models.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,557 +1,557 @@
-import subprocess
-from dataclasses import asdict, dataclass, field
-from datetime import datetime
-from functools import cached_property
-from typing import Any
-
-import black
-import dacite
-import isort
-import requests
-from bs4 import BeautifulSoup, Tag
-from packagelister import packagelister
-from pathier import Pathier, Pathish
-from typing_extensions import Self
-
-from hassle import utilities
-
-root = Pathier(__file__).parent
-
-
-@dataclass
-class Sdist:
-    exclude: list[str]
-
-
-@dataclass
-class Targets:
-    sdist: Sdist
-
-
-@dataclass
-class Build:
-    targets: Targets
-
-
-@dataclass
-class BuildSystem:
-    requires: list[str]
-    build_backend: str
-
-
-@dataclass
-class Urls:
-    Homepage: str = ""
-    Documentation: str = ""
-    Source_code: str = ""
-
-
-@dataclass
-class Author:
-    name: str = ""
-    email: str = ""
-
-
-@dataclass
-class Git:
-    tag_prefix: str = ""
-
-
-@dataclass
-class IniOptions:
-    addopts: list[str]
-    pythonpath: str
-
-
-@dataclass
-class Pytest:
-    ini_options: IniOptions
-
-
-@dataclass
-class Hatch:
-    build: Build
-
-
-@dataclass
-class Tool:
-    pytest: Pytest
-    hatch: Hatch
-
-
-@dataclass
-class Project:
-    name: str
-    authors: list[Author] = field(default_factory=list)
-    description: str = ""
-    requires_python: str = ""
-    version: str = ""
-    dependencies: list[str] = field(default_factory=list)
-    readme: str = ""
-    keywords: list[str] = field(default_factory=list)
-    classifiers: list[str] = field(default_factory=list)
-    urls: Urls = field(default_factory=Urls)
-    scripts: dict[str, str] = field(default_factory=dict)
-
-
-@dataclass
-class Pyproject:
-    build_system: BuildSystem
-    project: Project
-    tool: Tool
-
-    @staticmethod
-    def _swap_keys(data: dict[str, Any]) -> dict[str, Any]:
-        """Swap between original toml key and valid Python variable."""
-        if "build-system" in data:
-            data = utilities.swap_keys(data, ("build-system", "build_system"))
-            if "build-backend" in data["build_system"]:
-                data["build_system"] = utilities.swap_keys(
-                    data["build_system"], ("build-backend", "build_backend")
-                )
-        elif "build_system" in data:
-            data = utilities.swap_keys(data, ("build-system", "build_system"))
-            if "build_backend" in data["build-system"]:
-                data["build-system"] = utilities.swap_keys(
-                    data["build-system"], ("build-backend", "build_backend")
-                )
-
-        if "project" in data and (
-            "requires-python" in data["project"] or "requires_python"
-        ):
-            data["project"] = utilities.swap_keys(
-                data["project"], ("requires-python", "requires_python")
-            )
-        if all(
-            [
-                "project" in data,
-                "urls" in data["project"],
-                (
-                    "Source code" in data["project"]["urls"]
-                    or "Source_code" in data["project"]["urls"]
-                ),
-            ]
-        ):
-            data["project"]["urls"] = utilities.swap_keys(
-                data["project"]["urls"], ("Source code", "Source_code")
-            )
-
-        return data
-
-    @classmethod
-    def load(cls, path: Pathish = Pathier("pyproject.toml")) -> Self:
-        """Return a `datamodel` object populated from `path`."""
-        data = Pathier(path).loads()
-        data = cls._swap_keys(data)
-        return dacite.from_dict(cls, data)
-
-    def dump(self, path: Pathish = Pathier("pyproject.toml")):
-        """Write the contents of this `datamodel` object to `path`."""
-        data = asdict(self)
-        data = self._swap_keys(data)
-        Pathier(path).dumps(data)
-
-    @classmethod
-    def from_template(cls) -> Self:
-        """Return a `Pyproject` object using `templates/pyproject_template.toml`."""
-        return cls.load(root / "templates" / "pyproject.toml")
-
-
-@dataclass
-class HassleConfig:
-    authors: list[Author] = field(default_factory=list)
-    project_urls: Urls = field(default_factory=Urls)
-    git: Git = field(default_factory=Git)
-
-    @classmethod
-    def load(
-        cls, path: Pathish = Pathier(__file__).parent / "hassle_config.toml"
-    ) -> Self:
-        """Return a `datamodel` object populated from `path`."""
-        path = Pathier(path)
-        if not path.exists():
-            raise FileNotFoundError(
-                f"Could not find hassle config at {path}.\nRun hassle_config in a terminal to set it."
-            )
-        data = path.loads()
-        data["project_urls"] = utilities.swap_keys(
-            data["project_urls"], ("Source_code", "Source code")
-        )
-        return dacite.from_dict(cls, data)
-
-    def dump(self, path: Pathish = Pathier(__file__).parent / "hassle_config.toml"):
-        """Write the contents of this `datamodel` object to `path`."""
-        data = asdict(self)
-        data["project_urls"] = utilities.swap_keys(
-            data["project_urls"], ("Source_code", "Source code")
-        )
-        Pathier(path).dumps(data)
-
-    @staticmethod
-    def warn():
-        print("hassle_config.toml has not been set.")
-        print("Run hassle_config to set it.")
-        print("Run 'hassle config -h' for help.")
-
-    @staticmethod
-    def exists(path: Pathish = Pathier(__file__).parent / "hassle_config.toml") -> bool:
-        return Pathier(path).exists()
-
-    @classmethod
-    def configure(
-        cls,
-        name: str | None = None,
-        email: str | None = None,
-        github_username: str | None = None,
-        docs_url: str | None = None,
-        tag_prefix: str | None = None,
-        config_path: Pathish = Pathier(__file__).parent / "hassle_config.toml",
-    ):
-        """Create or edit `hassle_config.toml` from given params."""
-        print(f"Manual edits can be made at {config_path}")
-        if not cls.exists(config_path):
-            config = cls()
-        else:
-            config = cls.load(config_path)
-        # Add an author to config if a name or email is given.
-        if name or email:
-            config.authors.append(Author(name or "", email or ""))
-        if github_username:
-            homepage = f"https://github.com/{github_username}/$name"
-            config.project_urls.Homepage = homepage
-            config.project_urls.Source_code = f"{homepage}/tree/main/src/$name"
-        if not config.project_urls.Documentation:
-            if github_username and not docs_url:
-                config.project_urls.Documentation = (
-                    f"https://github.com/{github_username}/$name/tree/main/docs"
-                )
-            elif docs_url:
-                config.project_urls.Documentation = docs_url
-        if tag_prefix:
-            config.git.tag_prefix = tag_prefix
-        config.dump(config_path)
-
-
-@dataclass
-class HassleProject:
-    pyproject: Pyproject
-    projectdir: Pathier
-    source_files: list[str]
-    templatedir: Pathier = root / "templates"
-
-    @property
-    def source_code(self) -> str:
-        """Join and return all code from any `.py` files in `self.srcdir`.
-
-        Useful if a tool needs to scan all the source code for something."""
-        return "\n".join(file.read_text() for file in self.srcdir.rglob("*.py"))
-
-    @cached_property
-    def srcdir(self) -> Pathier:
-        return self.projectdir / "src" / self.pyproject.project.name
-
-    @cached_property
-    def changelog_path(self) -> Pathier:
-        return self.projectdir / "CHANGELOG.md"
-
-    @cached_property
-    def pyproject_path(self) -> Pathier:
-        return self.projectdir / "pyproject.toml"
-
-    @cached_property
-    def docsdir(self) -> Pathier:
-        return self.projectdir / "docs"
-
-    @cached_property
-    def testsdir(self) -> Pathier:
-        return self.projectdir / "tests"
-
-    @cached_property
-    def vsdir(self) -> Pathier:
-        return self.projectdir / ".vscode"
-
-    @cached_property
-    def distdir(self) -> Pathier:
-        return self.projectdir / "dist"
-
-    @property
-    def name(self) -> str:
-        """This package's name."""
-        return self.pyproject.project.name
-
-    @property
-    def version(self) -> str:
-        """This package's version."""
-        return self.pyproject.project.version
-
-    @version.setter
-    def version(self, new_version: str):
-        self.pyproject.project.version = new_version
-
-    @classmethod
-    def load(cls, projectdir: Pathish) -> Self:
-        """Load a project given `projectdir`."""
-        projectdir = Pathier(projectdir)
-        pyproject = Pyproject.load(projectdir / "pyproject.toml")
-        name = pyproject.project.name
-        # Convert source files to path stems relative to projectdir/src/name
-        # e.g `C:/python/projects/hassle/src/hassle/templates/pyproject.toml`
-        # becomes `templates/pyproject.toml`
-        source_files = [
-            str(file.separate(name))
-            for file in (projectdir / "src" / name).rglob("*")
-            if file.is_file()
-        ]
-        return cls(pyproject, projectdir, source_files)
-
-    @classmethod
-    def new(
-        cls,
-        targetdir: Pathier,
-        name: str,
-        description: str = "",
-        dependencies: list[str] = [],
-        keywords: list[str] = [],
-        source_files: list[str] = [],
-        add_script: bool = False,
-        no_license: bool = False,
-    ) -> Self:
-        """Create and return a new hassle project."""
-        pyproject = Pyproject.from_template()
-        config = HassleConfig.load()
-        pyproject.project.name = name
-        pyproject.project.authors = config.authors
-        pyproject.project.description = description
-        pyproject.project.dependencies = dependencies
-        pyproject.project.keywords = keywords
-        pyproject.project.urls.Homepage = config.project_urls.Homepage.replace(
-            "$name", name
-        )
-        pyproject.project.urls.Documentation = (
-            config.project_urls.Documentation.replace("$name", name)
-        )
-        pyproject.project.urls.Source_code = config.project_urls.Source_code.replace(
-            "$name", name
-        )
-        hassle = cls(pyproject, targetdir, source_files)
-        if add_script:
-            hassle.add_script(name, name)
-        hassle.generate_files()
-        if no_license:
-            hassle.pyproject.project.classifiers.pop(1)
-            (hassle.projectdir / "LICENSE.txt").delete()
-        hassle.save()
-        return hassle
-
-    def get_template(self, file_name: str) -> str:
-        """Open are return the content of `{self.templatedir}/{file_name}`."""
-        return (self.templatedir / file_name).read_text()
-
-    def save(self):
-        """Dump `self.pyproject` to `{self.projectdir}/pyproject.toml`."""
-        self.pyproject.dump(self.pyproject_path)
-
-    def format_source_files(self):
-        """Use isort and black to format files"""
-        for file in self.projectdir.rglob("*.py"):
-            isort.file(file)
-        try:
-            black.main([str(self.projectdir)])
-        except SystemExit as e:
-            ...
-        except Exception as e:
-            raise e
-
-    def latest_version_is_published(self) -> bool:
-        """Check if the current version of this project has been published to pypi.org."""
-        pypi_url = f"https://pypi.org/project/{self.name}"
-        response = requests.get(pypi_url)
-        if response.status_code != 200:
-            raise RuntimeError(
-                f"{pypi_url} returned status code {response.status_code} :/"
-            )
-        soup = BeautifulSoup(response.text, "html.parser")
-        header = soup.find("h1", class_="package-header__name")
-        assert isinstance(header, Tag)
-        text = header.text.strip()
-        pypi_version = text[text.rfind(" ") + 1 :]
-        return self.version == pypi_version
-
-    # ====================================================================================
-    # Updaters ===========================================================================
-    # ====================================================================================
-    def add_script(self, name: str, file_stem: str, function: str = "main"):
-        """Add a script to `pyproject.project.scripts` in the format `{name} = "{package_name}.{file_stem}:{function}"`"""
-        self.pyproject.project.scripts[name] = f"{self.name}.{file_stem}:{function}"
-
-    def update_init_version(self):
-        """Update the `__version__` in this projects `__init__.py` file
-        to the current value of `self.pyproject.project.version`
-        if it exists and has a `__version__` string.
-
-        If it doesn't have a `__version__` string, append one to it."""
-        init_file = self.srcdir / "__init__.py"
-        version = f'__version__ = "{self.version}"'
-        if init_file.exists():
-            content = init_file.read_text()
-            if "__version__" in content:
-                lines = content.splitlines()
-                for i, line in enumerate(lines):
-                    if line.startswith("__version__"):
-                        lines[i] = version
-                content = "\n".join(lines)
-            else:
-                content += f"\n{version}"
-            init_file.write_text(content)
-
-    def bump_version(self, bump_type: str):
-        """Bump the version of this project.
-
-        `bump_type` should be `major`, `minor`, or `patch`."""
-        # bump pyproject version
-        self.version = utilities.bump_version(self.version, bump_type)
-        # bump `__version__` in __init__.py if the file exists and has a `__version__`.
-        self.update_init_version()
-
-    def update_dependencies(
-        self, overwrite_existing_packages: bool, include_versions: bool
-    ):
-        """Scan project for dependencies and update the corresponding field in the pyproject model.
-
-        If `overwrite_existing_packages` is `False`, this function will only add a package if it isn't already listed,
-        but won't remove anything currently in the list.
-        Use this option to preserve manually added dependencies."""
-        project = packagelister.scan_dir(self.srcdir)
-        version_conditional = ">=" if include_versions else None
-        if overwrite_existing_packages:
-            self.pyproject.project.dependencies = project.get_formatted_requirements(
-                version_conditional
-            )
-        else:
-            # Only add a package if it isn't already in the dependency list
-            self.pyproject.project.dependencies.extend(
-                [
-                    (
-                        package.get_formatted_requirement(version_conditional)
-                        if version_conditional
-                        else package.distribution_name
-                    )
-                    for package in project.requirements
-                    if all(
-                        package.distribution_name not in existing_dependency
-                        for existing_dependency in self.pyproject.project.dependencies
-                    )
-                ]
-            )
-
-    def _generate_changelog(self) -> list[str]:
-        if HassleConfig.exists():
-            tag_prefix = HassleConfig.load().git.tag_prefix
-        else:
-            HassleConfig.warn()
-            print("Assuming no tag prefix.")
-            tag_prefix = ""
-        raw_changelog = [
-            line
-            for line in subprocess.run(
-                [
-                    "auto-changelog",
-                    "-p",
-                    self.projectdir,
-                    "--tag-prefix",
-                    tag_prefix,
-                    "--stdout",
-                ],
-                stdout=subprocess.PIPE,
-                text=True,
-            ).stdout.splitlines(True)
-            if not line.startswith(
-                (
-                    "Full set of changes:",
-                    f"* build {tag_prefix}",
-                    "* update changelog",
-                )
-            )
-        ]
-        return raw_changelog
-
-    def update_changelog(self):
-        """Update `CHANGELOG.md` by invoking the `auto-changelog` module.
-
-        If `hassle_config.toml` doesn't exist, an empty tag prefix will be assumed."""
-        raw_changelog = self._generate_changelog()
-        # If there's no existing changelog, dump the generated one and get out of here.
-        if not self.changelog_path.exists():
-            self.changelog_path.join(raw_changelog)
-            return
-
-        # Don't want to overwrite previously existing manual changes/edits
-        existing_changelog = self.changelog_path.read_text().splitlines(True)[
-            2:
-        ]  # First two elements are "# Changelog\n" and "\n"
-        new_changes = raw_changelog
-        for line in existing_changelog:
-            # Release headers are prefixed with "## "
-            if line.startswith("## "):
-                new_changes = raw_changelog[: raw_changelog.index(line)]
-                break
-        changes = "".join(new_changes)
-        # "#### OTHERS" gets added to the changelog even when there's nothing for that category,
-        # so we'll get rid of it if that's the case
-        others = "#### Others"
-        if changes.strip("\n").endswith(others):
-            changes = changes.strip("\n").replace(others, "\n\n")
-        # If changes == "# Changelog\n\n" then there weren't actually any new changes
-        if not changes == "# Changelog\n\n":
-            self.changelog_path.write_text(changes + "".join(existing_changelog))
-
-    # ====================================================================================
-    # File/Project creation ==============================================================
-    # ====================================================================================
-
-    def create_source_files(self):
-        """Generate source files in `self.srcdir`."""
-        for file in self.source_files:
-            (self.srcdir / file).touch()
-        init = self.srcdir / "__init__.py"
-        if init.exists():
-            init.append(f'__version__ = "{self.version}"')
-
-    def create_readme(self):
-        readme = self.get_template("README.md")
-        readme = readme.replace("$name", self.name)
-        readme = readme.replace("$description", self.pyproject.project.description)
-        (self.projectdir / "README.md").write_text(readme)
-
-    def create_license(self):
-        license_ = self.get_template("license.txt")
-        license_ = license_.replace("$year", str(datetime.now().year))
-        (self.projectdir / "LICENSE.txt").write_text(license_)
-
-    def create_gitignore(self):
-        (self.templatedir / ".gitignore.txt").copy(self.projectdir / ".gitignore")
-
-    def create_vscode_settings(self):
-        self.vsdir.mkdir()
-        (self.templatedir / "vscode_settings.json").copy(self.vsdir / "settings.json")
-
-    def create_tests(self):
-        (self.testsdir / f"test_{self.name}.py").touch()
-
-    def create_py_typed(self):
-        (self.projectdir / "py.typed").touch()
-
-    def generate_files(self):
-        """Create all the necessary files.
-
-        Note: This will overwrite any existing files."""
-        self.projectdir.mkdir()
-        for func in dir(self):
-            if func.startswith("create_"):
-                getattr(self, func)()
-        self.pyproject.dump(self.pyproject_path)
-
-    def generate_docs(self):
-        """Generate docs by invoking `pdoc`"""
-        self.docsdir.delete()
-        subprocess.run(["pdoc", "-o", self.docsdir, self.srcdir])
+import subprocess
+from dataclasses import asdict, dataclass, field
+from datetime import datetime
+from functools import cached_property
+from typing import Any
+
+import black
+import dacite
+import isort
+import requests
+from bs4 import BeautifulSoup, Tag
+from packagelister import packagelister
+from pathier import Pathier, Pathish
+from typing_extensions import Self
+
+from hassle import utilities
+
+root = Pathier(__file__).parent
+
+
+@dataclass
+class Sdist:
+    exclude: list[str]
+
+
+@dataclass
+class Targets:
+    sdist: Sdist
+
+
+@dataclass
+class Build:
+    targets: Targets
+
+
+@dataclass
+class BuildSystem:
+    requires: list[str]
+    build_backend: str
+
+
+@dataclass
+class Urls:
+    Homepage: str = ""
+    Documentation: str = ""
+    Source_code: str = ""
+
+
+@dataclass
+class Author:
+    name: str = ""
+    email: str = ""
+
+
+@dataclass
+class Git:
+    tag_prefix: str = ""
+
+
+@dataclass
+class IniOptions:
+    addopts: list[str]
+    pythonpath: str
+
+
+@dataclass
+class Pytest:
+    ini_options: IniOptions
+
+
+@dataclass
+class Hatch:
+    build: Build
+
+
+@dataclass
+class Tool:
+    pytest: Pytest
+    hatch: Hatch
+
+
+@dataclass
+class Project:
+    name: str
+    authors: list[Author] = field(default_factory=list)
+    description: str = ""
+    requires_python: str = ""
+    version: str = ""
+    dependencies: list[str] = field(default_factory=list)
+    readme: str = ""
+    keywords: list[str] = field(default_factory=list)
+    classifiers: list[str] = field(default_factory=list)
+    urls: Urls = field(default_factory=Urls)
+    scripts: dict[str, str] = field(default_factory=dict)
+
+
+@dataclass
+class Pyproject:
+    build_system: BuildSystem
+    project: Project
+    tool: Tool
+
+    @staticmethod
+    def _swap_keys(data: dict[str, Any]) -> dict[str, Any]:
+        """Swap between original toml key and valid Python variable."""
+        if "build-system" in data:
+            data = utilities.swap_keys(data, ("build-system", "build_system"))
+            if "build-backend" in data["build_system"]:
+                data["build_system"] = utilities.swap_keys(
+                    data["build_system"], ("build-backend", "build_backend")
+                )
+        elif "build_system" in data:
+            data = utilities.swap_keys(data, ("build-system", "build_system"))
+            if "build_backend" in data["build-system"]:
+                data["build-system"] = utilities.swap_keys(
+                    data["build-system"], ("build-backend", "build_backend")
+                )
+
+        if "project" in data and (
+            "requires-python" in data["project"] or "requires_python"
+        ):
+            data["project"] = utilities.swap_keys(
+                data["project"], ("requires-python", "requires_python")
+            )
+        if all(
+            [
+                "project" in data,
+                "urls" in data["project"],
+                (
+                    "Source code" in data["project"]["urls"]
+                    or "Source_code" in data["project"]["urls"]
+                ),
+            ]
+        ):
+            data["project"]["urls"] = utilities.swap_keys(
+                data["project"]["urls"], ("Source code", "Source_code")
+            )
+
+        return data
+
+    @classmethod
+    def load(cls, path: Pathish = Pathier("pyproject.toml")) -> Self:
+        """Return a `datamodel` object populated from `path`."""
+        data = Pathier(path).loads()
+        data = cls._swap_keys(data)
+        return dacite.from_dict(cls, data)
+
+    def dump(self, path: Pathish = Pathier("pyproject.toml")):
+        """Write the contents of this `datamodel` object to `path`."""
+        data = asdict(self)
+        data = self._swap_keys(data)
+        Pathier(path).dumps(data)
+
+    @classmethod
+    def from_template(cls) -> Self:
+        """Return a `Pyproject` object using `templates/pyproject_template.toml`."""
+        return cls.load(root / "templates" / "pyproject.toml")
+
+
+@dataclass
+class HassleConfig:
+    authors: list[Author] = field(default_factory=list)
+    project_urls: Urls = field(default_factory=Urls)
+    git: Git = field(default_factory=Git)
+
+    @classmethod
+    def load(
+        cls, path: Pathish = Pathier(__file__).parent / "hassle_config.toml"
+    ) -> Self:
+        """Return a `datamodel` object populated from `path`."""
+        path = Pathier(path)
+        if not path.exists():
+            raise FileNotFoundError(
+                f"Could not find hassle config at {path}.\nRun hassle_config in a terminal to set it."
+            )
+        data = path.loads()
+        data["project_urls"] = utilities.swap_keys(
+            data["project_urls"], ("Source_code", "Source code")
+        )
+        return dacite.from_dict(cls, data)
+
+    def dump(self, path: Pathish = Pathier(__file__).parent / "hassle_config.toml"):
+        """Write the contents of this `datamodel` object to `path`."""
+        data = asdict(self)
+        data["project_urls"] = utilities.swap_keys(
+            data["project_urls"], ("Source_code", "Source code")
+        )
+        Pathier(path).dumps(data)
+
+    @staticmethod
+    def warn():
+        print("hassle_config.toml has not been set.")
+        print("Run hassle_config to set it.")
+        print("Run 'hassle config -h' for help.")
+
+    @staticmethod
+    def exists(path: Pathish = Pathier(__file__).parent / "hassle_config.toml") -> bool:
+        return Pathier(path).exists()
+
+    @classmethod
+    def configure(
+        cls,
+        name: str | None = None,
+        email: str | None = None,
+        github_username: str | None = None,
+        docs_url: str | None = None,
+        tag_prefix: str | None = None,
+        config_path: Pathish = Pathier(__file__).parent / "hassle_config.toml",
+    ):
+        """Create or edit `hassle_config.toml` from given params."""
+        print(f"Manual edits can be made at {config_path}")
+        if not cls.exists(config_path):
+            config = cls()
+        else:
+            config = cls.load(config_path)
+        # Add an author to config if a name or email is given.
+        if name or email:
+            config.authors.append(Author(name or "", email or ""))
+        if github_username:
+            homepage = f"https://github.com/{github_username}/$name"
+            config.project_urls.Homepage = homepage
+            config.project_urls.Source_code = f"{homepage}/tree/main/src/$name"
+        if not config.project_urls.Documentation:
+            if github_username and not docs_url:
+                config.project_urls.Documentation = (
+                    f"https://github.com/{github_username}/$name/tree/main/docs"
+                )
+            elif docs_url:
+                config.project_urls.Documentation = docs_url
+        if tag_prefix:
+            config.git.tag_prefix = tag_prefix
+        config.dump(config_path)
+
+
+@dataclass
+class HassleProject:
+    pyproject: Pyproject
+    projectdir: Pathier
+    source_files: list[str]
+    templatedir: Pathier = root / "templates"
+
+    @property
+    def source_code(self) -> str:
+        """Join and return all code from any `.py` files in `self.srcdir`.
+
+        Useful if a tool needs to scan all the source code for something."""
+        return "\n".join(file.read_text() for file in self.srcdir.rglob("*.py"))
+
+    @cached_property
+    def srcdir(self) -> Pathier:
+        return self.projectdir / "src" / self.pyproject.project.name
+
+    @cached_property
+    def changelog_path(self) -> Pathier:
+        return self.projectdir / "CHANGELOG.md"
+
+    @cached_property
+    def pyproject_path(self) -> Pathier:
+        return self.projectdir / "pyproject.toml"
+
+    @cached_property
+    def docsdir(self) -> Pathier:
+        return self.projectdir / "docs"
+
+    @cached_property
+    def testsdir(self) -> Pathier:
+        return self.projectdir / "tests"
+
+    @cached_property
+    def vsdir(self) -> Pathier:
+        return self.projectdir / ".vscode"
+
+    @cached_property
+    def distdir(self) -> Pathier:
+        return self.projectdir / "dist"
+
+    @property
+    def name(self) -> str:
+        """This package's name."""
+        return self.pyproject.project.name
+
+    @property
+    def version(self) -> str:
+        """This package's version."""
+        return self.pyproject.project.version
+
+    @version.setter
+    def version(self, new_version: str):
+        self.pyproject.project.version = new_version
+
+    @classmethod
+    def load(cls, projectdir: Pathish) -> Self:
+        """Load a project given `projectdir`."""
+        projectdir = Pathier(projectdir)
+        pyproject = Pyproject.load(projectdir / "pyproject.toml")
+        name = pyproject.project.name
+        # Convert source files to path stems relative to projectdir/src/name
+        # e.g `C:/python/projects/hassle/src/hassle/templates/pyproject.toml`
+        # becomes `templates/pyproject.toml`
+        source_files = [
+            str(file.separate(name))
+            for file in (projectdir / "src" / name).rglob("*")
+            if file.is_file()
+        ]
+        return cls(pyproject, projectdir, source_files)
+
+    @classmethod
+    def new(
+        cls,
+        targetdir: Pathier,
+        name: str,
+        description: str = "",
+        dependencies: list[str] = [],
+        keywords: list[str] = [],
+        source_files: list[str] = [],
+        add_script: bool = False,
+        no_license: bool = False,
+    ) -> Self:
+        """Create and return a new hassle project."""
+        pyproject = Pyproject.from_template()
+        config = HassleConfig.load()
+        pyproject.project.name = name
+        pyproject.project.authors = config.authors
+        pyproject.project.description = description
+        pyproject.project.dependencies = dependencies
+        pyproject.project.keywords = keywords
+        pyproject.project.urls.Homepage = config.project_urls.Homepage.replace(
+            "$name", name
+        )
+        pyproject.project.urls.Documentation = (
+            config.project_urls.Documentation.replace("$name", name)
+        )
+        pyproject.project.urls.Source_code = config.project_urls.Source_code.replace(
+            "$name", name
+        )
+        hassle = cls(pyproject, targetdir, source_files)
+        if add_script:
+            hassle.add_script(name, name)
+        hassle.generate_files()
+        if no_license:
+            hassle.pyproject.project.classifiers.pop(1)
+            (hassle.projectdir / "LICENSE.txt").delete()
+        hassle.save()
+        return hassle
+
+    def get_template(self, file_name: str) -> str:
+        """Open are return the content of `{self.templatedir}/{file_name}`."""
+        return (self.templatedir / file_name).read_text()
+
+    def save(self):
+        """Dump `self.pyproject` to `{self.projectdir}/pyproject.toml`."""
+        self.pyproject.dump(self.pyproject_path)
+
+    def format_source_files(self):
+        """Use isort and black to format files"""
+        for file in self.projectdir.rglob("*.py"):
+            isort.file(file)
+        try:
+            black.main([str(self.projectdir)])
+        except SystemExit as e:
+            ...
+        except Exception as e:
+            raise e
+
+    def latest_version_is_published(self) -> bool:
+        """Check if the current version of this project has been published to pypi.org."""
+        pypi_url = f"https://pypi.org/project/{self.name}"
+        response = requests.get(pypi_url)
+        if response.status_code != 200:
+            raise RuntimeError(
+                f"{pypi_url} returned status code {response.status_code} :/"
+            )
+        soup = BeautifulSoup(response.text, "html.parser")
+        header = soup.find("h1", class_="package-header__name")
+        assert isinstance(header, Tag)
+        text = header.text.strip()
+        pypi_version = text[text.rfind(" ") + 1 :]
+        return self.version == pypi_version
+
+    # ====================================================================================
+    # Updaters ===========================================================================
+    # ====================================================================================
+    def add_script(self, name: str, file_stem: str, function: str = "main"):
+        """Add a script to `pyproject.project.scripts` in the format `{name} = "{package_name}.{file_stem}:{function}"`"""
+        self.pyproject.project.scripts[name] = f"{self.name}.{file_stem}:{function}"
+
+    def update_init_version(self):
+        """Update the `__version__` in this projects `__init__.py` file
+        to the current value of `self.pyproject.project.version`
+        if it exists and has a `__version__` string.
+
+        If it doesn't have a `__version__` string, append one to it."""
+        init_file = self.srcdir / "__init__.py"
+        version = f'__version__ = "{self.version}"'
+        if init_file.exists():
+            content = init_file.read_text()
+            if "__version__" in content:
+                lines = content.splitlines()
+                for i, line in enumerate(lines):
+                    if line.startswith("__version__"):
+                        lines[i] = version
+                content = "\n".join(lines)
+            else:
+                content += f"\n{version}"
+            init_file.write_text(content)
+
+    def bump_version(self, bump_type: str):
+        """Bump the version of this project.
+
+        `bump_type` should be `major`, `minor`, or `patch`."""
+        # bump pyproject version
+        self.version = utilities.bump_version(self.version, bump_type)
+        # bump `__version__` in __init__.py if the file exists and has a `__version__`.
+        self.update_init_version()
+
+    def update_dependencies(
+        self, overwrite_existing_packages: bool, include_versions: bool
+    ):
+        """Scan project for dependencies and update the corresponding field in the pyproject model.
+
+        If `overwrite_existing_packages` is `False`, this function will only add a package if it isn't already listed,
+        but won't remove anything currently in the list.
+        Use this option to preserve manually added dependencies."""
+        project = packagelister.scan_dir(self.srcdir)
+        version_conditional = ">=" if include_versions else None
+        if overwrite_existing_packages:
+            self.pyproject.project.dependencies = project.get_formatted_requirements(
+                version_conditional
+            )
+        else:
+            # Only add a package if it isn't already in the dependency list
+            self.pyproject.project.dependencies.extend(
+                [
+                    (
+                        package.get_formatted_requirement(version_conditional)
+                        if version_conditional
+                        else package.distribution_name
+                    )
+                    for package in project.requirements
+                    if all(
+                        package.distribution_name not in existing_dependency
+                        for existing_dependency in self.pyproject.project.dependencies
+                    )
+                ]
+            )
+
+    def _generate_changelog(self) -> list[str]:
+        if HassleConfig.exists():
+            tag_prefix = HassleConfig.load().git.tag_prefix
+        else:
+            HassleConfig.warn()
+            print("Assuming no tag prefix.")
+            tag_prefix = ""
+        raw_changelog = [
+            line
+            for line in subprocess.run(
+                [
+                    "auto-changelog",
+                    "-p",
+                    self.projectdir,
+                    "--tag-prefix",
+                    tag_prefix,
+                    "--stdout",
+                ],
+                stdout=subprocess.PIPE,
+                text=True,
+            ).stdout.splitlines(True)
+            if not line.startswith(
+                (
+                    "Full set of changes:",
+                    f"* build {tag_prefix}",
+                    "* update changelog",
+                )
+            )
+        ]
+        return raw_changelog
+
+    def update_changelog(self):
+        """Update `CHANGELOG.md` by invoking the `auto-changelog` module.
+
+        If `hassle_config.toml` doesn't exist, an empty tag prefix will be assumed."""
+        raw_changelog = self._generate_changelog()
+        # If there's no existing changelog, dump the generated one and get out of here.
+        if not self.changelog_path.exists():
+            self.changelog_path.join(raw_changelog)
+            return
+
+        # Don't want to overwrite previously existing manual changes/edits
+        existing_changelog = self.changelog_path.read_text().splitlines(True)[
+            2:
+        ]  # First two elements are "# Changelog\n" and "\n"
+        new_changes = raw_changelog
+        for line in existing_changelog:
+            # Release headers are prefixed with "## "
+            if line.startswith("## "):
+                new_changes = raw_changelog[: raw_changelog.index(line)]
+                break
+        changes = "".join(new_changes)
+        # "#### OTHERS" gets added to the changelog even when there's nothing for that category,
+        # so we'll get rid of it if that's the case
+        others = "#### Others"
+        if changes.strip("\n").endswith(others):
+            changes = changes.strip("\n").replace(others, "\n\n")
+        # If changes == "# Changelog\n\n" then there weren't actually any new changes
+        if not changes == "# Changelog\n\n":
+            self.changelog_path.write_text(changes + "".join(existing_changelog))
+
+    # ====================================================================================
+    # File/Project creation ==============================================================
+    # ====================================================================================
+
+    def create_source_files(self):
+        """Generate source files in `self.srcdir`."""
+        for file in self.source_files:
+            (self.srcdir / file).touch()
+        init = self.srcdir / "__init__.py"
+        if init.exists():
+            init.append(f'__version__ = "{self.version}"')
+
+    def create_readme(self):
+        readme = self.get_template("README.md")
+        readme = readme.replace("$name", self.name)
+        readme = readme.replace("$description", self.pyproject.project.description)
+        (self.projectdir / "README.md").write_text(readme)
+
+    def create_license(self):
+        license_ = self.get_template("license.txt")
+        license_ = license_.replace("$year", str(datetime.now().year))
+        (self.projectdir / "LICENSE.txt").write_text(license_)
+
+    def create_gitignore(self):
+        (self.templatedir / ".gitignore.txt").copy(self.projectdir / ".gitignore")
+
+    def create_vscode_settings(self):
+        self.vsdir.mkdir()
+        (self.templatedir / "vscode_settings.json").copy(self.vsdir / "settings.json")
+
+    def create_tests(self):
+        (self.testsdir / f"test_{self.name}.py").touch()
+
+    def create_py_typed(self):
+        (self.projectdir / "py.typed").touch()
+
+    def generate_files(self):
+        """Create all the necessary files.
+
+        Note: This will overwrite any existing files."""
+        self.projectdir.mkdir()
+        for func in dir(self):
+            if func.startswith("create_"):
+                getattr(self, func)()
+        self.pyproject.dump(self.pyproject_path)
+
+    def generate_docs(self):
+        """Generate docs by invoking `pdoc`"""
+        self.docsdir.delete()
+        subprocess.run(["pdoc", "-o", self.docsdir, self.srcdir])
```

### Comparing `hassle-3.1.8/src/hassle/utilities.py` & `hassle-3.1.9/src/hassle/utilities.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import re
-import subprocess
-from typing import Any
-
-import requests
-from bs4 import BeautifulSoup
-from gitbetter import Git
-from pathier import Pathier
-
-root = Pathier(__file__).parent
-
-
-def swap_keys(data: dict[str, Any], keys: tuple[str, str]) -> dict[str, Any]:
-    """Convert between keys in `data`.
-    The order of `keys` doesn't matter.
-    >>> data = {"one two": 1}
-    >>> data = swap_keys(data, ("one two", "one-two"))
-    >>> print(data)
-    >>> {"one-two": 1}
-    >>> data = swap_keys(data, ("one two", "one-two"))
-    >>> print(data)
-    >>> {"one two": 1}
-    """
-    key1, key2 = keys
-    data_keys = data.keys()
-    if key1 in data_keys:
-        data[key2] = data.pop(key1)
-    elif key2 in data_keys:
-        data[key1] = data.pop(key2)
-    return data
-
-
-def run_tests(pytest_args: list[str] = []) -> bool:
-    """Invoke `coverage` and `pytest -s`.
-
-    Returns `True` if all tests passed or if no tests were found."""
-    results = subprocess.run(["coverage", "run", "-m", "pytest", "-s"] + pytest_args)
-    subprocess.run(["coverage", "report", f"--include={Pathier.cwd()}/*"])
-    subprocess.run(["coverage", "html", f"--include={Pathier.cwd()}/*"])
-    return results.returncode in [0, 5]
-
-
-def check_pypi(package_name: str) -> bool:
-    """Check if a package with package_name already exists on `pypi.org`.
-    Returns `True` if package name exists.
-    Only checks the first page of results."""
-    url = f"https://pypi.org/search/?q={package_name.lower()}"
-    response = requests.get(url)
-    if response.status_code != 200:
-        raise RuntimeError(
-            f"Error: pypi.org returned status code: {response.status_code}"
-        )
-    soup = BeautifulSoup(response.text, "html.parser")
-    pypi_packages = [
-        span.text.lower()
-        for span in soup.find_all("span", class_="package-snippet__name")
-    ]
-    return package_name in pypi_packages
-
-
-def get_answer(question: str) -> bool | None:
-    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received."""
-    ans = ""
-    question = question.strip()
-    if "?" not in question:
-        question += "?"
-    question += " (y/n): "
-    while ans not in ["y", "yes", "no", "n"]:
-        ans = input(question).strip().lower()
-        if ans in ["y", "yes"]:
-            return True
-        elif ans in ["n", "no"]:
-            return False
-        else:
-            print("Invalid answer.")
-
-
-def bump_version(current_version: str, bump_type: str) -> str:
-    """Bump `current_version` according to `bump_type` and return the new version.
-
-    #### :params:
-
-    `current_version`: A version string conforming to Semantic Versioning standards.
-    i.e. `{major}.{minor}.{patch}`
-
-    `bump_type` can be one of `major`, `minor`, or `patch`.
-
-    Raises an exception if `current_version` is formatted incorrectly or if `bump_type` isn't one of the aforementioned types.
-    """
-    if not re.findall(r"[0-9]+.[0-9]+.[0-9]+", current_version):
-        raise ValueError(
-            f"{current_version} does not appear to match the required format of `x.x.x`."
-        )
-    bump_type = bump_type.lower().strip()
-    if bump_type not in ["major", "minor", "patch"]:
-        raise ValueError(
-            f"`bump_type` {bump_type} is not one of `major`, `minor`, or `patch`."
-        )
-    major, minor, patch = [int(part) for part in current_version.split(".")]
-    if bump_type == "major":
-        major += 1
-        minor = 0
-        patch = 0
-    elif bump_type == "minor":
-        minor += 1
-        patch = 0
-    elif bump_type == "patch":
-        patch += 1
-    return f"{major}.{minor}.{patch}"
-
-
-def on_primary_branch() -> bool:
-    """Returns `False` if repo is not currently on `main` or `master` branch."""
-    git = Git(True)
-    if git.current_branch not in ["main", "master"]:
-        return False
-    return True
+import re
+import subprocess
+from typing import Any
+
+import requests
+from bs4 import BeautifulSoup
+from gitbetter import Git
+from pathier import Pathier
+
+root = Pathier(__file__).parent
+
+
+def swap_keys(data: dict[str, Any], keys: tuple[str, str]) -> dict[str, Any]:
+    """Convert between keys in `data`.
+    The order of `keys` doesn't matter.
+    >>> data = {"one two": 1}
+    >>> data = swap_keys(data, ("one two", "one-two"))
+    >>> print(data)
+    >>> {"one-two": 1}
+    >>> data = swap_keys(data, ("one two", "one-two"))
+    >>> print(data)
+    >>> {"one two": 1}
+    """
+    key1, key2 = keys
+    data_keys = data.keys()
+    if key1 in data_keys:
+        data[key2] = data.pop(key1)
+    elif key2 in data_keys:
+        data[key1] = data.pop(key2)
+    return data
+
+
+def run_tests(pytest_args: list[str] = []) -> bool:
+    """Invoke `coverage` and `pytest -s`.
+
+    Returns `True` if all tests passed or if no tests were found."""
+    results = subprocess.run(["coverage", "run", "-m", "pytest", "-s"] + pytest_args)
+    subprocess.run(["coverage", "report", f"--include={Pathier.cwd()}/*"])
+    subprocess.run(["coverage", "html", f"--include={Pathier.cwd()}/*"])
+    return results.returncode in [0, 5]
+
+
+def check_pypi(package_name: str) -> bool:
+    """Check if a package with package_name already exists on `pypi.org`.
+    Returns `True` if package name exists.
+    Only checks the first page of results."""
+    url = f"https://pypi.org/search/?q={package_name.lower()}"
+    response = requests.get(url)
+    if response.status_code != 200:
+        raise RuntimeError(
+            f"Error: pypi.org returned status code: {response.status_code}"
+        )
+    soup = BeautifulSoup(response.text, "html.parser")
+    pypi_packages = [
+        span.text.lower()
+        for span in soup.find_all("span", class_="package-snippet__name")
+    ]
+    return package_name in pypi_packages
+
+
+def get_answer(question: str) -> bool | None:
+    """Repeatedly ask the user a yes/no question until a 'y' or a 'n' is received."""
+    ans = ""
+    question = question.strip()
+    if "?" not in question:
+        question += "?"
+    question += " (y/n): "
+    while ans not in ["y", "yes", "no", "n"]:
+        ans = input(question).strip().lower()
+        if ans in ["y", "yes"]:
+            return True
+        elif ans in ["n", "no"]:
+            return False
+        else:
+            print("Invalid answer.")
+
+
+def bump_version(current_version: str, bump_type: str) -> str:
+    """Bump `current_version` according to `bump_type` and return the new version.
+
+    #### :params:
+
+    `current_version`: A version string conforming to Semantic Versioning standards.
+    i.e. `{major}.{minor}.{patch}`
+
+    `bump_type` can be one of `major`, `minor`, or `patch`.
+
+    Raises an exception if `current_version` is formatted incorrectly or if `bump_type` isn't one of the aforementioned types.
+    """
+    if not re.findall(r"[0-9]+.[0-9]+.[0-9]+", current_version):
+        raise ValueError(
+            f"{current_version} does not appear to match the required format of `x.x.x`."
+        )
+    bump_type = bump_type.lower().strip()
+    if bump_type not in ["major", "minor", "patch"]:
+        raise ValueError(
+            f"`bump_type` {bump_type} is not one of `major`, `minor`, or `patch`."
+        )
+    major, minor, patch = [int(part) for part in current_version.split(".")]
+    if bump_type == "major":
+        major += 1
+        minor = 0
+        patch = 0
+    elif bump_type == "minor":
+        minor += 1
+        patch = 0
+    elif bump_type == "patch":
+        patch += 1
+    return f"{major}.{minor}.{patch}"
+
+
+def on_primary_branch() -> bool:
+    """Returns `False` if repo is not currently on `main` or `master` branch."""
+    git = Git(True)
+    if git.current_branch not in ["main", "master"]:
+        return False
+    return True
```

### Comparing `hassle-3.1.8/src/hassle/templates/license.txt` & `hassle-3.1.9/src/hassle/templates/license.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) $year Matt Manes
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) $year Matt Manes
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `hassle-3.1.8/LICENSE.txt` & `hassle-3.1.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Matt Manes
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Matt Manes
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `hassle-3.1.8/README.md` & `hassle-3.1.9/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# Hassle
-
-Automate creating, building, testing, and publishing Python packages from the command line.   
-
-
-## Installation
-
-Install with:
-
-<pre>
-pip install hassle
-</pre>
-
-You should be able to type `hassle help` in your terminal and see a list of commands:
-![](imgs/hassle_HassleShell.svg)
-
-
-### Additional setup:
-
-Install git and add it to your PATH if it isn't already.  
-Some parts of this tool may require [communicating with Github]((https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git)).  
-You will also need to register a [pypi account](https://pypi.org/account/register/) if you want to publish packages to https://pypi.org with this tool.  
-Once you've created and validated an account, you will need to follow the directions to generate an [api key](https://pypi.org/help/#apitoken).  
-Copy the key and in your home directory, create a '.pypirc' file if it doesn't already exist.  
-Edit the file so it contains the following (don't include the brackets around your api key):
-
-![](imgs/pypirc.svg)
-
-## Configuration
-
-After installation and the above additional setup, it is a good idea to run the 'configure' command.
-This isn't required and a blank config will be generated whenever it is needed if it doesn't exist.
-This info, if provided, is used to populate a new project's 'pyproject.toml' file.
-Typing `hassle help configure`:
-![](imgs/hassle_configure.svg)
-
-You can also view the current contents with the `config` command:
-![](imgs/config.svg)
-
-## Generating New Projects
-New projects are generated with the `new` command:  
-![](imgs/hassle_new.svg)
-
-Most of these options pertain to prefilling the generated 'pyproject.toml' file.  
-As a simple example we'll create a new package called 'nyquil':
-![](imgs/new_use.svg)
-
-A new folder in your current working directory called 'nyquil' should now exist.  
-It should have the following structure:
-![](imgs/folder_tree.svg)
-
-
-**Note: By default an MIT License is added to the project. Pass the `-nl/--no_license` flag to prevent this behavior.**  
-If you open the 'pyproject.toml' file it should look like the following except
-for the 'project.authors' and 'project.urls' sections:
-![](imgs/pyproject.svg)
-
-The package would do absolutely nothing, but with the generated files we do have the
-viable minimum to build an installable python package.
-
-
-## Running Tests
-
-Hassle uses [Pytest](https://pypi.org/project/pytest/) and [Coverage](https://pypi.org/project/coverage/) to run tests.  
-When we invoke the `hassle test` command,
-we should see something like this (pretending we have added test functions to `tests/test_nyquil.py`):
-![](imgs/test.svg)
-
-
-## Building
-
-Building the package is as simple as using:
-
-<pre>
->hassle build
-</pre>
-
-By default, the build command will:  
-1. Run any tests in the `tests` folder (abandoning the build if any fail).  
-2. Format source files with isort and black.  
-3. Scan project import statements and add any missing packages to the pyproject `dependencies` field.  
-4. Use [pdoc](https://pypi.org/project/pdoc/) to generate documentation (located in a created `docs` folder).  
-5. Run `python -m build .` to generate the `tar.gz` and `.whl` files (located in a created `dist` folder).  
-
-
-## Publishing
-
-Assuming you've set up a [PyPi](https://pypi.org/) account, generated the api key, and configured the '.pypirc' 
-file as mentioned earlier, then you can publish the current version of your package by running:
-
-<pre>
->hassle publish
-</pre>
-
-
-## Updating
-
-When the time comes to make changes to your package, the `hassle update` command makes it easy.  
-This command needs at least one argument according to the type of update: `major`, `minor`, or `patch`.  
-This argument tells Hassle how to increment the project version.  
-Hassle uses the [semantic versioning standard](https://semver.org/),
-so, for example, if your current version is `1.2.3` then 
-
-`>hassle update major` bumps to `2.0.0`,  
-`>hassle update minor` bumps to `1.3.0`,  
-and  
-`>hassle update patch` bumps to `1.2.4`.  
-
-By default, the update command will:  
-1. Run any tests in the `tests` folder (abandoning the update if any fail).  
-2. Increment the project version.  
-3. Run the build process as outlined above (minus step 1.).  
-4. Make a commit with the message `chore: build {project_version}`.  
-5. Git tag using the tag prefix in your `hassle_config.toml` file and the new project version.  
-6. Generate/update the `CHANGELOG.md` file using [auto-changelog](https://pypi.org/project/auto-changelog/).  
-(Normally `auto-changelog` overwrites the changelog file, but Hassle does some extra things so that any manual changes you make to the changelog are preserved).  
-7. Git commit the changelog.  
-8. Pull/push the current branch with the remote origin.  
-9. Publish the updated package if the update command was run with the `-p` flag.  
-10. Install the updated package if the update command was run with the `-i` flag.  
-
+# Hassle
+
+Automate creating, building, testing, and publishing Python packages from the command line.   
+
+
+## Installation
+
+Install with:
+
+<pre>
+pip install hassle
+</pre>
+
+You should be able to type `hassle help` in your terminal and see a list of commands:
+![](imgs/hassle_HassleShell.svg)
+
+
+### Additional setup:
+
+Install git and add it to your PATH if it isn't already.  
+Some parts of this tool may require [communicating with Github]((https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git)).  
+You will also need to register a [pypi account](https://pypi.org/account/register/) if you want to publish packages to https://pypi.org with this tool.  
+Once you've created and validated an account, you will need to follow the directions to generate an [api key](https://pypi.org/help/#apitoken).  
+Copy the key and in your home directory, create a '.pypirc' file if it doesn't already exist.  
+Edit the file so it contains the following (don't include the brackets around your api key):
+
+![](imgs/pypirc.svg)
+
+## Configuration
+
+After installation and the above additional setup, it is a good idea to run the 'configure' command.
+This isn't required and a blank config will be generated whenever it is needed if it doesn't exist.
+This info, if provided, is used to populate a new project's 'pyproject.toml' file.
+Typing `hassle help configure`:
+![](imgs/hassle_configure.svg)
+
+You can also view the current contents with the `config` command:
+![](imgs/config.svg)
+
+## Generating New Projects
+New projects are generated with the `new` command:  
+![](imgs/hassle_new.svg)
+
+Most of these options pertain to prefilling the generated 'pyproject.toml' file.  
+As a simple example we'll create a new package called 'nyquil':
+![](imgs/new_use.svg)
+
+A new folder in your current working directory called 'nyquil' should now exist.  
+It should have the following structure:
+![](imgs/folder_tree.svg)
+
+
+**Note: By default an MIT License is added to the project. Pass the `-nl/--no_license` flag to prevent this behavior.**  
+If you open the 'pyproject.toml' file it should look like the following except
+for the 'project.authors' and 'project.urls' sections:
+![](imgs/pyproject.svg)
+
+The package would do absolutely nothing, but with the generated files we do have the
+viable minimum to build an installable python package.
+
+
+## Running Tests
+
+Hassle uses [Pytest](https://pypi.org/project/pytest/) and [Coverage](https://pypi.org/project/coverage/) to run tests.  
+When we invoke the `hassle test` command,
+we should see something like this (pretending we have added test functions to `tests/test_nyquil.py`):
+![](imgs/test.svg)
+
+
+## Building
+
+Building the package is as simple as using:
+
+<pre>
+>hassle build
+</pre>
+
+By default, the build command will:  
+1. Run any tests in the `tests` folder (abandoning the build if any fail).  
+2. Format source files with isort and black.  
+3. Scan project import statements and add any missing packages to the pyproject `dependencies` field.  
+4. Use [pdoc](https://pypi.org/project/pdoc/) to generate documentation (located in a created `docs` folder).  
+5. Run `python -m build .` to generate the `tar.gz` and `.whl` files (located in a created `dist` folder).  
+
+
+## Publishing
+
+Assuming you've set up a [PyPi](https://pypi.org/) account, generated the api key, and configured the '.pypirc' 
+file as mentioned earlier, then you can publish the current version of your package by running:
+
+<pre>
+>hassle publish
+</pre>
+
+
+## Updating
+
+When the time comes to make changes to your package, the `hassle update` command makes it easy.  
+This command needs at least one argument according to the type of update: `major`, `minor`, or `patch`.  
+This argument tells Hassle how to increment the project version.  
+Hassle uses the [semantic versioning standard](https://semver.org/),
+so, for example, if your current version is `1.2.3` then 
+
+`>hassle update major` bumps to `2.0.0`,  
+`>hassle update minor` bumps to `1.3.0`,  
+and  
+`>hassle update patch` bumps to `1.2.4`.  
+
+By default, the update command will:  
+1. Run any tests in the `tests` folder (abandoning the update if any fail).  
+2. Increment the project version.  
+3. Run the build process as outlined above (minus step 1.).  
+4. Make a commit with the message `chore: build {project_version}`.  
+5. Git tag using the tag prefix in your `hassle_config.toml` file and the new project version.  
+6. Generate/update the `CHANGELOG.md` file using [auto-changelog](https://pypi.org/project/auto-changelog/).  
+(Normally `auto-changelog` overwrites the changelog file, but Hassle does some extra things so that any manual changes you make to the changelog are preserved).  
+7. Git commit the changelog.  
+8. Pull/push the current branch with the remote origin.  
+9. Publish the updated package if the update command was run with the `-p` flag.  
+10. Install the updated package if the update command was run with the `-i` flag.  
+
```

### Comparing `hassle-3.1.8/pyproject.toml` & `hassle-3.1.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-[project]
-name = "hassle"
-description = "Create, build, test, and publish Python projects and packages."
-version = "3.1.8"
-dependencies = ["black", "isort", "pytest~=7.2.1", "coverage", "packagelister", "pdoc", "twine", "auto-changelog", "bs4", "requests", "build", "pathier", "gitbetter", "argshell", "pip", "dacite", "typing_extensions", "beautifulsoup4"]
-readme = "README.md"
-keywords = ["devops", "packaging", "build", "test", "automation"]
-classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
-requires-python = ">=3.10, <3.12"
-
-[[project.authors]]
-name = "Matt Manes"
-email = "mattmanes@pm.me"
-
-[project.urls]
-Homepage = "https://github.com/matt-manes/hassle"
-Documentation = "https://github.com/matt-manes/hassle/tree/main/docs"
-"Source code" = "https://github.com/matt-manes/hassle/tree/main/src/hassle"
-
-[project.scripts]
-hassle = "hassle.hassle_cli:main"
-
-[tool]
-[tool.pytest.ini_options]
-addopts = ["--import-mode=importlib"]
-pythonpath = "src"
-
-[tool.hatch.build.targets.sdist]
-exclude = [".coverage", ".pytest_cache", ".vscode", "tests", "notes.txt", "hassle_config.toml", "docs", "htmlcov", "*.md", "imgs"]
-
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+[project]
+name = "hassle"
+description = "Create, build, test, and publish Python projects and packages."
+version = "3.1.9"
+dependencies = ["black", "isort", "pytest~=7.2.1", "coverage", "packagelister", "pdoc", "twine", "auto-changelog", "bs4", "requests", "build", "pathier", "gitbetter", "argshell", "pip", "dacite", "typing_extensions", "beautifulsoup4"]
+readme = "README.md"
+keywords = ["devops", "packaging", "build", "test", "automation"]
+classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
+requires-python = ">=3.10, <3.12"
+
+[[project.authors]]
+name = "Matt Manes"
+email = "mattmanes@pm.me"
+
+[project.urls]
+Homepage = "https://github.com/matt-manes/hassle"
+Documentation = "https://github.com/matt-manes/hassle/tree/main/docs"
+"Source code" = "https://github.com/matt-manes/hassle/tree/main/src/hassle"
+
+[project.scripts]
+hassle = "hassle.hassle_cli:main"
+
+[tool]
+[tool.pytest.ini_options]
+addopts = ["--import-mode=importlib"]
+pythonpath = "src"
+
+[tool.hatch.build.targets.sdist]
+exclude = [".coverage", ".pytest_cache", ".vscode", "tests", "notes.txt", "hassle_config.toml", "docs", "htmlcov", "imgs"]
+
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
```

### Comparing `hassle-3.1.8/PKG-INFO` & `hassle-3.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hassle
-Version: 3.1.8
+Version: 3.1.9
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

