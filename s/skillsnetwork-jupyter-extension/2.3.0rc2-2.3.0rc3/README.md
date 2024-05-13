# Comparing `tmp/skillsnetwork_jupyter_extension-2.3.0rc2.tar.gz` & `tmp/skillsnetwork_jupyter_extension-2.3.0rc3.tar.gz`

## Comparing `skillsnetwork_jupyter_extension-2.3.0rc2.tar` & `skillsnetwork_jupyter_extension-2.3.0rc3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.copier-answers.yml
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.prettierignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.tool-versions
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.whitesource
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.yarnrc.yml
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/CHANGELOG.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/CODEOWNERS
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/RELEASE.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/install.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/setup.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/tsconfig.json
--rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/yarn.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/schema/toolbar.json
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/package.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
--rw-r--r--   0        0        0    21429 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/496.0bb690d99ba98d842975.js
--rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.12441616b46d94b2507f.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/style.js
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/config.ts
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/dialog.ts
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/handler.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/index.ts
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/sn-file-library.ts
--rw-r--r--   0        0        0    23531 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/tools.ts
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/menu/index.ts
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/theme/index.ts
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/toolbar/index.ts
--rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/static/extension_demo.gif
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/style/index.js
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/LICENSE
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/README.md
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/pyproject.toml
--rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.copier-answers.yml
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.prettierignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.tool-versions
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.whitesource
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.yarnrc.yml
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/CHANGELOG.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/CODEOWNERS
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/install.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/setup.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/tsconfig.json
+-rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/yarn.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/schema/toolbar.json
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/package.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/496.19f20bc8675cb7e29725.js
+-rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.21734260f72cf178b653.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/config.ts
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/dialog.ts
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/handler.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/index.ts
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/sn-file-library.ts
+-rw-r--r--   0        0        0    23713 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/tools.ts
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/menu/index.ts
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/theme/index.ts
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/src/toolbar/index.ts
+-rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/static/extension_demo.gif
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/style/index.js
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/LICENSE
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/README.md
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc3/PKG-INFO
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/.copier-answers.yml` & `skillsnetwork_jupyter_extension-2.3.0rc3/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/CHANGELOG.md` & `skillsnetwork_jupyter_extension-2.3.0rc3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 2.3.0rc2
+## 2.3.0rc3
 
 No merged PRs
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 2.3.0rc2
+
+No merged PRs
+
 ## 2.3.0rc1
 
 No merged PRs
 
 ## 2.3.0rc0
 
 No merged PRs
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/CODEOWNERS` & `skillsnetwork_jupyter_extension-2.3.0rc3/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/RELEASE.md` & `skillsnetwork_jupyter_extension-2.3.0rc3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc3'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc2"
+    "version": "2.3.0-rc3"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/tsconfig.json` & `skillsnetwork_jupyter_extension-2.3.0rc3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/yarn.lock` & `skillsnetwork_jupyter_extension-2.3.0rc3/yarn.lock`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/schema/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc3/schema/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/__init__.py` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/handlers.py` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.21734260f72cf178b653.js'}}",*

 * * "'version'": "'2.3.0-rc3'"}*

```diff
@@ -111,15 +111,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.12441616b46d94b2507f.js",
+            "load": "static/remoteEntry.21734260f72cf178b653.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "skillsnetwork_jupyter_extension"
                 },
