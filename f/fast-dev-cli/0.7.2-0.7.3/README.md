# Comparing `tmp/fast_dev_cli-0.7.2.tar.gz` & `tmp/fast_dev_cli-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.7.2.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.7.3.tar", max compression
```

## Comparing `fast_dev_cli-0.7.2.tar` & `fast_dev_cli-0.7.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.2/LICENSE
--rw-r--r--   0        0        0     2109 2024-04-30 08:17:16.702283 fast_dev_cli-0.7.2/README.md
--rw-r--r--   0        0        0      392 2024-05-09 15:36:58.837450 fast_dev_cli-0.7.2/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.2/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    21875 2024-05-09 15:38:31.432614 fast_dev_cli-0.7.2/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.2/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1407 2024-05-10 01:54:44.688753 fast_dev_cli-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2171 2024-05-13 06:12:17.707278 fast_dev_cli-0.7.3/README.md
+-rw-r--r--   0        0        0      392 2024-05-09 15:36:58.837450 fast_dev_cli-0.7.3/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.7.3/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    22059 2024-05-13 06:44:01.994013 fast_dev_cli-0.7.3/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.7.3/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1407 2024-05-13 06:33:12.556585 fast_dev_cli-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 fast_dev_cli-0.7.3/PKG-INFO
```

### Comparing `fast_dev_cli-0.7.2/LICENSE` & `fast_dev_cli-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.7.2/README.md` & `fast_dev_cli-0.7.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ---
 
 **Source Code**: <a href="https://github.com/waketzheng/fast-dev-cli" target="_blank">https://github.com/waketzheng/fast-dev-cli</a>
 
 ## Requirements
 
-Python 3.11+
+Python 3.10+
 
 ## Installation
 
 <div class="termy">
 
 ```console
 $ pip install "fast-dev-cli[all]"
@@ -67,7 +67,11 @@
 ```bash
 fast sync
 ```
 - Upgrade main/dev dependencies to latest version
 ```bash
 fast upgrade
 ```
+- Start a fastapi server in development mode
+```
+fast dev
+```
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                          _S_t_a_t_u_s_]_[_R_u_f_f_]_[_M_y_p_y_ _C_o_v_e_r_a_g_e_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
-Python 3.11+ ## Installation
+Python 3.10+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
 fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
 Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
 fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
 requirement file and install `pip install -r ` ```bash fast sync ``` - Upgrade
-main/dev dependencies to latest version ```bash fast upgrade ```
+main/dev dependencies to latest version ```bash fast upgrade ``` - Start a
+fastapi server in development mode ``` fast dev ```
```

### Comparing `fast_dev_cli-0.7.2/fast_dev_cli/cli.py` & `fast_dev_cli-0.7.3/fast_dev_cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if sys.version_info >= (3, 11):
     from enum import StrEnum
     from typing import Self
 else:  # pragma: no cover
     from strenum import StrEnum  # type:ignore[no-redef,assignment]
     from typing_extensions import Self
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from typer.models import OptionInfo
 
 
 __version__ = importlib.metadata.version(Path(__file__).parent.name)
 
 
 def parse_files(args: list[str] | tuple[str, ...]) -> list[str]:
@@ -38,15 +38,15 @@
             sys.argv.append(".")
 except ModuleNotFoundError:
     import click
     from click import echo, secho
     from click.core import Group as _Group
     from click.exceptions import Exit
 
-    def Option(default, *shortcuts, help=None):  # type:ignore[no-redef]
+    def Option(default, *shortcuts, **kw):  # type:ignore[no-redef]
         return default
 
     def _command(self, *args, **kwargs):
         from click.decorators import command
 
         def decorator(f):
             if kwargs.get("name") == "lint":
@@ -94,14 +94,15 @@
 
 def _run_shell(cmd: str, **kw) -> CompletedProcess:
     kw.setdefault("shell", True)
     return subprocess.run(cmd, **kw)
 
 
 def run_and_echo(cmd: str, *, dry=False, verbose=True, **kw) -> int:
+    """Run shell command with subprocess and print it"""
     if verbose:
         echo(f"--> {cmd}")
     if dry:
         return 0
     return _run_shell(cmd, **kw).returncode
 
 
@@ -116,16 +117,15 @@
     r = subprocess.run(command, capture_output=True, **kw)
     return r.stdout.strip().decode()
 
 
 def get_current_version(verbose=False) -> str:
     cmd = ["poetry", "version", "-s"]
     if verbose:
-        command = " ".join(cmd)
-        echo(f"--> {command}")
+        echo(f"--> {' '.join(cmd)}")
     return capture_cmd_output(cmd)
 
 
 def _ensure_bool(value: bool | "OptionInfo") -> bool:
     if not isinstance(value, bool):
         value = getattr(value, "default", False)
     return value
@@ -227,30 +227,31 @@
     part: BumpUp.PartChoices,
     commit: bool = Option(
         False, "--commit", "-c", help="Whether run `git commit` after version changed"
     ),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
     """Bump up version string in pyproject.toml"""
