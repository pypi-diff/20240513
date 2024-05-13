# Comparing `tmp/linkmlformbuilder-0.1.9.tar.gz` & `tmp/linkmlformbuilder-1.0.0.tar.gz`

## Comparing `linkmlformbuilder-0.1.9.tar` & `linkmlformbuilder-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/__init__.py
--rw-r--r--   0        0        0   152766 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/bootstrap.css
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/constants.py
--rw-r--r--   0        0        0    11328 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/formbuilder.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/slot_code_generators.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/styles.css
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/utils.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/.gitignore
--rw-r--r--   0        0        0    35857 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/LICENSE
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/README.md
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 linkmlformbuilder-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/__init__.py
+-rw-r--r--   0        0        0   152766 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/bootstrap.css
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/constants.py
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/formbuilder.py
+-rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/slot_code_generators.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/styles.css
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/utils.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/.gitignore
+-rw-r--r--   0        0        0    35857 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/README.md
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 linkmlformbuilder-1.0.0/PKG-INFO
```

### Comparing `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/bootstrap.css` & `linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/bootstrap.css`

 * *Files identical despite different names*

### Comparing `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/constants.py` & `linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,35 +90,38 @@
         line-height: 1.5;
         color: #212529;
         text-align: center;
         white-space: nowrap;
         background-color: #f8f9fa;
         border: 1px solid #dee2e6;
         border-radius: 0.375rem;
-        width: 20%;
         float: left;
         min-height: 34px;
         white-space: pre-wrap;
     }
 
+    .width20 {
+        width: 20%
+    }
+
     .form-control {
         width: 80% !important;
         height: 100%;
     }
 
     .input-group {
         position: relative;
         display: flex;
         flex-wrap: wrap;
         align-items: stretch;
         width: 100%;
     }
 
     .hideField {
-        visibility: hidden;
+        display: none !important;
     }
 
     .form-check {
         width: fit-content;
         display: inline-block;
         margin-right: 5px;
     }
@@ -134,12 +137,39 @@
         float: left;
         width: calc(20% - 5px);
     }
 
     h2 {
         width: 100vw;
     }
