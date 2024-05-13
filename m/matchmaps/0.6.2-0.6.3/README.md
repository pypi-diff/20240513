# Comparing `tmp/matchmaps-0.6.2.tar.gz` & `tmp/matchmaps-0.6.3.tar.gz`

## Comparing `matchmaps-0.6.2.tar` & `matchmaps-0.6.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github_changelog_generator
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.6.2/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.6.2/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/workflows/cron.yml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.github/workflows/test_docs.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/Makefile
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/about.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/cli.md
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/conf.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/make.bat
--rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/quickstart.md
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/visualization.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/_static/custom.css
--rw-r--r--   0        0        0   217883 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/images/isdifferencemap.png
--rw-r--r--   0        0        0   116988 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/images/openmap.png
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 matchmaps-0.6.2/docs/images/rs-favicon_32x32.png
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.6.2/src/matchmaps/__init__.py
--rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 matchmaps-0.6.2/src/matchmaps/_compute_mr_diff.py
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 matchmaps-0.6.2/src/matchmaps/_compute_ncs_diff.py
--rwxr-xr-x   0        0        0    16597 2020-02-02 00:00:00.000000 matchmaps-0.6.2/src/matchmaps/_compute_realspace_diff.py
--rw-r--r--   0        0        0    32441 2020-02-02 00:00:00.000000 matchmaps-0.6.2/src/matchmaps/_utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 matchmaps-0.6.2/src/matchmaps/_version_util.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.6.2/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 matchmaps-0.6.2/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.6.2/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.6.2/README.md
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 matchmaps-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 matchmaps-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github_changelog_generator
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.6.3/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.6.3/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.github/workflows/test_docs.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/Makefile
+-rw-r--r--   0        0        0    10422 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/about.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/cli.md
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/conf.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/make.bat
+-rw-r--r--   0        0        0    10904 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/quickstart.md
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/visualization.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/_static/custom.css
+-rw-r--r--   0        0        0   217883 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/images/isdifferencemap.png
+-rw-r--r--   0        0        0   116988 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/images/openmap.png
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 matchmaps-0.6.3/docs/images/rs-favicon_32x32.png
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/__init__.py
+-rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_compute_mr_diff.py
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_compute_ncs_diff.py
+-rwxr-xr-x   0        0        0    16618 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    32935 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 matchmaps-0.6.3/src/matchmaps/_version_util.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.6.3/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 matchmaps-0.6.3/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.6.3/LICENSE
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.6.3/README.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 matchmaps-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 matchmaps-0.6.3/PKG-INFO
```

### Comparing `matchmaps-0.6.2/.pre-commit-config.yaml` & `matchmaps-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/setup.py` & `matchmaps-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/tox.ini` & `matchmaps-0.6.3/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/.github/workflows/build_docs.yml` & `matchmaps-0.6.3/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/.github/workflows/ci.yml` & `matchmaps-0.6.3/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       fail-fast: false
       matrix:
         python-version: ['3.9', '3.10']
         platform: [ubuntu-latest]
 
     steps:
       - name: Cancel Previous Runs
-        uses: styfle/cancel-workflow-action@0.12.0
+        uses: styfle/cancel-workflow-action@0.12.1
         with:
           access_token: ${{ github.token }}
 
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
@@ -37,15 +37,15 @@
           python -m pip install -U pip
           python -m pip install -e .[test]
 
       - name: Test
         run: pytest --color=yes --cov --cov-report=xml --cov-report=term-missing
 
       - name: Coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
 
   deploy:
     name: Deploy
     needs: test
     if: "success() && startsWith(github.ref, 'refs/tags/')"
     runs-on: ubuntu-latest
 