-    return BumpUp(_ensure_bool(commit), part.value, dry=dry).run()
+    return BumpUp(_ensure_bool(commit), getattr(part, "value", part), dry=dry).run()
 
 
 def bump() -> None:
     part, commit = "", False
     if args := sys.argv[2:]:
         if "-c" in args or "--commit" in args:
             commit = True
         for a in args:
             if not a.startswith("-"):
                 part = a
                 break
     return BumpUp(commit, part, dry="--dry" in args).run()
 
 
-class EnvError(Exception): ...
+class EnvError(Exception):
+    """Raise this when the project is expected to be managed by poetry, but toml file not found."""
 
 
 class Project:
     path_depth = 5
 
     @staticmethod
     def work_dir(name: str, parent: Path, depth: int) -> Path | None:
@@ -454,15 +455,16 @@
 
 
 class GitTag(DryRun):
     def __init__(self: Self, message: str, dry: bool) -> None:
         self.message = message
         super().__init__(dry=dry)
 
-    def has_v_prefix(self: Self) -> bool:
+    @staticmethod
+    def has_v_prefix() -> bool:
         return "v" in capture_cmd_output("git tag")
 
     def should_push(self: Self) -> bool:
         return "git push" in self.git_status
 
     def gen(self: Self) -> str:
         _version = get_current_version(verbose=False)
@@ -610,23 +612,14 @@
     Sync(filename, extras, save, dry=dry).run()
 
 
 def _should_run_test_script(path: Path) -> bool:
     return path.exists()
 
 
-@cli.command(name="test")
-def coverage_test(
-    dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-    ignore_script: bool = Option(False, "--ignore-script", "-i"),
-) -> None:
-    """Run unittest by pytest and report coverage"""
-    return test(dry, ignore_script)
-
-
 def test(dry: bool, ignore_script=False) -> None:
     cwd = Path.cwd()
     root = Project.get_work_dir(cwd=cwd, allow_cwd=True)
     test_script = root / "scripts" / "test.sh"
     if not _ensure_bool(ignore_script) and _should_run_test_script(test_script):
         cmd = f"sh {test_script.relative_to(root)}"
         if cwd != root:
@@ -635,14 +628,23 @@
         cmd = 'coverage run -m pytest -s && coverage report --omit="tests/*" -m'
         if not is_venv() or not check_call("coverage --version"):
             sep = " && "
             cmd = sep.join("poetry run " + i for i in cmd.split(sep))
     exit_if_run_failed(cmd, dry=dry)
 
 
+@cli.command(name="test")
+def coverage_test(
+    dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
+    ignore_script: bool = Option(False, "--ignore-script", "-i"),
+) -> None:
+    """Run unittest by pytest and report coverage"""
+    return test(dry, ignore_script)
+
+
 @cli.command()
 def upload(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
     """Shortcut for package publish"""
     cmd = "poetry publish --build"
     exit_if_run_failed(cmd, dry=dry)
@@ -664,13 +666,13 @@
 
 @cli.command(name="dev")
 def runserver(
     port: Optional[int] = Option(None, "-p", "--port"),
     host: Optional[str] = Option(None, "-h", "--host"),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
 ) -> None:
-    """Check code style without reformat"""
+    """Start a fastapi server(only for fastapi>=0.111.0)"""
     dev(port, host, dry=dry)
 
 
-if __name__ == "__main__":
-    cli()  # pragma: no cover
+if __name__ == "__main__":  # pragma: no cover
+    cli()
```

### Comparing `fast_dev_cli-0.7.2/pyproject.toml` & `fast_dev_cli-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-dev-cli"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_dev_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fast_dev_cli-0.7.2/PKG-INFO` & `fast_dev_cli-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-dev-cli
-Version: 0.7.2
+Version: 0.7.3
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -50,15 +50,15 @@
 
 ---
 
 **Source Code**: <a href="https://github.com/waketzheng/fast-dev-cli" target="_blank">https://github.com/waketzheng/fast-dev-cli</a>
 
 ## Requirements
 
-Python 3.11+
+Python 3.10+
 
 ## Installation
 
 <div class="termy">
 
 ```console
 $ pip install "fast-dev-cli[all]"
@@ -90,8 +90,12 @@
 ```bash
 fast sync
 ```
 - Upgrade main/dev dependencies to latest version
 ```bash
 fast upgrade
 ```
+- Start a fastapi server in development mode
+```
+fast dev
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.2 Summary: Author: Waket
+Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.7.3 Summary: Author: Waket
 Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: all
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all" Requires-Dist:
 click (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra == "all" Requires-
 Dist: mypy (>=1.10.0,<2.0.0) ; extra == "all" Requires-Dist: pytest
@@ -11,15 +11,16 @@
 Dist: type-extensions (>=0.1.2) ; python_version < "3.11" Requires-Dist: typer
 (>=0.12.3,<0.13.0) ; extra == "all" Description-Content-Type: text/markdown
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                          _S_t_a_t_u_s_]_[_R_u_f_f_]_[_M_y_p_y_ _C_o_v_e_r_a_g_e_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
-Python 3.11+ ## Installation
+Python 3.10+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
 fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
 Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
 fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
 requirement file and install `pip install -r ` ```bash fast sync ``` - Upgrade
-main/dev dependencies to latest version ```bash fast upgrade ```
+main/dev dependencies to latest version ```bash fast upgrade ``` - Start a
+fastapi server in development mode ``` fast dev ```
```