+
+    .answer-options {
+        padding-left: 0.667px;
+    }
+
+    details {
+        border: 1px solid #dee2e6;
+        border-radius: 0.375rem;
+        padding: 0.5em 0.5em 0;
+        width: fit-content;
+        margin-bottom: 0.5rem;
+    }
+    
+    summary {
+        font-weight: bold;
+        margin: -0.5em -0.5em 0;
+        padding: 0.5em;
+    }
+    
+    details[open] {
+        padding: 0.5em;
+    }
+    
+    details[open] summary {
+        border-bottom: 1px solid #dee2e6;
+        margin-bottom: 0.5em;
+    }
 </style>
 <body>
 '''
 HTML_END = '''</body>
 </html>'''
```

### Comparing `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/formbuilder.py` & `linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/formbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import argparse
 import yaml
 from LinkMLFormbuilder import utils
+# import utils
 import os
 import pdfkit
 from LinkMLFormbuilder import slot_code_generators
+# import slot_code_generators
 from shutil import which
 import pkg_resources
 from LinkMLFormbuilder import constants
+# import constants
 import warnings
 
 def retrieveFileContent(yamlfile):
     try:
         stream = open(os.path.abspath(yamlfile), "r")
         return yaml.safe_load(stream)
     except yaml.YAMLError:
@@ -22,48 +25,53 @@
 
 def getSlotFormCode(slotCode, content, default_range, subclasses, level, key):
     if (slotCode is None): return ""
     # if (constants.NAME not in slotCode): raise TypeError("Missing field: name")
     desc = utils.extractDescription(slotCode)
     required = constants.REQUIRED if (constants.REQUIRED in slotCode and slotCode.get(constants.REQUIRED) == True) else ""
     propertyName = slotCode.get(constants.NAME)
+    if (propertyName == None): propertyName = key
     title = utils.extractSlotName(slotCode, key)
     
     if (constants.VALUES_FROM in slotCode or (constants.RANGE in slotCode and constants.ENUMS in content and slotCode.get(constants.RANGE) in content.get(constants.ENUMS))):
         return slot_code_generators.getEnumSlotCode(slotCode, content, desc, required, propertyName, title)
     elif (constants.ENUM_RANGE in slotCode): # inlined enum
         return slot_code_generators.getInlineEnumSlotCode(slotCode, desc, required, propertyName, title)
     elif (constants.RANGE in slotCode):
         if (slotCode.get(constants.RANGE) in content.get(constants.CLASSES)):
             return getClassFormCode(content.get(constants.CLASSES).get(slotCode.get(constants.RANGE)), content, default_range, subclasses, level + 1, key) # the range is a class itself and should be treated as such
         elif (slotCode.get(constants.RANGE) == "integer" or slotCode.get(constants.RANGE) == "float"):
             return slot_code_generators.getNumberSlotCode(slotCode, desc, required, propertyName, title)
         elif (slotCode.get(constants.RANGE) == "string"): #assume textarea
-            return slot_code_generators.getTextareaSlotCode(desc, required, propertyName, title, slotCode)
+            return slot_code_generators.getTextareaSlotCode(desc, required, propertyName, title, slotCode, html_only)
         elif (slotCode.get(constants.RANGE) == "boolean"):
             return slot_code_generators.getBooleanSlotCode(desc, required, propertyName, title)
         else: # this is a basic pdf, so datetime should not be a datetime field, but a textfield
             return slot_code_generators.getStringSlotCode(desc, required, propertyName, title, slotCode)
     else: # rely on default range
         if (default_range is not None):
             if (default_range == "integer" or default_range == "float"):
                 return slot_code_generators.getNumberSlotCode(slotCode, desc, required, propertyName, title)
             elif (default_range == "string"): #assume textarea
-                return slot_code_generators.getTextareaSlotCode(desc, required, propertyName, title, slotCode)
+                return slot_code_generators.getTextareaSlotCode(desc, required, propertyName, title, slotCode, html_only)
             elif (default_range == "boolean"):
                 return slot_code_generators.getBooleanSlotCode(desc, required, propertyName, title)
             else: # this is a basic pdf, so datetime should not be a datetime field, but a textfield
                 return slot_code_generators.getStringSlotCode(desc, required, propertyName, title, slotCode)
         else:
             raise TypeError("Invalid LinkML. There should either be a explicitly defined range for slot {slot}, or a default_range.".format(slot=utils.extractName(slotCode, key)))
 
 def getClassFormCode(classCode, content, default_range, subclasses, level, key):
     title = utils.extractName(classCode, key)
     code = '''<h{level}>{title}</h{level}>\n'''.format(level = level + 1, title = title)
-    code += "<p class='form-description'>Form description: " + utils.capitalizeLabel(utils.extractDescription(classCode)) + "</p>\n"
+    global html_only
+    if(html_only == True):
+        code += "<details><summary style=\"display:list-item\">Form description</summary>" + utils.capitalizeLabel(utils.extractDescription(classCode)) + "</details>"
+    else:
+        code += "<p class='form-description'>Form description: " + utils.capitalizeLabel(utils.extractDescription(classCode)) + "</p>\n"
     if (constants.IS_A in classCode): # process superclass first
         superClassName = classCode.get(constants.IS_A)
         superClassCode = content.get(constants.CLASSES).get(superClassName)
         for slot in superClassCode.get(constants.SLOTS):
             if (slot not in classCode.get("slot_usage")): # this slot is not further specified in the class itself
                 slotCode = content.get(constants.SLOTS).get(slot)
                 code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
@@ -88,15 +96,17 @@
         gen2 = (slot for slot in classCode.get(constants.SLOTS) if (content.get(constants.SLOTS).get(slot).get(constants.RANGE) in subclasses and content.get(constants.SLOTS).get(slot) is not None))
         for slot in gen2: #process slots of this class where the range is a subclass
             slotCode = content.get(constants.SLOTS).get(slot)
             code += getSlotFormCode(slotCode, content, default_range, subclasses, level, slot)
     return code
 
 
-def buildForm(content, html_only, output_directory, name, testEnv = False):
+def buildForm(content, html_only_in, output_directory, name, testEnv = False):
+    global html_only
+    html_only = html_only_in #extra storage for test purposes
     if (constants.NAME not in content and name == constants.DEFAULT): 
         warnings.warn("WARNING: The model metadata does not contain a 'name' field. Please make sure your model is valid")
     NAME = name if (name != constants.DEFAULT) else (content.get(constants.NAME) if constants.NAME in content else "formDefault")
     OUTPUT_DIR = os.getcwd() if (output_directory == constants.CWD) else os.path.abspath(output_directory)
     HTML_PATH = os.path.join(OUTPUT_DIR, NAME + constants.HTML_EXT)
     
     with open(HTML_PATH, "w", encoding="utf-8") as f:
@@ -154,20 +164,22 @@
             html_result = f.read()
             f.close()
             return html_result
 
 def cli():
     if (which("wkhtmltopdf") is None):
         #install somehow, for now: error
-        os.error("wkhtmltopdf is not installed, please install from: https://wkhtmltopdf.org/downloads.html")
+        raise ImportError("wkhtmltopdf is not installed, please install from: https://wkhtmltopdf.org/downloads.html")
         exit(1)
     
     parser = argparse.ArgumentParser("linkmlformbuilder")
     parser.add_argument("yamlfile", help="The LinkML yaml file for which a form should be built")
     parser.add_argument("-html", "--html_only", dest="html_only", action="store_true", help="This flag is used when the user only wants an HTML file returned, there will be no PDF export", default=False)
     parser.add_argument("-dir", "--output_directory", dest="output_directory", help="Specify an output directory, the current working directory is used when this value not provided or the flag is missing", nargs="?", default=constants.CWD, const=constants.CWD)
     parser.add_argument("--name", help="Specify an alternative file name, do not specify a file extension. By default, the filename of the yamlfile is used for the HTML and optionally PDF files", nargs="?", default=constants.DEFAULT, const=constants.DEFAULT)
     args = parser.parse_args()
-    buildForm(retrieveFileContent(args.yamlfile), args.html_only, args.output_directory, args.name)
+    global html_only
+    html_only = args.html_only
+    buildForm(retrieveFileContent(args.yamlfile), html_only, args.output_directory, args.name)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/slot_code_generators.py` & `linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/slot_code_generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from LinkMLFormbuilder import constants, utils
 # import utils
+# import constants
 
 def getNumberSlotCode(slotCode, desc, required, propertyName, title):
     rangeDeclaration = utils.getRangeDeclaration(slotCode)
     multivalued = utils.isMultivalued(slotCode)
     minCardinality = utils.getMinCardinality(slotCode)
     maxCardinality = utils.getMaxCardinality(slotCode)   
     cardinalityStatement = ""
     
     code = '''<div class="mb-3">
     <div class="input-group">
