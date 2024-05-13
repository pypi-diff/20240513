# Comparing `tmp/jupyterlab_empinken_extension-0.5.1.tar.gz` & `tmp/jupyterlab_empinken_extension-0.5.2.tar.gz`

## Comparing `jupyterlab_empinken_extension-0.5.1.tar` & `jupyterlab_empinken_extension-0.5.2.tar`

### file list

```diff
@@ -1,75 +1,80 @@
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/.copier-answers.yml
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/.prettierignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/.prettierrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/Pipfile
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/Pipfile.lock
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/Untitled.ipynb
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/babel.config.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jest.config.js
--rw-r--r--   0        0        0   367820 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/package-lock.json
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/test.ipynb
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/tsconfig.test.json
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/_version.py
--rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/package.json
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/package.json.orig
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/plugin.json
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/static/127.f1adab6d80d8a45054d5.js
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/static/202.d9a675a2c24b3aba96af.js
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/static/747.c292333697b55558acec.js
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/static/remoteEntry.6e4f56ceecadbc3c0e04.js
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/static/style.js
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/schema/plugin.json
--rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/src/empinken_commands.ts
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/src/index.ts
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/src/__tests__/jupyterlab_empinken_extension.spec.ts
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/README.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/package.json
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   148138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_extension.spec.ts
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts-snapshots/nb-partial-toolbar-darwin.png
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/nb-toolbar-darwin.png
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A1-darwin.png
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A2-darwin.png
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A3-darwin.png
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L1-darwin.png
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L2-darwin.png
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L3-darwin.png
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S1-darwin.png
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S2-darwin.png
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S3-darwin.png
--rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T1-darwin.png
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T2-darwin.png
--rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T3-darwin.png
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-darwin.png
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb1-darwin.png
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb2-darwin.png
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/screenshots-panel-nb-darwin.png
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-A1-darwin.png
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-L1-darwin.png
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-S1-darwin.png
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-T1-darwin.png
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-darwin.png
--rw-r--r--   0        0        0    21212 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/test-notebook-darwin.png
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/notebooks/empinken_cells_demo_part.ipynb
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/notebooks/empinken_simple_md.ipynb
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/ui-tests/tests/notebooks/empty.ipynb
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/.gitignore
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/LICENSE
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/README.md
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/.copier-answers.yml
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/.prettierignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/Pipfile
+-rw-r--r--   0        0        0    18672 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/Pipfile.lock
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/Untitled.ipynb
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/babel.config.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jest.config.js
+-rw-r--r--   0        0        0   367820 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/package-lock.json
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/test.ipynb
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/tsconfig.test.json
+-rw-r--r--   0        0        0   375452 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/yarn.lock
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/_version.py
+-rw-r--r--   0        0        0    22401 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/build_log.json
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/package.json
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/package.json.orig
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/plugin.json
+-rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/lib_index_js.22fd585b0124320e8b17.js
+-rw-r--r--   0        0        0    17286 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/lib_index_js.22fd585b0124320e8b17.js.map
+-rw-r--r--   0        0        0    30574 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/remoteEntry.5792a47aee7240a49818.js
+-rw-r--r--   0        0        0    29535 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/remoteEntry.5792a47aee7240a49818.js.map
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/style.js
+-rw-r--r--   0        0        0    23167 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/style_index_js.52782c2bb22fbe305be4.js
+-rw-r--r--   0        0        0    19211 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/style_index_js.52782c2bb22fbe305be4.js.map
+-rw-r--r--   0        0        0    30679 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.420503f5113405cdf5ff.js
+-rw-r--r--   0        0        0    27947 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/static/vendors-node_modules_jupyterlab-celltagsclasses_lib_index_js.420503f5113405cdf5ff.js.map
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/schema/plugin.json
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/src/empinken_commands.ts
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/src/index.ts
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/src/__tests__/jupyterlab_empinken_extension.spec.ts
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/README.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/package.json
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   148138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_extension.spec.ts
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts-snapshots/nb-partial-toolbar-darwin.png
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/nb-toolbar-darwin.png
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A1-darwin.png
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A2-darwin.png
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A3-darwin.png
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L1-darwin.png
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L2-darwin.png
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L3-darwin.png
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S1-darwin.png
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S2-darwin.png
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S3-darwin.png
+-rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T1-darwin.png
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T2-darwin.png
+-rw-r--r--   0        0        0     7180 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T3-darwin.png
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-darwin.png
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb1-darwin.png
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb2-darwin.png
+-rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/screenshots-panel-nb-darwin.png
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-A1-darwin.png
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-L1-darwin.png
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-S1-darwin.png
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-T1-darwin.png
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-darwin.png
+-rw-r--r--   0        0        0    21212 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/test-notebook-darwin.png
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/notebooks/empinken_cells_demo_part.ipynb
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/notebooks/empinken_simple_md.ipynb
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/ui-tests/tests/notebooks/empty.ipynb
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 jupyterlab_empinken_extension-0.5.2/PKG-INFO
```

