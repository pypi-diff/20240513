# Comparing `tmp/activetigger-0.1.2.tar.gz` & `tmp/activetigger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activetigger-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "activetigger-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `activetigger-0.1.2.tar` & `activetigger-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      251 2024-05-07 13:46:44.712783 activetigger-0.1.2/.gitignore
--rw-r--r--   0        0        0     1119 2024-02-26 10:50:38.000000 activetigger-0.1.2/LICENSE
--rw-r--r--   0        0        0       47 2024-03-20 21:05:20.000000 activetigger-0.1.2/MANIFEST.in
--rw-r--r--   0        0        0     1567 2024-05-07 15:33:29.062626 activetigger-0.1.2/README.md
--rw-r--r--   0        0        0       52 2024-05-07 13:44:29.885746 activetigger-0.1.2/activetigger/__init__.py
--rw-r--r--   0        0        0     2348 2024-05-08 10:56:37.173857 activetigger-0.1.2/activetigger/__main__.py
--rw-r--r--   0        0        0    32737 2024-05-07 13:39:42.419994 activetigger-0.1.2/activetigger/api.py
--rw-r--r--   0        0        0     3459 2024-05-07 13:39:42.420236 activetigger-0.1.2/activetigger/datamodels.py
--rw-r--r--   0        0        0    42086 2024-05-08 12:32:14.842766 activetigger-0.1.2/activetigger/frontend.py
--rw-r--r--   0        0        0    16156 2024-05-07 13:39:42.420803 activetigger-0.1.2/activetigger/functions.py
--rw-r--r--   0        0        0      430 2024-03-20 09:12:27.000000 activetigger-0.1.2/activetigger/html/welcome.html
--rw-r--r--   0        0        0  1167848 2024-04-19 14:23:17.022833 activetigger-0.1.2/activetigger/img/active_tigger.png
--rw-r--r--   0        0        0    34298 2024-05-07 13:39:42.421040 activetigger-0.1.2/activetigger/models.py
--rw-r--r--   0        0        0    48558 2024-05-07 13:39:42.421425 activetigger-0.1.2/activetigger/server.py
--rw-r--r--   0        0        0    61374 2024-05-07 13:39:42.421917 activetigger-0.1.2/activetigger/widget.py
--rw-r--r--   0        0        0      180 2024-05-07 13:39:42.422144 activetigger-0.1.2/config.yaml
--rw-r--r--   0        0        0      838 2024-03-27 17:01:50.295115 activetigger-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       35 2024-02-09 19:50:15.000000 activetigger-0.1.2/pytest.ini
--rw-r--r--   0        0        0      633 2024-05-07 15:33:07.767556 activetigger-0.1.2/requirements.txt
--rw-r--r--   0        0        0       89 2024-02-09 14:40:46.000000 activetigger-0.1.2/tests/test_api.py
--rw-r--r--   0        0        0     2098 2024-02-18 21:23:56.000000 activetigger-0.1.2/tests/test_project.py
--rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 activetigger-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-07 13:46:44.712783 activetigger-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1119 2024-02-26 10:50:38.000000 activetigger-0.1.3/LICENSE
+-rw-r--r--   0        0        0       47 2024-03-20 21:05:20.000000 activetigger-0.1.3/MANIFEST.in
+-rw-r--r--   0        0        0     1567 2024-05-07 15:33:29.062626 activetigger-0.1.3/README.md
+-rw-r--r--   0        0        0       52 2024-05-13 10:14:59.621547 activetigger-0.1.3/activetigger/__init__.py
+-rw-r--r--   0        0        0     2341 2024-05-12 13:06:12.876605 activetigger-0.1.3/activetigger/__main__.py
+-rw-r--r--   0        0        0    34078 2024-05-12 19:03:51.127924 activetigger-0.1.3/activetigger/api.py
+-rw-r--r--   0        0        0     3506 2024-05-13 08:56:36.042466 activetigger-0.1.3/activetigger/datamodels.py
+-rw-r--r--   0        0        0    46829 2024-05-13 10:07:20.701050 activetigger-0.1.3/activetigger/frontend.py
+-rw-r--r--   0        0        0    16156 2024-05-07 13:39:42.420803 activetigger-0.1.3/activetigger/functions.py
+-rw-r--r--   0        0        0      430 2024-03-20 09:12:27.000000 activetigger-0.1.3/activetigger/html/welcome.html
+-rw-r--r--   0        0        0  1167848 2024-04-19 14:23:17.022833 activetigger-0.1.3/activetigger/img/active_tigger.png
+-rw-r--r--   0        0        0    34355 2024-05-13 09:12:30.243895 activetigger-0.1.3/activetigger/models.py
+-rw-r--r--   0        0        0    51979 2024-05-13 09:21:39.350949 activetigger-0.1.3/activetigger/server.py
+-rw-r--r--   0        0        0    61381 2024-05-12 16:11:40.283511 activetigger-0.1.3/activetigger/widget.py
+-rw-r--r--   0        0        0      180 2024-05-07 13:39:42.422144 activetigger-0.1.3/config.yaml
+-rw-r--r--   0        0        0      838 2024-03-27 17:01:50.295115 activetigger-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-02-09 19:50:15.000000 activetigger-0.1.3/pytest.ini
+-rw-r--r--   0        0        0      655 2024-05-13 09:33:20.381096 activetigger-0.1.3/requirements.txt
+-rw-r--r--   0        0        0       89 2024-02-09 14:40:46.000000 activetigger-0.1.3/tests/test_api.py
+-rw-r--r--   0        0        0     2098 2024-02-18 21:23:56.000000 activetigger-0.1.3/tests/test_project.py
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 activetigger-0.1.3/PKG-INFO
```

### Comparing `activetigger-0.1.2/LICENSE` & `activetigger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `activetigger-0.1.2/README.md` & `activetigger-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `activetigger-0.1.2/activetigger/__main__.py` & `activetigger-0.1.3/activetigger/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     # if no config file, create default one
     if not Path(args.config).exists():
         print("Creating config.yaml file by default")
         content = """path: ./projects
 secret_key: f63aeb7426d2c8a3defc02a3e788c2f311482d6cff557c2c5bdebc71d67b507a
 path_models: ./models
-users:
 """
         with open("./config.yaml","w") as f:
             f.write(content)
 
     # launch streamlit app
     if not args.server:
         print('Start streamlit app')
```

### Comparing `activetigger-0.1.2/activetigger/api.py` & `activetigger-0.1.3/activetigger/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from jose import JWTError
 import importlib
 from pydantic import ValidationError
 from activetigger.server import Server, Project
 import activetigger.functions as functions
 from activetigger.datamodels import ProjectModel, TableElementsModel, Action, AnnotationModel,\
       SchemeModel, ResponseModel, ProjectionModel, User, Token, RegexModel, SimpleModelModel, BertModelModel, ParamsModel,\