-      <span class="input-group-text" id="{propertyName}-addon">{title}</span>
-      <input type="number" class="form-control" id="{propertyName}" aria-describedby="{propertyName}-addon {propertyName}-description" {required}>
+      <span class="input-group-text width20" id="{propertyName}-addon">{title}</span>
+      <input type="number" class="form-control" id="{propertyName}" name="{propertyName}" aria-describedby="{propertyName}-addon {propertyName}-description" {required}>
     </div>'''.format(propertyName = propertyName, required = required, desc = utils.capitalizeLabel(desc), title = utils.capitalizeLabel(title), rangeDeclaration = rangeDeclaration)
 
     if (multivalued):
         for i in range(maxCardinality-1):
             code += '''<div class="input-group">
-        <span class="input-group-text hideField" id="{propertyName}-addon">{title}</span>
-        <input type="number" class="form-control" id="{propertyName}{n}" aria-describedby="{propertyName}-addon {propertyName}-description">
+        <span class="input-group-text width20 hideField" id="{propertyName}-addon">{title}</span>
+        <input type="number" class="form-control" id="{propertyName}{n}" name="{propertyName}{n}" aria-describedby="{propertyName}-addon {propertyName}-description">
         </div>'''.format(propertyName = propertyName, required = required, title = utils.capitalizeLabel(title), n = i+2)
         cardinalityStatement = ''' This field requires at least {minCardinality} value(s)'''.format(minCardinality = minCardinality)
 
     code += '''
     <div class="form-text" id="{propertyName}-description">{desc} {rangeDeclaration}{cardinalityStatement}</div>
   </div>\n'''.format(propertyName = propertyName, required = required, desc = utils.capitalizeLabel(desc), title = utils.capitalizeLabel(title), rangeDeclaration = rangeDeclaration, cardinalityStatement = cardinalityStatement)
     return code
@@ -31,18 +32,18 @@
     code = '''<div class="mb-3">
             <div class="input-group">\n'''
     code += '''<span class="input-group-text">{slotName}</span>\n'''.format(slotName = utils.capitalizeLabel(title))
     code += '''<input type="text" class="form-control hideField">\n</div>\n'''
     code += '''<div class="form-text" id="{propertyName}-description">{desc}</div>\n'''.format(propertyName = propertyName, desc = utils.capitalizeLabel(desc))
     code += "<div class='answer-options'>\n"
     code += '''<div class="form-check">
