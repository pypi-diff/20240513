# Comparing `tmp/workforce-1.0.8.tar.gz` & `tmp/workforce-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workforce-1.0.8.tar", last modified: Mon Jun 12 01:28:14 2023, max compression
+gzip compressed data, was "workforce-1.0.9.tar", last modified: Sun Mar 24 22:46:26 2024, max compression
```

## Comparing `workforce-1.0.8.tar` & `workforce-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:28:14.654784 workforce-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-12 01:28:04.000000 workforce-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 01:28:04.000000 workforce-1.0.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 01:28:04.000000 workforce-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 01:28:04.000000 workforce-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-12 01:28:14.654784 workforce-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-12 01:28:04.000000 workforce-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:28:14.650784 workforce-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4807 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 01:28:04.000000 workforce-1.0.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:28:14.654784 workforce-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-12 01:28:04.000000 workforce-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:28:14.654784 workforce-1.0.8/workforce/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-12 01:28:04.000000 workforce-1.0.8/workforce/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-12 01:28:04.000000 workforce-1.0.8/workforce/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4931 2023-06-12 01:28:04.000000 workforce-1.0.8/workforce/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-12 01:28:04.000000 workforce-1.0.8/workforce/workforce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:28:14.654784 workforce-1.0.8/workforce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-12 01:28:14.000000 workforce-1.0.8/workforce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-12 01:28:14.000000 workforce-1.0.8/workforce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:28:14.000000 workforce-1.0.8/workforce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 01:28:14.000000 workforce-1.0.8/workforce.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-12 01:28:14.000000 workforce-1.0.8/workforce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 01:28:14.000000 workforce-1.0.8/workforce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:46:26.221370 workforce-1.0.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-03-24 22:46:19.000000 workforce-1.0.9/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-03-24 22:46:19.000000 workforce-1.0.9/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-03-24 22:46:19.000000 workforce-1.0.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-03-24 22:46:19.000000 workforce-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-24 22:46:26.221370 workforce-1.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1455 2024-03-24 22:46:19.000000 workforce-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:46:26.221370 workforce-1.0.9/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      610 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4807 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       33 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      306 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1146 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      771 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/make.bat
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-03-24 22:46:19.000000 workforce-1.0.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 22:46:26.221370 workforce-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1372 2024-03-24 22:46:19.000000 workforce-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:46:26.221370 workforce-1.0.9/workforce/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      133 2024-03-24 22:46:19.000000 workforce-1.0.9/workforce/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5744 2024-03-24 22:46:19.000000 workforce-1.0.9/workforce/backupgui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-03-24 22:46:19.000000 workforce-1.0.9/workforce/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5555 2024-03-24 22:46:19.000000 workforce-1.0.9/workforce/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-03-24 22:46:19.000000 workforce-1.0.9/workforce/workforce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:46:26.221370 workforce-1.0.9/workforce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-24 22:46:26.000000 workforce-1.0.9/workforce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-24 22:46:26.000000 workforce-1.0.9/workforce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 22:46:26.000000 workforce-1.0.9/workforce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-24 22:46:26.000000 workforce-1.0.9/workforce.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-24 22:46:26.000000 workforce-1.0.9/workforce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 22:46:26.000000 workforce-1.0.9/workforce.egg-info/top_level.txt
```

### Comparing `workforce-1.0.8/LICENSE` & `workforce-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `workforce-1.0.8/PKG-INFO` & `workforce-1.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workforce
-Version: 1.0.8
+Version: 1.0.9
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
 Keywords: workforce
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: networkx
+Requires-Dist: pydot
+Requires-Dist: dash_cytoscape
+Requires-Dist: dash
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
 
 =========
 workforce
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/workforce.svg
@@ -74,22 +81,14 @@
 
    from workforce.workforce import worker
    steve = worker("<PLAN.CSV>")
    steve.run()
 
 The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
 
-Testing
--------
-Testing can be done within the github directory by running:
-
-.. code-block:: bash
-
-   python -m unittest -v
-
 
 =======
 History
 =======
 
 0.1.0 (2021-01-16)
 ------------------
```