-      UmapParams, TsneParams
+      UmapParams, TsneParams, NextModel
 
 
 logging.basicConfig(filename='log_server.log', level=logging.DEBUG,
                     format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
 logger = logging.getLogger('api')
 
@@ -182,14 +182,26 @@
 async def read_users_me(current_user: Annotated[User, Depends(get_current_user)]) -> ResponseModel:
     """
     Information on current user
     """
     r = ResponseModel(statut="success", data=current_user)
     return r
 
+@app.get("/users", dependencies=[Depends(verified_user)])
+async def existing_users() -> ResponseModel:
+    """
+    Get users information
+    TODO : users to specific projects ?
+    """
+    data = {
+        "users":server.existing_users()
+        }
+    r = ResponseModel(status="success", data=data)
+    return r
+
 @app.post("/users/create", dependencies=[Depends(verified_user)])
 async def create_user(username:str = Query(),
                       password:str = Query(),
                       projects:str = Query(None)) -> ResponseModel:
     """
     Create user
     """
@@ -202,14 +214,15 @@
 
 @app.post("/users/delete", dependencies=[Depends(verified_user)])
 async def delete_user(username:str = Query()) -> ResponseModel:
     """
     Delete user
     """
     r = server.delete_user(username)
+    print(r)
     if "success" in r:
         r = ResponseModel(status="success", message=r["success"])
     else:
         r = ResponseModel(status="error", message=r["success"])
     return r
 
 # Projects management
@@ -268,14 +281,15 @@
                       project_name:str = Form(),
                       col_text:str = Form(),
                       col_id:str = Form(),
                       col_label:str = Form(None),
                       cols_context:List[str] = Form(None),
                       n_train:int = Form(),
                       n_test:int = Form(),
+                      cols_test:List[str] = Form(None),
                       embeddings:list = Form(None),
                       n_skip:int = Form(None),
                       language:str = Form(None),
                       ) -> ResponseModel:
     """
     Load new project
         file (file)
@@ -288,14 +302,15 @@
     params_in = {
         "project_name":project_name,
         "user":username,         
         "col_text":col_text,
         "col_id":col_id,
         "n_train":n_train,
         "n_test":n_test,
+        "cols_test":cols_test,
         "embeddings":embeddings,
         "n_skip":n_skip,
         "language":language,
         "col_label":col_label,
         "cols_context":cols_context
         }
     
@@ -335,37 +350,60 @@
         return ResponseModel(status="error", message=r["error"])
     else:
         return ResponseModel(status="success",  message=r["success"])
 
 # Annotation management
 #----------------------
 
-@app.get("/elements/next", dependencies=[Depends(verified_user)])
+# @app.get("/elements/next", dependencies=[Depends(verified_user)])
+# async def get_next(project: Annotated[Project, Depends(get_project)],
+#                    username: Annotated[str, Header()],
+#                    scheme:str,
+#                    selection:str = "deterministic",
+#                    sample:str = "untagged",
+#                    tag:str|None = None,
+#                    history:list = [],
+#                    frame:list[float]|None = Query(None)) -> ResponseModel:
+#     """
+#     Get next element
+#     """
+#     r = project.get_next(
+#                         scheme = scheme,
+#                         selection = selection,
+#                         sample = sample,
+#                         user = username,
+#                         tag = tag,
+#                         history=history,
+#                         frame = frame
+#                         )
+#     if "error" in r:
+#         return ResponseModel(status="error", message=r["error"])
+#     return ResponseModel(status="success", data = r)
+
+@app.post("/elements/next", dependencies=[Depends(verified_user)])
 async def get_next(project: Annotated[Project, Depends(get_project)],
                    username: Annotated[str, Header()],
-                   scheme:str,
-                   selection:str = "deterministic",
-                   sample:str = "untagged",
-                   tag:str|None = None,
-                   frame:list[float]|None = Query(None)) -> ResponseModel:
+                   next:NextModel ) -> ResponseModel:
     """
     Get next element
     """
     r = project.get_next(
-                        scheme = scheme,
-                        selection = selection,
-                        sample = sample,
+                        scheme = next.scheme,
+                        selection = next.selection,
+                        sample = next.sample,
                         user = username,
-                        tag = tag,
-                        frame = frame
+                        tag = next.tag,
+                        history=next.history,
+                        frame = next.frame
                         )
     if "error" in r:
         return ResponseModel(status="error", message=r["error"])
     return ResponseModel(status="success", data = r)
 
+
 @app.get("/elements/projection/current", dependencies=[Depends(verified_user)])
 async def get_projection(project: Annotated[Project, Depends(get_project)],
                          username: Annotated[str, Header()],
                          scheme:str|None) -> ResponseModel:
     """
     Get projection data if computed
     """
```

### Comparing `activetigger-0.1.2/activetigger/datamodels.py` & `activetigger-0.1.3/activetigger/datamodels.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,34 +16,37 @@
     n_test:int
     dir:Path|None = None
     embeddings:list = []
     n_skip:int = 0
     default_scheme: list = []
     language:str = "fr"
     col_label:str|None = None # TODO: load existing tags
-    cols_context:list = [] # TODO: select variable to keep
+    cols_context:list = []
+    cols_test:list = []
+    test: bool = False
+
 
 class Action(str, Enum):
     delete = "delete"
     add = "add"
     update = "update"
 
 class Scheme(BaseModel):
     """
     Set of labels
     """
     labels:list[str]
 
 class NextModel(BaseModel):
-    """
-    Request of an element
-    """
-    scheme:str = "default"
-    mode:str = "deterministic"
-    on:str|None = "untagged"
+    scheme:str
+    selection:str = "deterministic"
+    sample:str = "untagged"
+    tag:str|None = None
+    frame:list[float]|None = None
+    history: list = []
 
 class SchemesModel(BaseModel):
     """
     Schemes model    
     """
     project_name:str
     availables:dict
```

### Comparing `activetigger-0.1.2/activetigger/frontend.py` & `activetigger-0.1.3/activetigger/frontend.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 import matplotlib.pyplot as plt
 import importlib
 import numpy as np
 from io import BytesIO
 import textwrap
 import streamlit as st
 from streamlit_autorefresh import st_autorefresh
+from streamlit_option_menu import option_menu
+
 
 URL_SERVER = "http://0.0.0.0:5000"
 update_time = 2000
