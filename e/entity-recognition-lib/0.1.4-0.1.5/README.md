# Comparing `tmp/entity_recognition_lib-0.1.4.tar.gz` & `tmp/entity_recognition_lib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entity_recognition_lib-0.1.4.tar", max compression
+gzip compressed data, was "entity_recognition_lib-0.1.5.tar", max compression
```

## Comparing `entity_recognition_lib-0.1.4.tar` & `entity_recognition_lib-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1053 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/LICENSE
--rw-r--r--   0        0        0     3698 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/README.md
--rw-r--r--   0        0        0     1311 2024-05-11 13:43:53.008228 entity_recognition_lib-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1798 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/EntityRecognizer.py
--rw-r--r--   0        0        0       61 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/__init__.py
--rw-r--r--   0        0        0    31581 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/data/tech_entities.json
--rw-r--r--   0        0        0        0 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/__init__.py
--rw-r--r--   0        0        0     2768 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/entity_extraction.py
--rw-r--r--   0        0        0     5232 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/recommendation_generation.py
--rw-r--r--   0        0        0     1271 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/topic_classification.py
--rw-r--r--   0        0        0     1725 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/models.py
--rw-r--r--   0        0        0     3267 2024-05-11 13:42:36.963997 entity_recognition_lib-0.1.4/src/entity_recognition_lib/utils.py
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 entity_recognition_lib-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3696 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/README.md
+-rw-r--r--   0        0        0     1828 2024-05-13 13:02:31.478689 entity_recognition_lib-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1821 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/EntityRecognizer.py
+-rw-r--r--   0        0        0       61 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/__init__.py
+-rw-r--r--   0        0        0    31573 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/data/tech_entities.json
+-rw-r--r--   0        0        0        0 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/__init__.py
+-rw-r--r--   0        0        0     2868 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/entity_extraction.py
+-rw-r--r--   0        0        0     5314 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/recommendation_generation.py
+-rw-r--r--   0        0        0     1271 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/topic_classification.py
+-rw-r--r--   0        0        0     1725 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/models.py
+-rw-r--r--   0        0        0     3279 2024-05-13 13:01:06.385285 entity_recognition_lib-0.1.5/src/entity_recognition_lib/utils.py
+-rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 entity_recognition_lib-0.1.5/PKG-INFO
```

### Comparing `entity_recognition_lib-0.1.4/LICENSE` & `entity_recognition_lib-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `entity_recognition_lib-0.1.4/README.md` & `entity_recognition_lib-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Entity-Recognition
 
-The Entity-Recognition library utilizes `spaCy`, `BERTopic`, and `Transformers` to provide a robust technology entity recognition system capable of identifying technological entities within texts and suggesting relevant technologies using advanced NLP techniques.
+The Entity-Recognition library utilizes `spaCy`, `BERTopic`, and `Transformers` to provide a robust technology entity
+recognition system capable of identifying technological entities within texts and suggesting relevant technologies using
+advanced NLP techniques.
 
 The library automatically downloads the required spaCy model if not installed, making it easy to get started.
 
-
 ## Features
 
 - **Technology Entity Extraction**: Automatically extract technology-related terms and tools from texts.
 - **Recommendation System**: Provides context-based technology recommendations.
 - **BERTopic Integration**: Leverages topic modeling to enhance the relevance of recommendations.
 - **spaCy Matchers**: Utilizes custom NLP patterns for precise entity recognition.
 
@@ -23,20 +24,18 @@
 
 Install the library directly from PyPI:
 
 ```bash
 pip install entity-recognition-lib
 ```
 
-The required spaCy model (`en_core_web_sm`) will be automatically downloaded and installed if not already present on your system.
-
-
+The required spaCy model (`en_core_web_sm`) will be automatically downloaded and installed if not already present on
+your system.
 
-Usage
------
+## Usage
 
 Here's how to use the Entity Recognition library in your Python scripts:
 
 ```python
 from entity_recognition_lib import EntityRecognizer
 
 # Create an instance of the recognizer
@@ -45,14 +44,15 @@
 # Example texts
 texts = ["I need an Express.js Mongo database backend"]
 
 # Process texts
 results = recognizer.process_texts(texts)
 print(results)
 ```
+
 Expected output:
 
 ```json
 [
     {
         "input_text": "I need an Express.js Mongo database backend",
         "predicted_topic_name": "575_databases_database_tables_schema",
@@ -81,56 +81,59 @@
     }
 ]
 ```
 
 For detailed usage examples and code snippets, please refer to the [examples directory](examples/EXAMPLES.md) in the repository.
 The examples cover various scenarios, including:
 
-1. Basic usage of the library for entity recognition and recommendation generation
-2. Advanced features such as result analysis and visualization
-3. Integration samples with popular frameworks like Flask and Streamlit
+- Basic usage of the library for entity recognition and recommendation generation
+- Advanced features such as result analysis and visualization
+- Integration samples with popular frameworks like Flask and Streamlit
 
-We recommend exploring the examples to understand how to effectively utilize the Entity-Recognition library in your projects.
+We recommend exploring the examples to understand how to effectively utilize the Entity-Recognition library in your
+projects.
 
 ## Development
 
 ### Setting Up a Development Environment
 
-1. **Clone the repository**:
-   ```
+- **Clone the repository**:
+
+   ```bash
    git clone https://github.com/cgoncalves94/entity-recognition.git
    cd entity-recognition
    ```
-2. **Create and Activate a Virtual Environment**:
+
+- **Create and Activate a Virtual Environment**:
+
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
-3. **Install Dependencies**:
-    ```
+
+- **Install Dependencies**:
+
+    ```bash
     pip install -r requirements.txt
     ```
 
-
 ## Testing
 
 Run tests to ensure the setup is correct:
 
-```
+```bash
 pytest
 ```
 
 ## Contributing
 
 Contributions are welcome! Please follow these steps:
 
-1. Fork the repository on GitHub.
-2. Clone the forked repository to your machine.
-3. Create a new branch for your changes.
-4. Make changes and test.
-5. Submit a pull request with a comprehensive description of changes.
+- Fork the repository on GitHub.
+- Clone the forked repository to your machine.
+- Create a new branch for your changes.
+- Make changes and test.
+- Submit a pull request with a comprehensive description of changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-
```

### Comparing `entity_recognition_lib-0.1.4/pyproject.toml` & `entity_recognition_lib-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "entity-recognition-lib"
-version = "0.1.4"
+version = "0.1.5"
 description = "A library for technology entity recognition and recommendation"
 authors = ["Cesar Goncalves <goncalves.cesaraugusto94@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
@@ -29,22 +29,15 @@
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-line-length = 160
-lint.select = [
-    "F",    # Pyflakes
-    "E",    # Pycodestyle
-    "W",    # Pycodestyle warnings
-    "I001", # isort
-]
-lint.ignore = []
+# Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
     ".mypy_cache",
@@ -58,13 +51,43 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "venv",
 ]
-lint.per-file-ignores = {}
-lint.dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+line-length = 120
+indent-width = 4
+
 target-version = "py311"
 
-[tool.ruff.lint.mccabe]
-max-complexity = 10
+[tool.ruff.lint]
+# Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
+select = [
+    "E4",
+    "E7",
+    "E9",
+    "F",
+    "I001"  # isort
+]
+ignore = []
+
+# Allow fix for all enabled rules (when `--fix`) is provided.
+fixable = ["ALL"]
+unfixable = []
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+[tool.ruff.format]
+# Like Black, use double quotes for strings.
+quote-style = "double"
+
+# Like Black, indent with spaces, rather than tabs.
+indent-style = "space"
+
+# Like Black, respect magic trailing commas.
+skip-magic-trailing-comma = false
+
+# Like Black, automatically detect the appropriate line ending.
+line-ending = "auto"
```

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/EntityRecognizer.py` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/EntityRecognizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,18 @@
         sorted_entities = dynamic_score_entities(extracted_entities, topic_keywords, text, self.tech_entities)
         recommendations = recommend_technologies(sorted_entities)
 
         return {
             "input_text": text,
             "predicted_topic_name": topic_name,
             "extracted_entities": sorted_entities,
-            "recommendations": recommendations
+            "recommendations": recommendations,
         }
 
     def process_texts(self, texts):
         results = []
         for text in texts:
             result = self.process_text(text)
             results.append(result)