### Comparing `jupyterlab_empinken_extension-0.5.1/.copier-answers.yml` & `jupyterlab_empinken_extension-0.5.2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/RELEASE.md` & `jupyterlab_empinken_extension-0.5.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/jest.config.js` & `jupyterlab_empinken_extension-0.5.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/package-lock.json` & `jupyterlab_empinken_extension-0.5.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/package.json` & `jupyterlab_empinken_extension-0.5.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.5.2'"}*

```diff
@@ -193,9 +193,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `jupyterlab_empinken_extension-0.5.1/test.ipynb` & `jupyterlab_empinken_extension-0.5.2/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/tsconfig.json` & `jupyterlab_empinken_extension-0.5.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/__init__.py` & `jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/package.json` & `jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5792a47aee7240a49818.js'}}",*

 * * "'version'": "'0.5.2'"}*

```diff
@@ -111,15 +111,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/innovationOUtside/jupyterlab_empinken_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6e4f56ceecadbc3c0e04.js",
+            "load": "static/remoteEntry.5792a47aee7240a49818.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_empinken_extension/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -198,9 +198,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/package.json.orig` & `jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.5.2'"}*

```diff
@@ -193,9 +193,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `jupyterlab_empinken_extension-0.5.1/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/plugin.json` & `jupyterlab_empinken_extension-0.5.2/jupyterlab_empinken_extension/labextension/schemas/jupyterlab_empinken_extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/schema/plugin.json` & `jupyterlab_empinken_extension-0.5.2/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/src/empinken_commands.ts` & `jupyterlab_empinken_extension-0.5.2/src/empinken_commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/src/index.ts` & `jupyterlab_empinken_extension-0.5.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/README.md` & `jupyterlab_empinken_extension-0.5.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/jupyter_server_test_config.py` & `jupyterlab_empinken_extension-0.5.2/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/yarn.lock` & `jupyterlab_empinken_extension-0.5.2/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_extension.spec.ts` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts-snapshots/nb-partial-toolbar-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_button_display.spec.ts-snapshots/nb-partial-toolbar-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/nb-toolbar-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/nb-toolbar-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A2-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A2-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A3-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-A3-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L2-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L2-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L3-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-L3-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S2-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S2-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S3-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-S3-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T2-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T2-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T3-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-T3-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb2-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/panel-nb2-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/screenshots-panel-nb-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/screenshots-panel-nb-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-A1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-A1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-L1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-L1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-S1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-S1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-T1-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-T1-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/tags-nb-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/test-notebook-darwin.png` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/jupyterlab_empinken_nb.spec.ts-snapshots/test-notebook-darwin.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/notebooks/empinken_cells_demo_part.ipynb` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/notebooks/empinken_cells_demo_part.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/ui-tests/tests/notebooks/empinken_simple_md.ipynb` & `jupyterlab_empinken_extension-0.5.2/ui-tests/tests/notebooks/empinken_simple_md.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/.gitignore` & `jupyterlab_empinken_extension-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/LICENSE` & `jupyterlab_empinken_extension-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/README.md` & `jupyterlab_empinken_extension-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_empinken_extension-0.5.1/pyproject.toml` & `jupyterlab_empinken_extension-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["hatchling==1.21.1", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version>=0.3.2"]
+requires = ["hatchling>=1.22.4,<1.23",
+    "pkginfo>=1.10,<1.11", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version>=0.3.2"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyterlab_empinken_extension"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `jupyterlab_empinken_extension-0.5.1/PKG-INFO` & `jupyterlab_empinken_extension-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyterlab_empinken_extension
-Version: 0.5.1
+Version: 0.5.2
+Dynamic: Keywords
 Summary: A JupyterLab extension for colouring notebook cell backgrounds.
 Project-URL: Homepage, https://github.com/innovationOUtside/jupyterlab_empinken_extension
 Project-URL: Bug Tracker, https://github.com/innovationOUtside/jupyterlab_empinken_extension/issues
 Project-URL: Repository, https://github.com/innovationOUtside/jupyterlab_empinken_extension.git
 Author-email: jupyterlab_empinken_extension <tony.hirst@gmail.com>
 License: BSD 3-Clause License
```