+st.set_page_config(page_title="pyActiveTigger v0.1")
+
 count = st_autorefresh(interval=update_time, limit=None, key="fizzbuzzcounter")
 
 if not "header" in st.session_state:
     st.session_state.header = None
 if not "history" in st.session_state:
     st.session_state.history = []
 
 # TODO : see the computational use ...
-# TODO : windows of selection -> need to move to Dash ?
+# TODO : windows of selection -> need to move to Dash
 
 # Interface organization
 #-----------------------
 
 def main():
     # initialize variables
     if 'logged_in' not in st.session_state:
@@ -35,21 +39,20 @@
     if 'page' not in st.session_state:
         st.session_state['page'] = "Projects"
     st.session_state.state = _get_state()   
     data_path = importlib.resources.files("activetigger")
     image_path = "img/active_tigger.png"
     img = open(data_path / image_path, 'rb').read()
     st.sidebar.image(img)
-    #st.sidebar.write(datetime.datetime.now())
     # start the interface
     if not st.session_state['logged_in']:
         login_page()
     else:
-        st.sidebar.write(f"Current user: {st.session_state.user}")
         app_navigation()
+        st.sidebar.write(f"Current user: {st.session_state.user}")
 
 def login_page():
     """
     Page to log in
     """
     st.title("Login")
     username = st.text_input("Username")
