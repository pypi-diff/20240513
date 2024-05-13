# Comparing `tmp/r3xa-2024.5.dev1.tar.gz` & `tmp/r3xa-2024.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3xa-2024.5.dev1.tar", max compression
+gzip compressed data, was "r3xa-2024.5.dev2.tar", max compression
```

## Comparing `r3xa-2024.5.dev1.tar` & `r3xa-2024.5.dev2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      778 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/README.md
--rw-r--r--   0        0        0     1758 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 14:46:43.547690 r3xa-2024.5.dev1/r3xa/__init__.py
--rw-r--r--   0        0        0    37619 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/r3xa/gui.py
--rw-r--r--   0        0        0    11708 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/r3xa/metadata.py
--rw-r--r--   0        0        0     2644 2024-05-06 14:46:43.521691 r3xa-2024.5.dev1/r3xa/scripts.py
--rw-r--r--   0        0        0     3701 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/r3xa/utils.py
--rw-r--r--   0        0        0     1183 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/r3xa/validation.py
--rw-r--r--   0        0        0     3468 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/r3xa/visualisation.py
--rw-r--r--   0        0        0    29007 2024-05-06 14:46:43.522691 r3xa-2024.5.dev1/resources/schema.json
--rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 r3xa-2024.5.dev1/PKG-INFO
+-rw-r--r--   0        0        0      778 2024-05-13 07:47:42.663335 r3xa-2024.5.dev2/README.md
+-rw-r--r--   0        0        0     1758 2024-05-13 07:47:42.664335 r3xa-2024.5.dev2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 07:47:42.699335 r3xa-2024.5.dev2/r3xa/__init__.py
+-rw-r--r--   0        0        0    38379 2024-05-13 07:47:42.664335 r3xa-2024.5.dev2/r3xa/gui.py
+-rw-r--r--   0        0        0    11672 2024-05-13 07:47:42.664335 r3xa-2024.5.dev2/r3xa/metadata.py
+-rw-r--r--   0        0        0     2644 2024-05-13 07:47:42.665335 r3xa-2024.5.dev2/r3xa/scripts.py
+-rw-r--r--   0        0        0     3701 2024-05-13 07:47:42.665335 r3xa-2024.5.dev2/r3xa/utils.py
+-rw-r--r--   0        0        0     1185 2024-05-13 07:47:42.665335 r3xa-2024.5.dev2/r3xa/validation.py
+-rw-r--r--   0        0        0     3468 2024-05-13 07:47:42.665335 r3xa-2024.5.dev2/r3xa/visualisation.py
+-rw-r--r--   0        0        0    32842 2024-05-13 07:47:42.665335 r3xa-2024.5.dev2/resources/schema.json
+-rw-r--r--   0        0        0     1749 1970-01-01 00:00:00.000000 r3xa-2024.5.dev2/PKG-INFO
```

### Comparing `r3xa-2024.5.dev1/README.md` & `r3xa-2024.5.dev2/README.md`

 * *Files identical despite different names*

### Comparing `r3xa-2024.5.dev1/pyproject.toml` & `r3xa-2024.5.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "r3xa"
-version = "2024.5.dev1"
+version = "2024.5.dev2"
 description = "Remember, Reuse and Replicate eXperiments and Analyses"
 authors = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 maintainers = ["Emmanuel Roubin <emmanuel.roubin@univ-grenoble-alpes.fr>"]
 homepage = "https://photomecanics.gitlab.io/r3xa/doc"
 repository = "https://gitlab.com/photomecanics/r3xa"
 keywords = []
 readme = "README.md"
```

### Comparing `r3xa-2024.5.dev1/r3xa/gui.py` & `r3xa-2024.5.dev2/r3xa/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,20 +164,19 @@
             self.tab_widget.widget(i).setSizePolicy(policy)
 
         policy.setVerticalPolicy(QSizePolicy.Minimum)
         current = self.tab_widget.currentWidget()
         current.setSizePolicy(policy)
 
     def headerWidget(self):
-        header = f"""<h3>{self.schema["title"]}</h3>
-        <p>{self.schema["description"]}</p>
-        <p><i>Version {self.schema["properties"]["version"]["const"]}</i></p>
-        <p></p>
-        """
-        return QLabel(header)
+        header = QLabel(f'<h3>{self.schema["title"]}</h3><p align="justify">{self.schema["description"]}</p>')
+        # <p><i>Version {self.schema["properties"]["version"]["const"]}</i></p>
+        header.setWordWrap(True)
+        header.setStyleSheet("margin-bottom: 10px;")
+        return header
 
     def display_form_add_row(self, section_key, data_id):
         """adds a row for an array of items
         section_key: field:settings/specimen, field:data_source/specimen or field:data_set/generic
         data_id: the id slug of the data
         """
         p = self.parse_attribute(section_key)