-                  <input class="form-check-input" type="radio" name="{enumName}" id="{item}" {required}>
+                  <input class="form-check-input" type="radio" name="{enumName}" id="{item}" value="{item}" {required}>
                   <label class="form-check-label" for="{item}">{item}</label></div>\n'''.format(enumName = propertyName, item = "True", required = required)
     code += '''<div class="form-check">
-                  <input class="form-check-input" type="radio" name="{enumName}" id="{item}" {required}>
+                  <input class="form-check-input" type="radio" name="{enumName}" id="{item}" value="{item}" {required}>
                   <label class="form-check-label" for="{item}">{item}</label></div>\n'''.format(enumName = propertyName, item = "False", required = required)
     code += "</div>\n</div>\n"     
     return code
 
 def getEnumSlotCode(slotCode, content, desc, required, propertyName, title):
     multivalued = utils.isMultivalued(slotCode)
     
@@ -54,99 +55,100 @@
     enumList = []
     if (constants.VALUES_FROM in slotCode):
        for enum in slotCode.get(constants.VALUES_FROM): enumList.append(enum)
     if (constants.RANGE in slotCode and constants.RANGE in content.get(constants.ENUMS)): enumList.append(slotCode.get(constants.RANGE))
     
     for enum in enumList:
       if (enum not in content.get(constants.ENUMS)):
-          return getTextareaSlotCode(desc, required, propertyName, title, slotCode)
+          return getTextareaSlotCode(desc, required, propertyName, title, slotCode, True)
       enumCode = content.get(constants.ENUMS).get(enum)
       enumName = utils.extractName(enumCode, "")
       if (constants.PERMISSIBLE_VALUES in enumCode):
         code += getPermissibleValuesCode(enumCode.get(constants.PERMISSIBLE_VALUES), enumName, multivalued, required)
       else:
-        code += '''<div class='answer-options'>\n<span class='values-from-dynamic'>{enumName}:</span>\n<textarea rows="6" class="form-control" id="{propertyName}"></textarea></div>'''.format(enumName = utils.capitalizeLabel(enumName), propertyName = enumCode.get(constants.NAME))
+        code += '''<div class='answer-options'>\n<span class='values-from-dynamic'>{enumName}:</span>\n<textarea rows="6" class="form-control" id="{propertyName}" name="{propertyName}"></textarea></div>'''.format(enumName = utils.capitalizeLabel(enumName), propertyName = enumCode.get(constants.NAME))
     code += "</div>\n"        
     return code
 
 def getPermissibleValuesCode(permissible_values, enumName, multivalued, required):
     code = "<div class='answer-options'>\n<span class='values-from'>" + utils.capitalizeLabel(enumName) + ":</span>\n"
     for value in permissible_values:
       if (not multivalued):
         code += '''<div class="form-check">
-            <input class="form-check-input" type="radio" name="{enumName}" id="{itemNoSpace}" {required}>
+            <input class="form-check-input" type="radio" name="{enumName}" id="{itemNoSpace}" value="{itemNoSpace}" {required}>
             <label class="form-check-label" for="{itemNoSpace}">{itemCap}</label></div>\n'''.format(enumName = enumName.replace(" ", "_"), required = required, itemNoSpace = value.replace(" ", "_"), itemCap = utils.capitalizeLabel(value))
       else:
             code += '''<div class="form-check">