### Comparing `workforce-1.0.8/README.rst` & `workforce-1.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,7 @@
 .. code-block:: python
 
    from workforce.workforce import worker
    steve = worker("<PLAN.CSV>")
    steve.run()
 
 The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
-
-Testing
--------
-Testing can be done within the github directory by running:
-
-.. code-block:: bash
-
-   python -m unittest -v
```

### Comparing `workforce-1.0.8/docs/Makefile` & `workforce-1.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `workforce-1.0.8/docs/conf.py` & `workforce-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `workforce-1.0.8/docs/installation.rst` & `workforce-1.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `workforce-1.0.8/docs/make.bat` & `workforce-1.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `workforce-1.0.8/setup.py` & `workforce-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     keywords='workforce',
     name='workforce',
     packages = ["workforce"],
     url='https://github.com/theoportlock/workforce',
-    version='1.0.8',
+    version='1.0.9',
 )
```

### Comparing `workforce-1.0.8/workforce/gui.py` & `workforce-1.0.9/workforce/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,151 @@
 from dash import Dash, html, Input, Output, State, dcc, ctx
+import base64
 import dash_cytoscape as cyto
+import os
+import io
+import subprocess
 import numpy as np
 import pandas as pd
 
 def gui():
     app = Dash(__name__)
+    app.layout = create_layout()
+    register_callbacks(app)
+    app.run_server()
 
-    # define app
-    app.layout = html.Div([
+def create_layout():
+    layout = html.Div([
         html.Div([
-                dcc.Upload(html.Button('Load'), id='upload-data'),
-                html.Button('Save', id='btn-download'), dcc.Download(id='download-data')],
-                ),
-        html.Div(['Input: ',
-                  dcc.Input(id='txt_from', value='from', type='text'),
-                  dcc.Input(id='txt_to', value='to', type='text')
-                  ]),
+            dcc.Upload(html.Button('Load'), id='upload-data'),
+            html.Button('Save', id='btn-download'),
+            dcc.Download(id='download-data')
+        ]),
+        html.Div([
+            'Input: ',
+            dcc.Input(id='txt_from', value='from', type='text'),
+            dcc.Input(id='txt_to', value='to', type='text')
+        ]),
         html.Div([
             html.Button('Add Node', id='btn-add', n_clicks=0),
             html.Button('Remove Node', id='btn-remove', n_clicks=0),
+            html.Button('Run Process', id='btn-run', n_clicks=0),
+            html.Button('Execute Pipeline', id='btn-exe', n_clicks=0),
         ]),
+        html.Hr(),
         cyto.Cytoscape(
             id='cytoscape-elements',
-            layout={'name': 'breadthfirst',
-                    'directed':True},
+            layout={'name': 'breadthfirst', 'directed': True},
             style={'width': '100%', 'height': '650px'},
-            stylesheet=[
-                {
-                    'selector': 'node',
-                    'style': {
-                        'background-color': 'steelblue',
-                        'label': 'data(id)',
-                        'font-size': '14px',
-                        'width': '30px',
-                        'height': '30px',
-                    }
-                },
-                {
-                    'selector': 'edge',
-                    'style': {
-                        'curve-style': 'taxi',
-                        'target-arrow-shape': 'triangle',
-                        #'events': 'yes'
-                    }}],
+            stylesheet=create_stylesheet(),
             elements=[]
-        )
+        ),
+        html.Hr()
     ])
+    return layout
 