@@ -207,9 +207,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc2"
+    "version": "2.3.0-rc3"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc3'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc2"
+    "version": "2.3.0-rc3"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/496.0bb690d99ba98d842975.js` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/496.19f20bc8675cb7e29725.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -716,15 +716,15 @@
                                 await e.context.save()
                             } catch (e) {
                                 console.error("[loadLabContents] Error saving notebook:", e)
                             }
                         } else console.error("[loadLabContents] Notebook model is not initialized or environment is local.")
                     }, E = (e, t) => {
                         let o = e;
-                        return e.includes(t) || ("" !== i.C.extname(e) && (o = i.C.dirname(e)), o = i.C.join(o, t)), i.C.removeSlash(o)
+                        return e.includes(t) || (e.includes(i.C.dirname(t)) && (t = i.C.basename(t)), "" !== i.C.extname(e) && (o = i.C.dirname(e)), o = i.C.join(o, t)), i.C.removeSlash(o)
                     };
                     async function L(e, t) {
                         try {
                             return await t.get(e)
                         } catch (e) {
                             if (e instanceof Error) {
                                 const t = e;
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.12441616b46d94b2507f.js` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.21734260f72cf178b653.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b, m, y, g, w, _, k, j, S = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, b, v, m, y, g, w, _, k, j, S = {
             344: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
                         "./extension": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
                         "./style": () => t.e(736).then((() => () => t(736)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -37,18 +37,18 @@
         return S[e](t, t.exports, E), t.exports
     }
     E.m = S, E.c = x, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && e.d < 1 && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
     }, E.a = (o, a, i) => {
         var u;
         i && ((u = []).d = -1);
-        var l, f, s, d = new Set,
+        var l, s, f, d = new Set,
             p = o.exports,
             c = new Promise(((e, r) => {
-                s = r, f = e
+                f = r, s = e
             }));
         c[r] = p, c[e] = e => (u && e(u), d.forEach(e), c.catch((e => {}))), o.exports = c, a((o => {
             var a;
             l = (o => o.map((o => {
                 if (null !== o && "object" == typeof o) {
                     if (o[e]) return o;
                     if (o.then) {
@@ -65,40 +65,40 @@
                 var u = {};
                 return u[e] = e => {}, u[r] = o, u
             })))(o);
             var i = () => l.map((e => {
                     if (e[t]) throw e[t];
                     return e[r]
                 })),
-                f = new Promise((r => {
+                s = new Promise((r => {
                     (a = () => r(i)).r = 0;
                     var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
                     l.map((r => r[e](t)))
                 }));
-            return a.r ? f : i()
-        }), (e => (e ? s(c[t] = e) : f(p), n(u)))), u && u.d < 0 && (u.d = 0)
+            return a.r ? s : i()
+        }), (e => (e ? f(c[t] = e) : s(p), n(u)))), u && u.d < 0 && (u.d = 0)
     }, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return E.d(r, {
             a: r
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        496: "0bb690d99ba98d842975",
+        496: "19f20bc8675cb7e29725",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
         736: "7b5f76df818add15df8b",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e] + ".js?v=" + {
-        496: "0bb690d99ba98d842975",
+        496: "19f20bc8675cb7e29725",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
         736: "7b5f76df818add15df8b",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
@@ -108,18 +108,18 @@
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork_jupyter_extension:", E.l = (e, r, t, n) => {
         if (o[e]) o[e].push(r);
         else {
             var i, u;
             if (void 0 !== t)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
-                    if (s.getAttribute("src") == e || s.getAttribute("data-webpack") == a + t) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
             var d = (r, t) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = o[e];
@@ -155,15 +155,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc2", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc3", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -206,70 +206,70 @@
             a.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? a.pop() + " " + a.pop() : l(i))
         }
         return u();
 
         function u() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, f = (e, r) => {
+    }, s = (e, r) => {
         if (0 in e) {
             r = i(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
             for (var o = 0, a = 1, u = !0;; a++, o++) {
-                var l, s, d = a < e.length ? (typeof e[a])[0] : "";
-                if (o >= r.length || "o" == (s = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
-                if ("u" == s) {
+                var l, f, d = a < e.length ? (typeof e[a])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
+                if ("u" == f) {
                     if (!u || "u" != d) return !1
                 } else if (u)
-                    if (d == s)
+                    if (d == f)
                         if (a <= t) {
                             if (l != e[a]) return !1
                         } else {
                             if (n ? l > e[a] : l < e[a]) return !1;
                             l != e[a] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (n || a <= t) return !1;
                     u = !1, a--
                 } else {
-                    if (a <= t || s < d != n) return !1;
+                    if (a <= t || f < d != n) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, a--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? f(h, r) : !c())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? s(h, r) : !c())
         }
         return !!c()
-    }, s = (e, r) => {
+    }, f = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
     }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
         var o = d(e, t);
-        return f(n, o) || v(p(e, t, o, n)), b(e[t][o])
+        return s(n, o) || b(p(e, t, o, n)), v(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !f(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
-    }, v = e => {
+        return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
+    }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, b = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
+    }, v = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (s(e, t), c(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (f(e, t), c(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
         var a = r && E.o(r, t) && h(r, t, n);
-        return a ? b(a) : o()
+        return a ? v(a) : o()
     })), w = {}, _ = {
         0: () => y("default", "@jupyterlab/docmanager", [1, 4, 2, 0]),
         88: () => y("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
         252: () => y("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
         400: () => y("default", "@jupyterlab/services", [1, 7, 2, 0]),
         416: () => g("default", "jwt-decode", [1, 3, 1, 2], (() => E.e(648).then((() => () => E(648))))),
         500: () => g("default", "axios", [1, 1, 6, 0], (() => E.e(636).then((() => () => E(636))))),
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json` & `skillsnetwork_jupyter_extension-2.3.0rc3/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/config.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/dialog.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/handler.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/sn-file-library.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/tools.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/tools.ts`

 * *Files 0% similar despite different names*

```diff
@@ -595,14 +595,18 @@
   filePath: string,
   labFilename: string
 ): string => {
   let finalPath = filePath;
 
   // See if the filePath includes the lab filename
   if (!filePath.includes(labFilename)) {
+    // Check if just the non-path part of the lab name is missing
+    if (filePath.includes(PathExt.dirname(labFilename))) {
+      labFilename = PathExt.basename(labFilename);
+    }
     // Check if the path includes a filename and remove it if so
     if (PathExt.extname(filePath) !== '') {
       finalPath = PathExt.dirname(filePath);
     }
     finalPath = PathExt.join(finalPath, labFilename);
   }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/menu/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/theme/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/theme/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/src/toolbar/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc3/src/toolbar/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/static/extension_demo.gif` & `skillsnetwork_jupyter_extension-2.3.0rc3/static/extension_demo.gif`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/.gitignore` & `skillsnetwork_jupyter_extension-2.3.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/LICENSE` & `skillsnetwork_jupyter_extension-2.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/README.md` & `skillsnetwork_jupyter_extension-2.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/pyproject.toml` & `skillsnetwork_jupyter_extension-2.3.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc2/PKG-INFO` & `skillsnetwork_jupyter_extension-2.3.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skillsnetwork_jupyter_extension
-Version: 2.3.0rc2
+Version: 2.3.0rc3
 Dynamic: Keywords
 Summary: JupterLab/JupyerLite extension for Skills Network Labs
 Project-URL: Homepage, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/issues
 Project-URL: Repository, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension.git
 Author-email: IBM Skills Network <skills.network@ibm.com>
 License:                                  Apache License
```