-            <input class="form-check-input" type="checkbox" name="{enumName}" id="{itemNoSpace}" {required}>
+            <input class="form-check-input" type="checkbox" name="{enumName}" id="{itemNoSpace}" value="{itemNoSpace}" {required}>
             <label class="form-check-label" for="{itemNoSpace}">{itemCap}</label></div>\n'''.format(enumName = enumName.replace(" ", "_"), required = required, itemNoSpace = value.replace(" ", "_"), itemCap = utils.capitalizeLabel(value))
     return code + "</div>\n"
 
 def getInlineEnumSlotCode(slotCode, desc, required, propertyName, title):
     multivalued = utils.isMultivalued(slotCode)
 
     if (constants.ENUM_RANGE not in slotCode or (constants.PERMISSIBLE_VALUES not in slotCode.get(constants.ENUM_RANGE) and "reachable_from" not in slotCode.get(constants.ENUM_RANGE))):
-        return getTextareaSlotCode(desc, required, propertyName, title, slotCode)
+        return getTextareaSlotCode(desc, required, propertyName, title, slotCode, True)
 
     code = '''<div class="mb-3">
             <div class="input-group">\n'''
     code += '''<span class="input-group-text">{slotName}</span>\n'''.format(slotName = utils.capitalizeLabel(title))
     code += '''<input type="text" class="form-control hideField">\n</div>\n'''
     code += '''<div class="form-text" id="{propertyName}-description">{desc}</div>\n'''.format(propertyName = propertyName, desc = utils.capitalizeLabel(desc))
     enumCode = slotCode.get(constants.ENUM_RANGE)
     enumName = utils.extractName(slotCode, "") + " valueset" #inlined enums don't have names and titles, so it's generated from the slot itself
     if (constants.PERMISSIBLE_VALUES in enumCode):
         code += getPermissibleValuesCode(enumCode.get(constants.PERMISSIBLE_VALUES), enumName, multivalued, required)
     else:
-      code += '''<div class='answer-options'>\n<span class='values-from-dynamic'>{enumName}:</span>\n<textarea rows="6" class="form-control" id="{enumNameNoSpace}"></textarea>\n</div>\n'''.format(enumName = utils.capitalizeLabel(enumName), propertyName = enumCode.get(constants.NAME), enumNameNoSpace = enumName.replace(" ", "_"))
+      code += '''<div class='answer-options'>\n<span class='values-from-dynamic'>{enumName}:</span>\n<textarea rows="6" class="form-control" id="{enumNameNoSpace}" name="{enumNameNoSpace}"></textarea>\n</div>\n'''.format(enumName = utils.capitalizeLabel(enumName), propertyName = enumCode.get(constants.NAME), enumNameNoSpace = enumName.replace(" ", "_"))
     code += "</div>\n"     
     return code
 
 def getStringSlotCode(desc, required, propertyName, title, slotCode):
     multivalued = utils.isMultivalued(slotCode)
     minCardinality = utils.getMinCardinality(slotCode)
     maxCardinality = utils.getMaxCardinality(slotCode)   
     cardinalityStatement = ""
 
     code =  '''<div class="mb-3">
     <div class="input-group">
-      <span class="input-group-text" id="{propertyName}-addon">{title}</span>
-      <input type="text" class="form-control" id="{propertyName}" aria-describedby="{propertyName}-addon {propertyName}-description" {required}>
+      <span class="input-group-text width20" id="{propertyName}-addon">{title}</span>
+      <input type="text" class="form-control" id="{propertyName}" name="{propertyName}" aria-describedby="{propertyName}-addon {propertyName}-description" {required}>
     </div>
     '''.format(propertyName = propertyName, required = required, title = utils.capitalizeLabel(title))
     if (multivalued):
         for i in range(maxCardinality-1):
             code += '''<div class="input-group">