@@ -77,43 +80,49 @@
     }</style>""", unsafe_allow_html=True)
     st.markdown("""
     <style>.element-container:has(#button-blue) + div button {
     background-color: #58afff;
     }</style>""", unsafe_allow_html=True)
 
     options = ["Projects",
-               "Schemes",
-               "Features",
                "Annotate",
                "Description",
                "Active Model",
                "Global Model",
+               "Test Model",
                "Export"]
-    st.session_state['page'] = st.sidebar.radio("Navigate", 
-                                                options, 
-                                                key="menu", 
-                                                index = options.index(st.session_state['page']))
+    
+    # add user management
+    if st.session_state.user == "root":
+        options = options + ["Configuration"]    
+
+    with st.sidebar:
+        st.session_state['page'] = option_menu("Navigate", options, menu_icon="cast")
 
     # navigating
     if st.session_state['page'] == "Projects":
         projects()
-    elif st.session_state['page'] == "Schemes":
-        schemes()
-    elif st.session_state['page'] == "Features":
-        features()
-    elif st.session_state['page'] == "Annotate":
-        annotate()
-    elif st.session_state['page'] == "Description":
-        description()
-    elif st.session_state['page'] == "Active Model":
-        simplemodels()
-    elif st.session_state['page'] == "Global Model":
-        bertmodels()
-    elif st.session_state['page'] == "Export":
-        export()
+    else:
+        if not "current_project" in st.session_state:
+            st.write("Select a project first")
+            return
+        elif st.session_state['page'] == "Annotate":
+            annotate()
+        elif st.session_state['page'] == "Description":
+            description()
+        elif st.session_state['page'] == "Active Model":
+            simplemodels()
+        elif st.session_state['page'] == "Global Model":
+            bertmodels()
+        elif st.session_state['page'] == "Test Model":
+            test_model()
+        elif st.session_state['page'] == "Export":
+            export()
+        elif st.session_state['page'] == "Configuration":
+            configuration()
 
 def projects():
     """
     Projects page
     - select a project
     - create one
     """
@@ -132,16 +141,17 @@
     
     col1, col2, col3 = st.columns(3)
 
     # load a project
     with col1:
         st.markdown('<span id="button-green"></span>', unsafe_allow_html=True)
         if st.button("Load"):
-            st.session_state.current_project = option
-            st.session_state.page = "Schemes"
+            if option:
+                st.session_state.current_project = option
+            #st.session_state.page = "Schemes"
             return None
 
     # delete a project
     with col2:
         st.markdown('<span id="button-red"></span>', unsafe_allow_html=True)
         if st.button("Delete"):
             #st.write(f"Deleting {option}")
@@ -149,15 +159,15 @@
 
     # create a project
     with col3:
         st.markdown('<span id="button-blue"></span>', unsafe_allow_html=True)
         if st.button("New project"):
             st.session_state['new_project'] = True
 
-    # display the creation menu
+    # display the creation menu if create a project
     if st.session_state.get('new_project', True):
         project_name = st.text_input("Project name", value="")
         dic_langage = {"French":"fr",
                        "English":"en",
                        "Spanish":"es"}
         language = st.selectbox("Language:",list(dic_langage))
         file = st.file_uploader("Load file (CSV or Parquet)", 
@@ -173,85 +183,73 @@
             st.dataframe(df.head())
             st.write("Select columns")
             column_id = st.selectbox("Ids:",list(df.columns))
             column_text = st.selectbox("Texts:",list(df.columns))
             column_label = st.selectbox("Labels:",list(df.columns))
             columns_context = st.multiselect("Context:",list(df.columns))
             n_train = st.number_input("N train", min_value=100, max_value=len(df),key="n_train")
-            n_test = st.number_input("N test", min_value=100, max_value=len(df),key="n_test")
+            n_test = st.number_input("N test (0 if no test set)", min_value=0, max_value=len(df),key="n_test")
+            cols_test = st.multiselect("Stratify by", list(df.columns))
             data = {
                     "project_name": project_name,
                     "user":st.session_state.user,
                     "col_text": column_text,
                     "col_id":column_id,
                     "col_label":column_label,
                     "cols_context": columns_context,
                     "n_train":n_train,
                     "n_test":n_test, 
+                    "cols_test":cols_test,
                     "language":dic_langage[language]
                     }
             if st.button("Create"):
                 _create_project(data, df, file.name)
                 st.session_state.new_project = False
-    return None
 
-
-def schemes():
-    """
-    Scheme page
-    """
+    # display the scheme menu if project loaded
     if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
+                st.subheader("Select a project")
+                return
 
-    st.title("Schemes")
-    st.write("Interface to manage schemes & label")
-    st.subheader("Schemes")
-    options_schemes = list(st.session_state.state["schemes"]["available"].keys())
-    scheme = st.selectbox("Current scheme:", options = options_schemes, index=0, placeholder="Select a scheme")
-    st.session_state.current_scheme = scheme # select scheme
-    if st.button("Delete scheme"):
-        if scheme is not None:
-            st.write(f"Deleting scheme {scheme}")
-            _delete_scheme(scheme)
-    new_scheme = st.text_input(label="New scheme", placeholder="New scheme name", label_visibility="hidden")
-    if st.button("Create scheme"):
-        if new_scheme is not None:
-            st.write(f"Creating scheme {new_scheme}")
-            _create_scheme(new_scheme)
-    st.markdown("<hr>", unsafe_allow_html=True)
-    st.subheader("Labels")
-    options_labels = []
-    if st.session_state.current_scheme is not None:
-        options_labels = st.session_state.state["schemes"]["available"][st.session_state.current_scheme]
-    label = st.selectbox(label="Label",options = options_labels, index=None, 
-                         placeholder="Select a label", label_visibility="hidden")
-    if st.button("Delete label"):
-        if label is not None:
-            st.write(f"Deleting label {label}")
-            _delete_label(label)
-    new_label = st.text_input(label="New label", placeholder="New label name", label_visibility="hidden")
-    if st.button("Create label"):
-        if new_label is not None:
-            st.write(f"Creating label {new_label}")
-            _create_label(new_label)
+    if "current_project" in st.session_state:
+        with st.expander("Manage schemes"):
+            st.markdown("<hr>", unsafe_allow_html=True)
+            options_schemes = list(st.session_state.state["schemes"]["available"].keys())
+            col1, col2 = st.columns(2)
+            with col1:
+                scheme = st.selectbox("Select scheme to use:", options = options_schemes, index=0, placeholder="Select a scheme")
+                st.session_state.current_scheme = scheme
+            with col2:
+                st.markdown("<br>", unsafe_allow_html=True)
+                if st.button("Delete scheme"):
+                    if scheme is not None:
+                        st.write(f"Deleting scheme {scheme}")
+                        _delete_scheme(scheme)
+            col1, col2 = st.columns(2)
+            with col1:
+                new_scheme = st.text_input(label="New scheme", placeholder="New scheme name", label_visibility="hidden")
+            with col2:
+                st.markdown("<br>", unsafe_allow_html=True)
+                if st.button("Create scheme"):
+                    if new_scheme is not None:
+                        st.write(f"Creating scheme {new_scheme}")
+                        _create_scheme(new_scheme)
+
+    with st.expander("Manage features"):
+        if st.session_state.current_project:
+           features()
+    
+    return None
 
-    st.markdown("<hr>", unsafe_allow_html=True)
 
 def features():
     """
     Feature page
     """
-    if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
-
-    st.title("Features")
-    st.write("Interface to manage features.")
-
+    st.write("Manage features")
     c = st.session_state.state["features"]["training"]
     if not len(c) == 0:
         st.html(f"<div style='background-color: #ffcc00; padding: 10px;'>Processes currently running: {c}</div>")
 
     feature = st.selectbox(label="Available",
                            options = st.session_state.state["features"]["available"])
     if st.button("Delete feature"):
@@ -286,90 +284,95 @@
         if st.session_state.current_scheme is not None:
             st.session_state.page = "Annotate"
 
 def annotate():
     """
     Annotate page
     """
-    if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
-    
-    mode_selection = st.session_state.state["next"]["methods_min"] # default options
+    # configure menu
+    mode_selection = st.session_state.state["next"]["methods_min"]
     if _is_simplemodel():
         mode_selection = st.session_state.state["next"]["methods"]
     mode_sample = st.session_state.state["next"]["sample"]
 
     # default element if not defined
     if "selection" not in st.session_state:
         st.session_state.selection = mode_selection[0]
     if "sample" not in st.session_state:
         st.session_state.sample = mode_sample[0]
     if "tag" not in st.session_state:
         st.session_state.tag = None
         
     # get next element with the current options
-    if "current_element" not in st.session_state:
+    if not "current_element" in st.session_state:
         _get_next_element()
+#        st.session_state.current_element = None
 
     # display page
-    st.title("Annotate")
-    st.write("Interface to annotate data.")
-    col1, col2, col3 = st.columns(3)
+    st.title("Annotate data")
+    st.write("Current history (reload to reset):", len(st.session_state.history))
+    col1, col2, col3, col4 = st.columns(4)
     with col1:
         st.selectbox(label="Selection", options = mode_selection, key = "selection", label_visibility="hidden")
     with col2:
         st.selectbox(label="Sample", options = mode_sample, key = "sample", label_visibility="hidden")
     with col3:
         tag_options = []
         if st.session_state.selection == "maxprob":
             tag_options = st.session_state.state["schemes"]["available"][st.session_state.current_scheme]
         st.selectbox(label="Tag", options = tag_options, key = "tag", label_visibility="hidden")
-    if st.button("Back"):
-                st.write("Back")
-                _get_previous_element()
-    st.markdown(f"""
-        <div>{st.session_state.current_element["predict"]}</div>
-        <div>{st.session_state.current_element['info']}</div>
-        <div style="
-            border: 2px solid #4CAF50;
-            padding: 10px;
-            border-radius: 5px;
-            color: #4CAF50;
-            font-family: sans-serif;
-            text-align: justify;
-            margin: 10px;
-            min-height: 300px;
-        ">
-            {st.session_state.current_element["text"]}
-        </div>
-
-    """, unsafe_allow_html=True)
-
-    labels = st.session_state.state["schemes"]["available"][st.session_state.current_scheme]
-    cols = st.columns(len(labels)+1)
-    for col, label in zip(cols[:-1], labels):
-        with col:
-            if st.button(label):
-                _send_tag(label)
-                _get_next_element()
-
-    st.markdown("<hr>", unsafe_allow_html=True)
+    with col4:
+        st.markdown("<br>", unsafe_allow_html=True)
+        if st.button("Back"):
+                    _get_previous_element()
+    if st.session_state.current_element:
+        st.markdown(f"""
+            <div>{st.session_state.current_element["predict"]}</div>
+            <div>{st.session_state.current_element['info']}</div>
+            <div style="
+                border: 2px solid #4CAF50;
+                padding: 10px;
+                border-radius: 5px;
+                color: #4CAF50;
+                font-family: sans-serif;
+                text-align: justify;
+                margin: 10px;
+                min-height: 300px;
+            ">
+                {st.session_state.current_element["text"]}
+            </div>
+
+        """, unsafe_allow_html=True)
+
+        _display_labels()
+
+    with st.expander("Manage tags"):
+        col1, col2 = st.columns(2)
+        options_labels = []
+        options_labels = st.session_state.state["schemes"]["available"][st.session_state.current_scheme]
+        with col1:
+            new_label = st.text_input(label="New label", placeholder="New label name", label_visibility="hidden")
+        with col2:
+            st.markdown("<br>", unsafe_allow_html=True)
+            if st.button("Create label"):
+                if new_label is not None:
+                    st.write(f"Creating label {new_label}")
+                    _create_label(new_label)
+        with col1:
+            label = st.selectbox(label="Label",options = options_labels, index=None, 
+                                placeholder="Select a label", label_visibility="hidden")
+        with col2:
+            st.markdown("<br>", unsafe_allow_html=True)
+            if st.button("Delete label"):
+                if label is not None:
+                    st.write(f"Deleting label {label}")
+                    _delete_label(label)
+        col1, col2 = st.columns(2)
 
-    # managing projection display
-    if "projection" not in st.session_state:
-        st.session_state.projection = False
-    # switch button
-    if st.button("Projection"):
-        if not st.session_state.projection:
-            st.session_state.projection = True
-        else:
-            st.session_state.projection = False
-    # displaying menu
-    if st.session_state.projection:
+    with st.expander("Projection"):
         st.selectbox(label="Method", 
                      options = list(st.session_state.state["projections"]["available"].keys()), 
                      key = "projection_method")
         st.text_area(label="Parameters", 
                      value=json.dumps(st.session_state.state["projections"]["available"]["umap"], indent=2),
                      key = "projection_params", label_visibility="hidden")
         st.multiselect(label="Features", options=st.session_state.state["features"]["available"],
@@ -386,58 +389,64 @@
                 if not "projection_visualization" in st.session_state:
                     st.session_state.projection_visualization = _plot_visualisation()
                     st.session_state.projection_visualization.update_layout({"uirevision": "foo"}, overwrite=True)
 
         if "projection_visualization" in st.session_state:
             st.plotly_chart(st.session_state.projection_visualization, use_container_width=True)            
 
+
+def _display_labels():
+    """
+    Display labels
+    """
+    labels = st.session_state.state["schemes"]["available"][st.session_state.current_scheme]
+    cols = st.columns(len(labels)+1)
+    for col, label in zip(cols[:-1], labels):
+        with col:
+            if st.button(label):
+                _send_tag(label)
+                _get_next_element()
+
 def description():
     """
     Description page
     """
-    if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
-
     st.title("Description")
     st.subheader("Statistics")
     st.write("Description of the current data")
     statistics = _get_statistics()
-    st.markdown(statistics, unsafe_allow_html=True)
+    #st.markdown(statistics, unsafe_allow_html=True)
+    st.dataframe(statistics, width=500)
     st.markdown("<hr>", unsafe_allow_html=True)
     st.subheader("Display data")
     col1, col2, col3 = st.columns(3)
     with col1:
         st.selectbox(label="Sample", options=["all","tagged","untagged","recent"], index=3, key="data_mode") 
     with col2:
         st.number_input(label="min", key="data_min", min_value=0, value=0, step=1)
     with col3:
         st.number_input(label="min", key="data_max", min_value=0, value=10, step=1)
     if st.button(label="Send changes"):
         st.write("Send changes")
         _send_table()
 
-    st.session_state.data_df = df = _get_table()
+    st.session_state.data_df = _get_table()
+    
 
     # make the table editable
     labels =  st.session_state.state["schemes"]["available"][st.session_state.current_scheme]
     st.session_state.data_df["labels"] = (
-        st.session_state.data_df["labels"].astype("category").cat.remove_categories(
-            st.session_state.data_df['labels']).cat.add_categories(labels)
-    )
+        (st.session_state.data_df["labels"].astype("category")).cat.add_categories([l for l in labels if not l in st.session_state.data_df["labels"].unique()])
+            )
     st.data_editor(st.session_state.data_df[["labels", "text"]], disabled=["text"])
 
 def simplemodels():
     """
     Simplemodel page
     """
-    if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
-
     if not "computing_simplemodel" in st.session_state:
         st.session_state.computing_simplemodel = False
 
     current_model = None
     statistics = ""
     params = None
     status = ""
@@ -484,18 +493,14 @@
         _train_simplemodel()
 
 def bertmodels():
     """
     Bertmodel page
     TODO : améliorer la présentation
     """
-    if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
-
     st.title("Global model")
     st.write("Train, test and predict with final model") 
 
     if st.session_state.user in st.session_state.state["bertmodels"]["training"]:
         st.session_state.bert_training = True
         st.html(f"<div style='background-color: #ffcc00; padding: 10px;'>Model under training</div>")
     else:
@@ -532,17 +537,22 @@
         data = _bert_informations()
         if data:
             st.pyplot(data[0])
             st.html(data[1])
 
     st.markdown("<hr>", unsafe_allow_html=True)
     st.subheader("Training model")
-    st.selectbox(label="Select model", 
-                 options = st.session_state.state["bertmodels"]["options"], 
-                 key = "bm_train")
+    col1, col2 = st.columns(2)
+    with col1:
+        st.selectbox(label="Select model", 
+                    options = st.session_state.state["bertmodels"]["options"], 
+                    key = "bm_train")
+    with col2:
+        # TO IMPLEMENT BACKEND
+        st.text_input("HuggingFace model to use", key="bm_train_hf", disabled=True, placeholder="Not implemented yet")
     st.text_area(label="Parameters", key = "bm_params", 
                  value=json.dumps(st.session_state.state["bertmodels"]["base_parameters"], 
                                   indent=2))
     
     if not st.session_state.bert_training:
         if st.button("⚙️Train"):
             st.write("⚙️Train")
@@ -552,18 +562,14 @@
             st.write("⚙️Stop")
             _stop_bertmodel()
 
 def export():
     """
     Export page
     """
-    if not "current_project" in st.session_state:
-        st.write("Select a project first")
-        return
-
     st.title("Export")
     st.write("Export your data and models") 
 
     col1, col2 = st.columns((2,10))
     with col1:
         st.selectbox(label="Format", options=["csv", "parquet"], key="export_format")
 
@@ -602,14 +608,92 @@
                            file_name=f"{st.session_state.bert_model}.tar.gz")
         
         # TODO : test if available ...
         st.download_button(label="Download predictions", 
                            data=_export_predictions(), 
                            file_name=f"predictions.{st.session_state.export_format}")
 
+def configuration():
+    """
+    Configuration panel
+    - User creation
+    """
+    st.title("Configuration")
+    st.subheader("User management")
+
+    col1, col2 = st.columns(2)
+    with col1:
+        existing_users = _get_users()
+        users = st.selectbox("Existing users:",existing_users)
+    with col2:
+        st.markdown("<br>", unsafe_allow_html=True)
+        if st.button("Delete"):
+            _delete_user()
+            st.write("Delete user")
+
+    st.write("Add user")
+    col1, col2, col3 = st.columns(3)
+    with col1:
+        new_user = st.text_input("New user")
+    with col2:
+        new_password = st.text_input("Password")
+    with col3:
+        st.markdown("<br>", unsafe_allow_html=True)
+        if st.button("Create"):
+            _create_user(new_user, new_password)
+            st.write("Create user")
+
+def test_model():
+    """
+    Test annotation interface
+    """
+    st.title("Test the model")
+    st.write("TODO : display the number of elements ? How many to code ?")
+    st.write("TODO : display only if bertmodel trained ?")
+
+    # Case there is no test set
+    if not st.session_state.state["params"]["test"]:
+        file = st.file_uploader("Load file (CSV or Parquet)", 
+                        type=['csv', 'parquet'], 
+                        accept_multiple_files=False)
+        if file:
+            if file.name.endswith('.csv'):
+                df = pd.read_csv(file)
+            elif file.name.endswith('.parquet'):
+                df = pd.read_parquet(file)
+            else:
+                st.error("Type not supported")
+        # TODO : send the file to load 
+
+    else:
+        st.session_state.selection = "test"
+        st.session_state.tag = None
+        st.session_state.sample = None
+
+        _get_next_element()
+
+        st.markdown(f"""
+            <div style="
+                border: 2px solid #4CAF50;
+                padding: 10px;
+                border-radius: 5px;
+                color: #4CAF50;
+                font-family: sans-serif;
+                text-align: justify;
+                margin: 10px;
+                min-height: 300px;
+            ">
+                {st.session_state.current_element["text"]}
+            </div>
+
+        """, unsafe_allow_html=True)
+
+        _display_labels()
+    # si un fichier de test existe, l'utiliser
+    # sinon proposer de charger un fichier de test
 
 # Internal functions
 # ------------------
 
 def _post(route:str, 
         params:dict|None = None, 
         files:str|None = None,
@@ -679,14 +763,52 @@
         state = _get(route = f"/state/{st.session_state.current_project}")
         if state["status"]=="error":
             print(state)
             return {}
         return state["data"]
     return {}
 
+
+def _get_users():
+    """
+    Get existing users
+    """
+    r = _get(route="/users")
+    return r["data"]["users"]
+
+def _create_user(username:str, password:str):
+    """
+    Create user
+    """
+    params = {"username":username,
+              "password":password, 
+              "projects":"all"}
+    r = _post(route="/users/create", 
+                params=params
+                )
+    if r["status"] == "error":
+        print(r["message"])
+        st.write(r["message"])
+        return False
+    return r
+
+def _delete_user(username:str):
+    """
+    Delete user
+    """
+    params = {"username":username}
+    r = _post(route="/users/delete", 
+                params=params
+                )
+    if r["status"] == "error":
+        print(r["message"])
+        st.write(r["message"])
+        return False
+    return r    
+
 def _create_project(data, df, name):
     """
     Create project
     """
     buffer = BytesIO()
     df.to_csv(buffer)
     buffer.seek(0)
@@ -834,27 +956,44 @@
     #                 f['layout']['yaxis']['range'][0],
     #                 f['layout']['xaxis']['range'][1], 
     #                 f['layout']['yaxis']['range'][1]]
     # except:
     #     x1y1x2y2 = []
     x1y1x2y2 = []
 
+    # params = {
+    #         "project_name":st.session_state.current_project,
+    #         "user":st.session_state.user,
+    #         "scheme":st.session_state.current_scheme,
+    #         "selection":st.session_state.selection,
+    #         "sample":st.session_state.sample,
+    #         "tag":st.session_state.tag,
+    #         "history":st.session_state.history,
+    #         "frame":x1y1x2y2
+    #         }
     params = {
             "project_name":st.session_state.current_project,
+            "user":st.session_state.user
+    }
+    data = {
             "scheme":st.session_state.current_scheme,
             "selection":st.session_state.selection,
             "sample":st.session_state.sample,
-            "user":st.session_state.user,
             "tag":st.session_state.tag,
+            "history":st.session_state.history,
             "frame":x1y1x2y2
             }
     
-    r = _get(route = "/elements/next",
-                    params = params)
-    
+    # r = _get(route = "/elements/next",
+    #                 params = params)
+    r = _post(route = "/elements/next",
+              params = params,
+              json_data = data)
+
+    print(r)
     if r["status"] == "error":
         print(r["message"])
         st.write(r["message"])
         return False
 
     st.session_state.current_element = r["data"]
 #    self._textarea.value = self.current_element["text"]
@@ -986,18 +1125,20 @@
 def _get_statistics():
     params = {"project_name":st.session_state.current_project, 
             "scheme":st.session_state.current_scheme, 
             "user":st.session_state.user}
     r = _get("/description",params = params)
     if r["status"]=="error":
         return r["message"]
-    text = ""
-    for k,v in r["data"].items():
-        text += f"<br>- <b>{k}</b>: {v}"
-    return text
+    #text = ""
+    tab = pd.DataFrame([[k,v] for k,v in r["data"].items()], columns=["information","values"]).set_index("information")
+    #for k,v in r["data"].items():
+    #    text += f"<br>- <b>{k}</b>: {v}"
+    #return text
+    return tab
 
 def _get_table():
     """
     Get data as a table
     """
     params = {
                 "project_name":st.session_state.current_project,
@@ -1135,20 +1276,26 @@
     """
     try:
         bert_params = json.loads(st.session_state.bm_params)
     except:
         raise ValueError("Problem in the json parameters")
     
     params = {"project_name":st.session_state.current_project}