@@ -68,10 +68,10 @@
 
       - name: Build and publish
         run: twine upload dist/*
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_API_KEY }}
 
-      - uses: softprops/action-gh-release@v1
+      - uses: softprops/action-gh-release@v2
         with:
           generate_release_notes: true
```

### Comparing `matchmaps-0.6.2/.github/workflows/cron.yml` & `matchmaps-0.6.3/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/.github/workflows/test_docs.yml` & `matchmaps-0.6.3/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/docs/Makefile` & `matchmaps-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/docs/conf.py` & `matchmaps-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/docs/index.md` & `matchmaps-0.6.3/docs/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # `matchmaps` Documentation
 
 Welcome to the docs for `matchmaps`, a python package for aligning and subtracting non-isomorphous crystallographic datasets. Do you have a pair of datasets for which an isomorphous difference maps doesn't quite work due to changes in your unit cell dimensions? If so, this is the package for you.
 
 The [quickstart guide](quickstart.md) contains installation instructions and sample usage of the basic `matchmaps` utility, along with other useful tips.
 
-If you'd like to learn more about `matchmaps` and see the package in action, please check out our pre-print!
-> [MatchMaps: Non-isomorphous difference maps for X-ray crystallography](https://www.biorxiv.org/content/10.1101/2023.09.01.555333v1.full.pdf+html)
+If you'd like to learn more about `matchmaps`, you can find our exploration of the package [here](about.md). For even more information, and see the package in action, please check out our pre-print!
+> [MatchMaps: Non-isomorphous difference maps for X-ray crystallography](https://www.biorxiv.org/content/10.1101/2023.09.01.555333v2.full.pdf+html)
 
 This software is part of the [Reciprocal Space Station](https://rs-station.github.io/) family of open-source crystallography software and was conceived in [Doeke Hekstra's Lab](https://hekstralab.fas.harvard.edu/) at Harvard by [Dennis Brookner](https://dennisbrookner.github.io/)
 
 ## The `matchmaps` functions in brief
 
 `matchmaps` consists of three command-line utilities. A walkthrough of the core utility can be found [here](quickstart.md), and all options for all three utilites are documented [here](cli.md). All three utilities produce a real-space difference map and require a single starting model for phasing, but differ in the types of reflection data they require. Briefly:
```

### Comparing `matchmaps-0.6.2/docs/make.bat` & `matchmaps-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/docs/quickstart.md` & `matchmaps-0.6.3/docs/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Getting started with `matchmaps`
 
-On this page, we'll explore how to use the basic `matchmaps` utility and examine its outputs.  Full documation of all options for all three command-line utilities can be found [here](cli.md) or by typing the command plus `--help` into the command line.
+On this page, we'll explore how to use the basic `matchmaps` utility and examine its outputs.  Full documation of all options for all three command-line utilities can be found [here](cli.md) or by typing the command plus `--help` into the command line. A more detailed exploration of the `matchmaps` algorithm can be found [here](about.md).
 
 ## Installation
 
 `matchmaps` and its python dependencies can be installed via `pip`:
 ```bash
 pip install matchmaps
 ```
@@ -24,14 +24,18 @@
 ### Additional dependencies
 
 Though `matchmaps` is a python package, it relies on two pieces of external software that are not (yet!) `pip`-installable. If they do become `pip`-installable in the future, I will excitedly update this package and save you the trouble. For the time being, you will need to install:
 
  - [ccp4](https://www.ccp4.ac.uk/download/#os=mac)
  - [phenix](https://phenix-online.org/documentation/install-setup-run.html)
 
+```{eval-rst}
+.. note::
+    Please note that phenix 1.21 is **not** supported at this time. I hope to update `matchmaps` to support this in the near future. In the meantime, make sure you're using phenix 1.20 or earlier, and everything should work fine. 
+```
 When actually using `matchmaps` in the command-line, you'll need to have both ccp4 and phenix active. Doing that will look something like:
 ```bash
 source /path/to/phenix/phenix_env.sh
 /path/to/ccp4/start
 ```
 
 At this point, you should be good to go! Please [file an issue on github](https://github.com/dennisbrookner/matchmaps/issues) is this is not working.
@@ -66,15 +70,15 @@
 
 ```bash
 matchmaps --mtzoff apo_data.mtz Fobs SIGFobs \
     --mtzon bound_data.mtz Fobs SIGFobs \
     --pdboff apo.pdb \
     --ligands weird_solvent_1.cif weird_solvent_2.cif
 ```
- 
+
 If you'd like read or write files from somewhere other than your current directory, you can! There are three ways to specify input files:
  - Provide relative paths directly for all input files
  - Provide only file names, and add the `--input-dir` option to specify where those files live. If you do this, the same `--input-dir` will be preprended to all filenames, so your files should all live in the same place.
  - Provide absolute paths to input files. For any input supplied as an absolute path, the `--input-dir` will be ignored.
 
 To direct output files to a specific directory, use the `--output-dir` flag. By default, all of the temporary files created by `matchmaps` will be deleted when the program finishes. Only the `.map` files described below are kept. If you would like to keep all files, you may additionally supply a `--keep-temp-files` directory, which will be created inside of `--output-dir`.
```

### Comparing `matchmaps-0.6.2/docs/visualization.md` & `matchmaps-0.6.3/docs/visualization.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 isomesh differencemesh_positive, difference_map, 2, pdb and resi 20
 ```
 
 ### Normalization
 
 `matchmaps` outputs are **already normalized**. This means that when looking at `matchmaps` outputs, the `normalize_ccp4_maps` option should always be set to `off`. If this option is turned on, then the map's contour levels are likely to be very different from, say, how they look in Coot.
 
-### Symmetry expansion.
+### Symmetry expansion
 As mentioned above, `matchmaps` outputs are always in spacegroup P1. This means that the only relevant symmetry operation is the periodic boundary condition. But there is a catch - even though your map is always in P1, your structural model is unlikely to be! PyMOL looks for symmetry operations wherever it can find them. This means that if `map_auto_expand_sym` is on, and you use the `isomesh` command as such:
 
 ```
 isomesh my_new_mesh, map_from_matchmaps, 2, pdb_in_high_symmetry_spacegroup and resi 20
 ```
 
 then the map produced will be expanded by a series of nonsense symmetry operators that in no way apply!
```

### Comparing `matchmaps-0.6.2/docs/images/isdifferencemap.png` & `matchmaps-0.6.3/docs/images/isdifferencemap.png`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/docs/images/openmap.png` & `matchmaps-0.6.3/docs/images/openmap.png`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/docs/images/rs-favicon_32x32.png` & `matchmaps-0.6.3/docs/images/rs-favicon_32x32.png`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/src/matchmaps/_compute_mr_diff.py` & `matchmaps-0.6.3/src/matchmaps/_compute_mr_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/src/matchmaps/_compute_ncs_diff.py` & `matchmaps-0.6.3/src/matchmaps/_compute_ncs_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/src/matchmaps/_compute_realspace_diff.py` & `matchmaps-0.6.3/src/matchmaps/_compute_realspace_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     mtzon_scaled = output_dir / (on_name + "_scaled.mtz")
 
     print(
         f"{time.strftime('%H:%M:%S')}: Running scaleit to scale 'on' data to 'off' data..."
     )
 
     subprocess.run(
-        f"rs.scaleit -r {mtzoff} {Foff} {SigFoff} -i {mtzon} {Fon} {SigFon} -o {mtzon_scaled}",
+        f"rs.scaleit -r {mtzoff} {Foff} {SigFoff} -i {mtzon} {Fon} {SigFon} -o {mtzon_scaled} --ignore-isomorphism",
         shell=True,
         capture_output=(not verbose),
     )
 
     ## now that scaleit has run, let's swap out the spacegroup from the scaled file
     mtzon_scaled_py = rs.read_mtz(str(mtzon_scaled))
     mtzon_original_py = rs.read_mtz(str(mtzon))
```

### Comparing `matchmaps-0.6.2/src/matchmaps/_utils.py` & `matchmaps-0.6.3/src/matchmaps/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,25 @@
 
     if shutil.which("phenix.refine") is None:
         raise OSError(
             "phenix is not active in your current environment. Please activate phenix and try again."
             "\n"
             "For more information, see https://rs-station.github.io/matchmaps/quickstart.html#additional-dependencies"
         )
+    else:
+        version_printout = subprocess.run(
+            "phenix.version | grep Version", shell=True, capture_output=True
+        )
+        
+        version_string = str(version_printout.stdout)
+        
+        if version_string.find('21') > 0:
+            raise NotImplementedError("It seems that you are using phenix 1.21, which is not yet supported by matchmaps"
+                                      "\n"
+                                      "Please use phenix 1.20 or earlier.")
 
     if ccp4:
         if shutil.which("scaleit") is None:
             raise OSError(
                 "ccp4 is not active in your current environment. Please activate ccp4 and try again."
                 "\n"
                 "For more information, see https://rs-station.github.io/matchmaps/quickstart.html#additional-dependencies"
```

### Comparing `matchmaps-0.6.2/.gitignore` & `matchmaps-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/LICENSE` & `matchmaps-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/README.md` & `matchmaps-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.6.2/pyproject.toml` & `matchmaps-0.6.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -22,19 +22,20 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
+
 dependencies = [
     "numpy",
     "tqdm",
     "reciprocalspaceship>=1.0.1",
-    "rs-booster>=0.0.1",
+    "rs-booster>=0.1.2",
     "gemmi"
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = ["pytest>=6.0", "pytest-cov"]
@@ -66,7 +67,11 @@
 "matchmaps.ncs" = "matchmaps._compute_ncs_diff:main"
 "matchmaps.mr" = "matchmaps._compute_mr_diff:main"
 "matchmaps.version" = "matchmaps._version_util:main"
 
 # https://hatch.pypa.io/latest/config/metadata/
 [tool.hatch.version]
 source = "vcs"
+
+# # this can be deleted once a new rs-booster version has been released
+# [tool.hatch.metadata]
+# allow-direct-references = true
```

### Comparing `matchmaps-0.6.2/PKG-INFO` & `matchmaps-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: matchmaps
-Version: 0.6.2
+Version: 0.6.3
 Summary: Make unbiased difference maps even for non-isomorphous inputs
 Project-URL: homepage, https://rs-station.github.io/matchmaps/
 Project-URL: repository, https://github.com/rs-station/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: gemmi
 Requires-Dist: numpy
 Requires-Dist: reciprocalspaceship>=1.0.1
-Requires-Dist: rs-booster>=0.0.1
+Requires-Dist: rs-booster>=0.1.2
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