-    # Update Graph through load or add
-    @app.callback(Output('cytoscape-elements', 'elements'),
-                  Input('upload-data', 'contents'),
-                  Input('btn-add', 'n_clicks_timestamp'),
-                  Input('txt_from', 'value'),
-                  Input('txt_to', 'value'),
-                  State('upload-data', 'filename'),
-                  State('upload-data', 'last_modified'),
-                  State('cytoscape-elements', 'elements'),
-                  prevent_initial_call=True)
-    def load_data(contents, n_clicks, txt_from, txt_to, filename, last_modified, elements):
+def create_stylesheet():
+    return [
+        {
+            'selector': 'node',
+            'style': {
+                'label': 'data(id)',
+                'font-size': '14px',
+                'width': '30px',
+                'height': '30px',
+            }
+        },
+        {
+            'selector': 'edge',
+            'style': {
+                'curve-style': 'taxi',
+                'target-arrow-shape': 'triangle',
+            }
+        }
+    ]
+
+def register_callbacks(app):
+    @app.callback(
+        Output('cytoscape-elements', 'elements'),
+        [Input('upload-data', 'contents'),
+         Input('btn-add', 'n_clicks_timestamp'),
+         Input('btn-remove', 'n_clicks_timestamp')],
+        [State('txt_from', 'value'),
+         State('txt_to', 'value'),
+         State('upload-data', 'filename'),
+         State('upload-data', 'last_modified'),
+         State('cytoscape-elements', 'elements'),
+         State("cytoscape-elements", "selectedNodeData")],
+        prevent_initial_call=True
+    )
+    def load_data(contents, add_clicks, remove_clicks, txt_from, txt_to, filename, last_modified, elements, selected):
         # For data load
         if ctx.triggered_id == 'upload-data':
-            elements, edges, nodes =[], [], []
+            elements, edges, nodes = [], [], []
             edges = parse_contents(contents, filename)
-            nodes = np.concatenate([edges.source.unique(), edges.target.unique()])
-            nodes = [{'data': {'id': name, 'label': name}} for name in nodes]
-            edges = [
-                {'data': {'source': source, 'target': target}}
-                for source, target in edges[['source','target']].values
-            ]
-            elements = edges+nodes
+            if edges is not None:
+                nodes = np.concatenate([edges.source.unique(), edges.target.unique()])
+                nodes = [{'data': {'id': name, 'label': name}} for name in nodes]
+                edges = [
+                    {'data': {'source': source, 'target': target}}
+                    for source, target in edges[['source','target']].values
+                ]
+                elements = edges+nodes
         # For adding data
         elif ctx.triggered_id == 'btn-add':
             edges = elements_to_edges(elements) if elements else pd.DataFrame()
             edges = pd.concat([edges, pd.DataFrame([txt_from,txt_to], index=['source','target']).T], axis=0, ignore_index=True).drop_duplicates()
             elements = edges_to_elements(edges)
+        elif ctx.triggered_id == 'btn-remove':
+            if selected[0]:
+                edges = elements_to_edges(elements) if elements else pd.DataFrame()
+                edges = edges.loc[(edges.source != selected[0]['id']) & (edges.target != selected[0]['id'])] 
+                elements = edges_to_elements(edges)
         return elements
-
-    # Save data
-    @app.callback(Output('download-data', 'data'),
-                  Input('btn-download', 'n_clicks'),
-                  State('cytoscape-elements', 'elements'),
-                  prevent_initial_call=True)
+    @app.callback(
+        Output('download-data', 'data'),
+        [Input('btn-download', 'n_clicks')],
+        [State('cytoscape-elements', 'elements')],
+        prevent_initial_call=True
+    )
     def save_data(n_clicks, elements):
         ele = pd.concat([pd.DataFrame.from_dict(i) for i in elements], axis=1).T.set_index('id')
         edges = ele.drop('label', axis=1).dropna().set_index('source')
-        return dcc.send_data_frame(edges.to_csv, 'mydf.csv', header=False)
+        return dcc.send_data_frame(edges.to_csv, 'mydf.tsv', sep='\t', header=False)
+    @app.callback(
+        Output('cytoscape-elements', 'btn-run'),
+        [Input('btn-run', 'n_clicks')],
+        [State('cytoscape-elements', 'selectedNodeData')],
+        prevent_initial_call=True
+    )
+    def run_process(n_clicks, data):
+        for process in data:
+            subprocess.call(process['label'], shell=True)
+
+
+def parse_contents(contents, filename):
+    content_type, content_string = contents.split(',')
+    decoded = base64.b64decode(content_string)
+    try:
+        edges = pd.read_csv(io.StringIO(decoded.decode('utf-8')), sep='\t', header=None).set_axis(['source','target'], axis=1)
+    except:
+        print('There was an error processing this file.')
+        edges = None
+    return edges
+
+def elements_to_edges(elements):
+    ele = pd.concat([pd.DataFrame.from_dict(i) for i in elements], axis=1).T.set_index('id')
+    edges = ele.drop('label', axis=1).dropna().reset_index(drop=True)
+    return edges
+
+def edges_to_elements(edges):
+    nodes = np.concatenate([edges.source.unique(), edges.target.unique()])
+    nodes = [{'data': {'id': name, 'label': name}} for name in nodes]
+    edges = [
+        {'data': {'source': source, 'target': target}}
+        for source, target in edges[['source','target']].values
+    ]
+    elements = edges+nodes
+    return elements
 