+
+    # Specific or generic model
+    model_name = st.session_state.bm_train
+    if st.session_state.bm_train_hf:
+        model_name = st.session_state.bm_train_hf
+
     data = {
             "project_name":st.session_state.current_project,
             "scheme":st.session_state.current_scheme,
             "user":st.session_state.user,
             "name":f"_{st.session_state.user}", # générique
-            "base_model":st.session_state.bm_train,
+            "base_model":model_name,
             "params":bert_params,
             "test_size":0.2
             }
     
     r = _post("/models/bert/train", 
                     params = params, 
                     json_data = data)
```

### Comparing `activetigger-0.1.2/activetigger/functions.py` & `activetigger-0.1.3/activetigger/functions.py`

 * *Files identical despite different names*

### Comparing `activetigger-0.1.2/activetigger/img/active_tigger.png` & `activetigger-0.1.3/activetigger/img/active_tigger.png`

 * *Files identical despite different names*

### Comparing `activetigger-0.1.2/activetigger/models.py` & `activetigger-0.1.3/activetigger/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,17 @@
         name (str): name of the model
         df (DataFrame): labelled data
         col_text (str): text column
         col_label (str): label column
         model (str): model to use
         params (dict) : training parameters
         test_size (dict): train/test distribution
+
+        TODO : add possibility to check models from HF
+
         """
 
         # pour le moment fichier status.log existe tant que l'entrainement est en cours
 
         #  create repertory for the specific model
         current_path = path / name
         if not current_path.exists():
```

### Comparing `activetigger-0.1.2/activetigger/server.py` & `activetigger-0.1.3/activetigger/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,24 +138,37 @@
         if not self.db.exists():
             self.create_db()
 
         # activity of the server
         self.projects: dict = {}
         self.queue = Queue(self.n_workers, self.path)
 
-        # update users from YAML config file
-        existing = self.existing_users()
-        current = config["users"]
-        if current is not None:
-            for u in current:
-                if not u in existing:
-                    self.add_user(u, current[u])
-            for u in existing:
-                if (not u in current) and u != self.default_user:
-                    self.delete_user(u)
+        # add users if add_users.yaml exists
+        if Path("add_users.yaml").exists():
+            existing = self.existing_users()
+            with open('add_users.yaml') as f:
+                add_users = yaml.safe_load(f)
+            for user,password in add_users.items():
+                if not user in existing:
+                    self.add_user(user, password)
+                else:
+                    print(f"Not possible to add {user}, already exists")
+            # rename the file
+            os.rename('add_users.yaml', 'add_users_processed.yaml')
+
+        #existing = self.existing_users()
+        #current = config["users"]
+        # only creating users in the config file
+        #if current is not None:
+        #    for u in current:
+        #        if not u in existing:
+        #            self.add_user(u, current[u])
+            #for u in existing:
+            #    if (not u in current) and u != self.default_user:
+            #        self.delete_user(u)
 
         # starting time
         self.starting_time = time.time()
                 
     def __del__(self): 
         """
         Close the server