@@ -232,18 +231,18 @@
 
         string_like = ["string", "number", "#/$defs/types/string", "#/$defs/types/uint"]
         # number_like = ["number", "#/$defs/types/uint"]
 
         if k in ["id"]:
             # handle special ID field
             pk = self.parse_attribute(section_key)
-            title = f'{pk["base"].title()} -> {" -> ".join(pk["keys"])}'
-            l1 = QLabel(f"<b>type [id]</b>")
-            l2 = QLabel(f"{title} [{payload.get(k)}]")
-            layout.addRow(l1, l2)
+            # title = f'{pk["base"].title()} -> {" -> ".join(pk["keys"])}'
+            # l1 = QLabel(f"<b>type [id]</b>")
+            # l2 = QLabel(f"{title} [{payload.get(k)}]")
+            # layout.addRow(l1, l2)
             setattr(self, attribute_key, QLabel(payload.get(k)))
 
         elif v.get("type") in string_like or v.get("$ref") in string_like:
             # handle field type and default value
             if k == "description":
                 input_field = CustomTextEdit()
                 input_field.setFixedHeight(150)
@@ -479,25 +478,29 @@
         section_key: something like field:settings/specimen used to setup the input attribute name
         payload: the current value of the meta data like {'title': "I'm setting 3", 'description': 'This is my second setting', ...}
         ignored: the fields from the schema we don't want to display
         layout: QFormLayout
         """
 
         #  the schema properties and required from the section_key
-        if section_key == "field:root":
+        p = self.parse_attribute(section_key)
+        if p["depth"] == 1:
             properties = {k: v for k, v in self.schema["properties"].items() if k not in ignored}
             required = self.schema["required"]
+        elif p["depth"] == 2:
+            properties = self.schema["$defs"][p["base"]][p["keys"][0]]["properties"]
+            required = self.schema["$defs"][p["base"]][p["keys"][0]]["required"]
+            title = self.schema["$defs"][p["base"]][p["keys"][0]]["title"]
+            description = self.schema["$defs"][p["base"]][p["keys"][0]]["description"]
+            l1 = QLabel(f'<p align="justify"><b>{title}:</b> <i>{description}</i></p>')
+            l1.setWordWrap(True)
+            l1.setStyleSheet("QLabel { margin-bottom: 10px; }")
+            layout.addRow(l1)
         else:
-            # print(section_key)
-            if len(section_key.split("/")) > 2:
-                print(f"WARNING: section key with two /: {section_key}")
-            a = section_key.split("/")[0].split(":")[1]
-            b = section_key.split("/")[1]
-            properties = self.schema["$defs"][a][b]["properties"]
-            required = self.schema["$defs"][a][b]["required"]
+            print(f"WARNING: section key with two /: {section_key} ({p})")
 
         # get required arguments for root parameters
         for k, v in properties.items():
             if v.get("type") in ["array"]:
                 # print(section_key, k, v)
                 v_array = v.copy()
                 if "type" in v["items"]:
@@ -625,14 +628,23 @@
         mainLayout = QVBoxLayout()
 
         #######
         # Combo box to select edit/create setting
         #######
 
         selectLayout = QFormLayout()
+
+        # set the generic text above the combo box
+        title = self.schema["properties"][data_type]["title"]
+        description = self.schema["properties"][data_type]["description"]
+        label = QLabel(f'<b>{title}</b><p align="justify">{description}</p>')
+        label.setWordWrap(True)
+        mainLayout.addWidget(label)
+
+        # set the combo box
         setattr(self, f"{data_type}_combo_box", QComboBox())
         combo_box = getattr(self, f"{data_type}_combo_box")
         self.set_data_combo_box(data_type)
 
         # setup layout
         selectLayout.addRow(combo_box)
         selectWidget = QWidget()
@@ -640,16 +652,14 @@
         mainLayout.addWidget(selectWidget)
 
         ######
         # Form to edit/create settings
         ######
         setattr(self, f"{data_type}_form_layout", QFormLayout())
 
-        print("data_type", data_type)
-
         layout = getattr(self, f"{data_type}_form_layout")
         formWidget = QWidget()
         formWidget.setLayout(layout)
         mainLayout.addWidget(formWidget)
         mainLayout.addStretch()
 
         tab = QWidget()
@@ -776,14 +786,16 @@
         # get root
         splt = k.split("/")
         parsed_key["key"] = k
         parsed_key["attribute"] = True
         parsed_key["depth"] = len(splt)
         parsed_key["base"] = splt[0]
         parsed_key["keys"] = [_.split("__")[0] for _ in splt[1:]]
+        if splt[0] == "root":
+            return parsed_key
 
         if len(splt) == 2:
             # WARNING this will break if root have lists which is not the case for now
             return parsed_key
 
         if "__" in splt[2]:
             # we have a list
```

### Comparing `r3xa-2024.5.dev1/r3xa/metadata.py` & `r3xa-2024.5.dev2/r3xa/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
 
             # case value is empty, delete if already set in the past
             if not obj_is_true(to_be_assigned):
                 if hasattr(self, k):
                     delattr(self, k)
                 continue
 
-            print(k, to_be_assigned)
             setattr(self, k, to_be_assigned)
 
     def guess_kind(self, data_type):
         # check for data_sets, data_sources and settings
         schema = get_schema()
 
         # get all attributes
@@ -180,15 +179,15 @@
             properties = set(v["properties"]) - {"id", "kind"}
             required = set(v["required"]) - {"id", "kind"}
 
             missing = len(properties - keys)
             missing_required = len(required - keys)
             extra = len(keys - properties)
 
-            # if more keys then propertiesor less than required then discard
+            # if more keys then properties or less than required then discard
             if extra or missing_required:
                 continue
 
             missing_keys[kind] = missing
 
         if not len(missing_keys):
             raise ValueError(f"No kind guessed from {data_type}")
```

### Comparing `r3xa-2024.5.dev1/r3xa/scripts.py` & `r3xa-2024.5.dev2/r3xa/scripts.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.5.dev1/r3xa/utils.py` & `r3xa-2024.5.dev2/r3xa/utils.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.5.dev1/r3xa/validation.py` & `r3xa-2024.5.dev2/r3xa/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def validate(instance):
     schema = get_schema()
 
     validator = jsonschema.validators.Draft202012Validator(schema)
     errors = sorted(validator.iter_errors(instance), key=jsonschema.exceptions.relevance)
 
     if not len(errors):
-        print("Valid json file")
+        # print("Valid json file")
         return
 
     error_messages = []
 
     for error in errors:
         p = f"{list(error.path)[0]} validation error" if error.path.count(0) else "root validation error"
         error_message = [f"{p}: {error.message}"] + [make_context_message(error, e) for e in error.context]
```

### Comparing `r3xa-2024.5.dev1/r3xa/visualisation.py` & `r3xa-2024.5.dev2/r3xa/visualisation.py`

 * *Files identical despite different names*

### Comparing `r3xa-2024.5.dev1/resources/schema.json` & `r3xa-2024.5.dev2/resources/schema.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9190807339645927%*

 * *Differences: {"'$defs'": "{'settings': {'generic': {'title': 'Setting (generic)', 'description': 'Generic "*

 * *            "setting with the minimal number of fields.', 'properties': {'id': {'description': 'ID "*

 * *            "of the setting.'}, 'kind': {'description': 'Only required for specs implementation "*

 * *            "purposes.'}, 'title': {'description': 'Title of setting.'}, 'description': "*

 * *            "{'description': 'Description of the setting.'}}}, 'specimen': {'description': "*

 * *            "'Specimen.', 'properti […]*

```diff
@@ -1,311 +1,378 @@
 {
     "$defs": {
         "data_sets": {
             "file": {
                 "additionalProperties": false,
-                "description": "When all the data is stored in a single table like file (csv, txt)",
+                "description": "When all the timestamps and data is stored in a single tablular like file (like csv or txt). If the timesamps and data are in two separate files they should be in the same folder.",
                 "properties": {
                     "data": {
                         "$ref": "#/$defs/types/data_set_file",
                         "description": "Path and range to the data file",
                         "title": "Data"
                     },
                     "data_sources": {
-                        "description": "List if IDs of the data sources",
+                        "description": "List of IDs of the data sources.",
                         "items": {
                             "$ref": "#/$defs/types/data_source_id"
                         },
                         "title": "Data sources",
                         "type": "array"
                     },
                     "description": {
-                        "description": "The description of the data set",
+                        "description": "Description of the data set.",
                         "title": "Description",
                         "type": "string"
                     },
-                    "file_type": {
-                        "description": "MIME of the file",
+                    "folder": {
+                        "description": "Relative path to the folder containing the timestamps and data file(s).",
                         "examples": [
-                            "text/csv"
+                            "..",
+                            ".",
+                            "my_folder/my_tabular.txt"
                         ],
-                        "title": "Fiel type",
+                        "title": "Folder",
                         "type": "string"
                     },
                     "id": {
-                        "description": "ID of the data set",
+                        "description": "ID of the data set.",
                         "title": "ID",
                         "type": "string"
                     },
                     "keywords": {
-                        "description": "A list of keywords",
+                        "description": "List of keywords.",
                         "items": {
                             "type": "string"
                         },
                         "title": "Keywords",
                         "type": "array"
                     },
                     "kind": {
                         "const": "data_sets/file",
-                        "description": "Only required for specs implementation purposes",
+                        "description": "Only required for specs implementation purposes.",
                         "title": "Kind of data source",
                         "type": "string"
                     },
-                    "path": {
-                        "description": "relative path to the data folder",
-                        "examples": [
-                            "..",
-                            "my_folder"
-                        ],
-                        "title": "Path",
-                        "type": "string"
-                    },
                     "time_reference": {
-                        "description": "The reference time",
+                        "description": "Time serving as a reference to the whole data set.",
                         "title": "Time reference",
                         "type": "number"
                     },
                     "timestamps": {
                         "$ref": "#/$defs/types/data_set_file",
                         "description": "Path and range to the timestamps file",
                         "title": "Timesamps"
                     },
                     "title": {
-                        "description": "The title of the data set",
+                        "description": "Title of the data set.",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
                     "data_sources",
-                    "file_type",
                     "time_reference",
                     "timestamps",
                     "data"
                 ],
-                "title": "Data set (file)",
+                "title": "Data set (single file)",
+                "type": "object"
+            },
+            "generic": {
+                "additionalProperties": false,
+                "description": "Description of the data set.",
+                "properties": {
+                    "data_sources": {
+                        "description": "List of IDs of the data sources.",
+                        "items": {
+                            "$ref": "#/$defs/types/data_source_id"
+                        },
+                        "title": "Data sources",
+                        "type": "array"
+                    },
+                    "description": {
+                        "description": "Description of the data set.",
+                        "title": "Description",
+                        "type": "string"
+                    },
+                    "file_type": {
+                        "description": "MIME type of the file.",
+                        "examples": [
+                            "text/csv"
+                        ],
+                        "title": "MIME",
+                        "type": "string"
+                    },
+                    "id": {
+                        "description": "ID of the data set.",
+                        "title": "ID",
+                        "type": "string"
+                    },
+                    "kind": {
+                        "const": "data_sets/generic",
+                        "description": "Only required for specs implementation purposes.",
+                        "title": "Kind of data source",
+                        "type": "string"
+                    },
+                    "path": {
+                        "description": "Relative path to the data file.",
+                        "examples": [
+                            "../my_values.csv",
+                            "my_folder/my_image.tif"
+                        ],
+                        "title": "Path",
+                        "type": "string"
+                    },
+                    "title": {
+                        "description": "Title of the data set.",
+                        "title": "Title",
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "id",
+                    "kind",
+                    "title",
+                    "description",
+                    "data_sources",
+                    "file_type",
+                    "path"
+                ],
+                "title": "Data set (generic)",
                 "type": "object"
             },
             "list": {
                 "additionalProperties": false,
-                "description": "When all the data is stored in separated files (like a list of images)",
+                "description": "When all the data is stored in separated files (like a list of images). They should all be in the same folder.",
                 "properties": {
                     "data": {
-                        "description": "List of the data files",
+                        "description": "List of the data files.",
                         "items": {
                             "type": "string"
                         },
                         "title": "Data",
                         "type": "array"
                     },
                     "data_sources": {
-                        "description": "List if IDs of the data sources",
+                        "description": "List if IDs of the data sources.",
                         "items": {
                             "$ref": "#/$defs/types/data_source_id"
                         },
                         "title": "Data sources",
                         "type": "array"
                     },
                     "description": {
-                        "description": "The description of the data set",
+                        "description": "Description of the data set.",
                         "title": "Description",
                         "type": "string"
                     },
+                    "file_type": {
+                        "description": "MIME type of the data files.",
+                        "examples": [
+                            "text/csv"
+                        ],
+                        "title": "MIME",
+                        "type": "string"
+                    },
                     "id": {
-                        "description": "ID of the data set",
+                        "description": "ID of the data set.",
                         "title": "ID",
                         "type": "string"
                     },
                     "keywords": {
-                        "description": "A list of keywords",
+                        "description": "List of keywords.",
                         "items": {
                             "type": "string"
                         },
                         "title": "Keywords",
                         "type": "array"
                     },
                     "kind": {
                         "const": "data_sets/list",
-                        "description": "Only required for specs implementation purposes",
+                        "description": "Only required for specs implementation purposes.",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "path": {
-                        "description": "relative path to the data folder",
+                        "description": "Relative path to the data folder.",
                         "examples": [
                             "..",
                             "my_folder"
                         ],
                         "title": "Path",
                         "type": "string"
                     },
                     "time_reference": {
-                        "description": "The reference time",
+                        "description": "Time serving as a reference to the whole data set.",
                         "title": "Time reference",
                         "type": "number"
                     },
                     "timestamps": {
-                        "description": "List of the timestamps",
+                        "description": "List of the timestamps.",
                         "items": {
                             "type": "number"
                         },
                         "title": "Timesamps",
                         "type": "array"
                     },
                     "title": {
-                        "description": "The title of the data set",
+                        "description": "Title of the data set.",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description",
+                    "file_type",
                     "data_sources",
                     "time_reference",
                     "timestamps",
                     "data"
                 ],
-                "title": "Data set (list)",
+                "title": "Data set (list of files)",
                 "type": "object"
             }
         },
         "data_sources": {
             "camera": {
                 "additionalProperties": false,
-                "description": "A generic camera (visible).",
+                "description": "Generic camera in visible range.",
                 "properties": {
                     "aperture": {
-                        "description": "Aperture value",
+                        "description": "Aperture of the lens.",
                         "examples": "f/8",
-                        "title": "Aperture of the lens",
+                        "title": "Aperture",
                         "type": "string"
                     },
                     "description": {
-                        "description": "The description of your data source",
+                        "description": "Description of the camera.",
                         "title": "Description",
                         "type": "string"
                     },
                     "documentation": {
-                        "description": "Name, path or ULR of the documentation (no spaces, no accents)",
+                        "description": "Name, path or ULR of the documentation.",
                         "title": "Documentation",
                         "type": "string"
                     },
                     "exposure": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "Exposure time in ms",
-                        "title": "Exposure time"
+                        "description": "Exposure time (milliseconds).",
+                        "title": "Exposure"
                     },
                     "field_of_view": {
-                        "description": "Size of the field of view in m times m",
+                        "description": "Size of the field of view in (meters x meters).",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
                         "title": "Field of view",
                         "type": "array"
                     },
                     "filter": {
-                        "description": "Filter type, manufacturer and model",
+                        "description": "Filter type, manufacturer and model.",
                         "title": "Camera or lens filter",
                         "type": "string"
                     },
                     "focal_length": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "Focal length of the lens in mm",
+                        "description": "Focal length of the lens (millimetres).",
                         "title": "Focal length"
                     },
                     "id": {
-                        "description": "ID of the data source",
+                        "description": "ID of the data source.",
                         "title": "ID",
                         "type": "string"
                     },
                     "image_scale": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "Scale of the image in pix / m",
+                        "description": "Scale of the image (pixels per meter).",
                         "title": "Image scale"
                     },
                     "image_size": {
-                        "description": "Size of the image in pix times pix",
+                        "description": "Size of the image (pixels x pixels).",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
                         "title": "Image size",
                         "type": "array"
                     },
                     "input_data_sets": {
-                        "description": "The data sets IDs serving as an input to the source",
+                        "description": "Data sets IDs serving as an input to the source.",
                         "items": {
                             "$ref": "#/$defs/types/data_set_id"
                         },
                         "title": "List of the data sets",
                         "type": "array"
                     },
                     "kind": {
                         "const": "data_sources/generic",
-                        "description": "Only required for specs implementation purposes",
+                        "description": "Only required for specs implementation purposes.",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "lens": {
-                        "description": "Camera lens manufacturer and model",
+                        "description": "Camera lens manufacturer and model.",
                         "title": "Camera lens",
                         "type": "string"
                     },
                     "manufacturer": {
-                        "description": "Manufacturer / vendor / software editor",
+                        "description": "Manufacturer, vendor or software editor.",
                         "title": "Manufacturer",
                         "type": "string"
                     },
                     "model": {
-                        "description": "model or software version",
+                        "description": "Model or software version.",
                         "title": "Model",
                         "type": "string"
                     },
                     "noise": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "Quantity of noise of the camera",
+                        "description": "Quantity of noise of the camera.",
+                        "examples": [
+                            "???"
+                        ],
                         "title": "Noise level"
                     },
                     "output_components": {
                         "$ref": "#/$defs/types/uint",
-                        "description": "Number of componants / channels of the ouput data",
+                        "description": "Number of componants or channels of the ouput data.",
                         "title": "Output components"
                     },
                     "output_dimension": {
-                        "description": "Dimension of the output data",
+                        "description": "Dimension of the output data.",
                         "enum": [
                             "point",
                             "curve",
                             "surface",
                             "volume"
                         ],
                         "title": "Output dimension",
                         "type": "string"
                     },
                     "output_units": {
-                        "description": "Unit of the output data",
+                        "description": "Unit of the output data.",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
                         "title": "Output units",
                         "type": "array"
                     },
                     "standoff_distance": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "Standoff distance between the camera and the sample, in m",
+                        "description": "Standoff distance between the camera and the sample (in meters).",
                         "title": "Standoff distance"
                     },
                     "title": {
-                        "description": "The title of your data source",
+                        "description": "Title of the camera.",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
@@ -314,86 +381,86 @@
                     "output_components",
                     "output_dimension",
                     "output_units",
                     "manufacturer",
                     "model",
                     "image_size"
                 ],
-                "title": "Camera",
+                "title": "Camera (visible)",
                 "type": "object"
             },
             "generic": {
                 "additionalProperties": false,
                 "description": "A data source is a procedure or a system that generates a data set. If it is a sensor then his parameters must be specified. If it is an analysis specifies his parameters are specified along with the input parameters. It also indicates the dimension, the number of components and the unit of the output data.",
                 "properties": {
                     "description": {
-                        "description": "The description of your data source",
+                        "description": "Description of the data source.",
                         "title": "Description",
                         "type": "string"
                     },
                     "documentation": {
-                        "description": "Name, path or ULR of the documentation (no spaces, no accents)",
+                        "description": "Name, path or ULR of the documentation.",
                         "title": "Documentation",
                         "type": "string"
                     },
                     "id": {
                         "description": "ID of the data source",
                         "title": "ID",
                         "type": "string"
                     },
                     "input_data_sets": {
-                        "description": "The data sets IDs serving as an input to the source",
+                        "description": "Data sets IDs serving as inputs of the source.",
                         "items": {
                             "$ref": "#/$defs/types/data_set_id"
                         },
                         "title": "List of the data sets",
                         "type": "array"
                     },
                     "kind": {
                         "const": "data_sources/generic",
-                        "description": "Only required for specs implementation purposes",
+                        "description": "Only required for specs implementation purposes.",
                         "title": "Kind of data source",
                         "type": "string"
                     },
                     "manufacturer": {
-                        "description": "Manufacturer / vendor / software editor",
+                        "description": "Manufacturer, vendor or software editor.",
                         "title": "Manufacturer",
                         "type": "string"
                     },
                     "model": {
-                        "description": "model or software version",
+                        "description": "Model of the source or software version.",
                         "title": "Model",
                         "type": "string"
                     },
                     "output_components": {
                         "$ref": "#/$defs/types/uint",
-                        "description": "Number of componants / channels of the ouput data",
+                        "description": "Number of componants or channels of the ouput data.",
                         "title": "Output components"
                     },
                     "output_dimension": {
-                        "description": "Dimension of the output data",
+                        "description": "Dimension of the output data.",
                         "enum": [
                             "point",
                             "curve",
                             "surface",
                             "volume"
                         ],
                         "title": "Output dimension",
                         "type": "string"
                     },
                     "output_units": {
-                        "description": "Unit of the output data",
+                        "description": "Unit of the output data.",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
                         "title": "Output units",
                         "type": "array"
                     },
                     "title": {
-                        "description": "The title of your data source",
+                        "description": "Title of the data source.",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
@@ -401,105 +468,105 @@
                     "description",
                     "output_components",
                     "output_dimension",
                     "output_units",
                     "manufacturer",
                     "model"
                 ],
-                "title": "Generic data source",
+                "title": "Data source (generic)",
                 "type": "object"
             }
         },
         "settings": {
             "generic": {
                 "additionalProperties": false,
-                "description": "Experimental parameters should be the specimen, patterning technique and machines used (light, testing rig, environmental chamber...). Describe the experimental techniques/apparatus and devices used / light / environment chamber ...",
+                "description": "Generic setting with the minimal number of fields.",
                 "properties": {
                     "description": {
-                        "description": "The description of your setting",
+                        "description": "Description of the setting.",
                         "title": "Description",
                         "type": "string"
                     },
                     "id": {
-                        "description": "ID of the setting",
+                        "description": "ID of the setting.",
                         "title": "ID",
                         "type": "string"
                     },
                     "kind": {
                         "const": "settings/generic",
-                        "description": "Only required for specs implementation purposes",
+                        "description": "Only required for specs implementation purposes.",
                         "title": "Kind of object",
                         "type": "string"
                     },
                     "title": {
-                        "description": "The title of setting",
+                        "description": "Title of setting.",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
                     "title",
                     "description"
                 ],
-                "title": "Generic setting",
+                "title": "Setting (generic)",
                 "type": "object"
             },
             "specimen": {
                 "additionalProperties": false,
-                "description": "A specimen.",
+                "description": "Specimen.",
                 "properties": {
                     "cad": {
-                        "description": "Path to the design of the specimen",
+                        "description": "Path to the design of the specimen.",
                         "examples": [
                             "my-specimen.vtk"
                         ],
                         "title": "CAD",
                         "type": "string"
                     },
                     "description": {
-                        "description": "The description of your setting",
+                        "description": "Description of the specimen.",
                         "title": "Description",
                         "type": "string"
                     },
                     "id": {
-                        "description": "ID of the setting",
+                        "description": "ID of the setting.",
                         "title": "ID",
                         "type": "string"
                     },
                     "kind": {
                         "const": "settings/specimen",
-                        "description": "Only required for specs implementation purposes",
+                        "description": "Only required for specs implementation purposes.",
                         "title": "Kind of object",
                         "type": "string"
                     },
                     "patterning_feature_size": {
                         "$ref": "#/$defs/types/unit",
-                        "description": "The characteristic size of the pattern",
+                        "description": "Characteristic size of the pattern.",
                         "title": "Patterning feature size"
                     },
                     "patterning_technique": {
-                        "description": "The patterning technique used on the specimen",
+                        "description": "Patterning technique used on the specimen.",
                         "examples": [
                             "Base coat of white spray paint with ink stamped speckles"
                         ],
                         "title": "Patterning technique",
                         "type": "string"
                     },
                     "sizes": {
-                        "description": "The sizes of the specimen",
+                        "description": "Sizes of the specimen.",
                         "items": {
                             "$ref": "#/$defs/types/unit"
                         },
                         "title": "Sizes",
                         "type": "array"
                     },
                     "title": {
-                        "description": "The title of setting",
+                        "description": "Title of the setting.",
                         "title": "Title",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
                     "kind",
@@ -533,14 +600,23 @@
                             ";",
                             ",",
                             ":",
                             "\t"
                         ],
                         "type": "string"
                     },
+                    "file_type": {
+                        "description": "MIME type of the file.",
+                        "examples": [
+                            "text/csv",
+                            "text/txt"
+                        ],
+                        "title": "MIME",
+                        "type": "string"
+                    },
                     "filename": {
                         "type": "string"
                     },
                     "kind": {
                         "const": "data_set_file",
                         "description": "Only required for specs implementation purposes",
                         "title": "Kind of object",
@@ -550,23 +626,23 @@
                 "required": [
                     "filename",
                     "kind"
                 ],
                 "type": "object"
             },
             "data_set_id": {
-                "description": "The ID of a data set",
+                "description": "ID of a data set.",
                 "type": "string"
             },
             "data_source_id": {
-                "description": "The ID of a data source",
+                "description": "ID of a data source.",
                 "type": "string"
             },
             "setting_id": {
-                "description": "The ID of a setting",
+                "description": "ID of a setting.",
                 "type": "string"
             },
             "uint": {
                 "description": "Unsigned int",
                 "minimum": 0,
                 "title": "uint",
                 "type": "integer"
@@ -581,102 +657,105 @@
                     },
                     "scale": {
                         "description": "Factor with respect to the standard system",
                         "title": "Scale",
                         "type": "number"
                     },
                     "title": {
-                        "description": "The title of the unit",
+                        "description": "Title of the unit.",
                         "examples": [
                             "length",
                             "width",
                             "speed"
                         ],
                         "title": "Title",
                         "type": "string"
                     },
                     "unit": {
-                        "description": "The unit",
+                        "description": "Sign of the unit.",
                         "examples": [
                             "m",
                             "kN",
                             "kg",
                             "m/s"
                         ],
                         "title": "Unit",
                         "type": "string"
                     },
                     "value": {
-                        "description": "A numerical value",
+                        "description": "Numerical value.",
                         "title": "Value",
                         "type": "number"
                     }
                 },
                 "required": [
                     "kind",
                     "unit"
                 ],
                 "type": "object"
             }
         }
     },
     "additionalProperties": false,
-    "description": "This is the specs for the R3XA experiments and analysis meta data template.",
+    "description": "Yet another metadata file format whose goal is to provide a data representation scheme compatible with the variety of data types encountered in experimental and computational photomechanics, and to provide a convenient framework for software coupling and data fusion.",
     "properties": {
         "authors": {
-            "description": "Authors of the data sets",
+            "description": "Authors of the data sets.",
             "examples": [
                 "M. Palin, J. Cleese",
                 "ORCID",
                 "HAL-ID"
             ],
             "title": "Author",
             "type": "string"
         },
         "data_sets": {
-            "description": "The data sets :)",
+            "description": "A data set gives the organisation of the measured or generated data and time resolution.",
             "items": {
                 "anyOf": [
                     {
+                        "$ref": "#/$defs/data_sets/generic"
+                    },
+                    {
                         "$ref": "#/$defs/data_sets/file"
                     },
                     {
                         "$ref": "#/$defs/data_sets/list"
                     }
                 ]
             },
             "title": "Data sets",
             "type": "array"
         },
         "data_sources": {
-            "description": "The sources of the data (sensor or analysis)",
+            "description": "A data source is a procedure or a system that generates a data set. If it is a sensor then its parameters must be specified. If it is an analysis, its parameters are specified along with the input parameters. It also indicates the dimension, the number of components and the unit of the output data.",
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/data_sources/generic"
                     },
                     {
                         "$ref": "#/$defs/data_sources/camera"
                     }
                 ]
             },
             "title": "Data sources",
             "type": "array"
         },
         "date": {
-            "description": "Global date of the experiment (YYYY-MM-DD)",
+            "description": "Global date of the experiment (YYYY-MM-DD).",
             "examples": [
                 "2020-03-17"
             ],
             "pattern": "^[1-2]{1}[0-9]{3}-(0[1-9]|1[0-2])-(0[1-9]|[12][0-9]|3[01])$",
             "title": "Date",
             "type": "string"
         },
         "description": {
-            "description": "The description of the data sets",
+            "description": "Description of the data sets.",
             "title": "Description",
             "type": "string"
         },
         "documentation": {
             "description": "URI to the documentation (pdf)",
             "examples": [
                 "./doc/my_doc.pdf",
@@ -690,48 +769,48 @@
             "examples": [
                 "Creative common"
             ],
             "title": "License",
             "type": "string"
         },
         "repository": {
-            "description": "URL to the repository where the data sets are stored",
+            "description": "URL to the repository where the data sets are stored.",
             "examples": [
                 "https://zenodo.org/records/42"
             ],
             "title": "Repository",
             "type": "string"
         },
         "settings": {
-            "description": "List of parameters, devices or software that don't explicitly interact with the data sets",
+            "description": "Experimental parameters should be the specimen, patterning technique and machines used (light, testing rig, environmental chamber...). Describe the experimental techniques/apparatus and devices used / light / environment chamber...",
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/settings/generic"
                     },
                     {
                         "$ref": "#/$defs/settings/specimen"
                     }
                 ]
             },
             "title": "Settings",
             "type": "array"
         },
         "title": {
-            "description": "The title of the data sets",
+            "description": "Title of the data sets.",
             "example": [
                 "DICComposite2.0",
                 "My awesome data sets"
             ],
             "title": "Title",
             "type": "string"
         },
         "version": {
-            "const": "2024.5.dev1",
-            "description": "Version of the schema used",
+            "const": "2024.5.dev2",
+            "description": "Version of the schema used.",
             "title": "Version",
             "type": "string"
         }
     },
     "required": [
         "title",
         "description",
```

### Comparing `r3xa-2024.5.dev1/PKG-INFO` & `r3xa-2024.5.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3xa
-Version: 2024.5.dev1
+Version: 2024.5.dev2
 Summary: Remember, Reuse and Replicate eXperiments and Analyses
 Home-page: https://photomecanics.gitlab.io/r3xa/doc
 Author: Emmanuel Roubin
 Author-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Maintainer: Emmanuel Roubin
 Maintainer-email: emmanuel.roubin@univ-grenoble-alpes.fr
 Requires-Python: >=3.8.1,<4.0.0
```