-    # Other functions
-    def parse_contents(contents, filename):
-        import base64
-        import io
-        content_type, content_string = contents.split(',')
-        decoded = base64.b64decode(content_string)
-        try:
-            if 'csv' in filename:
-                df = pd.read_csv(io.StringIO(decoded.decode('utf-8'))).set_axis(['source','target'], axis=1)
-            elif 'xls' in filename:
-                df = pd.read_excel(io.BytesIO(decoded))
-        except Exception as e:
-            return html.Div([
-                'There was an error processing this file.'
-            ])
-        return df
+#setup_gui()
 
-    def elements_to_edges(elements):
-        ele = pd.concat([pd.DataFrame.from_dict(i) for i in elements], axis=1).T.set_index('id')
-        edges = ele.drop('label', axis=1).dropna().reset_index(drop=True)
-        return edges
-
-    def edges_to_elements(edges):
-        nodes = np.concatenate([edges.source.unique(), edges.target.unique()])
-        nodes = [{'data': {'id': name, 'label': name}} for name in nodes]
-        edges = [
-            {'data': {'source': source, 'target': target}}
-            for source, target in edges[['source','target']].values
-        ]
-        elements = edges+nodes
-        return elements
-
-    app.run_server()
```

### Comparing `workforce-1.0.8/workforce/workforce.py` & `workforce-1.0.9/workforce/workforce.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 import subprocess
 
 class worker:
     def __init__(self, plan_file):
         # Load plan
         self.plan_file = plan_file
         with open(self.plan_file) as csvfile:
-            self.plan = list(csv.reader(csvfile, skipinitialspace=True))
+            self.plan = list(csv.reader(csvfile, delimiter="\t", skipinitialspace=True))
 
     def run(self):
         # Run loaded plan beginning from the first row
         self.init_time = str(time())
         logging.basicConfig(
-                filename=str(Path.home())+"/.wflog.csv",
-                filemode="a",
+                filename=str(Path.cwd())+"/wflog.csv",
+                filemode="w",
                 format="%(created).6f, "+self.init_time+", "+str(os.getpid())+", %(processName)s, %(message)s",
                 level=logging.INFO)
         logging.info("start %s", self.plan_file)
 
         def begin():
             def task(curr):
                 logging.info("%s, running", curr)
```

### Comparing `workforce-1.0.8/workforce.egg-info/PKG-INFO` & `workforce-1.0.9/workforce.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workforce
-Version: 1.0.8
+Version: 1.0.9
 Summary: Run bash commands with python multiprocessing according to a csv file edgelist.
 Home-page: https://github.com/theoportlock/workforce
 Author: Theo Portlock
 Author-email: zn.tportlock@gmail.com
 License: MIT license
 Keywords: workforce
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: networkx
+Requires-Dist: pydot
+Requires-Dist: dash_cytoscape
+Requires-Dist: dash
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: openpyxl
 
 =========
 workforce
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/workforce.svg
@@ -74,22 +81,14 @@
 
    from workforce.workforce import worker
    steve = worker("<PLAN.CSV>")
    steve.run()
 
 The schema should be in the format of a csv with two columns. On the left and right column is the source and target command respectively (see example). Produces a logfile for each run.
 
-Testing
--------
-Testing can be done within the github directory by running:
-
-.. code-block:: bash
-
-   python -m unittest -v
-
 
 =======
 History
 =======
 
 0.1.0 (2021-01-16)
 ------------------
```