@@ -348,14 +361,15 @@
         """
         if not name in self.existing_users():
             return {"error":"Username does not exist"}
         conn = sqlite3.connect(self.db)
         cursor = conn.cursor()
         query = "DELETE FROM users WHERE user = ?"
         cursor.execute(query, (name,))
+        conn.commit()
         conn.close()
         return {"success":"User deleted"}    
     
     def get_user(self, name) -> UserInDB|dict:
         """
         Get user from database
         """
@@ -453,34 +467,77 @@
         # copy total dataset
         with open(params.dir / "data_raw.csv","wb") as f:
             f.write(file.file.read())
 
         # TODO : maximise the aleardy tagged in the annotate dataset, and None in the test
         # if possible, annotated data in the annotation dataset
         # if possible, test data without annotation
+        # if n_test = 0, no test set
+        # stratified if possible by cols_test
 
-        # random sample of the needed data
-        n_rows = params.n_train + params.n_test
+        # Step 1 : load all data and index to str
         content = pd.read_csv(params.dir / "data_raw.csv")
-        content = content.sample(n_rows)
         content = content.set_index(params.col_id)
         content.index = [str(i) for i in list(content.index)] #type: ignore
+        if len(content) < params.n_test + params.n_train:
+            return {"error":f"Not enought data for creating the train/test dataset. Current : {len(content)} ; Selected : {params.n_test + params.n_train}"}
+        # TODO : drop duplicates ?
+
+        # Step 2 : test dataset, no already labelled data, random + stratification
+        rows_test = []
+        params.test = False
+        if params.n_test != 0:
+            # only on non labelled data
+            f = content[params.col_label].isna()
+            if (f.sum()) < params.n_test:
+                return {"error":"Not enought data for creating the test dataset"}
+            if len(params.cols_test) == 0: # if no stratification
+                testset = content[f].sample(params.n_test)
+            else: #if stratification, total cat, number of element per cat, sample with a lim
+                df_grouped = content[f].groupby(params.col_label, group_keys=False)
+                nb_cat = len(df_grouped)
+                nb_elements_cat = round(params.n_test/nb_cat)
+                testset = df_grouped.apply(lambda x: x.sample(min(len(x), nb_elements_cat)))
+            testset.to_parquet(params.dir / self.test_file, index=True)
+            params.test = True
+            rows_test = list(testset.index)
+        
+        # Step 3 : train dataset, remove test rows, prioritize labelled data
+        content = content.drop(rows_test)
+        f_notna = content[params.col_label].notna()
+        f_na = content[params.col_label].isna()
+        if f_notna.sum()>params.n_train: # case where there is more labelled data than needed
+            trainset = content[f_notna].sample(params.n_train)
+        else:
+            n_train_random = params.n_train - f_notna.sum() # number of element to pick
+            trainset = pd.concat([content[f_notna], content[f_na].sample(n_train_random)])
+
+        trainset.to_parquet(params.dir / self.data_file, index=True)
+        trainset[[params.col_text]+params.cols_context].to_parquet(params.dir / self.labels_file, index=True)
+        trainset[[]].to_parquet(params.dir / self.features_file, index=True)
+
+        # random sample of the needed data
+        # n_rows = params.n_train + params.n_test
+        # content = pd.read_csv(params.dir / "data_raw.csv")
+        # content = content.sample(n_rows)
+        # content = content.set_index(params.col_id)
+        # content.index = [str(i) for i in list(content.index)] #type: ignore
     
         # create the empty annotated file / features file
         # Put the id column as index for the rest of the treatment
-        content[0:params.n_train].to_parquet(params.dir / self.data_file, index=True)
-        content[params.n_train:].to_parquet(params.dir / self.test_file, index=True)
+        # content[0:params.n_train].to_parquet(params.dir / self.data_file, index=True)
+        # content[params.n_train:].to_parquet(params.dir / self.test_file, index=True)
         # only for the training set for the moment
         # keep the text and the context available
-        content[0:params.n_train][[params.col_text]+params.cols_context].to_parquet(params.dir / self.labels_file, index=True)
-        content[0:params.n_train][[]].to_parquet(params.dir / self.features_file, index=True)
+        # content[0:params.n_train][[params.col_text]+params.cols_context].to_parquet(params.dir / self.labels_file, index=True)
+        # content[0:params.n_train][[]].to_parquet(params.dir / self.features_file, index=True)
 
         # if the case, add labels in the database
-        if (not params.col_label is None) and (params.col_label in content.columns):
-            df = content[params.col_label].dropna()
+        if (not params.col_label is None) and (params.col_label in trainset.columns):
+            df = trainset[params.col_label].dropna()
             params.default_scheme = list(df.unique())
             # add the scheme in the database
             conn = sqlite3.connect(self.db)
             cursor = conn.cursor()
             query = '''
                     INSERT INTO schemes (project, name, params) 
                     VALUES (?, ?, ?)
@@ -635,24 +692,25 @@
 
     def get_next(self,
                  scheme:str,
                  selection:str = "deterministic",
                  sample:str = "untagged",
                  user:str = "user",
                  tag:None|str = None,
+                 history:list = [],
                  frame:None|list = None) -> dict:
         """
         Get next item for a specific scheme with a specific method
         - deterministic
         - random
         - active
         - maxprob
         - test
         """
-
+        print("history",history)
         # specific case of test, random element
         if selection == "test": 
             df = self.schemes.get_scheme_data(scheme, complete=True, kind="test")
             f = df["labels"].isnull()
             element_id = df[f].sample(random_state=42).index[0]
             element =  {
             "element_id":element_id,
@@ -690,34 +748,36 @@
 
         # test if there is at least one element available
         if sum(f) == 0:
             return {"error":"No element available"}
 
         # select type of selection
         if selection == "deterministic": # next row
-            element_id = df[f].index[0]
+            element_id = df[f].drop(history, errors="ignore").index[0]
             indicator = None
         if selection == "random": # random row
-            element_id = df[f].sample(random_state=42).index[0]
+            element_id = df[f].drop(history, errors="ignore").sample(random_state=42).index[0]
             indicator = None
         if selection == "maxprob": # higher prob, only possible if the model has been trained
             if not self.simplemodels.exists(user,scheme):
                 return {"error":"Simplemodel doesn't exist"}
             if tag is None: # default label to first
                 return {"error":"Select a tag"}
             sm = self.simplemodels.get_model(user, scheme) # get model
             proba = sm.proba.reindex(f.index)
-            element_id = proba[f][tag].sort_values(ascending=False).index[0] # get max proba id
+            # use the history to not send already tagged data
+            element_id = proba[f][tag].drop(history, errors="ignore").sort_values(ascending=False).index[0] # get max proba id
             indicator = f"probability: {round(proba.loc[element_id,tag],2)}"
         if selection == "active": #higher entropy, only possible if the model has been trained
             if not self.simplemodels.exists(user,scheme):
                 return  {"error":"Simplemodel doesn't exist"}
             sm = self.simplemodels.get_model(user, scheme) # get model
             proba = sm.proba.reindex(f.index)
-            element_id = proba[f]["entropy"].sort_values(ascending=False).index[0] # get max entropy id
+            # use the history to not send already tagged data
+            element_id = proba[f]["entropy"].drop(history, errors="ignore").sort_values(ascending=False).index[0] # get max entropy id
             indicator = round(proba.loc[element_id,'entropy'],2)
             indicator = f"entropy: {indicator}"
         
         # get prediction of the id if it exists
         predict = {"label":None,
                    "proba":None}
 
@@ -759,16 +819,20 @@
                 predict = {"label":predicted_label, 
                         "proba":predicted_proba}
         r = { 
             "element_id":element_id,
             "text":self.content.loc[element_id,self.params.col_text],
             "context":dict(self.content.fillna("NA").loc[element_id, self.params.cols_context]),
             "selection":"request",
-            "predict":predict
+            "predict":predict,
+            "info":"get specific",
+            "frame":None
             }
+        
+
         return r
 
     def get_params(self) -> ProjectModel:
         """
         Send parameters
         """
         return self.params
@@ -805,16 +869,16 @@
     def get_state(self):
         """
         Send state of the project
         """
         r = {
             "params":self.params,
             "next":{
-                    "methods_min":["deterministic","random","test"],
-                    "methods":["deterministic","random","maxprob","active","test"],
+                    "methods_min":["deterministic","random"],
+                    "methods":["deterministic","random","maxprob","active"],
                     "sample":["untagged","all","tagged"],
                     },
             "schemes":{
                     "available":self.schemes.available()
                     },
             "features":{
                     "options":self.features.options,
```

### Comparing `activetigger-0.1.2/activetigger/widget.py` & `activetigger-0.1.3/activetigger/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.global_output = widgets.VBox([],layout=Layout(width='100%'))
         self.start()
 
     def __del__(self): 
         Widget.async_update = False
         print("Widget closed")
 
+
     def _post(self,
              route:str, 
              params:dict|None = None, 
              files:str|None = None,
              json_data:dict|None = None,
              data:dict|None = None) -> dict:
         """