-      <span class="input-group-text hideField" id="{propertyName}-addon">{title}</span>
-      <input type="text" class="form-control" id="{propertyName}{n}" aria-describedby="{propertyName}-addon {propertyName}-description">
+      <span class="input-group-text width20 hideField" id="{propertyName}-addon">{title}</span>
+      <input type="text" class="form-control" id="{propertyName}{n}" name="{propertyName}{n}" aria-describedby="{propertyName}-addon {propertyName}-description">
     </div>'''.format(propertyName = propertyName, required = required, title = utils.capitalizeLabel(title), n = i+2)
         cardinalityStatement = ''' This field requires at least {minCardinality} value(s)'''.format(minCardinality = minCardinality)
 
 
     code += '''<div class="form-text" id="{propertyName}-description">{desc}{cardinalityStatement}</div>
   </div>\n'''.format(propertyName = propertyName, desc = utils.capitalizeLabel(desc), cardinalityStatement = cardinalityStatement)
     return code
 
-def getTextareaSlotCode(desc, required, propertyName, title, slotCode):
+def getTextareaSlotCode(desc, required, propertyName, title, slotCode, html_only):
     multivalued = utils.isMultivalued(slotCode)
     minCardinality = utils.getMinCardinality(slotCode)
     maxCardinality = utils.getMaxCardinality(slotCode)   
     cardinalityStatement = ""
+    rows = 2 if html_only else 6
 
     code = '''<div class="mb-3">
     <div class="input-group">