-        return json.dumps(results, indent=4)  # Serialize the list of results to a JSON formatted string with indentation
+        return json.dumps(
+            results, indent=4
+        )  # Serialize the list of results to a JSON formatted string with indentation
```

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/data/tech_entities.json` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/data/tech_entities.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -1013,962 +1013,962 @@
 00003f40: 4c4f 5745 5222 3a20 7b20 2246 555a 5a59  LOWER": { "FUZZY
 00003f50: 3122 3a20 226d 6174 6572 6961 6c20 7569  1": "material ui
 00003f60: 2220 7d20 7d5d 2c0a 2020 2020 2020 2020  " } }],.        
 00003f70: 2020 5b7b 2022 4c4f 5745 5222 3a20 7b20    [{ "LOWER": { 
 00003f80: 2246 555a 5a59 3122 3a20 226d 6174 6572  "FUZZY1": "mater
 00003f90: 6961 6c2d 7569 2220 7d20 7d5d 0a20 2020  ial-ui" } }].   
 00003fa0: 2020 205d 2c0a 2020 2020 2020 2273 636f     ],.      "sco
-00003fb0: 7265 223a 2039 0a20 207d 2c0a 2020 0a20  re": 9.  },.  . 
-00003fc0: 2022 4157 5322 3a20 7b0a 2020 2020 2020   "AWS": {.      
-00003fd0: 2274 7970 6522 3a20 2243 6c6f 7564 2043  "type": "Cloud C
-00003fe0: 6f6d 7075 7469 6e67 222c 0a20 2020 2020  omputing",.     
-00003ff0: 2022 6361 7465 676f 7279 223a 2022 436c   "category": "Cl
-00004000: 6f75 6420 5365 7276 6963 6520 5072 6f76  oud Service Prov
-00004010: 6964 6572 7322 2c0a 2020 2020 2020 2264  iders",.      "d
-00004020: 6573 6372 6970 7469 6f6e 223a 2022 416d  escription": "Am
-00004030: 617a 6f6e 2057 6562 2053 6572 7669 6365  azon Web Service
-00004040: 7320 6f66 6665 7273 2072 656c 6961 626c  s offers reliabl
-00004050: 652c 2073 6361 6c61 626c 652c 2061 6e64  e, scalable, and
-00004060: 2069 6e65 7870 656e 7369 7665 2063 6c6f   inexpensive clo
-00004070: 7564 2063 6f6d 7075 7469 6e67 2073 6572  ud computing ser
-00004080: 7669 6365 732e 2049 7427 7320 7468 6520  vices. It's the 
-00004090: 776f 726c 6427 7320 6d6f 7374 2063 6f6d  world's most com
-000040a0: 7072 6568 656e 7369 7665 2061 6e64 2062  prehensive and b
-000040b0: 726f 6164 6c79 2061 646f 7074 6564 2063  roadly adopted c
-000040c0: 6c6f 7564 2070 6c61 7466 6f72 6d2c 206f  loud platform, o
-000040d0: 6666 6572 696e 6720 6f76 6572 2031 3735  ffering over 175
-000040e0: 2066 756c 6c79 2d66 6561 7475 7265 6420   fully-featured 
-000040f0: 7365 7276 6963 6573 2066 726f 6d20 6461  services from da
-00004100: 7461 2063 656e 7465 7273 2067 6c6f 6261  ta centers globa
-00004110: 6c6c 792e 222c 0a20 2020 2020 2022 7061  lly.",.      "pa
-00004120: 7474 6572 6e73 223a 205b 0a20 2020 2020  tterns": [.     
-00004130: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
-00004140: 2022 6177 7322 207d 5d2c 0a20 2020 2020   "aws" }],.     
-00004150: 2020 2020 205b 7b20 2254 4558 5422 3a20       [{ "TEXT": 
-00004160: 7b20 2246 555a 5a59 3122 3a20 2241 6d61  { "FUZZY1": "Ama
-00004170: 7a6f 6e20 5765 6220 5365 7276 6963 6573  zon Web Services
-00004180: 2220 7d20 7d5d 0a20 2020 2020 205d 2c0a  " } }].      ],.
-00004190: 2020 2020 2020 2273 636f 7265 223a 2039        "score": 9
-000041a0: 0a20 207d 2c0a 2020 2241 7a75 7265 223a  .  },.  "Azure":
-000041b0: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
-000041c0: 2022 436c 6f75 6420 436f 6d70 7574 696e   "Cloud Computin
-000041d0: 6722 2c0a 2020 2020 2020 2263 6174 6567  g",.      "categ
-000041e0: 6f72 7922 3a20 2243 6c6f 7564 2053 6572  ory": "Cloud Ser
-000041f0: 7669 6365 2050 726f 7669 6465 7273 222c  vice Providers",
-00004200: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
-00004210: 696f 6e22 3a20 224d 6963 726f 736f 6674  ion": "Microsoft
-00004220: 2041 7a75 7265 2069 7320 6120 636c 6f75   Azure is a clou
-00004230: 6420 636f 6d70 7574 696e 6720 7365 7276  d computing serv
-00004240: 6963 6520 666f 7220 6275 696c 6469 6e67  ice for building
-00004250: 2c20 7465 7374 696e 672c 2064 6570 6c6f  , testing, deplo
-00004260: 7969 6e67 2c20 616e 6420 6d61 6e61 6769  ying, and managi
-00004270: 6e67 2061 7070 6c69 6361 7469 6f6e 7320  ng applications 
-00004280: 616e 6420 7365 7276 6963 6573 2074 6872  and services thr
-00004290: 6f75 6768 204d 6963 726f 736f 6674 2d6d  ough Microsoft-m
-000042a0: 616e 6167 6564 2064 6174 6120 6365 6e74  anaged data cent
-000042b0: 6572 732e 2049 7420 7072 6f76 6964 6573  ers. It provides
-000042c0: 2073 6f66 7477 6172 6520 6173 2061 2073   software as a s
-000042d0: 6572 7669 6365 2028 5361 6153 292c 2070  ervice (SaaS), p
-000042e0: 6c61 7466 6f72 6d20 6173 2061 2073 6572  latform as a ser
-000042f0: 7669 6365 2028 5061 6153 292c 2061 6e64  vice (PaaS), and
-00004300: 2069 6e66 7261 7374 7275 6374 7572 6520   infrastructure 
-00004310: 6173 2061 2073 6572 7669 6365 2028 4961  as a service (Ia
-00004320: 6153 292e 222c 0a20 2020 2020 2022 7061  aS).",.      "pa
-00004330: 7474 6572 6e73 223a 205b 0a20 2020 2020  tterns": [.     
-00004340: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
-00004350: 207b 2022 4655 5a5a 5931 223a 2022 617a   { "FUZZY1": "az
-00004360: 7572 6522 207d 207d 5d2c 0a20 2020 2020  ure" } }],.     
-00004370: 2020 2020 205b 7b20 2254 4558 5422 3a20       [{ "TEXT": 
-00004380: 7b20 2246 555a 5a59 3122 3a20 224d 6963  { "FUZZY1": "Mic
-00004390: 726f 736f 6674 2041 7a75 7265 2220 7d20  rosoft Azure" } 
-000043a0: 7d5d 0a20 2020 2020 205d 2c0a 2020 2020  }].      ],.    
-000043b0: 2020 2273 636f 7265 223a 2039 0a20 207d    "score": 9.  }
-000043c0: 2c0a 2020 2247 6f6f 676c 6543 6c6f 7564  ,.  "GoogleCloud
-000043d0: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
-000043e0: 223a 2022 436c 6f75 6420 436f 6d70 7574  ": "Cloud Comput
-000043f0: 696e 6722 2c0a 2020 2020 2020 2263 6174  ing",.      "cat
-00004400: 6567 6f72 7922 3a20 2243 6c6f 7564 2053  egory": "Cloud S
-00004410: 6572 7669 6365 2050 726f 7669 6465 7273  ervice Providers
-00004420: 222c 0a20 2020 2020 2022 6465 7363 7269  ",.      "descri
-00004430: 7074 696f 6e22 3a20 2247 6f6f 676c 6520  ption": "Google 
-00004440: 436c 6f75 6420 506c 6174 666f 726d 2c20  Cloud Platform, 
-00004450: 6f66 6665 7265 6420 6279 2047 6f6f 676c  offered by Googl
-00004460: 652c 2069 7320 6120 7375 6974 6520 6f66  e, is a suite of
-00004470: 2063 6c6f 7564 2063 6f6d 7075 7469 6e67   cloud computing
-00004480: 2073 6572 7669 6365 7320 7468 6174 2072   services that r
-00004490: 756e 7320 6f6e 2074 6865 2073 616d 6520  uns on the same 
-000044a0: 696e 6672 6173 7472 7563 7475 7265 2074  infrastructure t
-000044b0: 6861 7420 476f 6f67 6c65 2075 7365 7320  hat Google uses 
-000044c0: 696e 7465 726e 616c 6c79 2066 6f72 2069  internally for i
-000044d0: 7473 2065 6e64 2d75 7365 7220 7072 6f64  ts end-user prod
-000044e0: 7563 7473 2c20 7375 6368 2061 7320 476f  ucts, such as Go
-000044f0: 6f67 6c65 2053 6561 7263 682c 2047 6d61  ogle Search, Gma
-00004500: 696c 2c20 6669 6c65 2073 746f 7261 6765  il, file storage
-00004510: 2c20 616e 6420 596f 7554 7562 652e 222c  , and YouTube.",
-00004520: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
-00004530: 223a 205b 0a20 2020 2020 2020 2020 205b  ": [.          [
-00004540: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00004550: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
-00004560: 5a59 3122 3a20 2267 6f6f 676c 6522 207d  ZY1": "google" }
-00004570: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00004580: 2020 7b20 224c 4f57 4552 223a 207b 2022    { "LOWER": { "
-00004590: 4655 5a5a 5931 223a 2022 636c 6f75 6422  FUZZY1": "cloud"
-000045a0: 207d 207d 0a20 2020 2020 2020 2020 205d   } }.          ]
-000045b0: 2c0a 2020 2020 2020 2020 2020 5b7b 2022  ,.          [{ "
-000045c0: 4c4f 5745 5222 3a20 2267 6370 2220 7d5d  LOWER": "gcp" }]
-000045d0: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-000045e0: 2273 636f 7265 223a 2039 0a20 207d 2c0a  "score": 9.  },.
-000045f0: 2020 2247 6974 4875 6222 3a20 7b0a 2020    "GitHub": {.  
-00004600: 2020 2020 2274 7970 6522 3a20 2250 6c61      "type": "Pla
-00004610: 7466 6f72 6d22 2c0a 2020 2020 2020 2263  tform",.      "c
-00004620: 6174 6567 6f72 7922 3a20 2256 6572 7369  ategory": "Versi
-00004630: 6f6e 2043 6f6e 7472 6f6c 222c 0a20 2020  on Control",.   
-00004640: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00004650: 3a20 2247 6974 4875 6220 6973 2061 2077  : "GitHub is a w
-00004660: 6562 2d62 6173 6564 2076 6572 7369 6f6e  eb-based version
-00004670: 2063 6f6e 7472 6f6c 2061 6e64 2063 6f6c   control and col
-00004680: 6c61 626f 7261 7469 6f6e 2070 6c61 7466  laboration platf
-00004690: 6f72 6d20 666f 7220 736f 6674 7761 7265  orm for software
-000046a0: 2064 6576 656c 6f70 6572 732e 2049 7420   developers. It 
-000046b0: 656e 6162 6c65 7320 7573 6572 7320 746f  enables users to
-000046c0: 2073 746f 7265 2c20 6d61 6e61 6765 2c20   store, manage, 
-000046d0: 616e 6420 7472 6163 6b20 6368 616e 6765  and track change
-000046e0: 7320 746f 2074 6865 6972 2063 6f64 6520  s to their code 
-000046f0: 7072 6f6a 6563 7473 2075 7369 6e67 2074  projects using t
-00004700: 6865 2047 6974 2076 6572 7369 6f6e 2063  he Git version c
-00004710: 6f6e 7472 6f6c 2073 7973 7465 6d2e 222c  ontrol system.",
-00004720: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
-00004730: 223a 205b 5b7b 2022 4c4f 5745 5222 3a20  ": [[{ "LOWER": 
-00004740: 7b20 2246 555a 5a59 3122 3a20 2267 6974  { "FUZZY1": "git
-00004750: 6875 6222 207d 207d 5d5d 2c0a 2020 2020  hub" } }]],.    
-00004760: 2020 2273 636f 7265 223a 2037 0a20 207d    "score": 7.  }
-00004770: 2c0a 2020 2247 6974 4875 6220 4163 7469  ,.  "GitHub Acti
-00004780: 6f6e 7322 3a20 7b0a 2020 2020 2020 2274  ons": {.      "t
-00004790: 7970 6522 3a20 2241 7574 6f6d 6174 696f  ype": "Automatio
-000047a0: 6e20 576f 726b 666c 6f77 222c 0a20 2020  n Workflow",.   
-000047b0: 2020 2022 6361 7465 676f 7279 223a 2022     "category": "
-000047c0: 4349 2f43 4422 2c0a 2020 2020 2020 2264  CI/CD",.      "d
-000047d0: 6573 6372 6970 7469 6f6e 223a 2022 4769  escription": "Gi
-000047e0: 7448 7562 2041 6374 696f 6e73 2061 6c6c  tHub Actions all
-000047f0: 6f77 2079 6f75 2074 6f20 6372 6561 7465  ow you to create
-00004800: 2063 6f6e 7469 6e75 6f75 7320 696e 7465   continuous inte
-00004810: 6772 6174 696f 6e20 616e 6420 636f 6e74  gration and cont
-00004820: 696e 756f 7573 2064 6570 6c6f 796d 656e  inuous deploymen
-00004830: 7420 2843 492f 4344 2920 7069 7065 6c69  t (CI/CD) pipeli
-00004840: 6e65 7320 7269 6768 7420 696e 7369 6465  nes right inside
-00004850: 2079 6f75 7220 4769 7448 7562 2072 6570   your GitHub rep
-00004860: 6f73 6974 6f72 792e 222c 0a20 2020 2020  ository.",.     
-00004870: 2022 7061 7474 6572 6e73 223a 205b 0a20   "patterns": [. 
-00004880: 2020 2020 2020 2020 205b 7b20 224c 4f57           [{ "LOW
-00004890: 4552 223a 207b 2022 4655 5a5a 5931 223a  ER": { "FUZZY1":
-000048a0: 2022 6769 7468 7562 2061 6374 696f 6e73   "github actions
-000048b0: 2220 7d20 7d5d 2c0a 2020 2020 2020 2020  " } }],.        
-000048c0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000048d0: 2020 7b20 224c 4f57 4552 223a 207b 2022    { "LOWER": { "
-000048e0: 4655 5a5a 5931 223a 2022 6769 7468 7562  FUZZY1": "github
-000048f0: 2220 7d20 7d2c 0a20 2020 2020 2020 2020  " } },.         
-00004900: 2020 2020 207b 2022 4c4f 5745 5222 3a20       { "LOWER": 
-00004910: 7b20 2246 555a 5a59 3122 3a20 2261 6374  { "FUZZY1": "act
-00004920: 696f 6e73 2220 7d20 7d0a 2020 2020 2020  ions" } }.      
-00004930: 2020 2020 5d0a 2020 2020 2020 5d2c 0a20      ].      ],. 
-00004940: 2020 2020 2022 7363 6f72 6522 3a20 3130       "score": 10
-00004950: 0a20 207d 2c0a 2020 224a 656e 6b69 6e73  .  },.  "Jenkins
-00004960: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
-00004970: 223a 2022 4175 746f 6d61 7469 6f6e 2053  ": "Automation S
-00004980: 6572 7665 7222 2c0a 2020 2020 2020 2263  erver",.      "c
-00004990: 6174 6567 6f72 7922 3a20 2243 492f 4344  ategory": "CI/CD
-000049a0: 222c 0a20 2020 2020 2022 6465 7363 7269  ",.      "descri
-000049b0: 7074 696f 6e22 3a20 2241 6e20 6f70 656e  ption": "An open
-000049c0: 2d73 6f75 7263 6520 6175 746f 6d61 7469  -source automati
-000049d0: 6f6e 2073 6572 7665 7220 7468 6174 2065  on server that e
-000049e0: 6e61 626c 6573 2064 6576 656c 6f70 6572  nables developer
-000049f0: 7320 746f 2062 7569 6c64 2c20 7465 7374  s to build, test
-00004a00: 2c20 616e 6420 6465 706c 6f79 2074 6865  , and deploy the
-00004a10: 6972 2073 6f66 7477 6172 6520 6175 746f  ir software auto
-00004a20: 6d61 7469 6361 6c6c 792e 222c 0a20 2020  matically.",.   
-00004a30: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
-00004a40: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
-00004a50: 555a 5a59 3122 3a20 226a 656e 6b69 6e73  UZZY1": "jenkins
-00004a60: 2220 7d20 7d5d 5d2c 0a20 2020 2020 2022  " } }]],.      "
-00004a70: 7363 6f72 6522 3a20 380a 2020 7d2c 0a20  score": 8.  },. 
-00004a80: 2022 4369 7263 6c65 4349 223a 207b 0a20   "CircleCI": {. 
-00004a90: 2020 2020 2022 7479 7065 223a 2022 436f       "type": "Co
-00004aa0: 6e74 696e 756f 7573 2049 6e74 6567 7261  ntinuous Integra
-00004ab0: 7469 6f6e 2054 6f6f 6c22 2c0a 2020 2020  tion Tool",.    
-00004ac0: 2020 2263 6174 6567 6f72 7922 3a20 2243    "category": "C
-00004ad0: 492f 4344 222c 0a20 2020 2020 2022 6465  I/CD",.      "de
-00004ae0: 7363 7269 7074 696f 6e22 3a20 2243 6972  scription": "Cir
-00004af0: 636c 6543 4920 6973 2061 2063 6f6e 7469  cleCI is a conti
-00004b00: 6e75 6f75 7320 696e 7465 6772 6174 696f  nuous integratio
-00004b10: 6e20 616e 6420 636f 6e74 696e 756f 7573  n and continuous
-00004b20: 2064 656c 6976 6572 7920 706c 6174 666f   delivery platfo
-00004b30: 726d 2074 6861 7420 6865 6c70 7320 736f  rm that helps so
-00004b40: 6674 7761 7265 2074 6561 6d73 2077 6f72  ftware teams wor
-00004b50: 6b20 736d 6172 7465 722c 2066 6173 7465  k smarter, faste
-00004b60: 722e 222c 0a20 2020 2020 2022 7061 7474  r.",.      "patt
-00004b70: 6572 6e73 223a 205b 0a20 2020 2020 2020  erns": [.       
-00004b80: 205b 7b20 224c 4f57 4552 223a 207b 2022   [{ "LOWER": { "
-00004b90: 4655 5a5a 5931 223a 2022 6369 7263 6c65  FUZZY1": "circle
-00004ba0: 6369 2220 7d20 7d5d 2c0a 2020 2020 2020  ci" } }],.      
-00004bb0: 2020 5b7b 2022 4c4f 5745 5222 3a20 7b20    [{ "LOWER": { 
-00004bc0: 2246 555a 5a59 3122 3a20 2263 6972 636c  "FUZZY1": "circl
-00004bd0: 6522 207d 207d 2c20 7b20 224c 4f57 4552  e" } }, { "LOWER
-00004be0: 223a 2022 6369 2220 7d5d 0a20 2020 2020  ": "ci" }].     
-00004bf0: 205d 2c0a 2020 2020 2020 2273 636f 7265   ],.      "score
-00004c00: 223a 2038 0a20 207d 2c0a 2020 2254 6572  ": 8.  },.  "Ter
-00004c10: 7261 666f 726d 223a 207b 0a20 2020 2020  raform": {.     
-00004c20: 2022 7479 7065 223a 2022 546f 6f6c 222c   "type": "Tool",
-00004c30: 0a20 2020 2020 2022 6361 7465 676f 7279  .      "category
-00004c40: 223a 2022 496e 6672 6173 7472 7563 7475  ": "Infrastructu
-00004c50: 7265 2061 7320 436f 6465 222c 0a20 2020  re as Code",.   
-00004c60: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00004c70: 3a20 2241 6e20 6f70 656e 2d73 6f75 7263  : "An open-sourc
-00004c80: 6520 746f 6f6c 2074 6861 7420 616c 6c6f  e tool that allo
-00004c90: 7773 2064 6576 656c 6f70 6572 7320 746f  ws developers to
-00004ca0: 2064 6566 696e 6520 616e 6420 7072 6f76   define and prov
-00004cb0: 6973 696f 6e20 6461 7461 2063 656e 7465  ision data cente
-00004cc0: 7220 696e 6672 6173 7472 7563 7475 7265  r infrastructure
-00004cd0: 2075 7369 6e67 2061 2064 6563 6c61 7261   using a declara
-00004ce0: 7469 7665 2063 6f6e 6669 6775 7261 7469  tive configurati
-00004cf0: 6f6e 206c 616e 6775 6167 652e 222c 0a20  on language.",. 
-00004d00: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
-00004d10: 205b 5b7b 2022 4c4f 5745 5222 3a20 7b20   [[{ "LOWER": { 
-00004d20: 2246 555a 5a59 3122 3a20 2274 6572 7261  "FUZZY1": "terra
-00004d30: 666f 726d 2220 7d20 7d5d 5d2c 0a20 2020  form" } }]],.   
-00004d40: 2020 2022 7363 6f72 6522 3a20 3130 0a20     "score": 10. 
-00004d50: 207d 2c0a 2020 2250 726f 6d65 7468 6575   },.  "Prometheu
-00004d60: 7322 3a20 7b0a 2020 2020 2020 2274 7970  s": {.      "typ
-00004d70: 6522 3a20 2254 6f6f 6c22 2c0a 2020 2020  e": "Tool",.    
-00004d80: 2020 2263 6174 6567 6f72 7922 3a20 224d    "category": "M
-00004d90: 6f6e 6974 6f72 696e 6722 2c0a 2020 2020  onitoring",.    
-00004da0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00004db0: 2022 416e 206f 7065 6e2d 736f 7572 6365   "An open-source
-00004dc0: 2073 7973 7465 6d73 206d 6f6e 6974 6f72   systems monitor
-00004dd0: 696e 6720 616e 6420 616c 6572 7469 6e67  ing and alerting
-00004de0: 2074 6f6f 6c6b 6974 206f 7269 6769 6e61   toolkit origina
-00004df0: 6c6c 7920 6275 696c 7420 6174 2053 6f75  lly built at Sou
-00004e00: 6e64 436c 6f75 642e 222c 0a20 2020 2020  ndCloud.",.     
-00004e10: 2022 7061 7474 6572 6e73 223a 205b 5b7b   "patterns": [[{
-00004e20: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
-00004e30: 5a59 3122 3a20 2270 726f 6d65 7468 6575  ZY1": "prometheu
-00004e40: 7322 207d 207d 5d5d 2c0a 2020 2020 2020  s" } }]],.      
-00004e50: 2273 636f 7265 223a 2039 0a20 207d 2c0a  "score": 9.  },.
-00004e60: 2020 2244 6f63 6b65 7222 3a20 7b0a 2020    "Docker": {.  
-00004e70: 2020 2020 2274 7970 6522 3a20 2244 6576      "type": "Dev
-00004e80: 4f70 7322 2c0a 2020 2020 2020 2263 6174  Ops",.      "cat
-00004e90: 6567 6f72 7922 3a20 2243 6f6e 7461 696e  egory": "Contain
-00004ea0: 6572 697a 6174 696f 6e22 2c0a 2020 2020  erization",.    
-00004eb0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00004ec0: 2022 446f 636b 6572 2069 7320 616e 206f   "Docker is an o
-00004ed0: 7065 6e20 706c 6174 666f 726d 2066 6f72  pen platform for
-00004ee0: 2064 6576 656c 6f70 696e 672c 2073 6869   developing, shi
-00004ef0: 7070 696e 672c 2061 6e64 2072 756e 6e69  pping, and runni
-00004f00: 6e67 2061 7070 6c69 6361 7469 6f6e 732e  ng applications.
-00004f10: 2044 6f63 6b65 7220 656e 6162 6c65 7320   Docker enables 
-00004f20: 796f 7520 746f 2073 6570 6172 6174 6520  you to separate 
-00004f30: 796f 7572 2061 7070 6c69 6361 7469 6f6e  your application
-00004f40: 7320 6672 6f6d 2079 6f75 7220 696e 6672  s from your infr
-00004f50: 6173 7472 7563 7475 7265 2073 6f20 796f  astructure so yo
-00004f60: 7520 6361 6e20 6465 6c69 7665 7220 736f  u can deliver so
-00004f70: 6674 7761 7265 2071 7569 636b 6c79 2e20  ftware quickly. 
-00004f80: 5769 7468 2044 6f63 6b65 722c 2079 6f75  With Docker, you
-00004f90: 2063 616e 206d 616e 6167 6520 796f 7572   can manage your
-00004fa0: 2069 6e66 7261 7374 7275 6374 7572 6520   infrastructure 
-00004fb0: 696e 2074 6865 2073 616d 6520 7761 7973  in the same ways
-00004fc0: 2079 6f75 206d 616e 6167 6520 796f 7572   you manage your
-00004fd0: 2061 7070 6c69 6361 7469 6f6e 732e 222c   applications.",
-00004fe0: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
-00004ff0: 223a 205b 5b7b 2022 4c4f 5745 5222 3a20  ": [[{ "LOWER": 
-00005000: 7b20 2246 555a 5a59 3122 3a20 2264 6f63  { "FUZZY1": "doc
-00005010: 6b65 7222 207d 207d 5d5d 2c0a 2020 2020  ker" } }]],.    
-00005020: 2020 2273 636f 7265 223a 2031 300a 2020    "score": 10.  
-00005030: 7d2c 0a20 2022 4b75 6265 726e 6574 6573  },.  "Kubernetes
-00005040: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
-00005050: 223a 2022 4465 764f 7073 222c 0a20 2020  ": "DevOps",.   
-00005060: 2020 2022 6361 7465 676f 7279 223a 2022     "category": "
-00005070: 436f 6e74 6169 6e65 7220 4f72 6368 6573  Container Orches
-00005080: 7472 6174 696f 6e22 2c0a 2020 2020 2020  tration",.      
-00005090: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000050a0: 4b75 6265 726e 6574 6573 2c20 616c 736f  Kubernetes, also
-000050b0: 206b 6e6f 776e 2061 7320 4b38 732c 2069   known as K8s, i
-000050c0: 7320 616e 206f 7065 6e2d 736f 7572 6365  s an open-source
-000050d0: 2073 7973 7465 6d20 666f 7220 6175 746f   system for auto
-000050e0: 6d61 7469 6e67 2064 6570 6c6f 796d 656e  mating deploymen
-000050f0: 742c 2073 6361 6c69 6e67 2c20 616e 6420  t, scaling, and 
-00005100: 6d61 6e61 6765 6d65 6e74 206f 6620 636f  management of co
-00005110: 6e74 6169 6e65 7269 7a65 6420 6170 706c  ntainerized appl
-00005120: 6963 6174 696f 6e73 2e20 4974 2067 726f  ications. It gro
-00005130: 7570 7320 636f 6e74 6169 6e65 7273 2074  ups containers t
-00005140: 6861 7420 6d61 6b65 2075 7020 616e 2061  hat make up an a
-00005150: 7070 6c69 6361 7469 6f6e 2069 6e74 6f20  pplication into 
-00005160: 6c6f 6769 6361 6c20 756e 6974 7320 666f  logical units fo
-00005170: 7220 6561 7379 206d 616e 6167 656d 656e  r easy managemen
-00005180: 7420 616e 6420 6469 7363 6f76 6572 792e  t and discovery.
-00005190: 222c 0a20 2020 2020 2022 7061 7474 6572  ",.      "patter
-000051a0: 6e73 223a 205b 0a20 2020 2020 2020 2020  ns": [.         
-000051b0: 205b 7b20 224c 4f57 4552 223a 207b 2022   [{ "LOWER": { "
-000051c0: 4655 5a5a 5931 223a 2022 6b75 6265 726e  FUZZY1": "kubern
-000051d0: 6574 6573 2220 7d20 7d5d 2c0a 2020 2020  etes" } }],.    
-000051e0: 2020 2020 2020 5b7b 2022 4c4f 5745 5222        [{ "LOWER"
-000051f0: 3a20 226b 3873 2220 7d5d 0a20 2020 2020  : "k8s" }].     
-00005200: 205d 2c0a 2020 2020 2020 2273 636f 7265   ],.      "score
-00005210: 223a 2031 300a 2020 7d2c 0a20 2022 4865  ": 10.  },.  "He
-00005220: 6c6d 223a 207b 0a20 2020 2020 2022 7479  lm": {.      "ty
-00005230: 7065 223a 2022 4465 764f 7073 222c 0a20  pe": "DevOps",. 
-00005240: 2020 2020 2022 6361 7465 676f 7279 223a       "category":
-00005250: 2022 4b75 6265 726e 6574 6573 2050 6163   "Kubernetes Pac
-00005260: 6b61 6765 204d 616e 6167 6572 222c 0a20  kage Manager",. 
-00005270: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00005280: 6e22 3a20 2248 656c 6d20 6973 2061 2070  n": "Helm is a p
-00005290: 6163 6b61 6765 206d 616e 6167 6572 2066  ackage manager f
-000052a0: 6f72 204b 7562 6572 6e65 7465 7320 7468  or Kubernetes th
-000052b0: 6174 2061 6c6c 6f77 7320 796f 7520 746f  at allows you to
-000052c0: 2064 6566 696e 652c 2069 6e73 7461 6c6c   define, install
-000052d0: 2c20 616e 6420 7570 6772 6164 6520 6576  , and upgrade ev
-000052e0: 656e 2074 6865 206d 6f73 7420 636f 6d70  en the most comp
-000052f0: 6c65 7820 4b75 6265 726e 6574 6573 2061  lex Kubernetes a
-00005300: 7070 6c69 6361 7469 6f6e 732e 222c 0a20  pplications.",. 
-00005310: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
-00005320: 205b 5b7b 2022 4c4f 5745 5222 3a20 7b20   [[{ "LOWER": { 
-00005330: 2246 555a 5a59 3122 3a20 2268 656c 6d22  "FUZZY1": "helm"
-00005340: 207d 207d 5d5d 2c0a 2020 2020 2020 2273   } }]],.      "s
-00005350: 636f 7265 223a 2039 0a20 207d 2c0a 2020  core": 9.  },.  
-00005360: 0a20 2022 4772 6170 6851 4c22 3a20 7b0a  .  "GraphQL": {.
-00005370: 2020 2020 2020 2274 7970 6522 3a20 2251        "type": "Q
-00005380: 7565 7279 204c 616e 6775 6167 6522 2c0a  uery Language",.
-00005390: 2020 2020 2020 2263 6174 6567 6f72 7922        "category"
-000053a0: 3a20 2241 5049 2044 6576 656c 6f70 6d65  : "API Developme
-000053b0: 6e74 222c 0a20 2020 2020 2022 6465 7363  nt",.      "desc
-000053c0: 7269 7074 696f 6e22 3a20 2247 7261 7068  ription": "Graph
-000053d0: 514c 2069 7320 6120 7175 6572 7920 6c61  QL is a query la
-000053e0: 6e67 7561 6765 2066 6f72 2041 5049 7320  nguage for APIs 
-000053f0: 616e 6420 6120 7275 6e74 696d 6520 666f  and a runtime fo
-00005400: 7220 6578 6563 7574 696e 6720 7468 6f73  r executing thos
-00005410: 6520 7175 6572 6965 7320 6279 2075 7369  e queries by usi
-00005420: 6e67 2061 2074 7970 6520 7379 7374 656d  ng a type system
-00005430: 2079 6f75 2064 6566 696e 6520 666f 7220   you define for 
-00005440: 796f 7572 2064 6174 612e 2047 7261 7068  your data. Graph
-00005450: 514c 2069 736e 2774 2074 6965 6420 746f  QL isn't tied to
-00005460: 2061 6e79 2073 7065 6369 6669 6320 6461   any specific da
-00005470: 7461 6261 7365 206f 7220 7374 6f72 6167  tabase or storag
-00005480: 6520 656e 6769 6e65 2061 6e64 2069 7320  e engine and is 
-00005490: 696e 7374 6561 6420 6261 636b 6564 2062  instead backed b
-000054a0: 7920 796f 7572 2065 7869 7374 696e 6720  y your existing 
-000054b0: 636f 6465 2061 6e64 2064 6174 612e 222c  code and data.",
-000054c0: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
-000054d0: 223a 205b 0a20 2020 2020 2020 2020 205b  ": [.          [
-000054e0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-000054f0: 5a5a 5931 223a 2022 6772 6170 6871 6c22  ZZY1": "graphql"
-00005500: 207d 207d 5d2c 0a20 2020 2020 2020 2020   } }],.         
-00005510: 205b 7b20 224c 4f57 4552 223a 2022 6771   [{ "LOWER": "gq
-00005520: 6c22 207d 5d0a 2020 2020 2020 5d2c 0a20  l" }].      ],. 
-00005530: 2020 2020 2022 7363 6f72 6522 3a20 370a       "score": 7.
-00005540: 2020 7d2c 0a20 2022 5465 6e73 6f72 466c    },.  "TensorFl
-00005550: 6f77 223a 207b 0a20 2020 2020 2022 7479  ow": {.      "ty
-00005560: 7065 223a 2022 4c69 6272 6172 7922 2c0a  pe": "Library",.
-00005570: 2020 2020 2020 2263 6174 6567 6f72 7922        "category"
-00005580: 3a20 224d 6163 6869 6e65 204c 6561 726e  : "Machine Learn
-00005590: 696e 6722 2c0a 2020 2020 2020 2264 6573  ing",.      "des
-000055a0: 6372 6970 7469 6f6e 223a 2022 5465 6e73  cription": "Tens
-000055b0: 6f72 466c 6f77 2069 7320 616e 2065 6e64  orFlow is an end
-000055c0: 2d74 6f2d 656e 6420 6f70 656e 2d73 6f75  -to-end open-sou
-000055d0: 7263 6520 706c 6174 666f 726d 2066 6f72  rce platform for
-000055e0: 206d 6163 6869 6e65 206c 6561 726e 696e   machine learnin
-000055f0: 672e 2049 7420 6861 7320 6120 636f 6d70  g. It has a comp
-00005600: 7265 6865 6e73 6976 652c 2066 6c65 7869  rehensive, flexi
-00005610: 626c 6520 6563 6f73 7973 7465 6d20 6f66  ble ecosystem of
-00005620: 2074 6f6f 6c73 2c20 6c69 6272 6172 6965   tools, librarie
-00005630: 732c 2061 6e64 2063 6f6d 6d75 6e69 7479  s, and community
-00005640: 2072 6573 6f75 7263 6573 2074 6861 7420   resources that 
-00005650: 6c65 7473 2072 6573 6561 7263 6865 7273  lets researchers
-00005660: 2070 7573 6820 7468 6520 7374 6174 652d   push the state-
-00005670: 6f66 2d74 6865 2d61 7274 2069 6e20 4d4c  of-the-art in ML
-00005680: 2061 6e64 2064 6576 656c 6f70 6572 7320   and developers 
-00005690: 6561 7369 6c79 2062 7569 6c64 2061 6e64  easily build and
-000056a0: 2064 6570 6c6f 7920 4d4c 2d70 6f77 6572   deploy ML-power
-000056b0: 6564 2061 7070 6c69 6361 7469 6f6e 732e  ed applications.
-000056c0: 222c 0a20 2020 2020 2022 7061 7474 6572  ",.      "patter
-000056d0: 6e73 223a 205b 0a20 2020 2020 2020 2020  ns": [.         
-000056e0: 205b 7b20 224c 4f57 4552 223a 207b 2022   [{ "LOWER": { "
-000056f0: 4655 5a5a 5931 223a 2022 7465 6e7a 666c  FUZZY1": "tenzfl
-00005700: 6f77 2220 7d20 7d5d 2c0a 2020 2020 2020  ow" } }],.      
-00005710: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
-00005720: 7b20 2246 555a 5a59 3122 3a20 2274 656e  { "FUZZY1": "ten
-00005730: 736f 7266 6c6f 7722 207d 207d 5d0a 2020  sorflow" } }].  
-00005740: 2020 2020 5d2c 0a20 2020 2020 2022 7363      ],.      "sc
-00005750: 6f72 6522 3a20 3130 0a20 207d 2c0a 2020  ore": 10.  },.  
-00005760: 2250 7954 6f72 6368 223a 207b 0a20 2020  "PyTorch": {.   
-00005770: 2020 2022 7479 7065 223a 2022 4c69 6272     "type": "Libr
-00005780: 6172 7922 2c0a 2020 2020 2020 2263 6174  ary",.      "cat
-00005790: 6567 6f72 7922 3a20 224d 6163 6869 6e65  egory": "Machine
-000057a0: 204c 6561 726e 696e 6722 2c0a 2020 2020   Learning",.    
-000057b0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000057c0: 2022 5079 546f 7263 6820 6973 2061 6e20   "PyTorch is an 
-000057d0: 6f70 656e 2d73 6f75 7263 6520 6d61 6368  open-source mach
-000057e0: 696e 6520 6c65 6172 6e69 6e67 206c 6962  ine learning lib
-000057f0: 7261 7279 2062 6173 6564 206f 6e20 7468  rary based on th
-00005800: 6520 546f 7263 6820 6c69 6272 6172 792c  e Torch library,
-00005810: 2075 7365 6420 666f 7220 6170 706c 6963   used for applic
-00005820: 6174 696f 6e73 2073 7563 6820 6173 2063  ations such as c
-00005830: 6f6d 7075 7465 7220 7669 7369 6f6e 2061  omputer vision a
-00005840: 6e64 206e 6174 7572 616c 206c 616e 6775  nd natural langu
-00005850: 6167 6520 7072 6f63 6573 7369 6e67 2c20  age processing, 
-00005860: 7072 696d 6172 696c 7920 6465 7665 6c6f  primarily develo
-00005870: 7065 6420 6279 2046 6163 6562 6f6f 6b27  ped by Facebook'
-00005880: 7320 4149 2052 6573 6561 7263 6820 6c61  s AI Research la
-00005890: 6220 2846 4149 5229 2e22 2c0a 2020 2020  b (FAIR).",.    
-000058a0: 2020 2270 6174 7465 726e 7322 3a20 5b5b    "patterns": [[
-000058b0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-000058c0: 5a5a 5931 223a 2022 7079 746f 7263 6822  ZZY1": "pytorch"
-000058d0: 207d 207d 5d5d 2c0a 2020 2020 2020 2273   } }]],.      "s
-000058e0: 636f 7265 223a 2031 300a 2020 7d2c 0a20  core": 10.  },. 
-000058f0: 2022 5363 696b 6974 2d6c 6561 726e 223a   "Scikit-learn":
-00005900: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
-00005910: 2022 4c69 6272 6172 7922 2c0a 2020 2020   "Library",.    
-00005920: 2020 2263 6174 6567 6f72 7922 3a20 224d    "category": "M
-00005930: 6163 6869 6e65 204c 6561 726e 696e 6722  achine Learning"
-00005940: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
-00005950: 7469 6f6e 223a 2022 5363 696b 6974 2d6c  tion": "Scikit-l
-00005960: 6561 726e 2069 7320 6120 6672 6565 2073  earn is a free s
-00005970: 6f66 7477 6172 6520 6d61 6368 696e 6520  oftware machine 
-00005980: 6c65 6172 6e69 6e67 206c 6962 7261 7279  learning library
-00005990: 2066 6f72 2074 6865 2050 7974 686f 6e20   for the Python 
-000059a0: 7072 6f67 7261 6d6d 696e 6720 6c61 6e67  programming lang
-000059b0: 7561 6765 2e20 4974 2066 6561 7475 7265  uage. It feature
-000059c0: 7320 7661 7269 6f75 7320 636c 6173 7369  s various classi
-000059d0: 6669 6361 7469 6f6e 2c20 7265 6772 6573  fication, regres
-000059e0: 7369 6f6e 2c20 616e 6420 636c 7573 7465  sion, and cluste
-000059f0: 7269 6e67 2061 6c67 6f72 6974 686d 7320  ring algorithms 
-00005a00: 696e 636c 7564 696e 6720 7375 7070 6f72  including suppor
-00005a10: 7420 7665 6374 6f72 206d 6163 6869 6e65  t vector machine
-00005a20: 732c 2072 616e 646f 6d20 666f 7265 7374  s, random forest
-00005a30: 732c 2067 7261 6469 656e 7420 626f 6f73  s, gradient boos
-00005a40: 7469 6e67 2c20 6b2d 6d65 616e 732c 2061  ting, k-means, a
-00005a50: 6e64 2044 4253 4341 4e2e 222c 0a20 2020  nd DBSCAN.",.   
-00005a60: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
-00005a70: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
-00005a80: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
-00005a90: 223a 2022 7363 696b 6974 2d6c 6561 726e  ": "scikit-learn
-00005aa0: 2220 7d20 7d5d 2c0a 2020 2020 2020 2020  " } }],.        
-00005ab0: 2020 5b7b 2022 4c4f 5745 5222 3a20 7b20    [{ "LOWER": { 
-00005ac0: 2246 555a 5a59 3122 3a20 2273 6b6c 6561  "FUZZY1": "sklea
-00005ad0: 726e 2220 7d20 7d5d 0a20 2020 2020 205d  rn" } }].      ]
-00005ae0: 2c0a 2020 2020 2020 2273 636f 7265 223a  ,.      "score":
-00005af0: 2039 0a20 207d 2c0a 2020 2241 7061 6368   9.  },.  "Apach
-00005b00: 6520 4b61 666b 6122 3a20 7b0a 2020 2020  e Kafka": {.    
-00005b10: 2020 2274 7970 6522 3a20 2242 6967 2044    "type": "Big D
-00005b20: 6174 6120 546f 6f6c 222c 0a20 2020 2020  ata Tool",.     
-00005b30: 2022 6361 7465 676f 7279 223a 2022 4d65   "category": "Me
-00005b40: 7373 6167 6520 5374 7265 616d 696e 6722  ssage Streaming"
-00005b50: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
-00005b60: 7469 6f6e 223a 2022 4170 6163 6865 204b  tion": "Apache K
-00005b70: 6166 6b61 2069 7320 616e 206f 7065 6e2d  afka is an open-
-00005b80: 736f 7572 6365 2073 7472 6561 6d2d 7072  source stream-pr
-00005b90: 6f63 6573 7369 6e67 2073 6f66 7477 6172  ocessing softwar
-00005ba0: 6520 706c 6174 666f 726d 2064 6576 656c  e platform devel
-00005bb0: 6f70 6564 2062 7920 4c69 6e6b 6564 496e  oped by LinkedIn
-00005bc0: 2061 6e64 2064 6f6e 6174 6564 2074 6f20   and donated to 
-00005bd0: 7468 6520 4170 6163 6865 2053 6f66 7477  the Apache Softw
-00005be0: 6172 6520 466f 756e 6461 7469 6f6e 2c20  are Foundation, 
-00005bf0: 7772 6974 7465 6e20 696e 2053 6361 6c61  written in Scala
-00005c00: 2061 6e64 204a 6176 612e 2054 6865 2070   and Java. The p
-00005c10: 726f 6a65 6374 2061 696d 7320 746f 2070  roject aims to p
-00005c20: 726f 7669 6465 2061 2075 6e69 6669 6564  rovide a unified
-00005c30: 2c20 6869 6768 2d74 6872 6f75 6768 7075  , high-throughpu
-00005c40: 742c 206c 6f77 2d6c 6174 656e 6379 2070  t, low-latency p
-00005c50: 6c61 7466 6f72 6d20 666f 7220 6861 6e64  latform for hand
-00005c60: 6c69 6e67 2072 6561 6c2d 7469 6d65 2064  ling real-time d
-00005c70: 6174 6120 6665 6564 732e 222c 0a20 2020  ata feeds.",.   
-00005c80: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
-00005c90: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
-00005ca0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
-00005cb0: 223a 2022 6170 6163 6865 206b 6166 6b61  ": "apache kafka
-00005cc0: 2220 7d20 7d5d 2c0a 2020 2020 2020 2020  " } }],.        
-00005cd0: 2020 5b7b 2022 4c4f 5745 5222 3a20 7b20    [{ "LOWER": { 
-00005ce0: 2246 555a 5a59 3122 3a20 226b 6166 6b61  "FUZZY1": "kafka
-00005cf0: 2220 7d20 7d5d 0a20 2020 2020 205d 2c0a  " } }].      ],.
-00005d00: 2020 2020 2020 2273 636f 7265 223a 2039        "score": 9
-00005d10: 0a20 207d 2c0a 2020 2252 6162 6269 744d  .  },.  "RabbitM
-00005d20: 5122 3a20 7b0a 2020 2020 2020 2274 7970  Q": {.      "typ
-00005d30: 6522 3a20 224d 6964 646c 6577 6172 6522  e": "Middleware"
-00005d40: 2c0a 2020 2020 2020 2263 6174 6567 6f72  ,.      "categor
-00005d50: 7922 3a20 224d 6573 7361 6765 2042 726f  y": "Message Bro
-00005d60: 6b65 7222 2c0a 2020 2020 2020 2264 6573  ker",.      "des
-00005d70: 6372 6970 7469 6f6e 223a 2022 5261 6262  cription": "Rabb
-00005d80: 6974 4d51 2069 7320 616e 206f 7065 6e2d  itMQ is an open-
-00005d90: 736f 7572 6365 206d 6573 7361 6765 2d62  source message-b
-00005da0: 726f 6b65 7220 736f 6674 7761 7265 2074  roker software t
-00005db0: 6861 7420 6f72 6967 696e 616c 6c79 2069  hat originally i
-00005dc0: 6d70 6c65 6d65 6e74 6564 2074 6865 2041  mplemented the A
-00005dd0: 6476 616e 6365 6420 4d65 7373 6167 6520  dvanced Message 
-00005de0: 5175 6575 696e 6720 5072 6f74 6f63 6f6c  Queuing Protocol
-00005df0: 2028 414d 5150 2920 616e 6420 6861 7320   (AMQP) and has 
-00005e00: 7369 6e63 6520 6265 656e 2065 7874 656e  since been exten
-00005e10: 6465 6420 7769 7468 2061 2070 6c75 672d  ded with a plug-
-00005e20: 696e 2061 7263 6869 7465 6374 7572 6520  in architecture 
-00005e30: 746f 2073 7570 706f 7274 2053 7472 6561  to support Strea
-00005e40: 6d69 6e67 2054 6578 7420 4f72 6965 6e74  ming Text Orient
-00005e50: 6564 204d 6573 7361 6769 6e67 2050 726f  ed Messaging Pro
-00005e60: 746f 636f 6c20 2853 544f 4d50 292c 204d  tocol (STOMP), M
-00005e70: 5154 542c 2061 6e64 206f 7468 6572 2070  QTT, and other p
-00005e80: 726f 746f 636f 6c73 2e22 2c0a 2020 2020  rotocols.",.    
-00005e90: 2020 2270 6174 7465 726e 7322 3a20 5b5b    "patterns": [[
-00005ea0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-00005eb0: 5a5a 5931 223a 2022 7261 6262 6974 6d71  ZZY1": "rabbitmq
-00005ec0: 2220 7d20 7d5d 5d2c 0a20 2020 2020 2022  " } }]],.      "
-00005ed0: 7363 6f72 6522 3a20 382e 350a 2020 7d2c  score": 8.5.  },
-00005ee0: 0a20 2022 4861 646f 6f70 223a 207b 0a20  .  "Hadoop": {. 
-00005ef0: 2020 2020 2022 7479 7065 223a 2022 4672       "type": "Fr
-00005f00: 616d 6577 6f72 6b22 2c0a 2020 2020 2020  amework",.      
-00005f10: 2263 6174 6567 6f72 7922 3a20 2242 6967  "category": "Big
-00005f20: 2044 6174 6120 5072 6f63 6573 7369 6e67   Data Processing
-00005f30: 222c 0a20 2020 2020 2022 6465 7363 7269  ",.      "descri
-00005f40: 7074 696f 6e22 3a20 2241 7061 6368 6520  ption": "Apache 
-00005f50: 4861 646f 6f70 2069 7320 6120 636f 6c6c  Hadoop is a coll
-00005f60: 6563 7469 6f6e 206f 6620 6f70 656e 2d73  ection of open-s
-00005f70: 6f75 7263 6520 736f 6674 7761 7265 2075  ource software u
-00005f80: 7469 6c69 7469 6573 2074 6861 7420 6661  tilities that fa
-00005f90: 6369 6c69 7461 7465 2075 7369 6e67 2061  cilitate using a
-00005fa0: 206e 6574 776f 726b 206f 6620 6d61 6e79   network of many
-00005fb0: 2063 6f6d 7075 7465 7273 2074 6f20 736f   computers to so
-00005fc0: 6c76 6520 7072 6f62 6c65 6d73 2069 6e76  lve problems inv
-00005fd0: 6f6c 7669 6e67 206d 6173 7369 7665 2061  olving massive a
-00005fe0: 6d6f 756e 7473 206f 6620 6461 7461 2061  mounts of data a
-00005ff0: 6e64 2063 6f6d 7075 7461 7469 6f6e 2e20  nd computation. 
-00006000: 4974 2070 726f 7669 6465 7320 6120 736f  It provides a so
-00006010: 6674 7761 7265 2066 7261 6d65 776f 726b  ftware framework
-00006020: 2066 6f72 2064 6973 7472 6962 7574 6564   for distributed
-00006030: 2073 746f 7261 6765 2061 6e64 2070 726f   storage and pro
-00006040: 6365 7373 696e 6720 6f66 2062 6967 2064  cessing of big d
-00006050: 6174 6120 7573 696e 6720 7468 6520 4d61  ata using the Ma
-00006060: 7052 6564 7563 6520 7072 6f67 7261 6d6d  pReduce programm
-00006070: 696e 6720 6d6f 6465 6c2e 222c 0a20 2020  ing model.",.   
-00006080: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
-00006090: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
-000060a0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
-000060b0: 223a 2022 6170 6163 6865 2068 6164 6f6f  ": "apache hadoo
-000060c0: 7022 207d 207d 5d2c 0a20 2020 2020 2020  p" } }],.       
-000060d0: 2020 205b 7b20 224c 4f57 4552 223a 207b     [{ "LOWER": {
-000060e0: 2022 4655 5a5a 5931 223a 2022 6861 646f   "FUZZY1": "hado
-000060f0: 6f70 2220 7d20 7d5d 0a20 2020 2020 205d  op" } }].      ]
-00006100: 2c0a 2020 2020 2020 2273 636f 7265 223a  ,.      "score":
-00006110: 2038 0a20 207d 2c0a 2020 0a20 2022 5573   8.  },.  .  "Us
-00006120: 6572 2049 6e74 6572 6661 6365 223a 207b  er Interface": {
-00006130: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-00006140: 4672 6f6e 7465 6e64 222c 0a20 2020 2020  Frontend",.     
-00006150: 2022 6361 7465 676f 7279 223a 2022 5265   "category": "Re
-00006160: 7175 6972 656d 656e 7422 2c0a 2020 2020  quirement",.    
-00006170: 2020 2272 656c 6174 6564 5465 6368 6e6f    "relatedTechno
-00006180: 6c6f 6769 6573 223a 205b 0a20 2020 2020  logies": [.     
-00006190: 2020 2020 2022 5675 6522 2c0a 2020 2020       "Vue",.    
-000061a0: 2020 2020 2020 2252 6561 6374 222c 0a20        "React",. 
-000061b0: 2020 2020 2020 2020 2022 416e 6775 6c61           "Angula
-000061c0: 7222 2c0a 2020 2020 2020 2020 2020 2242  r",.          "B
-000061d0: 6f6f 7473 7472 6170 222c 0a20 2020 2020  ootstrap",.     
-000061e0: 2020 2020 2022 4d61 7465 7269 616c 2d55       "Material-U
-000061f0: 4922 2c0a 2020 2020 2020 2020 2020 2254  I",.          "T
-00006200: 6169 6c77 696e 6420 4353 5322 0a20 2020  ailwind CSS".   
-00006210: 2020 205d 2c0a 2020 2020 2020 2270 6174     ],.      "pat
-00006220: 7465 726e 7322 3a20 5b0a 2020 2020 2020  terns": [.      
-00006230: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
-00006240: 2275 6922 207d 5d2c 0a20 2020 2020 2020  "ui" }],.       
-00006250: 2020 205b 7b20 224c 4f57 4552 223a 2022     [{ "LOWER": "
-00006260: 7573 6572 2220 7d2c 207b 2022 4c4f 5745  user" }, { "LOWE
-00006270: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
-00006280: 2269 6e74 6572 6661 6365 2220 7d20 7d5d  "interface" } }]
-00006290: 2c0a 2020 2020 2020 2020 2020 5b7b 2022  ,.          [{ "
-000062a0: 4c4f 5745 5222 3a20 7b20 2246 555a 5a59  LOWER": { "FUZZY
-000062b0: 3122 3a20 2272 6573 706f 6e73 6976 6522  1": "responsive"
-000062c0: 207d 207d 5d0a 2020 2020 2020 5d2c 0a20   } }].      ],. 
-000062d0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000062e0: 6e22 3a20 2252 6566 6572 7320 746f 2074  n": "Refers to t
-000062f0: 6865 2064 6573 6967 6e20 616e 6420 6c61  he design and la
-00006300: 796f 7574 206f 6620 7468 6520 696e 7465  yout of the inte
-00006310: 7266 6163 6520 7468 726f 7567 6820 7768  rface through wh
-00006320: 6963 6820 7573 6572 7320 696e 7465 7261  ich users intera
-00006330: 6374 2077 6974 6820 7765 6220 6170 706c  ct with web appl
-00006340: 6963 6174 696f 6e73 2e20 5468 6973 2074  ications. This t
-00006350: 7970 6963 616c 6c79 2069 6e76 6f6c 7665  ypically involve
-00006360: 7320 7465 6368 6e6f 6c6f 6769 6573 2066  s technologies f
-00006370: 6f72 2062 7569 6c64 696e 6720 7573 6572  or building user
-00006380: 2069 6e74 6572 6661 6365 732c 2073 7563   interfaces, suc
-00006390: 6820 6173 204a 6176 6153 6372 6970 7420  h as JavaScript 
-000063a0: 6672 616d 6577 6f72 6b73 2f6c 6962 7261  frameworks/libra
-000063b0: 7269 6573 2061 6e64 2055 4920 636f 6d70  ries and UI comp
-000063c0: 6f6e 656e 7420 6c69 6272 6172 6965 732e  onent libraries.
-000063d0: 222c 0a20 2020 2020 2022 7363 6f72 6522  ",.      "score"
-000063e0: 3a20 350a 2020 7d2c 0a20 2022 5245 5354  : 5.  },.  "REST
-000063f0: 2041 5049 2044 6576 656c 6f70 6d65 6e74   API Development
-00006400: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
-00006410: 223a 2022 4150 4920 4465 7369 676e 222c  ": "API Design",
-00006420: 0a20 2020 2020 2022 6361 7465 676f 7279  .      "category
-00006430: 223a 2022 5265 7175 6972 656d 656e 7422  ": "Requirement"
-00006440: 2c0a 2020 2020 2020 2272 656c 6174 6564  ,.      "related
-00006450: 5465 6368 6e6f 6c6f 6769 6573 223a 205b  Technologies": [
-00006460: 0a20 2020 2020 2020 2020 2022 4578 7072  .          "Expr
-00006470: 6573 732e 6a73 222c 0a20 2020 2020 2020  ess.js",.       
-00006480: 2020 2022 4661 7374 4150 4922 2c0a 2020     "FastAPI",.  
-00006490: 2020 2020 2020 2020 2244 6a61 6e67 6f22          "Django"
-000064a0: 2c0a 2020 2020 2020 2020 2020 2246 6c61  ,.          "Fla
-000064b0: 736b 222c 0a20 2020 2020 2020 2020 2022  sk",.          "
-000064c0: 4153 502e 4e45 5422 2c0a 2020 2020 2020  ASP.NET",.      
-000064d0: 2020 2020 2253 7072 696e 6722 0a20 2020      "Spring".   
-000064e0: 2020 205d 2c0a 2020 2020 2020 2270 6174     ],.      "pat
-000064f0: 7465 726e 7322 3a20 5b0a 2020 2020 2020  terns": [.      
-00006500: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
-00006510: 7b20 2246 555a 5a59 3122 3a20 2272 6573  { "FUZZY1": "res
-00006520: 7466 756c 2220 7d20 7d5d 2c0a 2020 2020  tful" } }],.    
-00006530: 2020 2020 2020 5b7b 2022 4c4f 5745 5222        [{ "LOWER"
-00006540: 3a20 2272 6573 7422 207d 2c20 7b20 224c  : "rest" }, { "L
-00006550: 4f57 4552 223a 2022 6170 6922 207d 5d2c  OWER": "api" }],
-00006560: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
-00006570: 4f57 4552 223a 2022 7265 7374 2220 7d5d  OWER": "rest" }]
-00006580: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00006590: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000065a0: 5468 6520 7072 6f63 6573 7320 6f66 2064  The process of d
-000065b0: 6576 656c 6f70 696e 6720 6170 706c 6963  eveloping applic
-000065c0: 6174 696f 6e20 7072 6f67 7261 6d6d 696e  ation programmin
-000065d0: 6720 696e 7465 7266 6163 6573 2028 4150  g interfaces (AP
-000065e0: 4973 2920 666f 6c6c 6f77 696e 6720 7468  Is) following th
-000065f0: 6520 5265 7072 6573 656e 7461 7469 6f6e  e Representation
-00006600: 616c 2053 7461 7465 2054 7261 6e73 6665  al State Transfe
-00006610: 7220 2852 4553 5429 2061 7263 6869 7465  r (REST) archite
-00006620: 6374 7572 616c 2073 7479 6c65 2c20 656e  ctural style, en
-00006630: 6162 6c69 6e67 2063 6f6d 6d75 6e69 6361  abling communica
-00006640: 7469 6f6e 2062 6574 7765 656e 2064 6966  tion between dif
-00006650: 6665 7265 6e74 2073 6f66 7477 6172 6520  ferent software 
-00006660: 6170 706c 6963 6174 696f 6e73 2e22 2c0a  applications.",.
-00006670: 2020 2020 2020 2273 636f 7265 223a 2035        "score": 5
-00006680: 0a20 207d 2c0a 2020 2252 4442 4d53 223a  .  },.  "RDBMS":
-00006690: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
-000066a0: 2022 5265 6c61 7469 6f6e 616c 2044 6174   "Relational Dat
-000066b0: 6162 6173 6520 4d6f 6465 6c22 2c0a 2020  abase Model",.  
-000066c0: 2020 2020 2263 6174 6567 6f72 7922 3a20      "category": 
-000066d0: 2252 6571 7569 7265 6d65 6e74 222c 0a20  "Requirement",. 
-000066e0: 2020 2020 2022 7265 6c61 7465 6454 6563       "relatedTec
-000066f0: 686e 6f6c 6f67 6965 7322 3a20 5b22 4d79  hnologies": ["My
-00006700: 5351 4c22 2c20 2250 6f73 7467 7265 5351  SQL", "PostgreSQ
-00006710: 4c22 2c20 224d 6172 6961 4442 222c 2022  L", "MariaDB", "
-00006720: 4f72 6163 6c65 4442 225d 2c0a 2020 2020  OracleDB"],.    
-00006730: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00006740: 2022 4120 7479 7065 206f 6620 6461 7461   "A type of data
-00006750: 6261 7365 2073 7973 7465 6d20 7468 6174  base system that
-00006760: 2073 746f 7265 7320 6461 7461 2069 6e20   stores data in 
-00006770: 7461 626c 6573 2c20 6f72 6761 6e69 7a65  tables, organize
-00006780: 6420 6279 2072 6f77 7320 616e 6420 636f  d by rows and co
-00006790: 6c75 6d6e 732c 2066 6f6c 6c6f 7769 6e67  lumns, following
-000067a0: 2074 6865 2072 656c 6174 696f 6e61 6c20   the relational 
-000067b0: 6d6f 6465 6c2e 2052 4442 4d53 2070 726f  model. RDBMS pro
-000067c0: 7669 6465 7320 6120 7374 7275 6374 7572  vides a structur
-000067d0: 6564 2061 7070 726f 6163 6820 746f 206d  ed approach to m
-000067e0: 616e 6167 696e 6720 6461 7461 2c20 656e  anaging data, en
-000067f0: 7375 7269 6e67 2069 6e74 6567 7269 7479  suring integrity
-00006800: 2061 6e64 2063 6f6e 7369 7374 656e 6379   and consistency
-00006810: 2074 6872 6f75 6768 2041 4349 4420 7072   through ACID pr
-00006820: 6f70 6572 7469 6573 2e22 2c0a 2020 2020  operties.",.    
-00006830: 2020 2270 6174 7465 726e 7322 3a20 5b0a    "patterns": [.
-00006840: 2020 2020 2020 2020 2020 5b7b 2022 4c4f            [{ "LO
-00006850: 5745 5222 3a20 7b20 2246 555a 5a59 3122  WER": { "FUZZY1"
-00006860: 3a20 2272 656c 6174 696f 6e61 6c22 207d  : "relational" }
-00006870: 207d 2c20 7b20 224c 4f57 4552 223a 207b   }, { "LOWER": {
-00006880: 2022 4655 5a5a 5931 223a 2022 6461 7461   "FUZZY1": "data
-00006890: 6261 7365 2220 7d20 7d5d 2c0a 2020 2020  base" } }],.    
-000068a0: 2020 2020 2020 5b7b 2022 4c4f 5745 5222        [{ "LOWER"
-000068b0: 3a20 7b20 2246 555a 5a59 3122 3a20 2272  : { "FUZZY1": "r
-000068c0: 656c 6174 696f 6e61 6c22 207d 207d 2c20  elational" } }, 
-000068d0: 7b20 224c 4f57 4552 223a 2022 6462 2220  { "LOWER": "db" 
-000068e0: 7d5d 2c0a 2020 2020 2020 2020 2020 5b7b  }],.          [{
-000068f0: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
-00006900: 5a59 3122 3a20 2272 6462 6d73 2220 7d20  ZY1": "rdbms" } 
-00006910: 7d5d 2c0a 2020 2020 2020 2020 2020 5b7b  }],.          [{
-00006920: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
-00006930: 5a59 3122 3a20 2272 656c 6174 696f 6e61  ZY1": "relationa
-00006940: 6c22 207d 207d 5d0a 2020 2020 2020 5d2c  l" } }].      ],
-00006950: 0a20 2020 2020 2022 7363 6f72 6522 3a20  .      "score": 
-00006960: 350a 2020 7d2c 0a20 2022 4e6f 5351 4c22  5.  },.  "NoSQL"
-00006970: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
-00006980: 3a20 224e 6f6e 2d52 656c 6174 696f 6e61  : "Non-Relationa
-00006990: 6c20 4461 7461 6261 7365 204d 6f64 656c  l Database Model
-000069a0: 222c 0a20 2020 2020 2022 6361 7465 676f  ",.      "catego
-000069b0: 7279 223a 2022 5265 7175 6972 656d 656e  ry": "Requiremen
-000069c0: 7422 2c0a 2020 2020 2020 2272 656c 6174  t",.      "relat
-000069d0: 6564 5465 6368 6e6f 6c6f 6769 6573 223a  edTechnologies":
-000069e0: 205b 224d 6f6e 676f 4442 222c 2022 4170   ["MongoDB", "Ap
-000069f0: 6163 6865 2043 6173 7361 6e64 7261 225d  ache Cassandra"]
-00006a00: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
-00006a10: 7469 6f6e 223a 2022 4120 636f 6c6c 6563  tion": "A collec
-00006a20: 7469 6f6e 206f 6620 6e6f 6e2d 7265 6c61  tion of non-rela
-00006a30: 7469 6f6e 616c 2064 6174 6120 6d6f 6465  tional data mode
-00006a40: 6c73 2074 6861 7420 646f 206e 6f74 2066  ls that do not f
-00006a50: 6f6c 6c6f 7720 7468 6520 7472 6164 6974  ollow the tradit
-00006a60: 696f 6e61 6c20 7461 6275 6c61 7220 7363  ional tabular sc
-00006a70: 6865 6d61 2c20 656d 7068 6173 697a 696e  hema, emphasizin
-00006a80: 6720 7363 616c 6162 696c 6974 792c 2061  g scalability, a
-00006a90: 6769 6c69 7479 2c20 616e 6420 6164 6170  gility, and adap
-00006aa0: 7461 6269 6c69 7479 2e20 4e6f 5351 4c20  tability. NoSQL 
-00006ab0: 6461 7461 6261 7365 7320 6172 6520 6465  databases are de
-00006ac0: 7369 676e 6564 2074 6f20 6861 6e64 6c65  signed to handle
-00006ad0: 206c 6172 6765 2076 6f6c 756d 6573 206f   large volumes o
-00006ae0: 6620 756e 7374 7275 6374 7572 6564 206f  f unstructured o
-00006af0: 7220 7365 6d69 2d73 7472 7563 7475 7265  r semi-structure
-00006b00: 6420 6461 7461 2e22 2c0a 2020 2020 2020  d data.",.      
-00006b10: 2270 6174 7465 726e 7322 3a20 5b0a 2020  "patterns": [.  
-00006b20: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
-00006b30: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
-00006b40: 226e 6f73 716c 2220 7d20 7d5d 2c0a 2020  "nosql" } }],.  
-00006b50: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
-00006b60: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
-00006b70: 226e 6f6e 2d72 656c 6174 696f 6e61 6c22  "non-relational"
-00006b80: 207d 207d 2c20 7b20 224c 4f57 4552 223a   } }, { "LOWER":
-00006b90: 207b 2022 4655 5a5a 5931 223a 2022 6461   { "FUZZY1": "da
-00006ba0: 7461 6261 7365 2220 7d20 7d5d 0a20 2020  tabase" } }].   
-00006bb0: 2020 205d 2c0a 2020 2020 2020 2273 636f     ],.      "sco
-00006bc0: 7265 223a 2035 0a20 207d 2c0a 2020 0a20  re": 5.  },.  . 
-00006bd0: 2022 436c 6f75 6420 4465 706c 6f79 6d65   "Cloud Deployme
-00006be0: 6e74 223a 207b 0a20 2020 2020 2022 7479  nt": {.      "ty
-00006bf0: 7065 223a 2022 4465 706c 6f79 6d65 6e74  pe": "Deployment
-00006c00: 222c 0a20 2020 2020 2022 6361 7465 676f  ",.      "catego
-00006c10: 7279 223a 2022 5265 7175 6972 656d 656e  ry": "Requiremen
-00006c20: 7422 2c0a 2020 2020 2020 2272 656c 6174  t",.      "relat
-00006c30: 6564 5465 6368 6e6f 6c6f 6769 6573 223a  edTechnologies":
-00006c40: 205b 2241 5753 222c 2022 417a 7572 6522   ["AWS", "Azure"
-00006c50: 2c20 2247 6f6f 676c 6543 6c6f 7564 225d  , "GoogleCloud"]
-00006c60: 2c0a 2020 2020 2020 2270 6174 7465 726e  ,.      "pattern
-00006c70: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-00006c80: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
-00006c90: 555a 5a59 3122 3a20 2263 6c6f 7564 2220  UZZY1": "cloud" 
-00006ca0: 7d7d 2c20 7b20 224c 4f57 4552 223a 207b  }}, { "LOWER": {
-00006cb0: 2022 4655 5a5a 5931 223a 2022 6465 706c   "FUZZY1": "depl
-00006cc0: 6f79 6d65 6e74 2220 7d20 7d5d 2c0a 2020  oyment" } }],.  
-00006cd0: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
-00006ce0: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
-00006cf0: 2263 6c6f 7564 2220 7d7d 2c20 7b20 224c  "cloud" }}, { "L
-00006d00: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
-00006d10: 223a 2022 7072 6f76 6964 6572 2220 7d20  ": "provider" } 
-00006d20: 7d5d 0a20 2020 2020 205d 2c0a 2020 2020  }].      ],.    
-00006d30: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00006d40: 2022 5468 6520 7072 6f63 6573 7320 6f66   "The process of
-00006d50: 2064 6570 6c6f 7969 6e67 2061 7070 6c69   deploying appli
-00006d60: 6361 7469 6f6e 732c 2073 6572 7669 6365  cations, service
-00006d70: 732c 206f 7220 7265 736f 7572 6365 7320  s, or resources 
-00006d80: 6f6e 2061 2063 6c6f 7564 2070 6c61 7466  on a cloud platf
-00006d90: 6f72 6d20 7072 6f76 6964 6564 2062 7920  orm provided by 
-00006da0: 6120 636c 6f75 6420 7365 7276 6963 6520  a cloud service 
-00006db0: 7072 6f76 6964 6572 2e20 436c 6f75 6420  provider. Cloud 
-00006dc0: 6465 706c 6f79 6d65 6e74 206f 6666 6572  deployment offer
-00006dd0: 7320 7363 616c 6162 696c 6974 792c 2066  s scalability, f
-00006de0: 6c65 7869 6269 6c69 7479 2c20 616e 6420  lexibility, and 
-00006df0: 7265 6475 6365 6420 696e 6672 6173 7472  reduced infrastr
-00006e00: 7563 7475 7265 206d 6169 6e74 656e 616e  ucture maintenan
-00006e10: 6365 2e22 2c0a 2020 2020 2020 2273 636f  ce.",.      "sco
-00006e20: 7265 223a 2035 0a20 207d 2c0a 2020 2256  re": 5.  },.  "V
-00006e30: 6572 7369 6f6e 2043 6f6e 7472 6f6c 2053  ersion Control S
-00006e40: 7973 7465 6d22 3a20 7b0a 2020 2020 2020  ystem": {.      
-00006e50: 2274 7970 6522 3a20 2244 6576 4f70 7320  "type": "DevOps 
-00006e60: 5072 6163 7469 6365 7322 2c0a 2020 2020  Practices",.    
-00006e70: 2020 2263 6174 6567 6f72 7922 3a20 2252    "category": "R
-00006e80: 6571 7569 7265 6d65 6e74 222c 0a20 2020  equirement",.   
-00006e90: 2020 2022 7265 6c61 7465 6454 6563 686e     "relatedTechn
-00006ea0: 6f6c 6f67 6965 7322 3a20 5b22 4769 7448  ologies": ["GitH
-00006eb0: 7562 225d 2c0a 2020 2020 2020 2270 6174  ub"],.      "pat
-00006ec0: 7465 726e 7322 3a20 5b0a 2020 2020 2020  terns": [.      
-00006ed0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00006ee0: 2020 2020 7b20 224c 4f57 4552 223a 207b      { "LOWER": {
-00006ef0: 2022 4655 5a5a 5931 223a 2022 7665 7273   "FUZZY1": "vers
-00006f00: 696f 6e22 207d 207d 2c0a 2020 2020 2020  ion" } },.      
-00006f10: 2020 2020 2020 2020 7b20 224c 4f57 4552          { "LOWER
-00006f20: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
-00006f30: 636f 6e74 726f 6c22 207d 207d 0a20 2020  control" } }.   
-00006f40: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00006f50: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
-00006f60: 2267 6974 2220 7d5d 0a20 2020 2020 205d  "git" }].      ]
-00006f70: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
-00006f80: 7469 6f6e 223a 2022 4120 7379 7374 656d  tion": "A system
-00006f90: 2074 6861 7420 7265 636f 7264 7320 6368   that records ch
-00006fa0: 616e 6765 7320 746f 2061 2066 696c 6520  anges to a file 
-00006fb0: 6f72 2073 6574 206f 6620 6669 6c65 7320  or set of files 
-00006fc0: 6f76 6572 2074 696d 652c 2061 6c6c 6f77  over time, allow
-00006fd0: 696e 6720 6465 7665 6c6f 7065 7273 2074  ing developers t
-00006fe0: 6f20 636f 6c6c 6162 6f72 6174 6520 6f6e  o collaborate on
-00006ff0: 2063 6f64 652c 2074 7261 636b 2063 6861   code, track cha
-00007000: 6e67 6573 2c20 616e 6420 7265 7665 7274  nges, and revert
-00007010: 2074 6f20 7072 6576 696f 7573 2076 6572   to previous ver
-00007020: 7369 6f6e 7320 6966 206e 6565 6465 642e  sions if needed.
-00007030: 2056 6572 7369 6f6e 2063 6f6e 7472 6f6c   Version control
-00007040: 2073 7973 7465 6d73 206c 696b 6520 4769   systems like Gi
-00007050: 7420 706c 6179 2061 2063 7275 6369 616c  t play a crucial
-00007060: 2072 6f6c 6520 696e 2073 6f66 7477 6172   role in softwar
-00007070: 6520 6465 7665 6c6f 706d 656e 7420 776f  e development wo
-00007080: 726b 666c 6f77 732e 222c 0a20 2020 2020  rkflows.",.     
-00007090: 2022 7363 6f72 6522 3a20 350a 2020 7d2c   "score": 5.  },
-000070a0: 0a20 2022 4349 2f43 4422 3a20 7b0a 2020  .  "CI/CD": {.  
-000070b0: 2020 2020 2274 7970 6522 3a20 2244 6576      "type": "Dev
-000070c0: 4f70 7320 5072 6163 7469 6365 7322 2c0a  Ops Practices",.
-000070d0: 2020 2020 2020 2263 6174 6567 6f72 7922        "category"
-000070e0: 3a20 2252 6571 7569 7265 6d65 6e74 222c  : "Requirement",
-000070f0: 0a20 2020 2020 2022 7265 6c61 7465 6454  .      "relatedT
-00007100: 6563 686e 6f6c 6f67 6965 7322 3a20 5b22  echnologies": ["
-00007110: 4769 7448 7562 2041 6374 696f 6e73 222c  GitHub Actions",
-00007120: 224a 656e 6b69 6e73 222c 2243 6972 636c  "Jenkins","Circl
-00007130: 6543 4922 5d2c 0a20 2020 2020 2022 7061  eCI"],.      "pa
-00007140: 7474 6572 6e73 223a 205b 0a20 2020 2020  tterns": [.     
-00007150: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-00007160: 2020 2020 207b 2022 4c4f 5745 5222 3a20       { "LOWER": 
-00007170: 2263 6f6e 7469 6e75 6f75 7322 207d 2c0a  "continuous" },.
-00007180: 2020 2020 2020 2020 2020 2020 2020 7b20                { 
-00007190: 224c 4f57 4552 223a 2022 696e 7465 6772  "LOWER": "integr
-000071a0: 6174 696f 6e22 207d 2c0a 2020 2020 2020  ation" },.      
-000071b0: 2020 2020 2020 2020 7b20 224c 4f57 4552          { "LOWER
-000071c0: 223a 2022 616e 6422 207d 2c0a 2020 2020  ": "and" },.    
-000071d0: 2020 2020 2020 2020 2020 7b20 224c 4f57            { "LOW
-000071e0: 4552 223a 2022 6465 706c 6f79 6d65 6e74  ER": "deployment
-000071f0: 2220 7d0a 2020 2020 2020 2020 2020 5d2c  " }.          ],
-00007200: 0a20 2020 2020 2020 2020 205b 7b20 224f  .          [{ "O
-00007210: 5254 4822 3a20 2243 4922 207d 2c20 7b20  RTH": "CI" }, { 
-00007220: 224f 5254 4822 3a20 222f 2220 7d2c 207b  "ORTH": "/" }, {
-00007230: 2022 4f52 5448 223a 2022 4344 2220 7d5d   "ORTH": "CD" }]
-00007240: 2c0a 2020 2020 2020 2020 2020 5b7b 2022  ,.          [{ "
-00007250: 4f52 5448 223a 2022 4349 2f43 4422 207d  ORTH": "CI/CD" }
-00007260: 5d2c 0a20 2020 2020 2020 2020 205b 7b20  ],.          [{ 
-00007270: 224c 4f57 4552 223a 2022 6369 2220 7d2c  "LOWER": "ci" },
-00007280: 207b 2022 4f52 5448 223a 2022 2f22 207d   { "ORTH": "/" }
-00007290: 2c20 7b20 224c 4f57 4552 223a 2022 6364  , { "LOWER": "cd
-000072a0: 2220 7d5d 2c0a 2020 2020 2020 2020 2020  " }],.          
-000072b0: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
-000072c0: 555a 5a59 3122 3a20 2263 6963 6422 207d  UZZY1": "cicd" }
-000072d0: 207d 5d2c 0a20 2020 2020 2020 2020 205b   }],.          [
-000072e0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-000072f0: 5a5a 5931 223a 2022 776f 726b 666c 6f77  ZZY1": "workflow
-00007300: 2220 7d20 7d2c 207b 2022 4c4f 5745 5222  " } }, { "LOWER"
-00007310: 3a20 7b20 2246 555a 5a59 3122 3a20 2261  : { "FUZZY1": "a
-00007320: 7574 6f6d 6174 696f 6e22 207d 207d 5d2c  utomation" } }],
-00007330: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
-00007340: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
-00007350: 223a 2022 776f 726b 666c 6f77 2220 7d20  ": "workflow" } 
-00007360: 7d5d 2c0a 2020 2020 2020 2020 2020 5b7b  }],.          [{
-00007370: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
-00007380: 5a59 3122 3a20 2264 6570 6c6f 796d 656e  ZY1": "deploymen
-00007390: 7422 207d 207d 5d0a 2020 2020 2020 5d2c  t" } }].      ],
-000073a0: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
-000073b0: 696f 6e22 3a20 2243 6f6e 7469 6e75 6f75  ion": "Continuou
-000073c0: 7320 496e 7465 6772 6174 696f 6e20 616e  s Integration an
-000073d0: 6420 436f 6e74 696e 756f 7573 2044 6570  d Continuous Dep
-000073e0: 6c6f 796d 656e 7420 2843 492f 4344 2920  loyment (CI/CD) 
-000073f0: 6172 6520 4465 764f 7073 2070 7261 6374  are DevOps pract
-00007400: 6963 6573 2074 6861 7420 6175 746f 6d61  ices that automa
-00007410: 7465 2074 6865 2073 6f66 7477 6172 6520  te the software 
-00007420: 7265 6c65 6173 6520 7072 6f63 6573 732e  release process.
-00007430: 2043 4920 666f 6375 7365 7320 6f6e 2069   CI focuses on i
-00007440: 6e74 6567 7261 7469 6e67 2063 6f64 6520  ntegrating code 
-00007450: 6368 616e 6765 7320 6672 6571 7565 6e74  changes frequent
-00007460: 6c79 2c20 7768 6572 6561 7320 4344 2065  ly, whereas CD e
-00007470: 6e73 7572 6573 2074 6865 2064 656c 6976  nsures the deliv
-00007480: 6572 7920 6f66 2074 6865 7365 2063 6861  ery of these cha
-00007490: 6e67 6573 2074 6f20 7072 6f64 7563 7469  nges to producti
-000074a0: 6f6e 2065 6e76 6972 6f6e 6d65 6e74 7320  on environments 
-000074b0: 736d 6f6f 7468 6c79 2e22 2c0a 2020 2020  smoothly.",.    
-000074c0: 2020 2273 636f 7265 223a 2035 0a20 207d    "score": 5.  }
-000074d0: 2c0a 2020 2249 6e66 7261 7374 7275 6374  ,.  "Infrastruct
-000074e0: 7572 6520 6173 2043 6f64 6522 3a20 7b0a  ure as Code": {.
-000074f0: 2020 2020 2020 2274 7970 6522 3a20 2244        "type": "D
-00007500: 6576 4f70 7320 5072 6163 7469 6365 7322  evOps Practices"
-00007510: 2c0a 2020 2020 2020 2263 6174 6567 6f72  ,.      "categor
-00007520: 7922 3a20 2252 6571 7569 7265 6d65 6e74  y": "Requirement
-00007530: 222c 0a20 2020 2020 2022 7265 6c61 7465  ",.      "relate
-00007540: 6454 6563 686e 6f6c 6f67 6965 7322 3a20  dTechnologies": 
-00007550: 5b22 5465 7272 6166 6f72 6d22 5d2c 0a20  ["Terraform"],. 
-00007560: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
-00007570: 205b 0a20 2020 2020 2020 2020 205b 7b20   [.          [{ 
-00007580: 224c 4f57 4552 223a 207b 2022 4655 5a5a  "LOWER": { "FUZZ
-00007590: 5931 223a 2022 696e 6672 6173 7472 7563  Y1": "infrastruc
-000075a0: 7475 7265 2220 7d20 7d2c 207b 2022 4c4f  ture" } }, { "LO
-000075b0: 5745 5222 3a20 2261 7322 207d 2c20 7b20  WER": "as" }, { 
-000075c0: 224c 4f57 4552 223a 207b 2022 4655 5a5a  "LOWER": { "FUZZ
-000075d0: 5931 223a 2022 636f 6465 2220 7d20 7d5d  Y1": "code" } }]
-000075e0: 2c0a 2020 2020 2020 2020 2020 5b7b 2022  ,.          [{ "
-000075f0: 4c4f 5745 5222 3a20 2269 6163 2220 7d5d  LOWER": "iac" }]
-00007600: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00007610: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00007620: 5468 6520 7072 6f63 6573 7320 6f66 206d  The process of m
-00007630: 616e 6167 696e 6720 616e 6420 7072 6f76  anaging and prov
-00007640: 6973 696f 6e69 6e67 2063 6f6d 7075 7469  isioning computi
-00007650: 6e67 2069 6e66 7261 7374 7275 6374 7572  ng infrastructur
-00007660: 6520 7468 726f 7567 6820 6d61 6368 696e  e through machin
-00007670: 652d 7265 6164 6162 6c65 2064 6566 696e  e-readable defin
-00007680: 6974 696f 6e20 6669 6c65 732c 2072 6174  ition files, rat
-00007690: 6865 7220 7468 616e 2070 6879 7369 6361  her than physica
-000076a0: 6c20 6861 7264 7761 7265 2063 6f6e 6669  l hardware confi
-000076b0: 6775 7261 7469 6f6e 206f 7220 696e 7465  guration or inte
-000076c0: 7261 6374 6976 6520 636f 6e66 6967 7572  ractive configur
-000076d0: 6174 696f 6e20 746f 6f6c 732e 222c 0a20  ation tools.",. 
-000076e0: 2020 2020 2022 7363 6f72 6522 3a20 350a       "score": 5.
-000076f0: 2020 7d2c 0a20 2022 436f 6e74 6169 6e65    },.  "Containe
-00007700: 7269 7a61 7469 6f6e 223a 207b 0a20 2020  rization": {.   
-00007710: 2020 2022 7479 7065 223a 2022 4465 764f     "type": "DevO
-00007720: 7073 2050 7261 6374 6963 6573 222c 0a20  ps Practices",. 
-00007730: 2020 2020 2022 6361 7465 676f 7279 223a       "category":
-00007740: 2022 5265 7175 6972 656d 656e 7422 2c0a   "Requirement",.
-00007750: 2020 2020 2020 2272 656c 6174 6564 5465        "relatedTe
-00007760: 6368 6e6f 6c6f 6769 6573 223a 205b 2244  chnologies": ["D
-00007770: 6f63 6b65 7222 5d2c 0a20 2020 2020 2022  ocker"],.      "
-00007780: 7061 7474 6572 6e73 223a 205b 0a20 2020  patterns": [.   
-00007790: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
-000077a0: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
-000077b0: 636f 6e74 6169 6e65 7269 7a61 7469 6f6e  containerization
-000077c0: 2220 7d7d 5d2c 0a20 2020 2020 2020 2020  " }}],.         
-000077d0: 205b 7b20 224c 4f57 4552 223a 207b 2022   [{ "LOWER": { "
-000077e0: 4655 5a5a 5931 223a 2022 636f 6e74 6169  FUZZY1": "contai
-000077f0: 6e65 7273 2220 7d7d 5d2c 0a20 2020 2020  ners" }}],.     
-00007800: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
-00007810: 207b 2022 4655 5a5a 5931 223a 2022 636f   { "FUZZY1": "co
-00007820: 6e74 6169 6e65 7269 7a65 6422 7d7d 5d2c  ntainerized"}}],
-00007830: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
-00007840: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
-00007850: 223a 2022 6465 706c 6f79 6162 6c65 2220  ": "deployable" 
-00007860: 7d7d 5d2c 0a20 2020 2020 2020 2020 205b  }}],.          [
-00007870: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-00007880: 5a5a 5931 223a 2022 706f 7274 6162 696c  ZZY1": "portabil
-00007890: 6974 7922 207d 7d5d 0a20 2020 2020 205d  ity" }}].      ]
-000078a0: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
-000078b0: 7469 6f6e 223a 2022 5468 6520 7072 6f63  tion": "The proc
-000078c0: 6573 7320 6f66 2065 6e63 6170 7375 6c61  ess of encapsula
-000078d0: 7469 6e67 2061 6e20 6170 706c 6963 6174  ting an applicat
-000078e0: 696f 6e20 616e 6420 6974 7320 6465 7065  ion and its depe
-000078f0: 6e64 656e 6369 6573 2069 6e74 6f20 6120  ndencies into a 
-00007900: 636f 6e74 6169 6e65 722c 2061 6c6c 6f77  container, allow
-00007910: 696e 6720 6974 2074 6f20 7275 6e20 636f  ing it to run co
-00007920: 6e73 6973 7465 6e74 6c79 2061 6372 6f73  nsistently acros
-00007930: 7320 6469 6666 6572 656e 7420 656e 7669  s different envi
-00007940: 726f 6e6d 656e 7473 2e22 2c0a 2020 2020  ronments.",.    
-00007950: 2020 2273 636f 7265 223a 2035 0a20 207d    "score": 5.  }
-00007960: 2c0a 2020 2243 6f6e 7461 696e 6572 204f  ,.  "Container O
-00007970: 7263 6865 7374 7261 7469 6f6e 223a 207b  rchestration": {
-00007980: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
-00007990: 4465 764f 7073 2050 7261 6374 6963 6573  DevOps Practices
-000079a0: 222c 0a20 2020 2020 2022 6361 7465 676f  ",.      "catego
-000079b0: 7279 223a 2022 5265 7175 6972 656d 656e  ry": "Requiremen
-000079c0: 7422 2c0a 2020 2020 2020 2272 656c 6174  t",.      "relat
-000079d0: 6564 5465 6368 6e6f 6c6f 6769 6573 223a  edTechnologies":
-000079e0: 205b 224b 7562 6572 6e65 7465 7322 5d2c   ["Kubernetes"],
-000079f0: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
-00007a00: 223a 205b 0a20 2020 2020 2020 2020 205b  ": [.          [
-00007a10: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-00007a20: 5a5a 5931 223a 2022 636f 6e74 6169 6e65  ZZY1": "containe
-00007a30: 7222 207d 207d 2c20 7b20 224c 4f57 4552  r" } }, { "LOWER
-00007a40: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
-00007a50: 6f72 6368 6573 7472 6174 696f 6e22 207d  orchestration" }
-00007a60: 207d 5d2c 0a20 2020 2020 2020 2020 205b   }],.          [
-00007a70: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
-00007a80: 5a5a 5931 223a 2022 706f 6473 2220 7d7d  ZZY1": "pods" }}
-00007a90: 5d2c 0a20 2020 2020 2020 2020 205b 7b20  ],.          [{ 
-00007aa0: 224c 4f57 4552 223a 207b 2022 4655 5a5a  "LOWER": { "FUZZ
-00007ab0: 5931 223a 2022 7363 616c 6162 6c65 2220  Y1": "scalable" 
-00007ac0: 7d7d 5d0a 2020 2020 2020 5d2c 0a20 2020  }}].      ],.   
-00007ad0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00007ae0: 3a20 2254 6865 2070 726f 6365 7373 206f  : "The process o
-00007af0: 6620 6175 746f 6d61 7469 6e67 2074 6865  f automating the
-00007b00: 2064 6570 6c6f 796d 656e 742c 2073 6361   deployment, sca
-00007b10: 6c69 6e67 2c20 616e 6420 6d61 6e61 6765  ling, and manage
-00007b20: 6d65 6e74 206f 6620 636f 6e74 6169 6e65  ment of containe
-00007b30: 7269 7a65 6420 6170 706c 6963 6174 696f  rized applicatio
-00007b40: 6e73 2e22 2c0a 2020 2020 2020 2273 636f  ns.",.      "sco
-00007b50: 7265 223a 2035 0a20 207d 0a7d 0a         re": 5.  }.}.
+00003fb0: 7265 223a 2039 0a20 207d 2c0a 0a20 2022  re": 9.  },..  "
+00003fc0: 4157 5322 3a20 7b0a 2020 2020 2020 2274  AWS": {.      "t
+00003fd0: 7970 6522 3a20 2243 6c6f 7564 2043 6f6d  ype": "Cloud Com
+00003fe0: 7075 7469 6e67 222c 0a20 2020 2020 2022  puting",.      "
+00003ff0: 6361 7465 676f 7279 223a 2022 436c 6f75  category": "Clou
+00004000: 6420 5365 7276 6963 6520 5072 6f76 6964  d Service Provid
+00004010: 6572 7322 2c0a 2020 2020 2020 2264 6573  ers",.      "des
+00004020: 6372 6970 7469 6f6e 223a 2022 416d 617a  cription": "Amaz
+00004030: 6f6e 2057 6562 2053 6572 7669 6365 7320  on Web Services 
+00004040: 6f66 6665 7273 2072 656c 6961 626c 652c  offers reliable,
+00004050: 2073 6361 6c61 626c 652c 2061 6e64 2069   scalable, and i
+00004060: 6e65 7870 656e 7369 7665 2063 6c6f 7564  nexpensive cloud
+00004070: 2063 6f6d 7075 7469 6e67 2073 6572 7669   computing servi
+00004080: 6365 732e 2049 7427 7320 7468 6520 776f  ces. It's the wo
+00004090: 726c 6427 7320 6d6f 7374 2063 6f6d 7072  rld's most compr
+000040a0: 6568 656e 7369 7665 2061 6e64 2062 726f  ehensive and bro
+000040b0: 6164 6c79 2061 646f 7074 6564 2063 6c6f  adly adopted clo
+000040c0: 7564 2070 6c61 7466 6f72 6d2c 206f 6666  ud platform, off
+000040d0: 6572 696e 6720 6f76 6572 2031 3735 2066  ering over 175 f
+000040e0: 756c 6c79 2d66 6561 7475 7265 6420 7365  ully-featured se
+000040f0: 7276 6963 6573 2066 726f 6d20 6461 7461  rvices from data
+00004100: 2063 656e 7465 7273 2067 6c6f 6261 6c6c   centers globall
+00004110: 792e 222c 0a20 2020 2020 2022 7061 7474  y.",.      "patt
+00004120: 6572 6e73 223a 205b 0a20 2020 2020 2020  erns": [.       
+00004130: 2020 205b 7b20 224c 4f57 4552 223a 2022     [{ "LOWER": "
+00004140: 6177 7322 207d 5d2c 0a20 2020 2020 2020  aws" }],.       
+00004150: 2020 205b 7b20 2254 4558 5422 3a20 7b20     [{ "TEXT": { 
+00004160: 2246 555a 5a59 3122 3a20 2241 6d61 7a6f  "FUZZY1": "Amazo
+00004170: 6e20 5765 6220 5365 7276 6963 6573 2220  n Web Services" 
+00004180: 7d20 7d5d 0a20 2020 2020 205d 2c0a 2020  } }].      ],.  
+00004190: 2020 2020 2273 636f 7265 223a 2039 0a20      "score": 9. 
+000041a0: 207d 2c0a 2020 2241 7a75 7265 223a 207b   },.  "Azure": {
+000041b0: 0a20 2020 2020 2022 7479 7065 223a 2022  .      "type": "
+000041c0: 436c 6f75 6420 436f 6d70 7574 696e 6722  Cloud Computing"
+000041d0: 2c0a 2020 2020 2020 2263 6174 6567 6f72  ,.      "categor
+000041e0: 7922 3a20 2243 6c6f 7564 2053 6572 7669  y": "Cloud Servi
+000041f0: 6365 2050 726f 7669 6465 7273 222c 0a20  ce Providers",. 
+00004200: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00004210: 6e22 3a20 224d 6963 726f 736f 6674 2041  n": "Microsoft A
+00004220: 7a75 7265 2069 7320 6120 636c 6f75 6420  zure is a cloud 
+00004230: 636f 6d70 7574 696e 6720 7365 7276 6963  computing servic
+00004240: 6520 666f 7220 6275 696c 6469 6e67 2c20  e for building, 
+00004250: 7465 7374 696e 672c 2064 6570 6c6f 7969  testing, deployi
+00004260: 6e67 2c20 616e 6420 6d61 6e61 6769 6e67  ng, and managing
+00004270: 2061 7070 6c69 6361 7469 6f6e 7320 616e   applications an
+00004280: 6420 7365 7276 6963 6573 2074 6872 6f75  d services throu
+00004290: 6768 204d 6963 726f 736f 6674 2d6d 616e  gh Microsoft-man
+000042a0: 6167 6564 2064 6174 6120 6365 6e74 6572  aged data center
+000042b0: 732e 2049 7420 7072 6f76 6964 6573 2073  s. It provides s
+000042c0: 6f66 7477 6172 6520 6173 2061 2073 6572  oftware as a ser
+000042d0: 7669 6365 2028 5361 6153 292c 2070 6c61  vice (SaaS), pla
+000042e0: 7466 6f72 6d20 6173 2061 2073 6572 7669  tform as a servi
+000042f0: 6365 2028 5061 6153 292c 2061 6e64 2069  ce (PaaS), and i
+00004300: 6e66 7261 7374 7275 6374 7572 6520 6173  nfrastructure as
+00004310: 2061 2073 6572 7669 6365 2028 4961 6153   a service (IaaS
+00004320: 292e 222c 0a20 2020 2020 2022 7061 7474  ).",.      "patt
+00004330: 6572 6e73 223a 205b 0a20 2020 2020 2020  erns": [.       
+00004340: 2020 205b 7b20 224c 4f57 4552 223a 207b     [{ "LOWER": {
+00004350: 2022 4655 5a5a 5931 223a 2022 617a 7572   "FUZZY1": "azur
+00004360: 6522 207d 207d 5d2c 0a20 2020 2020 2020  e" } }],.       
+00004370: 2020 205b 7b20 2254 4558 5422 3a20 7b20     [{ "TEXT": { 
+00004380: 2246 555a 5a59 3122 3a20 224d 6963 726f  "FUZZY1": "Micro
+00004390: 736f 6674 2041 7a75 7265 2220 7d20 7d5d  soft Azure" } }]
+000043a0: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
+000043b0: 2273 636f 7265 223a 2039 0a20 207d 2c0a  "score": 9.  },.
+000043c0: 2020 2247 6f6f 676c 6543 6c6f 7564 223a    "GoogleCloud":
+000043d0: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+000043e0: 2022 436c 6f75 6420 436f 6d70 7574 696e   "Cloud Computin
+000043f0: 6722 2c0a 2020 2020 2020 2263 6174 6567  g",.      "categ
+00004400: 6f72 7922 3a20 2243 6c6f 7564 2053 6572  ory": "Cloud Ser
+00004410: 7669 6365 2050 726f 7669 6465 7273 222c  vice Providers",
+00004420: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
+00004430: 696f 6e22 3a20 2247 6f6f 676c 6520 436c  ion": "Google Cl
+00004440: 6f75 6420 506c 6174 666f 726d 2c20 6f66  oud Platform, of
+00004450: 6665 7265 6420 6279 2047 6f6f 676c 652c  fered by Google,
+00004460: 2069 7320 6120 7375 6974 6520 6f66 2063   is a suite of c
+00004470: 6c6f 7564 2063 6f6d 7075 7469 6e67 2073  loud computing s
+00004480: 6572 7669 6365 7320 7468 6174 2072 756e  ervices that run
+00004490: 7320 6f6e 2074 6865 2073 616d 6520 696e  s on the same in
+000044a0: 6672 6173 7472 7563 7475 7265 2074 6861  frastructure tha
+000044b0: 7420 476f 6f67 6c65 2075 7365 7320 696e  t Google uses in
+000044c0: 7465 726e 616c 6c79 2066 6f72 2069 7473  ternally for its
+000044d0: 2065 6e64 2d75 7365 7220 7072 6f64 7563   end-user produc
+000044e0: 7473 2c20 7375 6368 2061 7320 476f 6f67  ts, such as Goog
+000044f0: 6c65 2053 6561 7263 682c 2047 6d61 696c  le Search, Gmail
+00004500: 2c20 6669 6c65 2073 746f 7261 6765 2c20  , file storage, 
+00004510: 616e 6420 596f 7554 7562 652e 222c 0a20  and YouTube.",. 
+00004520: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
+00004530: 205b 0a20 2020 2020 2020 2020 205b 0a20   [.          [. 
+00004540: 2020 2020 2020 2020 2020 2020 207b 2022               { "
+00004550: 4c4f 5745 5222 3a20 7b20 2246 555a 5a59  LOWER": { "FUZZY
+00004560: 3122 3a20 2267 6f6f 676c 6522 207d 207d  1": "google" } }
+00004570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004580: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+00004590: 5a5a 5931 223a 2022 636c 6f75 6422 207d  ZZY1": "cloud" }
+000045a0: 207d 0a20 2020 2020 2020 2020 205d 2c0a   }.          ],.
+000045b0: 2020 2020 2020 2020 2020 5b7b 2022 4c4f            [{ "LO
+000045c0: 5745 5222 3a20 2267 6370 2220 7d5d 0a20  WER": "gcp" }]. 
+000045d0: 2020 2020 205d 2c0a 2020 2020 2020 2273       ],.      "s
+000045e0: 636f 7265 223a 2039 0a20 207d 2c0a 2020  core": 9.  },.  
+000045f0: 2247 6974 4875 6222 3a20 7b0a 2020 2020  "GitHub": {.    
+00004600: 2020 2274 7970 6522 3a20 2250 6c61 7466    "type": "Platf
+00004610: 6f72 6d22 2c0a 2020 2020 2020 2263 6174  orm",.      "cat
+00004620: 6567 6f72 7922 3a20 2256 6572 7369 6f6e  egory": "Version
+00004630: 2043 6f6e 7472 6f6c 222c 0a20 2020 2020   Control",.     
+00004640: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00004650: 2247 6974 4875 6220 6973 2061 2077 6562  "GitHub is a web
+00004660: 2d62 6173 6564 2076 6572 7369 6f6e 2063  -based version c
+00004670: 6f6e 7472 6f6c 2061 6e64 2063 6f6c 6c61  ontrol and colla
+00004680: 626f 7261 7469 6f6e 2070 6c61 7466 6f72  boration platfor
+00004690: 6d20 666f 7220 736f 6674 7761 7265 2064  m for software d
+000046a0: 6576 656c 6f70 6572 732e 2049 7420 656e  evelopers. It en
+000046b0: 6162 6c65 7320 7573 6572 7320 746f 2073  ables users to s
+000046c0: 746f 7265 2c20 6d61 6e61 6765 2c20 616e  tore, manage, an
+000046d0: 6420 7472 6163 6b20 6368 616e 6765 7320  d track changes 
+000046e0: 746f 2074 6865 6972 2063 6f64 6520 7072  to their code pr
+000046f0: 6f6a 6563 7473 2075 7369 6e67 2074 6865  ojects using the
+00004700: 2047 6974 2076 6572 7369 6f6e 2063 6f6e   Git version con
+00004710: 7472 6f6c 2073 7973 7465 6d2e 222c 0a20  trol system.",. 
+00004720: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
+00004730: 205b 5b7b 2022 4c4f 5745 5222 3a20 7b20   [[{ "LOWER": { 
+00004740: 2246 555a 5a59 3122 3a20 2267 6974 6875  "FUZZY1": "githu
+00004750: 6222 207d 207d 5d5d 2c0a 2020 2020 2020  b" } }]],.      
+00004760: 2273 636f 7265 223a 2037 0a20 207d 2c0a  "score": 7.  },.
+00004770: 2020 2247 6974 4875 6220 4163 7469 6f6e    "GitHub Action
+00004780: 7322 3a20 7b0a 2020 2020 2020 2274 7970  s": {.      "typ
+00004790: 6522 3a20 2241 7574 6f6d 6174 696f 6e20  e": "Automation 
+000047a0: 576f 726b 666c 6f77 222c 0a20 2020 2020  Workflow",.     
+000047b0: 2022 6361 7465 676f 7279 223a 2022 4349   "category": "CI
+000047c0: 2f43 4422 2c0a 2020 2020 2020 2264 6573  /CD",.      "des
+000047d0: 6372 6970 7469 6f6e 223a 2022 4769 7448  cription": "GitH
+000047e0: 7562 2041 6374 696f 6e73 2061 6c6c 6f77  ub Actions allow
+000047f0: 2079 6f75 2074 6f20 6372 6561 7465 2063   you to create c
+00004800: 6f6e 7469 6e75 6f75 7320 696e 7465 6772  ontinuous integr
+00004810: 6174 696f 6e20 616e 6420 636f 6e74 696e  ation and contin
+00004820: 756f 7573 2064 6570 6c6f 796d 656e 7420  uous deployment 
+00004830: 2843 492f 4344 2920 7069 7065 6c69 6e65  (CI/CD) pipeline
+00004840: 7320 7269 6768 7420 696e 7369 6465 2079  s right inside y
+00004850: 6f75 7220 4769 7448 7562 2072 6570 6f73  our GitHub repos
+00004860: 6974 6f72 792e 222c 0a20 2020 2020 2022  itory.",.      "
+00004870: 7061 7474 6572 6e73 223a 205b 0a20 2020  patterns": [.   
+00004880: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+00004890: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+000048a0: 6769 7468 7562 2061 6374 696f 6e73 2220  github actions" 
+000048b0: 7d20 7d5d 2c0a 2020 2020 2020 2020 2020  } }],.          
+000048c0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000048d0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+000048e0: 5a5a 5931 223a 2022 6769 7468 7562 2220  ZZY1": "github" 
+000048f0: 7d20 7d2c 0a20 2020 2020 2020 2020 2020  } },.           
+00004900: 2020 207b 2022 4c4f 5745 5222 3a20 7b20     { "LOWER": { 
+00004910: 2246 555a 5a59 3122 3a20 2261 6374 696f  "FUZZY1": "actio
+00004920: 6e73 2220 7d20 7d0a 2020 2020 2020 2020  ns" } }.        
+00004930: 2020 5d0a 2020 2020 2020 5d2c 0a20 2020    ].      ],.   
+00004940: 2020 2022 7363 6f72 6522 3a20 3130 0a20     "score": 10. 
+00004950: 207d 2c0a 2020 224a 656e 6b69 6e73 223a   },.  "Jenkins":
+00004960: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00004970: 2022 4175 746f 6d61 7469 6f6e 2053 6572   "Automation Ser
+00004980: 7665 7222 2c0a 2020 2020 2020 2263 6174  ver",.      "cat
+00004990: 6567 6f72 7922 3a20 2243 492f 4344 222c  egory": "CI/CD",
+000049a0: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
+000049b0: 696f 6e22 3a20 2241 6e20 6f70 656e 2d73  ion": "An open-s
+000049c0: 6f75 7263 6520 6175 746f 6d61 7469 6f6e  ource automation
+000049d0: 2073 6572 7665 7220 7468 6174 2065 6e61   server that ena
+000049e0: 626c 6573 2064 6576 656c 6f70 6572 7320  bles developers 
+000049f0: 746f 2062 7569 6c64 2c20 7465 7374 2c20  to build, test, 
+00004a00: 616e 6420 6465 706c 6f79 2074 6865 6972  and deploy their
+00004a10: 2073 6f66 7477 6172 6520 6175 746f 6d61   software automa
+00004a20: 7469 6361 6c6c 792e 222c 0a20 2020 2020  tically.",.     
+00004a30: 2022 7061 7474 6572 6e73 223a 205b 5b7b   "patterns": [[{
+00004a40: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
+00004a50: 5a59 3122 3a20 226a 656e 6b69 6e73 2220  ZY1": "jenkins" 
+00004a60: 7d20 7d5d 5d2c 0a20 2020 2020 2022 7363  } }]],.      "sc
+00004a70: 6f72 6522 3a20 380a 2020 7d2c 0a20 2022  ore": 8.  },.  "
+00004a80: 4369 7263 6c65 4349 223a 207b 0a20 2020  CircleCI": {.   
+00004a90: 2020 2022 7479 7065 223a 2022 436f 6e74     "type": "Cont
+00004aa0: 696e 756f 7573 2049 6e74 6567 7261 7469  inuous Integrati
+00004ab0: 6f6e 2054 6f6f 6c22 2c0a 2020 2020 2020  on Tool",.      
+00004ac0: 2263 6174 6567 6f72 7922 3a20 2243 492f  "category": "CI/
+00004ad0: 4344 222c 0a20 2020 2020 2022 6465 7363  CD",.      "desc
+00004ae0: 7269 7074 696f 6e22 3a20 2243 6972 636c  ription": "Circl
+00004af0: 6543 4920 6973 2061 2063 6f6e 7469 6e75  eCI is a continu
+00004b00: 6f75 7320 696e 7465 6772 6174 696f 6e20  ous integration 
+00004b10: 616e 6420 636f 6e74 696e 756f 7573 2064  and continuous d
+00004b20: 656c 6976 6572 7920 706c 6174 666f 726d  elivery platform
+00004b30: 2074 6861 7420 6865 6c70 7320 736f 6674   that helps soft
+00004b40: 7761 7265 2074 6561 6d73 2077 6f72 6b20  ware teams work 
+00004b50: 736d 6172 7465 722c 2066 6173 7465 722e  smarter, faster.
+00004b60: 222c 0a20 2020 2020 2022 7061 7474 6572  ",.      "patter
+00004b70: 6e73 223a 205b 0a20 2020 2020 2020 205b  ns": [.        [
+00004b80: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+00004b90: 5a5a 5931 223a 2022 6369 7263 6c65 6369  ZZY1": "circleci
+00004ba0: 2220 7d20 7d5d 2c0a 2020 2020 2020 2020  " } }],.        
+00004bb0: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
+00004bc0: 555a 5a59 3122 3a20 2263 6972 636c 6522  UZZY1": "circle"
+00004bd0: 207d 207d 2c20 7b20 224c 4f57 4552 223a   } }, { "LOWER":
+00004be0: 2022 6369 2220 7d5d 0a20 2020 2020 205d   "ci" }].      ]
+00004bf0: 2c0a 2020 2020 2020 2273 636f 7265 223a  ,.      "score":
+00004c00: 2038 0a20 207d 2c0a 2020 2254 6572 7261   8.  },.  "Terra
+00004c10: 666f 726d 223a 207b 0a20 2020 2020 2022  form": {.      "
+00004c20: 7479 7065 223a 2022 546f 6f6c 222c 0a20  type": "Tool",. 
+00004c30: 2020 2020 2022 6361 7465 676f 7279 223a       "category":
+00004c40: 2022 496e 6672 6173 7472 7563 7475 7265   "Infrastructure
+00004c50: 2061 7320 436f 6465 222c 0a20 2020 2020   as Code",.     
+00004c60: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00004c70: 2241 6e20 6f70 656e 2d73 6f75 7263 6520  "An open-source 
+00004c80: 746f 6f6c 2074 6861 7420 616c 6c6f 7773  tool that allows
+00004c90: 2064 6576 656c 6f70 6572 7320 746f 2064   developers to d
+00004ca0: 6566 696e 6520 616e 6420 7072 6f76 6973  efine and provis
+00004cb0: 696f 6e20 6461 7461 2063 656e 7465 7220  ion data center 
+00004cc0: 696e 6672 6173 7472 7563 7475 7265 2075  infrastructure u
+00004cd0: 7369 6e67 2061 2064 6563 6c61 7261 7469  sing a declarati
+00004ce0: 7665 2063 6f6e 6669 6775 7261 7469 6f6e  ve configuration
+00004cf0: 206c 616e 6775 6167 652e 222c 0a20 2020   language.",.   
+00004d00: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
+00004d10: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
+00004d20: 555a 5a59 3122 3a20 2274 6572 7261 666f  UZZY1": "terrafo
+00004d30: 726d 2220 7d20 7d5d 5d2c 0a20 2020 2020  rm" } }]],.     
+00004d40: 2022 7363 6f72 6522 3a20 3130 0a20 207d   "score": 10.  }
+00004d50: 2c0a 2020 2250 726f 6d65 7468 6575 7322  ,.  "Prometheus"
+00004d60: 3a20 7b0a 2020 2020 2020 2274 7970 6522  : {.      "type"
+00004d70: 3a20 2254 6f6f 6c22 2c0a 2020 2020 2020  : "Tool",.      
+00004d80: 2263 6174 6567 6f72 7922 3a20 224d 6f6e  "category": "Mon
+00004d90: 6974 6f72 696e 6722 2c0a 2020 2020 2020  itoring",.      
+00004da0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00004db0: 416e 206f 7065 6e2d 736f 7572 6365 2073  An open-source s
+00004dc0: 7973 7465 6d73 206d 6f6e 6974 6f72 696e  ystems monitorin
+00004dd0: 6720 616e 6420 616c 6572 7469 6e67 2074  g and alerting t
+00004de0: 6f6f 6c6b 6974 206f 7269 6769 6e61 6c6c  oolkit originall
+00004df0: 7920 6275 696c 7420 6174 2053 6f75 6e64  y built at Sound
+00004e00: 436c 6f75 642e 222c 0a20 2020 2020 2022  Cloud.",.      "
+00004e10: 7061 7474 6572 6e73 223a 205b 5b7b 2022  patterns": [[{ "
+00004e20: 4c4f 5745 5222 3a20 7b20 2246 555a 5a59  LOWER": { "FUZZY
+00004e30: 3122 3a20 2270 726f 6d65 7468 6575 7322  1": "prometheus"
+00004e40: 207d 207d 5d5d 2c0a 2020 2020 2020 2273   } }]],.      "s
+00004e50: 636f 7265 223a 2039 0a20 207d 2c0a 2020  core": 9.  },.  
+00004e60: 2244 6f63 6b65 7222 3a20 7b0a 2020 2020  "Docker": {.    
+00004e70: 2020 2274 7970 6522 3a20 2244 6576 4f70    "type": "DevOp
+00004e80: 7322 2c0a 2020 2020 2020 2263 6174 6567  s",.      "categ
+00004e90: 6f72 7922 3a20 2243 6f6e 7461 696e 6572  ory": "Container
+00004ea0: 697a 6174 696f 6e22 2c0a 2020 2020 2020  ization",.      
+00004eb0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00004ec0: 446f 636b 6572 2069 7320 616e 206f 7065  Docker is an ope
+00004ed0: 6e20 706c 6174 666f 726d 2066 6f72 2064  n platform for d
+00004ee0: 6576 656c 6f70 696e 672c 2073 6869 7070  eveloping, shipp
+00004ef0: 696e 672c 2061 6e64 2072 756e 6e69 6e67  ing, and running
+00004f00: 2061 7070 6c69 6361 7469 6f6e 732e 2044   applications. D
+00004f10: 6f63 6b65 7220 656e 6162 6c65 7320 796f  ocker enables yo
+00004f20: 7520 746f 2073 6570 6172 6174 6520 796f  u to separate yo
+00004f30: 7572 2061 7070 6c69 6361 7469 6f6e 7320  ur applications 
+00004f40: 6672 6f6d 2079 6f75 7220 696e 6672 6173  from your infras
+00004f50: 7472 7563 7475 7265 2073 6f20 796f 7520  tructure so you 
+00004f60: 6361 6e20 6465 6c69 7665 7220 736f 6674  can deliver soft
+00004f70: 7761 7265 2071 7569 636b 6c79 2e20 5769  ware quickly. Wi
+00004f80: 7468 2044 6f63 6b65 722c 2079 6f75 2063  th Docker, you c
+00004f90: 616e 206d 616e 6167 6520 796f 7572 2069  an manage your i
+00004fa0: 6e66 7261 7374 7275 6374 7572 6520 696e  nfrastructure in
+00004fb0: 2074 6865 2073 616d 6520 7761 7973 2079   the same ways y
+00004fc0: 6f75 206d 616e 6167 6520 796f 7572 2061  ou manage your a
+00004fd0: 7070 6c69 6361 7469 6f6e 732e 222c 0a20  pplications.",. 
+00004fe0: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
+00004ff0: 205b 5b7b 2022 4c4f 5745 5222 3a20 7b20   [[{ "LOWER": { 
+00005000: 2246 555a 5a59 3122 3a20 2264 6f63 6b65  "FUZZY1": "docke
+00005010: 7222 207d 207d 5d5d 2c0a 2020 2020 2020  r" } }]],.      
+00005020: 2273 636f 7265 223a 2031 300a 2020 7d2c  "score": 10.  },
+00005030: 0a20 2022 4b75 6265 726e 6574 6573 223a  .  "Kubernetes":
+00005040: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00005050: 2022 4465 764f 7073 222c 0a20 2020 2020   "DevOps",.     
+00005060: 2022 6361 7465 676f 7279 223a 2022 436f   "category": "Co
+00005070: 6e74 6169 6e65 7220 4f72 6368 6573 7472  ntainer Orchestr
+00005080: 6174 696f 6e22 2c0a 2020 2020 2020 2264  ation",.      "d
+00005090: 6573 6372 6970 7469 6f6e 223a 2022 4b75  escription": "Ku
+000050a0: 6265 726e 6574 6573 2c20 616c 736f 206b  bernetes, also k
+000050b0: 6e6f 776e 2061 7320 4b38 732c 2069 7320  nown as K8s, is 
+000050c0: 616e 206f 7065 6e2d 736f 7572 6365 2073  an open-source s
+000050d0: 7973 7465 6d20 666f 7220 6175 746f 6d61  ystem for automa
+000050e0: 7469 6e67 2064 6570 6c6f 796d 656e 742c  ting deployment,
+000050f0: 2073 6361 6c69 6e67 2c20 616e 6420 6d61   scaling, and ma
+00005100: 6e61 6765 6d65 6e74 206f 6620 636f 6e74  nagement of cont
+00005110: 6169 6e65 7269 7a65 6420 6170 706c 6963  ainerized applic
+00005120: 6174 696f 6e73 2e20 4974 2067 726f 7570  ations. It group
+00005130: 7320 636f 6e74 6169 6e65 7273 2074 6861  s containers tha
+00005140: 7420 6d61 6b65 2075 7020 616e 2061 7070  t make up an app
+00005150: 6c69 6361 7469 6f6e 2069 6e74 6f20 6c6f  lication into lo
+00005160: 6769 6361 6c20 756e 6974 7320 666f 7220  gical units for 
+00005170: 6561 7379 206d 616e 6167 656d 656e 7420  easy management 
+00005180: 616e 6420 6469 7363 6f76 6572 792e 222c  and discovery.",
+00005190: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
+000051a0: 223a 205b 0a20 2020 2020 2020 2020 205b  ": [.          [
+000051b0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+000051c0: 5a5a 5931 223a 2022 6b75 6265 726e 6574  ZZY1": "kubernet
+000051d0: 6573 2220 7d20 7d5d 2c0a 2020 2020 2020  es" } }],.      
+000051e0: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
+000051f0: 226b 3873 2220 7d5d 0a20 2020 2020 205d  "k8s" }].      ]
+00005200: 2c0a 2020 2020 2020 2273 636f 7265 223a  ,.      "score":
+00005210: 2031 300a 2020 7d2c 0a20 2022 4865 6c6d   10.  },.  "Helm
+00005220: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00005230: 223a 2022 4465 764f 7073 222c 0a20 2020  ": "DevOps",.   
+00005240: 2020 2022 6361 7465 676f 7279 223a 2022     "category": "
+00005250: 4b75 6265 726e 6574 6573 2050 6163 6b61  Kubernetes Packa
+00005260: 6765 204d 616e 6167 6572 222c 0a20 2020  ge Manager",.   
+00005270: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00005280: 3a20 2248 656c 6d20 6973 2061 2070 6163  : "Helm is a pac
+00005290: 6b61 6765 206d 616e 6167 6572 2066 6f72  kage manager for
+000052a0: 204b 7562 6572 6e65 7465 7320 7468 6174   Kubernetes that
+000052b0: 2061 6c6c 6f77 7320 796f 7520 746f 2064   allows you to d
+000052c0: 6566 696e 652c 2069 6e73 7461 6c6c 2c20  efine, install, 
+000052d0: 616e 6420 7570 6772 6164 6520 6576 656e  and upgrade even
+000052e0: 2074 6865 206d 6f73 7420 636f 6d70 6c65   the most comple
+000052f0: 7820 4b75 6265 726e 6574 6573 2061 7070  x Kubernetes app
+00005300: 6c69 6361 7469 6f6e 732e 222c 0a20 2020  lications.",.   
+00005310: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
+00005320: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
+00005330: 555a 5a59 3122 3a20 2268 656c 6d22 207d  UZZY1": "helm" }
+00005340: 207d 5d5d 2c0a 2020 2020 2020 2273 636f   }]],.      "sco
+00005350: 7265 223a 2039 0a20 207d 2c0a 0a20 2022  re": 9.  },..  "
+00005360: 4772 6170 6851 4c22 3a20 7b0a 2020 2020  GraphQL": {.    
+00005370: 2020 2274 7970 6522 3a20 2251 7565 7279    "type": "Query
+00005380: 204c 616e 6775 6167 6522 2c0a 2020 2020   Language",.    
+00005390: 2020 2263 6174 6567 6f72 7922 3a20 2241    "category": "A
+000053a0: 5049 2044 6576 656c 6f70 6d65 6e74 222c  PI Development",
+000053b0: 0a20 2020 2020 2022 6465 7363 7269 7074  .      "descript
+000053c0: 696f 6e22 3a20 2247 7261 7068 514c 2069  ion": "GraphQL i
+000053d0: 7320 6120 7175 6572 7920 6c61 6e67 7561  s a query langua
+000053e0: 6765 2066 6f72 2041 5049 7320 616e 6420  ge for APIs and 
+000053f0: 6120 7275 6e74 696d 6520 666f 7220 6578  a runtime for ex
+00005400: 6563 7574 696e 6720 7468 6f73 6520 7175  ecuting those qu
+00005410: 6572 6965 7320 6279 2075 7369 6e67 2061  eries by using a
+00005420: 2074 7970 6520 7379 7374 656d 2079 6f75   type system you
+00005430: 2064 6566 696e 6520 666f 7220 796f 7572   define for your
+00005440: 2064 6174 612e 2047 7261 7068 514c 2069   data. GraphQL i
+00005450: 736e 2774 2074 6965 6420 746f 2061 6e79  sn't tied to any
+00005460: 2073 7065 6369 6669 6320 6461 7461 6261   specific databa
+00005470: 7365 206f 7220 7374 6f72 6167 6520 656e  se or storage en
+00005480: 6769 6e65 2061 6e64 2069 7320 696e 7374  gine and is inst
+00005490: 6561 6420 6261 636b 6564 2062 7920 796f  ead backed by yo
+000054a0: 7572 2065 7869 7374 696e 6720 636f 6465  ur existing code
+000054b0: 2061 6e64 2064 6174 612e 222c 0a20 2020   and data.",.   
+000054c0: 2020 2022 7061 7474 6572 6e73 223a 205b     "patterns": [
+000054d0: 0a20 2020 2020 2020 2020 205b 7b20 224c  .          [{ "L
+000054e0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
+000054f0: 223a 2022 6772 6170 6871 6c22 207d 207d  ": "graphql" } }
+00005500: 5d2c 0a20 2020 2020 2020 2020 205b 7b20  ],.          [{ 
+00005510: 224c 4f57 4552 223a 2022 6771 6c22 207d  "LOWER": "gql" }
+00005520: 5d0a 2020 2020 2020 5d2c 0a20 2020 2020  ].      ],.     
+00005530: 2022 7363 6f72 6522 3a20 370a 2020 7d2c   "score": 7.  },
+00005540: 0a20 2022 5465 6e73 6f72 466c 6f77 223a  .  "TensorFlow":
+00005550: 207b 0a20 2020 2020 2022 7479 7065 223a   {.      "type":
+00005560: 2022 4c69 6272 6172 7922 2c0a 2020 2020   "Library",.    
+00005570: 2020 2263 6174 6567 6f72 7922 3a20 224d    "category": "M
+00005580: 6163 6869 6e65 204c 6561 726e 696e 6722  achine Learning"
+00005590: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
+000055a0: 7469 6f6e 223a 2022 5465 6e73 6f72 466c  tion": "TensorFl
+000055b0: 6f77 2069 7320 616e 2065 6e64 2d74 6f2d  ow is an end-to-
+000055c0: 656e 6420 6f70 656e 2d73 6f75 7263 6520  end open-source 
+000055d0: 706c 6174 666f 726d 2066 6f72 206d 6163  platform for mac
+000055e0: 6869 6e65 206c 6561 726e 696e 672e 2049  hine learning. I
+000055f0: 7420 6861 7320 6120 636f 6d70 7265 6865  t has a comprehe
+00005600: 6e73 6976 652c 2066 6c65 7869 626c 6520  nsive, flexible 
+00005610: 6563 6f73 7973 7465 6d20 6f66 2074 6f6f  ecosystem of too
+00005620: 6c73 2c20 6c69 6272 6172 6965 732c 2061  ls, libraries, a
+00005630: 6e64 2063 6f6d 6d75 6e69 7479 2072 6573  nd community res
+00005640: 6f75 7263 6573 2074 6861 7420 6c65 7473  ources that lets
+00005650: 2072 6573 6561 7263 6865 7273 2070 7573   researchers pus
+00005660: 6820 7468 6520 7374 6174 652d 6f66 2d74  h the state-of-t
+00005670: 6865 2d61 7274 2069 6e20 4d4c 2061 6e64  he-art in ML and
+00005680: 2064 6576 656c 6f70 6572 7320 6561 7369   developers easi
+00005690: 6c79 2062 7569 6c64 2061 6e64 2064 6570  ly build and dep
+000056a0: 6c6f 7920 4d4c 2d70 6f77 6572 6564 2061  loy ML-powered a
+000056b0: 7070 6c69 6361 7469 6f6e 732e 222c 0a20  pplications.",. 
+000056c0: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
+000056d0: 205b 0a20 2020 2020 2020 2020 205b 7b20   [.          [{ 
+000056e0: 224c 4f57 4552 223a 207b 2022 4655 5a5a  "LOWER": { "FUZZ
+000056f0: 5931 223a 2022 7465 6e7a 666c 6f77 2220  Y1": "tenzflow" 
+00005700: 7d20 7d5d 2c0a 2020 2020 2020 2020 2020  } }],.          
+00005710: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
+00005720: 555a 5a59 3122 3a20 2274 656e 736f 7266  UZZY1": "tensorf
+00005730: 6c6f 7722 207d 207d 5d0a 2020 2020 2020  low" } }].      
+00005740: 5d2c 0a20 2020 2020 2022 7363 6f72 6522  ],.      "score"
+00005750: 3a20 3130 0a20 207d 2c0a 2020 2250 7954  : 10.  },.  "PyT
+00005760: 6f72 6368 223a 207b 0a20 2020 2020 2022  orch": {.      "
+00005770: 7479 7065 223a 2022 4c69 6272 6172 7922  type": "Library"
+00005780: 2c0a 2020 2020 2020 2263 6174 6567 6f72  ,.      "categor
+00005790: 7922 3a20 224d 6163 6869 6e65 204c 6561  y": "Machine Lea
+000057a0: 726e 696e 6722 2c0a 2020 2020 2020 2264  rning",.      "d
+000057b0: 6573 6372 6970 7469 6f6e 223a 2022 5079  escription": "Py
+000057c0: 546f 7263 6820 6973 2061 6e20 6f70 656e  Torch is an open
+000057d0: 2d73 6f75 7263 6520 6d61 6368 696e 6520  -source machine 
+000057e0: 6c65 6172 6e69 6e67 206c 6962 7261 7279  learning library
+000057f0: 2062 6173 6564 206f 6e20 7468 6520 546f   based on the To
+00005800: 7263 6820 6c69 6272 6172 792c 2075 7365  rch library, use
+00005810: 6420 666f 7220 6170 706c 6963 6174 696f  d for applicatio
+00005820: 6e73 2073 7563 6820 6173 2063 6f6d 7075  ns such as compu
+00005830: 7465 7220 7669 7369 6f6e 2061 6e64 206e  ter vision and n
+00005840: 6174 7572 616c 206c 616e 6775 6167 6520  atural language 
+00005850: 7072 6f63 6573 7369 6e67 2c20 7072 696d  processing, prim
+00005860: 6172 696c 7920 6465 7665 6c6f 7065 6420  arily developed 
+00005870: 6279 2046 6163 6562 6f6f 6b27 7320 4149  by Facebook's AI
+00005880: 2052 6573 6561 7263 6820 6c61 6220 2846   Research lab (F
+00005890: 4149 5229 2e22 2c0a 2020 2020 2020 2270  AIR).",.      "p
+000058a0: 6174 7465 726e 7322 3a20 5b5b 7b20 224c  atterns": [[{ "L
+000058b0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
+000058c0: 223a 2022 7079 746f 7263 6822 207d 207d  ": "pytorch" } }
+000058d0: 5d5d 2c0a 2020 2020 2020 2273 636f 7265  ]],.      "score
+000058e0: 223a 2031 300a 2020 7d2c 0a20 2022 5363  ": 10.  },.  "Sc
+000058f0: 696b 6974 2d6c 6561 726e 223a 207b 0a20  ikit-learn": {. 
+00005900: 2020 2020 2022 7479 7065 223a 2022 4c69       "type": "Li
+00005910: 6272 6172 7922 2c0a 2020 2020 2020 2263  brary",.      "c
+00005920: 6174 6567 6f72 7922 3a20 224d 6163 6869  ategory": "Machi
+00005930: 6e65 204c 6561 726e 696e 6722 2c0a 2020  ne Learning",.  
+00005940: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005950: 223a 2022 5363 696b 6974 2d6c 6561 726e  ": "Scikit-learn
+00005960: 2069 7320 6120 6672 6565 2073 6f66 7477   is a free softw
+00005970: 6172 6520 6d61 6368 696e 6520 6c65 6172  are machine lear
+00005980: 6e69 6e67 206c 6962 7261 7279 2066 6f72  ning library for
+00005990: 2074 6865 2050 7974 686f 6e20 7072 6f67   the Python prog
+000059a0: 7261 6d6d 696e 6720 6c61 6e67 7561 6765  ramming language
+000059b0: 2e20 4974 2066 6561 7475 7265 7320 7661  . It features va
+000059c0: 7269 6f75 7320 636c 6173 7369 6669 6361  rious classifica
+000059d0: 7469 6f6e 2c20 7265 6772 6573 7369 6f6e  tion, regression
+000059e0: 2c20 616e 6420 636c 7573 7465 7269 6e67  , and clustering
+000059f0: 2061 6c67 6f72 6974 686d 7320 696e 636c   algorithms incl
+00005a00: 7564 696e 6720 7375 7070 6f72 7420 7665  uding support ve
+00005a10: 6374 6f72 206d 6163 6869 6e65 732c 2072  ctor machines, r
+00005a20: 616e 646f 6d20 666f 7265 7374 732c 2067  andom forests, g
+00005a30: 7261 6469 656e 7420 626f 6f73 7469 6e67  radient boosting
+00005a40: 2c20 6b2d 6d65 616e 732c 2061 6e64 2044  , k-means, and D
+00005a50: 4253 4341 4e2e 222c 0a20 2020 2020 2022  BSCAN.",.      "
+00005a60: 7061 7474 6572 6e73 223a 205b 0a20 2020  patterns": [.   
+00005a70: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+00005a80: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+00005a90: 7363 696b 6974 2d6c 6561 726e 2220 7d20  scikit-learn" } 
+00005aa0: 7d5d 2c0a 2020 2020 2020 2020 2020 5b7b  }],.          [{
+00005ab0: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
+00005ac0: 5a59 3122 3a20 2273 6b6c 6561 726e 2220  ZY1": "sklearn" 
+00005ad0: 7d20 7d5d 0a20 2020 2020 205d 2c0a 2020  } }].      ],.  
+00005ae0: 2020 2020 2273 636f 7265 223a 2039 0a20      "score": 9. 
+00005af0: 207d 2c0a 2020 2241 7061 6368 6520 4b61   },.  "Apache Ka
+00005b00: 666b 6122 3a20 7b0a 2020 2020 2020 2274  fka": {.      "t
+00005b10: 7970 6522 3a20 2242 6967 2044 6174 6120  ype": "Big Data 
+00005b20: 546f 6f6c 222c 0a20 2020 2020 2022 6361  Tool",.      "ca
+00005b30: 7465 676f 7279 223a 2022 4d65 7373 6167  tegory": "Messag
+00005b40: 6520 5374 7265 616d 696e 6722 2c0a 2020  e Streaming",.  
+00005b50: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005b60: 223a 2022 4170 6163 6865 204b 6166 6b61  ": "Apache Kafka
+00005b70: 2069 7320 616e 206f 7065 6e2d 736f 7572   is an open-sour
+00005b80: 6365 2073 7472 6561 6d2d 7072 6f63 6573  ce stream-proces
+00005b90: 7369 6e67 2073 6f66 7477 6172 6520 706c  sing software pl
+00005ba0: 6174 666f 726d 2064 6576 656c 6f70 6564  atform developed
+00005bb0: 2062 7920 4c69 6e6b 6564 496e 2061 6e64   by LinkedIn and
+00005bc0: 2064 6f6e 6174 6564 2074 6f20 7468 6520   donated to the 
+00005bd0: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+00005be0: 466f 756e 6461 7469 6f6e 2c20 7772 6974  Foundation, writ
+00005bf0: 7465 6e20 696e 2053 6361 6c61 2061 6e64  ten in Scala and
+00005c00: 204a 6176 612e 2054 6865 2070 726f 6a65   Java. The proje
+00005c10: 6374 2061 696d 7320 746f 2070 726f 7669  ct aims to provi
+00005c20: 6465 2061 2075 6e69 6669 6564 2c20 6869  de a unified, hi
+00005c30: 6768 2d74 6872 6f75 6768 7075 742c 206c  gh-throughput, l
+00005c40: 6f77 2d6c 6174 656e 6379 2070 6c61 7466  ow-latency platf
+00005c50: 6f72 6d20 666f 7220 6861 6e64 6c69 6e67  orm for handling
+00005c60: 2072 6561 6c2d 7469 6d65 2064 6174 6120   real-time data 
+00005c70: 6665 6564 732e 222c 0a20 2020 2020 2022  feeds.",.      "
+00005c80: 7061 7474 6572 6e73 223a 205b 0a20 2020  patterns": [.   
+00005c90: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+00005ca0: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+00005cb0: 6170 6163 6865 206b 6166 6b61 2220 7d20  apache kafka" } 
+00005cc0: 7d5d 2c0a 2020 2020 2020 2020 2020 5b7b  }],.          [{
+00005cd0: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
+00005ce0: 5a59 3122 3a20 226b 6166 6b61 2220 7d20  ZY1": "kafka" } 
+00005cf0: 7d5d 0a20 2020 2020 205d 2c0a 2020 2020  }].      ],.    
+00005d00: 2020 2273 636f 7265 223a 2039 0a20 207d    "score": 9.  }
+00005d10: 2c0a 2020 2252 6162 6269 744d 5122 3a20  ,.  "RabbitMQ": 
+00005d20: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+00005d30: 224d 6964 646c 6577 6172 6522 2c0a 2020  "Middleware",.  
+00005d40: 2020 2020 2263 6174 6567 6f72 7922 3a20      "category": 
+00005d50: 224d 6573 7361 6765 2042 726f 6b65 7222  "Message Broker"
+00005d60: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
+00005d70: 7469 6f6e 223a 2022 5261 6262 6974 4d51  tion": "RabbitMQ
+00005d80: 2069 7320 616e 206f 7065 6e2d 736f 7572   is an open-sour
+00005d90: 6365 206d 6573 7361 6765 2d62 726f 6b65  ce message-broke
+00005da0: 7220 736f 6674 7761 7265 2074 6861 7420  r software that 
+00005db0: 6f72 6967 696e 616c 6c79 2069 6d70 6c65  originally imple
+00005dc0: 6d65 6e74 6564 2074 6865 2041 6476 616e  mented the Advan
+00005dd0: 6365 6420 4d65 7373 6167 6520 5175 6575  ced Message Queu
+00005de0: 696e 6720 5072 6f74 6f63 6f6c 2028 414d  ing Protocol (AM
+00005df0: 5150 2920 616e 6420 6861 7320 7369 6e63  QP) and has sinc
+00005e00: 6520 6265 656e 2065 7874 656e 6465 6420  e been extended 
+00005e10: 7769 7468 2061 2070 6c75 672d 696e 2061  with a plug-in a
+00005e20: 7263 6869 7465 6374 7572 6520 746f 2073  rchitecture to s
+00005e30: 7570 706f 7274 2053 7472 6561 6d69 6e67  upport Streaming
+00005e40: 2054 6578 7420 4f72 6965 6e74 6564 204d   Text Oriented M
+00005e50: 6573 7361 6769 6e67 2050 726f 746f 636f  essaging Protoco
+00005e60: 6c20 2853 544f 4d50 292c 204d 5154 542c  l (STOMP), MQTT,
+00005e70: 2061 6e64 206f 7468 6572 2070 726f 746f   and other proto
+00005e80: 636f 6c73 2e22 2c0a 2020 2020 2020 2270  cols.",.      "p
+00005e90: 6174 7465 726e 7322 3a20 5b5b 7b20 224c  atterns": [[{ "L
+00005ea0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
+00005eb0: 223a 2022 7261 6262 6974 6d71 2220 7d20  ": "rabbitmq" } 
+00005ec0: 7d5d 5d2c 0a20 2020 2020 2022 7363 6f72  }]],.      "scor
+00005ed0: 6522 3a20 382e 350a 2020 7d2c 0a20 2022  e": 8.5.  },.  "
+00005ee0: 4861 646f 6f70 223a 207b 0a20 2020 2020  Hadoop": {.     
+00005ef0: 2022 7479 7065 223a 2022 4672 616d 6577   "type": "Framew
+00005f00: 6f72 6b22 2c0a 2020 2020 2020 2263 6174  ork",.      "cat
+00005f10: 6567 6f72 7922 3a20 2242 6967 2044 6174  egory": "Big Dat
+00005f20: 6120 5072 6f63 6573 7369 6e67 222c 0a20  a Processing",. 
+00005f30: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00005f40: 6e22 3a20 2241 7061 6368 6520 4861 646f  n": "Apache Hado
+00005f50: 6f70 2069 7320 6120 636f 6c6c 6563 7469  op is a collecti
+00005f60: 6f6e 206f 6620 6f70 656e 2d73 6f75 7263  on of open-sourc
+00005f70: 6520 736f 6674 7761 7265 2075 7469 6c69  e software utili
+00005f80: 7469 6573 2074 6861 7420 6661 6369 6c69  ties that facili
+00005f90: 7461 7465 2075 7369 6e67 2061 206e 6574  tate using a net
+00005fa0: 776f 726b 206f 6620 6d61 6e79 2063 6f6d  work of many com
+00005fb0: 7075 7465 7273 2074 6f20 736f 6c76 6520  puters to solve 
+00005fc0: 7072 6f62 6c65 6d73 2069 6e76 6f6c 7669  problems involvi
+00005fd0: 6e67 206d 6173 7369 7665 2061 6d6f 756e  ng massive amoun
+00005fe0: 7473 206f 6620 6461 7461 2061 6e64 2063  ts of data and c
+00005ff0: 6f6d 7075 7461 7469 6f6e 2e20 4974 2070  omputation. It p
+00006000: 726f 7669 6465 7320 6120 736f 6674 7761  rovides a softwa
+00006010: 7265 2066 7261 6d65 776f 726b 2066 6f72  re framework for
+00006020: 2064 6973 7472 6962 7574 6564 2073 746f   distributed sto
+00006030: 7261 6765 2061 6e64 2070 726f 6365 7373  rage and process
+00006040: 696e 6720 6f66 2062 6967 2064 6174 6120  ing of big data 
+00006050: 7573 696e 6720 7468 6520 4d61 7052 6564  using the MapRed
+00006060: 7563 6520 7072 6f67 7261 6d6d 696e 6720  uce programming 
+00006070: 6d6f 6465 6c2e 222c 0a20 2020 2020 2022  model.",.      "
+00006080: 7061 7474 6572 6e73 223a 205b 0a20 2020  patterns": [.   
+00006090: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+000060a0: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+000060b0: 6170 6163 6865 2068 6164 6f6f 7022 207d  apache hadoop" }
+000060c0: 207d 5d2c 0a20 2020 2020 2020 2020 205b   }],.          [
+000060d0: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+000060e0: 5a5a 5931 223a 2022 6861 646f 6f70 2220  ZZY1": "hadoop" 
+000060f0: 7d20 7d5d 0a20 2020 2020 205d 2c0a 2020  } }].      ],.  
+00006100: 2020 2020 2273 636f 7265 223a 2038 0a20      "score": 8. 
+00006110: 207d 2c0a 0a20 2022 5573 6572 2049 6e74   },..  "User Int
+00006120: 6572 6661 6365 223a 207b 0a20 2020 2020  erface": {.     
+00006130: 2022 7479 7065 223a 2022 4672 6f6e 7465   "type": "Fronte
+00006140: 6e64 222c 0a20 2020 2020 2022 6361 7465  nd",.      "cate
+00006150: 676f 7279 223a 2022 5265 7175 6972 656d  gory": "Requirem
+00006160: 656e 7422 2c0a 2020 2020 2020 2272 656c  ent",.      "rel
+00006170: 6174 6564 5465 6368 6e6f 6c6f 6769 6573  atedTechnologies
+00006180: 223a 205b 0a20 2020 2020 2020 2020 2022  ": [.          "
+00006190: 5675 6522 2c0a 2020 2020 2020 2020 2020  Vue",.          
+000061a0: 2252 6561 6374 222c 0a20 2020 2020 2020  "React",.       
+000061b0: 2020 2022 416e 6775 6c61 7222 2c0a 2020     "Angular",.  
+000061c0: 2020 2020 2020 2020 2242 6f6f 7473 7472          "Bootstr
+000061d0: 6170 222c 0a20 2020 2020 2020 2020 2022  ap",.          "
+000061e0: 4d61 7465 7269 616c 2d55 4922 2c0a 2020  Material-UI",.  
+000061f0: 2020 2020 2020 2020 2254 6169 6c77 696e          "Tailwin
+00006200: 6420 4353 5322 0a20 2020 2020 205d 2c0a  d CSS".      ],.
+00006210: 2020 2020 2020 2270 6174 7465 726e 7322        "patterns"
+00006220: 3a20 5b0a 2020 2020 2020 2020 2020 5b7b  : [.          [{
+00006230: 2022 4c4f 5745 5222 3a20 2275 6922 207d   "LOWER": "ui" }
+00006240: 5d2c 0a20 2020 2020 2020 2020 205b 7b20  ],.          [{ 
+00006250: 224c 4f57 4552 223a 2022 7573 6572 2220  "LOWER": "user" 
+00006260: 7d2c 207b 2022 4c4f 5745 5222 3a20 7b20  }, { "LOWER": { 
+00006270: 2246 555a 5a59 3122 3a20 2269 6e74 6572  "FUZZY1": "inter
+00006280: 6661 6365 2220 7d20 7d5d 2c0a 2020 2020  face" } }],.    
+00006290: 2020 2020 2020 5b7b 2022 4c4f 5745 5222        [{ "LOWER"
+000062a0: 3a20 7b20 2246 555a 5a59 3122 3a20 2272  : { "FUZZY1": "r
+000062b0: 6573 706f 6e73 6976 6522 207d 207d 5d0a  esponsive" } }].
+000062c0: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
+000062d0: 6465 7363 7269 7074 696f 6e22 3a20 2252  description": "R
+000062e0: 6566 6572 7320 746f 2074 6865 2064 6573  efers to the des
+000062f0: 6967 6e20 616e 6420 6c61 796f 7574 206f  ign and layout o
+00006300: 6620 7468 6520 696e 7465 7266 6163 6520  f the interface 
+00006310: 7468 726f 7567 6820 7768 6963 6820 7573  through which us
+00006320: 6572 7320 696e 7465 7261 6374 2077 6974  ers interact wit
+00006330: 6820 7765 6220 6170 706c 6963 6174 696f  h web applicatio
+00006340: 6e73 2e20 5468 6973 2074 7970 6963 616c  ns. This typical
+00006350: 6c79 2069 6e76 6f6c 7665 7320 7465 6368  ly involves tech
+00006360: 6e6f 6c6f 6769 6573 2066 6f72 2062 7569  nologies for bui
+00006370: 6c64 696e 6720 7573 6572 2069 6e74 6572  lding user inter
+00006380: 6661 6365 732c 2073 7563 6820 6173 204a  faces, such as J
+00006390: 6176 6153 6372 6970 7420 6672 616d 6577  avaScript framew
+000063a0: 6f72 6b73 2f6c 6962 7261 7269 6573 2061  orks/libraries a
+000063b0: 6e64 2055 4920 636f 6d70 6f6e 656e 7420  nd UI component 
+000063c0: 6c69 6272 6172 6965 732e 222c 0a20 2020  libraries.",.   
+000063d0: 2020 2022 7363 6f72 6522 3a20 350a 2020     "score": 5.  
+000063e0: 7d2c 0a20 2022 5245 5354 2041 5049 2044  },.  "REST API D
+000063f0: 6576 656c 6f70 6d65 6e74 223a 207b 0a20  evelopment": {. 
+00006400: 2020 2020 2022 7479 7065 223a 2022 4150       "type": "AP
+00006410: 4920 4465 7369 676e 222c 0a20 2020 2020  I Design",.     
+00006420: 2022 6361 7465 676f 7279 223a 2022 5265   "category": "Re
+00006430: 7175 6972 656d 656e 7422 2c0a 2020 2020  quirement",.    
+00006440: 2020 2272 656c 6174 6564 5465 6368 6e6f    "relatedTechno
+00006450: 6c6f 6769 6573 223a 205b 0a20 2020 2020  logies": [.     
+00006460: 2020 2020 2022 4578 7072 6573 732e 6a73       "Express.js
+00006470: 222c 0a20 2020 2020 2020 2020 2022 4661  ",.          "Fa
+00006480: 7374 4150 4922 2c0a 2020 2020 2020 2020  stAPI",.        
+00006490: 2020 2244 6a61 6e67 6f22 2c0a 2020 2020    "Django",.    
+000064a0: 2020 2020 2020 2246 6c61 736b 222c 0a20        "Flask",. 
+000064b0: 2020 2020 2020 2020 2022 4153 502e 4e45           "ASP.NE
+000064c0: 5422 2c0a 2020 2020 2020 2020 2020 2253  T",.          "S
+000064d0: 7072 696e 6722 0a20 2020 2020 205d 2c0a  pring".      ],.
+000064e0: 2020 2020 2020 2270 6174 7465 726e 7322        "patterns"
+000064f0: 3a20 5b0a 2020 2020 2020 2020 2020 5b7b  : [.          [{
+00006500: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
+00006510: 5a59 3122 3a20 2272 6573 7466 756c 2220  ZY1": "restful" 
+00006520: 7d20 7d5d 2c0a 2020 2020 2020 2020 2020  } }],.          
+00006530: 5b7b 2022 4c4f 5745 5222 3a20 2272 6573  [{ "LOWER": "res
+00006540: 7422 207d 2c20 7b20 224c 4f57 4552 223a  t" }, { "LOWER":
+00006550: 2022 6170 6922 207d 5d2c 0a20 2020 2020   "api" }],.     
+00006560: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
+00006570: 2022 7265 7374 2220 7d5d 0a20 2020 2020   "rest" }].     
+00006580: 205d 2c0a 2020 2020 2020 2264 6573 6372   ],.      "descr
+00006590: 6970 7469 6f6e 223a 2022 5468 6520 7072  iption": "The pr
+000065a0: 6f63 6573 7320 6f66 2064 6576 656c 6f70  ocess of develop
+000065b0: 696e 6720 6170 706c 6963 6174 696f 6e20  ing application 
+000065c0: 7072 6f67 7261 6d6d 696e 6720 696e 7465  programming inte
+000065d0: 7266 6163 6573 2028 4150 4973 2920 666f  rfaces (APIs) fo
+000065e0: 6c6c 6f77 696e 6720 7468 6520 5265 7072  llowing the Repr
+000065f0: 6573 656e 7461 7469 6f6e 616c 2053 7461  esentational Sta
+00006600: 7465 2054 7261 6e73 6665 7220 2852 4553  te Transfer (RES
+00006610: 5429 2061 7263 6869 7465 6374 7572 616c  T) architectural
+00006620: 2073 7479 6c65 2c20 656e 6162 6c69 6e67   style, enabling
+00006630: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2062   communication b
+00006640: 6574 7765 656e 2064 6966 6665 7265 6e74  etween different
+00006650: 2073 6f66 7477 6172 6520 6170 706c 6963   software applic
+00006660: 6174 696f 6e73 2e22 2c0a 2020 2020 2020  ations.",.      
+00006670: 2273 636f 7265 223a 2035 0a20 207d 2c0a  "score": 5.  },.
+00006680: 2020 2252 4442 4d53 223a 207b 0a20 2020    "RDBMS": {.   
+00006690: 2020 2022 7479 7065 223a 2022 5265 6c61     "type": "Rela
+000066a0: 7469 6f6e 616c 2044 6174 6162 6173 6520  tional Database 
+000066b0: 4d6f 6465 6c22 2c0a 2020 2020 2020 2263  Model",.      "c
+000066c0: 6174 6567 6f72 7922 3a20 2252 6571 7569  ategory": "Requi
+000066d0: 7265 6d65 6e74 222c 0a20 2020 2020 2022  rement",.      "
+000066e0: 7265 6c61 7465 6454 6563 686e 6f6c 6f67  relatedTechnolog
+000066f0: 6965 7322 3a20 5b22 4d79 5351 4c22 2c20  ies": ["MySQL", 
+00006700: 2250 6f73 7467 7265 5351 4c22 2c20 224d  "PostgreSQL", "M
+00006710: 6172 6961 4442 222c 2022 4f72 6163 6c65  ariaDB", "Oracle
+00006720: 4442 225d 2c0a 2020 2020 2020 2264 6573  DB"],.      "des
+00006730: 6372 6970 7469 6f6e 223a 2022 4120 7479  cription": "A ty
+00006740: 7065 206f 6620 6461 7461 6261 7365 2073  pe of database s
+00006750: 7973 7465 6d20 7468 6174 2073 746f 7265  ystem that store
+00006760: 7320 6461 7461 2069 6e20 7461 626c 6573  s data in tables
+00006770: 2c20 6f72 6761 6e69 7a65 6420 6279 2072  , organized by r
+00006780: 6f77 7320 616e 6420 636f 6c75 6d6e 732c  ows and columns,
+00006790: 2066 6f6c 6c6f 7769 6e67 2074 6865 2072   following the r
+000067a0: 656c 6174 696f 6e61 6c20 6d6f 6465 6c2e  elational model.
+000067b0: 2052 4442 4d53 2070 726f 7669 6465 7320   RDBMS provides 
+000067c0: 6120 7374 7275 6374 7572 6564 2061 7070  a structured app
+000067d0: 726f 6163 6820 746f 206d 616e 6167 696e  roach to managin
+000067e0: 6720 6461 7461 2c20 656e 7375 7269 6e67  g data, ensuring
+000067f0: 2069 6e74 6567 7269 7479 2061 6e64 2063   integrity and c
+00006800: 6f6e 7369 7374 656e 6379 2074 6872 6f75  onsistency throu
+00006810: 6768 2041 4349 4420 7072 6f70 6572 7469  gh ACID properti
+00006820: 6573 2e22 2c0a 2020 2020 2020 2270 6174  es.",.      "pat
+00006830: 7465 726e 7322 3a20 5b0a 2020 2020 2020  terns": [.      
+00006840: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
+00006850: 7b20 2246 555a 5a59 3122 3a20 2272 656c  { "FUZZY1": "rel
+00006860: 6174 696f 6e61 6c22 207d 207d 2c20 7b20  ational" } }, { 
+00006870: 224c 4f57 4552 223a 207b 2022 4655 5a5a  "LOWER": { "FUZZ
+00006880: 5931 223a 2022 6461 7461 6261 7365 2220  Y1": "database" 
+00006890: 7d20 7d5d 2c0a 2020 2020 2020 2020 2020  } }],.          
+000068a0: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
+000068b0: 555a 5a59 3122 3a20 2272 656c 6174 696f  UZZY1": "relatio
+000068c0: 6e61 6c22 207d 207d 2c20 7b20 224c 4f57  nal" } }, { "LOW
+000068d0: 4552 223a 2022 6462 2220 7d5d 2c0a 2020  ER": "db" }],.  
+000068e0: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
+000068f0: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
+00006900: 2272 6462 6d73 2220 7d20 7d5d 2c0a 2020  "rdbms" } }],.  
+00006910: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
+00006920: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
+00006930: 2272 656c 6174 696f 6e61 6c22 207d 207d  "relational" } }
+00006940: 5d0a 2020 2020 2020 5d2c 0a20 2020 2020  ].      ],.     
+00006950: 2022 7363 6f72 6522 3a20 350a 2020 7d2c   "score": 5.  },
+00006960: 0a20 2022 4e6f 5351 4c22 3a20 7b0a 2020  .  "NoSQL": {.  
+00006970: 2020 2020 2274 7970 6522 3a20 224e 6f6e      "type": "Non
+00006980: 2d52 656c 6174 696f 6e61 6c20 4461 7461  -Relational Data
+00006990: 6261 7365 204d 6f64 656c 222c 0a20 2020  base Model",.   
+000069a0: 2020 2022 6361 7465 676f 7279 223a 2022     "category": "
+000069b0: 5265 7175 6972 656d 656e 7422 2c0a 2020  Requirement",.  
+000069c0: 2020 2020 2272 656c 6174 6564 5465 6368      "relatedTech
+000069d0: 6e6f 6c6f 6769 6573 223a 205b 224d 6f6e  nologies": ["Mon
+000069e0: 676f 4442 222c 2022 4170 6163 6865 2043  goDB", "Apache C
+000069f0: 6173 7361 6e64 7261 225d 2c0a 2020 2020  assandra"],.    
+00006a00: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00006a10: 2022 4120 636f 6c6c 6563 7469 6f6e 206f   "A collection o
+00006a20: 6620 6e6f 6e2d 7265 6c61 7469 6f6e 616c  f non-relational
+00006a30: 2064 6174 6120 6d6f 6465 6c73 2074 6861   data models tha
+00006a40: 7420 646f 206e 6f74 2066 6f6c 6c6f 7720  t do not follow 
+00006a50: 7468 6520 7472 6164 6974 696f 6e61 6c20  the traditional 
+00006a60: 7461 6275 6c61 7220 7363 6865 6d61 2c20  tabular schema, 
+00006a70: 656d 7068 6173 697a 696e 6720 7363 616c  emphasizing scal
+00006a80: 6162 696c 6974 792c 2061 6769 6c69 7479  ability, agility
+00006a90: 2c20 616e 6420 6164 6170 7461 6269 6c69  , and adaptabili
+00006aa0: 7479 2e20 4e6f 5351 4c20 6461 7461 6261  ty. NoSQL databa
+00006ab0: 7365 7320 6172 6520 6465 7369 676e 6564  ses are designed
+00006ac0: 2074 6f20 6861 6e64 6c65 206c 6172 6765   to handle large
+00006ad0: 2076 6f6c 756d 6573 206f 6620 756e 7374   volumes of unst
+00006ae0: 7275 6374 7572 6564 206f 7220 7365 6d69  ructured or semi
+00006af0: 2d73 7472 7563 7475 7265 6420 6461 7461  -structured data
+00006b00: 2e22 2c0a 2020 2020 2020 2270 6174 7465  .",.      "patte
+00006b10: 726e 7322 3a20 5b0a 2020 2020 2020 2020  rns": [.        
+00006b20: 2020 5b7b 2022 4c4f 5745 5222 3a20 7b20    [{ "LOWER": { 
+00006b30: 2246 555a 5a59 3122 3a20 226e 6f73 716c  "FUZZY1": "nosql
+00006b40: 2220 7d20 7d5d 2c0a 2020 2020 2020 2020  " } }],.        
+00006b50: 2020 5b7b 2022 4c4f 5745 5222 3a20 7b20    [{ "LOWER": { 
+00006b60: 2246 555a 5a59 3122 3a20 226e 6f6e 2d72  "FUZZY1": "non-r
+00006b70: 656c 6174 696f 6e61 6c22 207d 207d 2c20  elational" } }, 
+00006b80: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+00006b90: 5a5a 5931 223a 2022 6461 7461 6261 7365  ZZY1": "database
+00006ba0: 2220 7d20 7d5d 0a20 2020 2020 205d 2c0a  " } }].      ],.
+00006bb0: 2020 2020 2020 2273 636f 7265 223a 2035        "score": 5
+00006bc0: 0a20 207d 2c0a 0a20 2022 436c 6f75 6420  .  },..  "Cloud 
+00006bd0: 4465 706c 6f79 6d65 6e74 223a 207b 0a20  Deployment": {. 
+00006be0: 2020 2020 2022 7479 7065 223a 2022 4465       "type": "De
+00006bf0: 706c 6f79 6d65 6e74 222c 0a20 2020 2020  ployment",.     
+00006c00: 2022 6361 7465 676f 7279 223a 2022 5265   "category": "Re
+00006c10: 7175 6972 656d 656e 7422 2c0a 2020 2020  quirement",.    
+00006c20: 2020 2272 656c 6174 6564 5465 6368 6e6f    "relatedTechno
+00006c30: 6c6f 6769 6573 223a 205b 2241 5753 222c  logies": ["AWS",
+00006c40: 2022 417a 7572 6522 2c20 2247 6f6f 676c   "Azure", "Googl
+00006c50: 6543 6c6f 7564 225d 2c0a 2020 2020 2020  eCloud"],.      
+00006c60: 2270 6174 7465 726e 7322 3a20 5b0a 2020  "patterns": [.  
+00006c70: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
+00006c80: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
+00006c90: 2263 6c6f 7564 2220 7d7d 2c20 7b20 224c  "cloud" }}, { "L
+00006ca0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
+00006cb0: 223a 2022 6465 706c 6f79 6d65 6e74 2220  ": "deployment" 
+00006cc0: 7d20 7d5d 2c0a 2020 2020 2020 2020 2020  } }],.          
+00006cd0: 5b7b 2022 4c4f 5745 5222 3a20 7b20 2246  [{ "LOWER": { "F
+00006ce0: 555a 5a59 3122 3a20 2263 6c6f 7564 2220  UZZY1": "cloud" 
+00006cf0: 7d7d 2c20 7b20 224c 4f57 4552 223a 207b  }}, { "LOWER": {
+00006d00: 2022 4655 5a5a 5931 223a 2022 7072 6f76   "FUZZY1": "prov
+00006d10: 6964 6572 2220 7d20 7d5d 0a20 2020 2020  ider" } }].     
+00006d20: 205d 2c0a 2020 2020 2020 2264 6573 6372   ],.      "descr
+00006d30: 6970 7469 6f6e 223a 2022 5468 6520 7072  iption": "The pr
+00006d40: 6f63 6573 7320 6f66 2064 6570 6c6f 7969  ocess of deployi
+00006d50: 6e67 2061 7070 6c69 6361 7469 6f6e 732c  ng applications,
+00006d60: 2073 6572 7669 6365 732c 206f 7220 7265   services, or re
+00006d70: 736f 7572 6365 7320 6f6e 2061 2063 6c6f  sources on a clo
+00006d80: 7564 2070 6c61 7466 6f72 6d20 7072 6f76  ud platform prov
+00006d90: 6964 6564 2062 7920 6120 636c 6f75 6420  ided by a cloud 
+00006da0: 7365 7276 6963 6520 7072 6f76 6964 6572  service provider
+00006db0: 2e20 436c 6f75 6420 6465 706c 6f79 6d65  . Cloud deployme
+00006dc0: 6e74 206f 6666 6572 7320 7363 616c 6162  nt offers scalab
+00006dd0: 696c 6974 792c 2066 6c65 7869 6269 6c69  ility, flexibili
+00006de0: 7479 2c20 616e 6420 7265 6475 6365 6420  ty, and reduced 
+00006df0: 696e 6672 6173 7472 7563 7475 7265 206d  infrastructure m
+00006e00: 6169 6e74 656e 616e 6365 2e22 2c0a 2020  aintenance.",.  
+00006e10: 2020 2020 2273 636f 7265 223a 2035 0a20      "score": 5. 
+00006e20: 207d 2c0a 2020 2256 6572 7369 6f6e 2043   },.  "Version C
+00006e30: 6f6e 7472 6f6c 2053 7973 7465 6d22 3a20  ontrol System": 
+00006e40: 7b0a 2020 2020 2020 2274 7970 6522 3a20  {.      "type": 
+00006e50: 2244 6576 4f70 7320 5072 6163 7469 6365  "DevOps Practice
+00006e60: 7322 2c0a 2020 2020 2020 2263 6174 6567  s",.      "categ
+00006e70: 6f72 7922 3a20 2252 6571 7569 7265 6d65  ory": "Requireme
+00006e80: 6e74 222c 0a20 2020 2020 2022 7265 6c61  nt",.      "rela
+00006e90: 7465 6454 6563 686e 6f6c 6f67 6965 7322  tedTechnologies"
+00006ea0: 3a20 5b22 4769 7448 7562 225d 2c0a 2020  : ["GitHub"],.  
+00006eb0: 2020 2020 2270 6174 7465 726e 7322 3a20      "patterns": 
+00006ec0: 5b0a 2020 2020 2020 2020 2020 5b0a 2020  [.          [.  
+00006ed0: 2020 2020 2020 2020 2020 2020 7b20 224c              { "L
+00006ee0: 4f57 4552 223a 207b 2022 4655 5a5a 5931  OWER": { "FUZZY1
+00006ef0: 223a 2022 7665 7273 696f 6e22 207d 207d  ": "version" } }
+00006f00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006f10: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+00006f20: 5a5a 5931 223a 2022 636f 6e74 726f 6c22  ZZY1": "control"
+00006f30: 207d 207d 0a20 2020 2020 2020 2020 205d   } }.          ]
+00006f40: 2c0a 2020 2020 2020 2020 2020 5b7b 2022  ,.          [{ "
+00006f50: 4c4f 5745 5222 3a20 2267 6974 2220 7d5d  LOWER": "git" }]
+00006f60: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
+00006f70: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00006f80: 4120 7379 7374 656d 2074 6861 7420 7265  A system that re
+00006f90: 636f 7264 7320 6368 616e 6765 7320 746f  cords changes to
+00006fa0: 2061 2066 696c 6520 6f72 2073 6574 206f   a file or set o
+00006fb0: 6620 6669 6c65 7320 6f76 6572 2074 696d  f files over tim
+00006fc0: 652c 2061 6c6c 6f77 696e 6720 6465 7665  e, allowing deve
+00006fd0: 6c6f 7065 7273 2074 6f20 636f 6c6c 6162  lopers to collab
+00006fe0: 6f72 6174 6520 6f6e 2063 6f64 652c 2074  orate on code, t
+00006ff0: 7261 636b 2063 6861 6e67 6573 2c20 616e  rack changes, an
+00007000: 6420 7265 7665 7274 2074 6f20 7072 6576  d revert to prev
+00007010: 696f 7573 2076 6572 7369 6f6e 7320 6966  ious versions if
+00007020: 206e 6565 6465 642e 2056 6572 7369 6f6e   needed. Version
+00007030: 2063 6f6e 7472 6f6c 2073 7973 7465 6d73   control systems
+00007040: 206c 696b 6520 4769 7420 706c 6179 2061   like Git play a
+00007050: 2063 7275 6369 616c 2072 6f6c 6520 696e   crucial role in
+00007060: 2073 6f66 7477 6172 6520 6465 7665 6c6f   software develo
+00007070: 706d 656e 7420 776f 726b 666c 6f77 732e  pment workflows.
+00007080: 222c 0a20 2020 2020 2022 7363 6f72 6522  ",.      "score"
+00007090: 3a20 350a 2020 7d2c 0a20 2022 4349 2f43  : 5.  },.  "CI/C
+000070a0: 4422 3a20 7b0a 2020 2020 2020 2274 7970  D": {.      "typ
+000070b0: 6522 3a20 2244 6576 4f70 7320 5072 6163  e": "DevOps Prac
+000070c0: 7469 6365 7322 2c0a 2020 2020 2020 2263  tices",.      "c
+000070d0: 6174 6567 6f72 7922 3a20 2252 6571 7569  ategory": "Requi
+000070e0: 7265 6d65 6e74 222c 0a20 2020 2020 2022  rement",.      "
+000070f0: 7265 6c61 7465 6454 6563 686e 6f6c 6f67  relatedTechnolog
+00007100: 6965 7322 3a20 5b22 4769 7448 7562 2041  ies": ["GitHub A
+00007110: 6374 696f 6e73 222c 224a 656e 6b69 6e73  ctions","Jenkins
+00007120: 222c 2243 6972 636c 6543 4922 5d2c 0a20  ","CircleCI"],. 
+00007130: 2020 2020 2022 7061 7474 6572 6e73 223a       "patterns":
+00007140: 205b 0a20 2020 2020 2020 2020 205b 0a20   [.          [. 
+00007150: 2020 2020 2020 2020 2020 2020 207b 2022               { "
+00007160: 4c4f 5745 5222 3a20 2263 6f6e 7469 6e75  LOWER": "continu
+00007170: 6f75 7322 207d 2c0a 2020 2020 2020 2020  ous" },.        
+00007180: 2020 2020 2020 7b20 224c 4f57 4552 223a        { "LOWER":
+00007190: 2022 696e 7465 6772 6174 696f 6e22 207d   "integration" }
+000071a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000071b0: 7b20 224c 4f57 4552 223a 2022 616e 6422  { "LOWER": "and"
+000071c0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+000071d0: 2020 7b20 224c 4f57 4552 223a 2022 6465    { "LOWER": "de
+000071e0: 706c 6f79 6d65 6e74 2220 7d0a 2020 2020  ployment" }.    
+000071f0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00007200: 2020 205b 7b20 224f 5254 4822 3a20 2243     [{ "ORTH": "C
+00007210: 4922 207d 2c20 7b20 224f 5254 4822 3a20  I" }, { "ORTH": 
+00007220: 222f 2220 7d2c 207b 2022 4f52 5448 223a  "/" }, { "ORTH":
+00007230: 2022 4344 2220 7d5d 2c0a 2020 2020 2020   "CD" }],.      
+00007240: 2020 2020 5b7b 2022 4f52 5448 223a 2022      [{ "ORTH": "
+00007250: 4349 2f43 4422 207d 5d2c 0a20 2020 2020  CI/CD" }],.     
+00007260: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
+00007270: 2022 6369 2220 7d2c 207b 2022 4f52 5448   "ci" }, { "ORTH
+00007280: 223a 2022 2f22 207d 2c20 7b20 224c 4f57  ": "/" }, { "LOW
+00007290: 4552 223a 2022 6364 2220 7d5d 2c0a 2020  ER": "cd" }],.  
+000072a0: 2020 2020 2020 2020 5b7b 2022 4c4f 5745          [{ "LOWE
+000072b0: 5222 3a20 7b20 2246 555a 5a59 3122 3a20  R": { "FUZZY1": 
+000072c0: 2263 6963 6422 207d 207d 5d2c 0a20 2020  "cicd" } }],.   
+000072d0: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+000072e0: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+000072f0: 776f 726b 666c 6f77 2220 7d20 7d2c 207b  workflow" } }, {
+00007300: 2022 4c4f 5745 5222 3a20 7b20 2246 555a   "LOWER": { "FUZ
+00007310: 5a59 3122 3a20 2261 7574 6f6d 6174 696f  ZY1": "automatio
+00007320: 6e22 207d 207d 5d2c 0a20 2020 2020 2020  n" } }],.       
+00007330: 2020 205b 7b20 224c 4f57 4552 223a 207b     [{ "LOWER": {
+00007340: 2022 4655 5a5a 5931 223a 2022 776f 726b   "FUZZY1": "work
+00007350: 666c 6f77 2220 7d20 7d5d 2c0a 2020 2020  flow" } }],.    
+00007360: 2020 2020 2020 5b7b 2022 4c4f 5745 5222        [{ "LOWER"
+00007370: 3a20 7b20 2246 555a 5a59 3122 3a20 2264  : { "FUZZY1": "d
+00007380: 6570 6c6f 796d 656e 7422 207d 207d 5d0a  eployment" } }].
+00007390: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
+000073a0: 6465 7363 7269 7074 696f 6e22 3a20 2243  description": "C
+000073b0: 6f6e 7469 6e75 6f75 7320 496e 7465 6772  ontinuous Integr
+000073c0: 6174 696f 6e20 616e 6420 436f 6e74 696e  ation and Contin
+000073d0: 756f 7573 2044 6570 6c6f 796d 656e 7420  uous Deployment 
+000073e0: 2843 492f 4344 2920 6172 6520 4465 764f  (CI/CD) are DevO
+000073f0: 7073 2070 7261 6374 6963 6573 2074 6861  ps practices tha
+00007400: 7420 6175 746f 6d61 7465 2074 6865 2073  t automate the s
+00007410: 6f66 7477 6172 6520 7265 6c65 6173 6520  oftware release 
+00007420: 7072 6f63 6573 732e 2043 4920 666f 6375  process. CI focu
+00007430: 7365 7320 6f6e 2069 6e74 6567 7261 7469  ses on integrati
+00007440: 6e67 2063 6f64 6520 6368 616e 6765 7320  ng code changes 
+00007450: 6672 6571 7565 6e74 6c79 2c20 7768 6572  frequently, wher
+00007460: 6561 7320 4344 2065 6e73 7572 6573 2074  eas CD ensures t
+00007470: 6865 2064 656c 6976 6572 7920 6f66 2074  he delivery of t
+00007480: 6865 7365 2063 6861 6e67 6573 2074 6f20  hese changes to 
+00007490: 7072 6f64 7563 7469 6f6e 2065 6e76 6972  production envir
+000074a0: 6f6e 6d65 6e74 7320 736d 6f6f 7468 6c79  onments smoothly
+000074b0: 2e22 2c0a 2020 2020 2020 2273 636f 7265  .",.      "score
+000074c0: 223a 2035 0a20 207d 2c0a 2020 2249 6e66  ": 5.  },.  "Inf
+000074d0: 7261 7374 7275 6374 7572 6520 6173 2043  rastructure as C
+000074e0: 6f64 6522 3a20 7b0a 2020 2020 2020 2274  ode": {.      "t
+000074f0: 7970 6522 3a20 2244 6576 4f70 7320 5072  ype": "DevOps Pr
+00007500: 6163 7469 6365 7322 2c0a 2020 2020 2020  actices",.      
+00007510: 2263 6174 6567 6f72 7922 3a20 2252 6571  "category": "Req
+00007520: 7569 7265 6d65 6e74 222c 0a20 2020 2020  uirement",.     
+00007530: 2022 7265 6c61 7465 6454 6563 686e 6f6c   "relatedTechnol
+00007540: 6f67 6965 7322 3a20 5b22 5465 7272 6166  ogies": ["Terraf
+00007550: 6f72 6d22 5d2c 0a20 2020 2020 2022 7061  orm"],.      "pa
+00007560: 7474 6572 6e73 223a 205b 0a20 2020 2020  tterns": [.     
+00007570: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
+00007580: 207b 2022 4655 5a5a 5931 223a 2022 696e   { "FUZZY1": "in
+00007590: 6672 6173 7472 7563 7475 7265 2220 7d20  frastructure" } 
+000075a0: 7d2c 207b 2022 4c4f 5745 5222 3a20 2261  }, { "LOWER": "a
+000075b0: 7322 207d 2c20 7b20 224c 4f57 4552 223a  s" }, { "LOWER":
+000075c0: 207b 2022 4655 5a5a 5931 223a 2022 636f   { "FUZZY1": "co
+000075d0: 6465 2220 7d20 7d5d 2c0a 2020 2020 2020  de" } }],.      
+000075e0: 2020 2020 5b7b 2022 4c4f 5745 5222 3a20      [{ "LOWER": 
+000075f0: 2269 6163 2220 7d5d 0a20 2020 2020 205d  "iac" }].      ]
+00007600: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
+00007610: 7469 6f6e 223a 2022 5468 6520 7072 6f63  tion": "The proc
+00007620: 6573 7320 6f66 206d 616e 6167 696e 6720  ess of managing 
+00007630: 616e 6420 7072 6f76 6973 696f 6e69 6e67  and provisioning
+00007640: 2063 6f6d 7075 7469 6e67 2069 6e66 7261   computing infra
+00007650: 7374 7275 6374 7572 6520 7468 726f 7567  structure throug
+00007660: 6820 6d61 6368 696e 652d 7265 6164 6162  h machine-readab
+00007670: 6c65 2064 6566 696e 6974 696f 6e20 6669  le definition fi
+00007680: 6c65 732c 2072 6174 6865 7220 7468 616e  les, rather than
+00007690: 2070 6879 7369 6361 6c20 6861 7264 7761   physical hardwa
+000076a0: 7265 2063 6f6e 6669 6775 7261 7469 6f6e  re configuration
+000076b0: 206f 7220 696e 7465 7261 6374 6976 6520   or interactive 
+000076c0: 636f 6e66 6967 7572 6174 696f 6e20 746f  configuration to
+000076d0: 6f6c 732e 222c 0a20 2020 2020 2022 7363  ols.",.      "sc
+000076e0: 6f72 6522 3a20 350a 2020 7d2c 0a20 2022  ore": 5.  },.  "
+000076f0: 436f 6e74 6169 6e65 7269 7a61 7469 6f6e  Containerization
+00007700: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00007710: 223a 2022 4465 764f 7073 2050 7261 6374  ": "DevOps Pract
+00007720: 6963 6573 222c 0a20 2020 2020 2022 6361  ices",.      "ca
+00007730: 7465 676f 7279 223a 2022 5265 7175 6972  tegory": "Requir
+00007740: 656d 656e 7422 2c0a 2020 2020 2020 2272  ement",.      "r
+00007750: 656c 6174 6564 5465 6368 6e6f 6c6f 6769  elatedTechnologi
+00007760: 6573 223a 205b 2244 6f63 6b65 7222 5d2c  es": ["Docker"],
+00007770: 0a20 2020 2020 2022 7061 7474 6572 6e73  .      "patterns
+00007780: 223a 205b 0a20 2020 2020 2020 2020 205b  ": [.          [
+00007790: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+000077a0: 5a5a 5931 223a 2022 636f 6e74 6169 6e65  ZZY1": "containe
+000077b0: 7269 7a61 7469 6f6e 2220 7d7d 5d2c 0a20  rization" }}],. 
+000077c0: 2020 2020 2020 2020 205b 7b20 224c 4f57           [{ "LOW
+000077d0: 4552 223a 207b 2022 4655 5a5a 5931 223a  ER": { "FUZZY1":
+000077e0: 2022 636f 6e74 6169 6e65 7273 2220 7d7d   "containers" }}
+000077f0: 5d2c 0a20 2020 2020 2020 2020 205b 7b20  ],.          [{ 
+00007800: 224c 4f57 4552 223a 207b 2022 4655 5a5a  "LOWER": { "FUZZ
+00007810: 5931 223a 2022 636f 6e74 6169 6e65 7269  Y1": "containeri
+00007820: 7a65 6422 7d7d 5d2c 0a20 2020 2020 2020  zed"}}],.       
+00007830: 2020 205b 7b20 224c 4f57 4552 223a 207b     [{ "LOWER": {
+00007840: 2022 4655 5a5a 5931 223a 2022 6465 706c   "FUZZY1": "depl
+00007850: 6f79 6162 6c65 2220 7d7d 5d2c 0a20 2020  oyable" }}],.   
+00007860: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+00007870: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+00007880: 706f 7274 6162 696c 6974 7922 207d 7d5d  portability" }}]
+00007890: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
+000078a0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000078b0: 5468 6520 7072 6f63 6573 7320 6f66 2065  The process of e
+000078c0: 6e63 6170 7375 6c61 7469 6e67 2061 6e20  ncapsulating an 
+000078d0: 6170 706c 6963 6174 696f 6e20 616e 6420  application and 
+000078e0: 6974 7320 6465 7065 6e64 656e 6369 6573  its dependencies
+000078f0: 2069 6e74 6f20 6120 636f 6e74 6169 6e65   into a containe
+00007900: 722c 2061 6c6c 6f77 696e 6720 6974 2074  r, allowing it t
+00007910: 6f20 7275 6e20 636f 6e73 6973 7465 6e74  o run consistent
+00007920: 6c79 2061 6372 6f73 7320 6469 6666 6572  ly across differ
+00007930: 656e 7420 656e 7669 726f 6e6d 656e 7473  ent environments
+00007940: 2e22 2c0a 2020 2020 2020 2273 636f 7265  .",.      "score
+00007950: 223a 2035 0a20 207d 2c0a 2020 2243 6f6e  ": 5.  },.  "Con
+00007960: 7461 696e 6572 204f 7263 6865 7374 7261  tainer Orchestra
+00007970: 7469 6f6e 223a 207b 0a20 2020 2020 2022  tion": {.      "
+00007980: 7479 7065 223a 2022 4465 764f 7073 2050  type": "DevOps P
+00007990: 7261 6374 6963 6573 222c 0a20 2020 2020  ractices",.     
+000079a0: 2022 6361 7465 676f 7279 223a 2022 5265   "category": "Re
+000079b0: 7175 6972 656d 656e 7422 2c0a 2020 2020  quirement",.    
+000079c0: 2020 2272 656c 6174 6564 5465 6368 6e6f    "relatedTechno
+000079d0: 6c6f 6769 6573 223a 205b 224b 7562 6572  logies": ["Kuber
+000079e0: 6e65 7465 7322 5d2c 0a20 2020 2020 2022  netes"],.      "
+000079f0: 7061 7474 6572 6e73 223a 205b 0a20 2020  patterns": [.   
+00007a00: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+00007a10: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+00007a20: 636f 6e74 6169 6e65 7222 207d 207d 2c20  container" } }, 
+00007a30: 7b20 224c 4f57 4552 223a 207b 2022 4655  { "LOWER": { "FU
+00007a40: 5a5a 5931 223a 2022 6f72 6368 6573 7472  ZZY1": "orchestr
+00007a50: 6174 696f 6e22 207d 207d 5d2c 0a20 2020  ation" } }],.   
+00007a60: 2020 2020 2020 205b 7b20 224c 4f57 4552         [{ "LOWER
+00007a70: 223a 207b 2022 4655 5a5a 5931 223a 2022  ": { "FUZZY1": "
+00007a80: 706f 6473 2220 7d7d 5d2c 0a20 2020 2020  pods" }}],.     
+00007a90: 2020 2020 205b 7b20 224c 4f57 4552 223a       [{ "LOWER":
+00007aa0: 207b 2022 4655 5a5a 5931 223a 2022 7363   { "FUZZY1": "sc
+00007ab0: 616c 6162 6c65 2220 7d7d 5d0a 2020 2020  alable" }}].    
+00007ac0: 2020 5d2c 0a20 2020 2020 2022 6465 7363    ],.      "desc
+00007ad0: 7269 7074 696f 6e22 3a20 2254 6865 2070  ription": "The p
+00007ae0: 726f 6365 7373 206f 6620 6175 746f 6d61  rocess of automa
+00007af0: 7469 6e67 2074 6865 2064 6570 6c6f 796d  ting the deploym
+00007b00: 656e 742c 2073 6361 6c69 6e67 2c20 616e  ent, scaling, an
+00007b10: 6420 6d61 6e61 6765 6d65 6e74 206f 6620  d management of 
+00007b20: 636f 6e74 6169 6e65 7269 7a65 6420 6170  containerized ap
+00007b30: 706c 6963 6174 696f 6e73 2e22 2c0a 2020  plications.",.  
+00007b40: 2020 2020 2273 636f 7265 223a 2035 0a20      "score": 5. 
+00007b50: 207d 0a7d 0a                              }.}.
```

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/entity_extraction.py` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/entity_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,65 +6,65 @@
 
 nlp = load_spacy_model()
 
 if nlp is None:
     # Exit the script or handle the missing model appropriately.
     sys.exit("Model not installed. Please download it before proceeding.")
 else:
-  def initialize_matcher_with_patterns(tech_entities):
-      """
-      Initialize a spaCy Matcher object with patterns for tech entities.
-
-      Args:
-          tech_entities (dict): A dictionary containing tech entity names as keys and their patterns as values.
-
-      Returns:
-          Matcher: A spaCy Matcher object initialized with the provided patterns.
-      """
-      matcher = Matcher(nlp.vocab)
-      for name, entity in tech_entities.items():
-          # Assuming entity["patterns"] is a list of pattern dictionaries
-          patterns = entity["patterns"]
-          # Define patterns for the matcher to identify tech entities in text
-          matcher.add(name, patterns)
-      # Return the matcher with all the added patterns
-      return matcher
-
-
-  def extract_tech_entities(text, tech_entities, matcher):
-      """
-      Extracts technology entities from the given text using a spaCy matcher.
-
-      Args:
-          text (str): The input text from which to extract entities.
-          tech_entities (dict): A dictionary containing information about the technology entities.
-          matcher (spacy.matcher.Matcher): The spaCy matcher object used for entity matching.
-
-      Returns:
-          list: A list of dictionaries containing information about the extracted entities.
-      """
-
-      # Process the text with the spaCy NLP pipeline to create a document object
-      doc = nlp(text)
-      # Use the matcher to find all matches in the document
-      matches = matcher(doc)
-      # Initialize a list to store entities found in the text
-      entities = []
-      # Iterate over each match to extract the entity details
-      for match_id, start, end in matches:
-          # Retrieve the string representation of the entity's match ID
-          entity_key = nlp.vocab.strings[match_id]
-          # Access the entity's details from the tech_entities dictionary using the entity_key
-          entity_details = tech_entities[entity_key]
-          # Create a dictionary with the entity's details
-          extracted_entity = {
-              "entity": entity_key,
-              "type": entity_details["type"],
-              "category": entity_details["category"],
-              "description": entity_details["description"],
-              "score": entity_details["score"],
-          }
-          # Append the entity's details to the list of unique entities
-          entities.append(extracted_entity)
 
-      # Return the list of entities
-      return entities
+    def initialize_matcher_with_patterns(tech_entities):
+        """
+        Initialize a spaCy Matcher object with patterns for tech entities.
+
+        Args:
+            tech_entities (dict): A dictionary containing tech entity names as keys and their patterns as values.
+
+        Returns:
+            Matcher: A spaCy Matcher object initialized with the provided patterns.
+        """
+        matcher = Matcher(nlp.vocab)
+        for name, entity in tech_entities.items():
+            # Assuming entity["patterns"] is a list of pattern dictionaries
+            patterns = entity["patterns"]
+            # Define patterns for the matcher to identify tech entities in text
+            matcher.add(name, patterns)
+        # Return the matcher with all the added patterns
+        return matcher
+
+    def extract_tech_entities(text, tech_entities, matcher):
+        """
+        Extracts technology entities from the given text using a spaCy matcher.
+
+        Args:
+            text (str): The input text from which to extract entities.
+            tech_entities (dict): A dictionary containing information about the technology entities.
+            matcher (spacy.matcher.Matcher): The spaCy matcher object used for entity matching.
+
+        Returns:
+            list: A list of dictionaries containing information about the extracted entities.
+        """
+
+        # Process the text with the spaCy NLP pipeline to create a document object
+        doc = nlp(text)
+        # Use the matcher to find all matches in the document
+        matches = matcher(doc)
+        # Initialize a list to store entities found in the text
+        entities = []
+        # Iterate over each match to extract the entity details
+        for match_id, start, end in matches:
+            # Retrieve the string representation of the entity's match ID
+            entity_key = nlp.vocab.strings[match_id]
+            # Access the entity's details from the tech_entities dictionary using the entity_key
+            entity_details = tech_entities[entity_key]
+            # Create a dictionary with the entity's details
+            extracted_entity = {
+                "entity": entity_key,
+                "type": entity_details["type"],
+                "category": entity_details["category"],
+                "description": entity_details["description"],
+                "score": entity_details["score"],
+            }
+            # Append the entity's details to the list of unique entities
+            entities.append(extracted_entity)
+
+        # Return the list of entities
+        return entities
```

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/recommendation_generation.py` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/recommendation_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
     # Get the embedding of the user input. This will be used to calculate the similarity
     # between the user input and each entity.
     input_embedding = get_embedding(user_input)
     scores = {}
 
     # Identify explicit mentions of entities in the user input.
-    explicit_mentions = [entity_dict["entity"] for entity_dict in entities if entity_dict["entity"].lower() in user_input.lower()]
+    explicit_mentions = [
+        entity_dict["entity"] for entity_dict in entities if entity_dict["entity"].lower() in user_input.lower()
+    ]
 
     # Prepare a list of entities to be scored. If an entity has related technologies,
     # add those to the list instead of the entity itself.
     updated_entities = []
     for entity_dict in entities:
         entity_name = entity_dict["entity"]
         if "relatedTechnologies" in tech_entities.get(entity_name, {}):
@@ -35,21 +37,25 @@
 
     # Score entities, applying a boost for explicit mentions
     for entity_name in updated_entities:
         # Get the information about the entity from the tech_entities dictionary.
         entity_info = tech_entities.get(entity_name, {})
         # Prepare the text that represents the entity. This includes the entity's description,
         # category, and type.
-        entity_text = f"{entity_info.get('description', '')} {entity_info.get('category', '')} {entity_info.get('type', '')}"
+        entity_text = (
+            f"{entity_info.get('description', '')} {entity_info.get('category', '')} {entity_info.get('type', '')}"
+        )
         # Get the embedding of the entity text.
         entity_embedding = get_embedding(entity_text)
         # Calculate the cosine similarity between the user input and the entity.
         similarity = cosine_similarity(input_embedding, entity_embedding)
         # Calculate the relevance score of the entity based on its similarity to the topic keywords.
-        relevance_score = sum(cosine_similarity(get_embedding(keyword), entity_embedding) for keyword in topic_keywords) / len(topic_keywords)
+        relevance_score = sum(
+            cosine_similarity(get_embedding(keyword), entity_embedding) for keyword in topic_keywords
+        ) / len(topic_keywords)
 
         # The combined score is the sum of the similarity and the relevance score.
         combined_score = similarity + relevance_score
 
         # Apply a scoring boost for explicit mentions of the entity in the user input.
         if entity_name in explicit_mentions:
             combined_score += 0.2  # Adjust this boost value as needed
@@ -97,10 +103,13 @@
     # Iterate through entities to find the highest-scoring entity for each category
     for entity in entities:
         category = entity["category"]
         if category not in best_entity_per_category or best_entity_per_category[category]["score"] < entity["score"]:
             best_entity_per_category[category] = entity
 
     # Prepare recommendations based on the best entity for each category
-    recommendations = [{"category": category, "recommendation": entity["entity_name"]} for category, entity in best_entity_per_category.items()]
+    recommendations = [
+        {"category": category, "recommendation": entity["entity_name"]}
+        for category, entity in best_entity_per_category.items()
+    ]
 
     return recommendations
```

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/functions/topic_classification.py` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/functions/topic_classification.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/models.py` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/models.py`

 * *Files identical despite different names*

### Comparing `entity_recognition_lib-0.1.4/src/entity_recognition_lib/utils.py` & `entity_recognition_lib-0.1.5/src/entity_recognition_lib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 from requests import JSONDecodeError
 from scipy.spatial.distance import cosine
 
 from entity_recognition_lib.models import load_embeddings_model
 
 tokenizer, model = asyncio.run(load_embeddings_model())
 
+
 def load_json_file(file_name):
     """
     Load a JSON file from the installed package resources.
 
     Args:
         file_name (str): The filename of the JSON file to load from the 'data' directory within the package.
 
     Returns:
         dict: The contents of the JSON file as a dictionary.
 
     Raises:
         FileNotFoundError: If the file does not exist within the package resources.
     """
-    package_path = 'entity_recognition_lib.data'  # Define the package path to the resources
+    package_path = "entity_recognition_lib.data"  # Define the package path to the resources
 
     try:
-      # Open the resource file within the context manager
-      with resources.files(package_path).joinpath(file_name).open() as file:
-        return json.load(file)
+        # Open the resource file within the context manager
+        with resources.files(package_path).joinpath(file_name).open() as file:
+            return json.load(file)
     except FileNotFoundError:
-      raise FileNotFoundError(f"File not found: {file_name} in package resources.")
+        raise FileNotFoundError(f"File not found: {file_name} in package resources.")
     except JSONDecodeError as e:
-      raise JSONDecodeError(f"An error occurred while loading {file_name}: {str(e)}")
+        raise JSONDecodeError(f"An error occurred while loading {file_name}: {str(e)}")
 
 
 def mean_pooling(model_output, attention_mask):
     """
     Apply mean pooling to get the sentence embedding
 
     Parameters:
@@ -61,15 +62,14 @@
     Parameters:
         text (str): The input text to be embedded.
 
     Returns:
         torch.Tensor: The embedding representation of the text.
     """
 
-
     # Tokenize the input text and prepare it for the model
     inputs = tokenizer(text, return_tensors="pt", padding=True, truncation=True, max_length=512)
     # Generate the embeddings by passing the inputs to the model
     with torch.no_grad():  # Disable gradient computation
         outputs = model(**inputs)
     # Extract the embeddings from the model's output, which is the mean of the last hidden state
     embeddings = mean_pooling(outputs, inputs["attention_mask"])
```

### Comparing `entity_recognition_lib-0.1.4/PKG-INFO` & `entity_recognition_lib-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entity-recognition-lib
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for technology entity recognition and recommendation
 License: MIT
 Author: Cesar Goncalves
 Author-email: goncalves.cesaraugusto94@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,19 +20,20 @@
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: transformers (>=4.40.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Entity-Recognition
 
-The Entity-Recognition library utilizes `spaCy`, `BERTopic`, and `Transformers` to provide a robust technology entity recognition system capable of identifying technological entities within texts and suggesting relevant technologies using advanced NLP techniques.
+The Entity-Recognition library utilizes `spaCy`, `BERTopic`, and `Transformers` to provide a robust technology entity
+recognition system capable of identifying technological entities within texts and suggesting relevant technologies using
+advanced NLP techniques.
 
 The library automatically downloads the required spaCy model if not installed, making it easy to get started.
 
-
 ## Features
 
 - **Technology Entity Extraction**: Automatically extract technology-related terms and tools from texts.
 - **Recommendation System**: Provides context-based technology recommendations.
 - **BERTopic Integration**: Leverages topic modeling to enhance the relevance of recommendations.
 - **spaCy Matchers**: Utilizes custom NLP patterns for precise entity recognition.
 
@@ -47,20 +48,18 @@
 
 Install the library directly from PyPI:
 
 ```bash
 pip install entity-recognition-lib
 ```
 
-The required spaCy model (`en_core_web_sm`) will be automatically downloaded and installed if not already present on your system.
-
-
+The required spaCy model (`en_core_web_sm`) will be automatically downloaded and installed if not already present on
+your system.
 
-Usage
------
+## Usage
 
 Here's how to use the Entity Recognition library in your Python scripts:
 
 ```python
 from entity_recognition_lib import EntityRecognizer
 
 # Create an instance of the recognizer
@@ -69,14 +68,15 @@
 # Example texts
 texts = ["I need an Express.js Mongo database backend"]
 
 # Process texts
 results = recognizer.process_texts(texts)
 print(results)
 ```
+
 Expected output:
 
 ```json
 [
     {
         "input_text": "I need an Express.js Mongo database backend",
         "predicted_topic_name": "575_databases_database_tables_schema",
@@ -105,57 +105,60 @@
     }
 ]
 ```
 
 For detailed usage examples and code snippets, please refer to the [examples directory](examples/EXAMPLES.md) in the repository.
 The examples cover various scenarios, including:
 
-1. Basic usage of the library for entity recognition and recommendation generation
-2. Advanced features such as result analysis and visualization
-3. Integration samples with popular frameworks like Flask and Streamlit
+- Basic usage of the library for entity recognition and recommendation generation
+- Advanced features such as result analysis and visualization
+- Integration samples with popular frameworks like Flask and Streamlit
 
-We recommend exploring the examples to understand how to effectively utilize the Entity-Recognition library in your projects.
+We recommend exploring the examples to understand how to effectively utilize the Entity-Recognition library in your
+projects.
 
 ## Development
 
 ### Setting Up a Development Environment
 
-1. **Clone the repository**:
-   ```
+- **Clone the repository**:
+
+   ```bash
    git clone https://github.com/cgoncalves94/entity-recognition.git
    cd entity-recognition
    ```
-2. **Create and Activate a Virtual Environment**:
+
+- **Create and Activate a Virtual Environment**:
+
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
-3. **Install Dependencies**:
-    ```
+
+- **Install Dependencies**:
+
+    ```bash
     pip install -r requirements.txt
     ```
 
-
 ## Testing
 
 Run tests to ensure the setup is correct:
 
-```
+```bash
 pytest
 ```
 
 ## Contributing
 
 Contributions are welcome! Please follow these steps:
 
-1. Fork the repository on GitHub.
-2. Clone the forked repository to your machine.
-3. Create a new branch for your changes.
-4. Make changes and test.
-5. Submit a pull request with a comprehensive description of changes.
+- Fork the repository on GitHub.
+- Clone the forked repository to your machine.
+- Create a new branch for your changes.
+- Make changes and test.
+- Submit a pull request with a comprehensive description of changes.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
-
-
```