@@ -683,14 +684,31 @@
                 }
         r = self._post("/schemes/add", 
                        params = params, 
                        json_data = data)
         self.update_tab_schemes()
         return r
     
+    def create_label(self, text_field):
+        """
+        Create label in a scheme
+        """
+        label = text_field.value
+        if label == "":
+            return "Empty"
+        params = {"project_name":self.project_name,
+                  "scheme":self.select_scheme.value,
+                  "label":label,
+                  "user":self.user}
+        r = self._post("/schemes/label/add", 
+                       params = params)
+        self.update_tab_schemes()
+        text_field.value = ""
+        return r
+    
     def delete_scheme(self, s):
         """
         Delete scheme
         """
         if s == "":
             return "Empty"
         params = {"project_name":self.project_name}
@@ -730,30 +748,15 @@
                   "user":self.user
                 }
         r = self._post("/models/bert/delete", 
                        params = params)
         self.update_tab_bertmodels()
         return r
 
-    def create_label(self, text_field):
-        """
-        Create label in a scheme
-        """
-        label = text_field.value
-        if label == "":
-            return "Empty"
-        params = {"project_name":self.project_name,
-                  "scheme":self.select_scheme.value,
-                  "label":label,
-                  "user":self.user}
-        r = self._post("/schemes/label/add", 
-                       params = params)
-        self.update_tab_schemes()
-        text_field.value = ""
-        return r
+
     
     def create_simplemodel(self, 
                            scheme:str, 
                            model:str, 
                            parameters:str, 
                            features:list):
         """
```

### Comparing `activetigger-0.1.2/pyproject.toml` & `activetigger-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `activetigger-0.1.2/requirements.txt` & `activetigger-0.1.3/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 argparse
 datasets
 sentence-transformers
 sentencepiece
 umap-learn
 sacremoses
 streamlit_autorefresh
+streamlit_option_menu
 fasttext @ git+https://github.com/facebookresearch/fastText.git@main
 https://github.com/explosion/spacy-models/releases/download/fr_core_news_sm-3.7.0/fr_core_news_sm-3.7.0.tar.gz#egg=fr_core_news_sm
 https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.7.1/en_core_web_sm-3.7.1.tar.gz#egg=en_core_web_sm
```

### Comparing `activetigger-0.1.2/tests/test_project.py` & `activetigger-0.1.3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `activetigger-0.1.2/PKG-INFO` & `activetigger-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activetigger
-Version: 0.1.2
+Version: 0.1.3
 Summary: ActiveTigger in Python
 Author-email: Émilien Schultz - Julien Boelaert - Étienne Ollion <emilien.schultz@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi[all]
 Requires-Dist: sentencepiece
 Requires-Dist: requests
```