-      <span class="input-group-text" id="{propertyName}-addon">{title}</span>
-      <textarea rows="6" class="form-control" id="{propertyName}" aria-describedby="{propertyName}-addon {propertyName}-description" {required}></textarea>
-    </div>'''.format(propertyName = propertyName, required = required, desc = utils.capitalizeLabel(desc), title = utils.capitalizeLabel(title))
+      <span class="input-group-text width20" id="{propertyName}-addon">{title}</span>
+      <textarea rows="{rows}" class="form-control" id="{propertyName}" name="{propertyName}" aria-describedby="{propertyName}-addon {propertyName}-description" {required}></textarea>
+    </div>'''.format(propertyName = propertyName, required = required, desc = utils.capitalizeLabel(desc), title = utils.capitalizeLabel(title), rows=rows)
 
     if (multivalued):
         for i in range(maxCardinality-1):
             code += '''<div class="input-group">
-      <span class="input-group-text hideField" id="{propertyName}-addon">{title}</span>
-      <textarea rows="6" class="form-control" id="{propertyName}{n}" aria-describedby="{propertyName}-addon {propertyName}-description"></textarea>
-    </div>'''.format(propertyName = propertyName, required = required, title = utils.capitalizeLabel(title), n = i+2)
+      <span class="input-group-text width20 hideField" id="{propertyName}-addon">{title}</span>
+      <textarea rows="{rows}" class="form-control" id="{propertyName}{n}" name="{propertyName}{n}" aria-describedby="{propertyName}-addon {propertyName}-description"></textarea>
+    </div>'''.format(propertyName = propertyName, required = required, title = utils.capitalizeLabel(title), n = i+2, rows=rows)
         cardinalityStatement = ''' This field requires at least {minCardinality} value(s)'''.format(minCardinality = minCardinality)
 
 
     code += '''<div class="form-text" id="{propertyName}-description">{desc}{cardinalityStatement}</div>
   </div>\n'''.format(propertyName = propertyName, required = required, desc = utils.capitalizeLabel(desc), title = utils.capitalizeLabel(title), cardinalityStatement = cardinalityStatement)
     return code
```

### Comparing `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/styles.css` & `linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/styles.css`

 * *Files 17% similar despite different names*

```diff
@@ -35,35 +35,38 @@
     line-height: 1.5;
     color: #212529;
     text-align: center;
     white-space: nowrap;
     background-color: #f8f9fa;
     border: 1px solid #dee2e6;
     border-radius: 0.375rem;
-    width: 20%;
     float: left;
     min-height: 34px;
     white-space: pre-wrap;
 }
 
+.width20 {
+    width: 20%
+}
+
 .form-control {
     width: 80% !important;
     height: 100%;
 }
 
 .input-group {
     position: relative;
     display: flex;
     flex-wrap: wrap;
     align-items: stretch;
     width: 100%;
 }
 
 .hideField {
-    visibility: hidden;
+    display: none !important;
 }
 
 .form-check {
     width: fit-content;
     display: inline-block;
     margin-right: 5px;
 }
@@ -79,7 +82,34 @@
     float: left;
     width: calc(20% - 5px);
 }
 
 h2 {
     width: 100vw;
 }
+
+.answer-options {
+    padding-left: 0.667px;
+}
+
+details {
+    border: 1px solid #dee2e6;
+    border-radius: 0.375rem;
+    padding: 0.5em 0.5em 0;
+    width: fit-content;
+    margin-bottom: 0.5rem;
+}
+  
+summary {
+    font-weight: bold;
+    margin: -0.5em -0.5em 0;
+    padding: 0.5em;
+}
+  
+details[open] {
+    padding: 0.5em;
+}
+  
+details[open] summary {
+    border-bottom: 1px solid #dee2e6;
+    margin-bottom: 0.5em;
+}
```

### Comparing `linkmlformbuilder-0.1.9/src/LinkMLFormbuilder/utils.py` & `linkmlformbuilder-1.0.0/src/LinkMLFormbuilder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from LinkMLFormbuilder import constants
+# import constants
 import warnings
 
 def extractAliases(sourceCode):
     name = ""
     if (constants.ALIASES in sourceCode or constants.STRUCTURED_ALIASES in sourceCode or constants.LOCAL_NAMES in sourceCode):
         name += " ("
         if (constants.ALIASES in sourceCode):
```

### Comparing `linkmlformbuilder-0.1.9/LICENSE` & `linkmlformbuilder-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linkmlformbuilder-0.1.9/README.md` & `linkmlformbuilder-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,21 @@
                         flag is missing
   --name [NAME]         Specify an alternative file name, do not specify a
                         file extension. By default, the filename of the
                         yamlfile is used for the HTML and optionally PDF files
 ```
 
 ## Changelog
+### Version 1.0.0
+- UI update for html-only forms
+### Version 0.1.11
+- Add value fields to radio buttons so they show up in FormData
+- Fix issue with inline attributes and slots without a name field
+### Version 0.1.10
+- Add name fields to input and textareas
 ### Version 0.1.9
 - Missing 'name' field error is now a warning
 - Default options for missing 'name' fields
 ### Version 0.1.8
 - Throw error when field 'name' is missing from a model element
 - Auto close file on error (with statement)
 ### Version 0.1.7
```

### Comparing `linkmlformbuilder-0.1.9/pyproject.toml` & `linkmlformbuilder-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build.targets.sdist]
 include = [
     "src/LinkMLFormbuilder"
 ]
 
 [project]
 name = "LinkMLFormbuilder"
-version = "0.1.9"
+version = "1.0.0"
 authors = [
   { name="N. van Brummelen" },
 ]
 description = "Build forms from LinkML. Export to HTML or (basic) PDF"
 dependencies = ["pdfkit", "pyyaml"]
 readme = "README.md"
 requires-python = ">=3"
```

### Comparing `linkmlformbuilder-0.1.9/PKG-INFO` & `linkmlformbuilder-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: LinkMLFormbuilder
-Version: 0.1.9
+Version: 1.0.0
 Summary: Build forms from LinkML. Export to HTML or (basic) PDF
 Project-URL: Homepage, https://github.com/AmsterdamUMC/LinkMLFormBuilder#
 Project-URL: Issues, https://github.com/AmsterdamUMC/LinkMLFormBuilder/issues
 Author: N. van Brummelen
 License-Expression: GPL-3.0-only
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -61,14 +61,21 @@
                         flag is missing
   --name [NAME]         Specify an alternative file name, do not specify a
                         file extension. By default, the filename of the
                         yamlfile is used for the HTML and optionally PDF files
 ```
 
 ## Changelog
+### Version 1.0.0
+- UI update for html-only forms
+### Version 0.1.11
+- Add value fields to radio buttons so they show up in FormData
+- Fix issue with inline attributes and slots without a name field
+### Version 0.1.10
+- Add name fields to input and textareas
 ### Version 0.1.9
 - Missing 'name' field error is now a warning
 - Default options for missing 'name' fields
 ### Version 0.1.8
 - Throw error when field 'name' is missing from a model element
 - Auto close file on error (with statement)
 ### Version 0.1.7
```

