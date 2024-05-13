# Comparing `tmp/surveyeval-0.1.8.tar.gz` & `tmp/surveyeval-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surveyeval-0.1.8.tar", last modified: Mon Apr 22 10:54:09 2024, max compression
+gzip compressed data, was "surveyeval-0.1.9.tar", last modified: Mon Apr 22 18:01:00 2024, max compression
```

## Comparing `surveyeval-0.1.8.tar` & `surveyeval-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 10:54:09.632363 surveyeval-0.1.8/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.8/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)    11284 2024-04-22 10:54:09.632064 surveyeval-0.1.8/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)    10734 2024-04-20 20:30:48.000000 surveyeval-0.1.8/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-22 10:54:09.632422 surveyeval-0.1.8/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     1450 2024-04-21 18:26:36.000000 surveyeval-0.1.8/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 10:54:09.615167 surveyeval-0.1.8/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 10:54:09.621016 surveyeval-0.1.8/src/surveyeval/
--rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-17 18:39:29.000000 surveyeval-0.1.8/src/surveyeval/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    59038 2024-04-18 19:09:56.000000 surveyeval-0.1.8/src/surveyeval/core_evaluation_lenses.py
--rw-r--r--   0 crobert    (501) staff       (20)    35350 2024-04-18 18:10:53.000000 surveyeval-0.1.8/src/surveyeval/evaluation_engine.py
--rw-r--r--   0 crobert    (501) staff       (20)     3739 2024-04-20 20:38:40.000000 surveyeval-0.1.8/src/surveyeval/html_tools.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 10:54:09.631060 surveyeval-0.1.8/src/surveyeval/resources/
--rw-r--r--   0 crobert    (501) staff       (20)    42632 2024-04-20 10:55:54.000000 surveyeval-0.1.8/src/surveyeval/resources/EmptyForm.xlsx
--rw-r--r--   0 crobert    (501) staff       (20)    79606 2024-04-22 10:30:58.000000 surveyeval-0.1.8/src/surveyeval/survey_parser.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 10:54:09.630789 surveyeval-0.1.8/src/surveyeval.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)    11284 2024-04-22 10:54:09.000000 surveyeval-0.1.8/src/surveyeval.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      421 2024-04-22 10:54:09.000000 surveyeval-0.1.8/src/surveyeval.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-22 10:54:09.000000 surveyeval-0.1.8/src/surveyeval.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-22 10:54:09.000000 surveyeval-0.1.8/src/surveyeval.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-22 10:54:09.000000 surveyeval-0.1.8/src/surveyeval.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 18:01:00.500377 surveyeval-0.1.9/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.9/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    11346 2024-04-22 18:01:00.499575 surveyeval-0.1.9/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10796 2024-04-22 11:22:14.000000 surveyeval-0.1.9/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-22 18:01:00.500466 surveyeval-0.1.9/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     1450 2024-04-22 18:00:50.000000 surveyeval-0.1.9/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 18:01:00.491543 surveyeval-0.1.9/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 18:01:00.495126 surveyeval-0.1.9/src/surveyeval/
+-rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-17 18:39:29.000000 surveyeval-0.1.9/src/surveyeval/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    60646 2024-04-22 17:53:14.000000 surveyeval-0.1.9/src/surveyeval/core_evaluation_lenses.py
+-rw-r--r--   0 crobert    (501) staff       (20)    36385 2024-04-22 16:11:56.000000 surveyeval-0.1.9/src/surveyeval/evaluation_engine.py
+-rw-r--r--   0 crobert    (501) staff       (20)     3739 2024-04-20 20:38:40.000000 surveyeval-0.1.9/src/surveyeval/html_tools.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 18:01:00.498146 surveyeval-0.1.9/src/surveyeval/resources/
+-rw-r--r--   0 crobert    (501) staff       (20)    42632 2024-04-20 10:55:54.000000 surveyeval-0.1.9/src/surveyeval/resources/EmptyForm.xlsx
+-rw-r--r--   0 crobert    (501) staff       (20)    79615 2024-04-22 16:29:06.000000 surveyeval-0.1.9/src/surveyeval/survey_parser.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-22 18:01:00.497583 surveyeval-0.1.9/src/surveyeval.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    11346 2024-04-22 18:01:00.000000 surveyeval-0.1.9/src/surveyeval.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      421 2024-04-22 18:01:00.000000 surveyeval-0.1.9/src/surveyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-22 18:01:00.000000 surveyeval-0.1.9/src/surveyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-22 18:01:00.000000 surveyeval-0.1.9/src/surveyeval.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-22 18:01:00.000000 surveyeval-0.1.9/src/surveyeval.egg-info/top_level.txt
```

### Comparing `surveyeval-0.1.8/LICENSE` & `surveyeval-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.8/PKG-INFO` & `surveyeval-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
@@ -83,29 +83,30 @@
 1. ``.docx``: Word files are read in the ``read_docx()`` function, using LangChain's ``UnstructuredFileLoader()`` function.
    Note that text within "content controls" is effectively invisible, so you might need to open your file, select all, 
    and select "Remove content controls" to render the text visible 
    (`see here for more on content controls <https://learn.microsoft.com/en-us/office/client-developer/word/content-controls-in-word>`_).
 2. ``.pdf``: PDF files are read in the ``read_pdf_combined()`` function, which tries to read the text and tables in a PDF
    (separately), combine them together, and then fall back to using an OCR reader if that process didn't find much 
    text. There is a ton of room for improvement here.
-3. ``.xlsx``: Excel files are read in the ``parse_xlsx()`` function, in two stages. First, it assumes that the file is in
-   `XLSForm format <https://xlsform.org/en/>`_ and uses `the pyxform library <https://github.com/XLSForm/pyxform>`_ to
-   read the survey. If it encounters an error, it falls back to using LangChain's ``UnstructuredExcelLoader()`` to load
-   the workbook in HTML format, then uses that HTML as the raw text for parsing. There is much that can be improved,
-   particularly in how XLSForms are handled (e.g., the current approach doesn't handle translations well).
-4. ``.csv``: CSV files are read in the ``parse_csv()`` function, also using two stages. First, it assumes that the file
-   is a REDCap data dictionary and parses the columns accordingly. If it encounters an error, it falls back to just
-   reading the file as raw text. There is much that can be improved here, particularly in how REDCap data 
-   dictionaries are handled (e.g., the current approach doesn't handle modules or translations).
+3. ``.xlsx``: Excel files are read in the ``parse_xlsx()`` function, in two ways. If the file looks like it's in
+   `XLSForm format <https://xlsform.org/en/>`_, it parses it accordingly; this parsing should be completely lossless
+   and requires no additional parsing at later stages. If the file does not appear to be an XLSForm, the reader falls
+   back to using LangChain's ``UnstructuredExcelLoader()`` to load the workbook in HTML format, then uses that HTML as
+   the raw text for parsing. XLSForm handling should be robust, but there is much that can be improved in how other
+   formats are handled.
+4. ``.csv``: CSV files are read in the ``parse_csv()`` function, also in two ways. If the file looks like a REDCap
+   data dictionary, it will parse the columns accordingly (requiring little to no later processing). Otherwise, it
+   falls back to just reading the file as raw text. There is much that can be improved here, particularly in how
+   REDCap data dictionaries are handled (e.g., the current approach doesn't handle modules or translations).
 5. ``.html``: HTML files are read in the ``read_html()`` function, then converted into markdown for parsing.
 
-All of the raw content is split into 6,000-character chunks with 500 characters of overlap, before being passed on
-for parsing. This is necessary to both (a) avoid overflowing LLM context windows, and (b) allow the LLM to focus on
-a tractable amount of text in any given request (with the latter becoming more important as the constraints on context
-windows are relaxed).
+All of the raw content is split into 3,000-character chunks with 500 characters of overlap, before being passed on
+for parsing. This is necessary to (a) avoid overflowing LLM context windows, (b) avoid overflowing output token
+limits, and (c) allow the LLM to focus on a tractable amount of text in any given request (with the latter becoming
+more important as the constraints on context windows are relaxed).
 
 Overall, the code for reading files performs pretty poorly for all but the simplest formats. There's much work to do
 here to improve quality.
 
 Parsing input files
 ^^^^^^^^^^^^^^^^^^^
 
@@ -126,15 +127,15 @@
 Roadmap
 -------
 
 There's much that can be improved here. For example:
 
 * We should track and report costs for the evaluation stage of the process.
 * We should generally overhaul the ``survey_parser`` module to better ingest different file formats into
-  raw text that works consistently well for parsing. Better PDF, XLSForm, and REDCap support, in particular, would be
+  raw text that works consistently well for parsing. Better PDF and REDCap support, in particular, would be
   nice.
 * We should add an LLM cache that avoids calling out to the LLM for responses that it already has from prior requests.
   After all, it's common to evaluate the same instrument multiple times, and it's incredibly wasteful to 
   keep going back to the LLM for the same responses every time (for requests that haven't changed in any way).
 * We should improve how findings are scored and filtered, to avoid giving overwhelming numbers of minor 
   recommendations.
 * We should improve the output format to be more user-friendly. (For example, a direct Word output with comments and
```

### Comparing `surveyeval-0.1.8/README.rst` & `surveyeval-0.1.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -65,29 +65,30 @@
 1. ``.docx``: Word files are read in the ``read_docx()`` function, using LangChain's ``UnstructuredFileLoader()`` function.
    Note that text within "content controls" is effectively invisible, so you might need to open your file, select all, 
    and select "Remove content controls" to render the text visible 
    (`see here for more on content controls <https://learn.microsoft.com/en-us/office/client-developer/word/content-controls-in-word>`_).
 2. ``.pdf``: PDF files are read in the ``read_pdf_combined()`` function, which tries to read the text and tables in a PDF
    (separately), combine them together, and then fall back to using an OCR reader if that process didn't find much 
    text. There is a ton of room for improvement here.
-3. ``.xlsx``: Excel files are read in the ``parse_xlsx()`` function, in two stages. First, it assumes that the file is in
-   `XLSForm format <https://xlsform.org/en/>`_ and uses `the pyxform library <https://github.com/XLSForm/pyxform>`_ to
-   read the survey. If it encounters an error, it falls back to using LangChain's ``UnstructuredExcelLoader()`` to load
-   the workbook in HTML format, then uses that HTML as the raw text for parsing. There is much that can be improved,
-   particularly in how XLSForms are handled (e.g., the current approach doesn't handle translations well).
-4. ``.csv``: CSV files are read in the ``parse_csv()`` function, also using two stages. First, it assumes that the file
-   is a REDCap data dictionary and parses the columns accordingly. If it encounters an error, it falls back to just
-   reading the file as raw text. There is much that can be improved here, particularly in how REDCap data 
-   dictionaries are handled (e.g., the current approach doesn't handle modules or translations).
+3. ``.xlsx``: Excel files are read in the ``parse_xlsx()`` function, in two ways. If the file looks like it's in
+   `XLSForm format <https://xlsform.org/en/>`_, it parses it accordingly; this parsing should be completely lossless
+   and requires no additional parsing at later stages. If the file does not appear to be an XLSForm, the reader falls
+   back to using LangChain's ``UnstructuredExcelLoader()`` to load the workbook in HTML format, then uses that HTML as
+   the raw text for parsing. XLSForm handling should be robust, but there is much that can be improved in how other
+   formats are handled.
+4. ``.csv``: CSV files are read in the ``parse_csv()`` function, also in two ways. If the file looks like a REDCap
+   data dictionary, it will parse the columns accordingly (requiring little to no later processing). Otherwise, it
+   falls back to just reading the file as raw text. There is much that can be improved here, particularly in how
+   REDCap data dictionaries are handled (e.g., the current approach doesn't handle modules or translations).
 5. ``.html``: HTML files are read in the ``read_html()`` function, then converted into markdown for parsing.
 
-All of the raw content is split into 6,000-character chunks with 500 characters of overlap, before being passed on
-for parsing. This is necessary to both (a) avoid overflowing LLM context windows, and (b) allow the LLM to focus on
-a tractable amount of text in any given request (with the latter becoming more important as the constraints on context
-windows are relaxed).
+All of the raw content is split into 3,000-character chunks with 500 characters of overlap, before being passed on
+for parsing. This is necessary to (a) avoid overflowing LLM context windows, (b) avoid overflowing output token
+limits, and (c) allow the LLM to focus on a tractable amount of text in any given request (with the latter becoming
+more important as the constraints on context windows are relaxed).
 
 Overall, the code for reading files performs pretty poorly for all but the simplest formats. There's much work to do
 here to improve quality.
 
 Parsing input files
 ^^^^^^^^^^^^^^^^^^^
 
@@ -108,15 +109,15 @@
 Roadmap
 -------
 
 There's much that can be improved here. For example:
 
 * We should track and report costs for the evaluation stage of the process.
 * We should generally overhaul the ``survey_parser`` module to better ingest different file formats into
-  raw text that works consistently well for parsing. Better PDF, XLSForm, and REDCap support, in particular, would be
+  raw text that works consistently well for parsing. Better PDF and REDCap support, in particular, would be
   nice.
 * We should add an LLM cache that avoids calling out to the LLM for responses that it already has from prior requests.
   After all, it's common to evaluate the same instrument multiple times, and it's incredibly wasteful to 
   keep going back to the LLM for the same responses every time (for requests that haven't changed in any way).
 * We should improve how findings are scored and filtered, to avoid giving overwhelming numbers of minor 
   recommendations.
 * We should improve the output format to be more user-friendly. (For example, a direct Word output with comments and
```

### Comparing `surveyeval-0.1.8/setup.py` & `surveyeval-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='surveyeval',
-    version='0.1.8',
+    version='0.1.9',
     packages=['surveyeval'],
     python_requires='>=3.10',
     install_requires=[
         'tiktoken~=0.5.2',
         'openai~=1.10.0',
         'langchain~=0.1.15',
         'langchain-openai~=0.0.5',
```

### Comparing `surveyeval-0.1.8/src/surveyeval/__init__.py` & `surveyeval-0.1.9/src/surveyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.8/src/surveyeval/core_evaluation_lenses.py` & `surveyeval-0.1.9/src/surveyeval/core_evaluation_lenses.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,20 +176,22 @@
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt),
                                         survey_question=EvaluationEngine.clean_whitespace(survey_question),
                                         **kwargs)
 
-    def format_result(self, result: dict | None = None) -> str:
+    def format_result(self, result: dict | None = None, minimum_importance: int = 0) -> str:
         """
         Format the evaluation result as a human-readable string.
 
         :param result: Evaluation result to format (or None to use the evaluation_result attribute).
         :type result: dict | None
+        :param minimum_importance: Minimum importance score for filtering results (defaults to 0, which doesn't filter).
+        :type minimum_importance: int
         :return: Formatted evaluation result.
         :rtype: str
         """
 
         # use evaluation_result attribute if no result is passed
         if result is not None:
             result_to_format = result
@@ -202,18 +204,21 @@
 
         # format and return result
         try:
             formatted_result = ""
             sorted_indices = sorted(range(len(result_to_format["Severities"])),
                                     key=lambda idx: result_to_format["Severities"][idx], reverse=True)
             for i in sorted_indices:
-                formatted_result += f"Severity {result_to_format['Severities'][i]} finding (out of 5):\n\n"
-                formatted_result += f"Existing phrase: {result_to_format['Phrases'][i]}\n"
-                formatted_result += f"Recommended replacement: {result_to_format['Recommendations'][i]}\n"
-                formatted_result += f"Explanation: {result_to_format['Explanations'][i]}\n\n"
+                severity = result_to_format['Severities'][i]
+                # only report findings with severity greater than or equal to minimum_importance
+                if severity >= minimum_importance:
+                    formatted_result += f"Severity {severity} finding (out of 5):\n\n"
+                    formatted_result += f"{result_to_format['Explanations'][i]}\n\n"
+                    formatted_result += f"Recommend replacing: {result_to_format['Phrases'][i]}\n"
+                    formatted_result += f"          With this: {result_to_format['Recommendations'][i]}\n\n"
         except Exception as e:
             # include exception in returned results, with raw JSON results
             formatted_result = (f"Error occurred formatting result: {str(e)}\n\n"
                                 f"Raw JSON: {json.dumps(result_to_format, indent=4)}")
             self.evaluation_engine.logger.error(formatted_result)
         return formatted_result
 
@@ -461,20 +466,22 @@
         :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
-    def format_result(self, result: dict | None = None) -> str:
+    def format_result(self, result: dict | None = None, minimum_importance: int = 0) -> str:
         """
         Format the evaluation result as a human-readable string.
 
         :param result: Evaluation result to format (or None to use the evaluation_result attribute).
         :type result: dict | None
+        :param minimum_importance: Minimum importance score for filtering results (defaults to 0, which doesn't filter).
+        :type minimum_importance: int
         :return: Formatted evaluation result.
         :rtype: str
         """
 
         # use evaluation_result attribute if no result is passed
         if result is not None:
             result_to_format = result
@@ -483,14 +490,19 @@
 
         # return empty string if no result is available to format
         if result_to_format is None:
             return ""
 
         # format and return result
         try:
+            if minimum_importance > 0 and (not result_to_format["Recommendation"]
+                                           or result_to_format["Recommendation strength"] < minimum_importance):
+                # filter this result since as not important enough
+                return ""
+
             if len(result_to_format["Measuring"]) == 0:
                 measuring_str = ""
             elif len(result_to_format["Measuring"]) == 1:
                 measuring_str = str(result_to_format["Measuring"][0])
             else:
                 measuring_str = ', '.join(result_to_format["Measuring"])
             formatted_result = f"FYI: Excerpt likely attempting to measure {measuring_str}\n\n"
@@ -742,20 +754,22 @@
         :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
-    def format_result(self, result: dict | None = None) -> str:
+    def format_result(self, result: dict | None = None, minimum_importance: int = 0) -> str:
         """
         Format the evaluation result as a human-readable string.
 
         :param result: Evaluation result to format (or None to use the evaluation_result attribute).
         :type result: dict | None
+        :param minimum_importance: Minimum importance score for filtering results (defaults to 0, which doesn't filter).
+        :type minimum_importance: int
         :return: Formatted evaluation result.
         :rtype: str
         """
 
         # use evaluation_result attribute if no result is passed
         if result is not None:
             result_to_format = result
@@ -768,18 +782,21 @@
 
         # format and return result
         try:
             formatted_result = ""
             sorted_indices = sorted(range(len(result_to_format["Severities"])),
                                     key=lambda idx: result_to_format["Severities"][idx], reverse=True)
             for i in sorted_indices:
-                formatted_result += f"Severity {result_to_format['Severities'][i]} finding (out of 5):\n\n"
-                formatted_result += f"Existing phrase: {result_to_format['Phrases'][i]}\n"
-                formatted_result += f"Recommended replacement: {result_to_format['Recommendations'][i]}\n"
-                formatted_result += f"Explanation: {result_to_format['Explanations'][i]}\n\n"
+                severity = result_to_format['Severities'][i]
+                # only report findings with severity greater than or equal to minimum_importance
+                if severity >= minimum_importance:
+                    formatted_result += f"Severity {severity} finding (out of 5):\n\n"
+                    formatted_result += f"{result_to_format['Explanations'][i]}\n\n"
+                    formatted_result += f"Recommend replacing: {result_to_format['Phrases'][i]}\n"
+                    formatted_result += f"          With this: {result_to_format['Recommendations'][i]}\n\n"
         except Exception as e:
             # include exception in returned results, with raw JSON results
             formatted_result = (f"Error occurred formatting result: {str(e)}\n\n"
                                 f"Raw JSON: {json.dumps(result_to_format, indent=4)}")
             self.evaluation_engine.logger.error(formatted_result)
         return formatted_result
 
@@ -964,20 +981,22 @@
         :rtype: dict
         """
 
         return await super().a_evaluate(chat_history=chat_history, survey_context=survey_context,
                                         survey_locations=survey_locations,
                                         survey_excerpt=EvaluationEngine.clean_whitespace(survey_excerpt), **kwargs)
 
-    def format_result(self, result: dict | None = None) -> str:
+    def format_result(self, result: dict | None = None, minimum_importance: int = 0) -> str:
         """
         Format the evaluation result as a human-readable string.
 
         :param result: Evaluation result to format (or None to use the evaluation_result attribute).
         :type result: dict | None
+        :param minimum_importance: Minimum importance score for filtering results (defaults to 0, which doesn't filter).
+        :type minimum_importance: int
         :return: Formatted evaluation result.
         :rtype: str
         """
 
         # use evaluation_result attribute if no result is passed
         if result is not None:
             result_to_format = result
@@ -990,18 +1009,21 @@
 
         # format and return result
         try:
             formatted_result = ""
             sorted_indices = sorted(range(len(result_to_format["Severities"])),
                                     key=lambda idx: result_to_format["Severities"][idx], reverse=True)
             for i in sorted_indices:
-                formatted_result += f"Severity {result_to_format['Severities'][i]} finding (out of 5):\n\n"
-                formatted_result += f"Existing phrase: {result_to_format['Phrases'][i]}\n"
-                formatted_result += f"Recommended replacement: {result_to_format['Recommendations'][i]}\n"
-                formatted_result += f"Explanation: {result_to_format['Explanations'][i]}\n\n"
+                severity = result_to_format['Severities'][i]
+                # only report findings with severity greater than or equal to minimum_importance
+                if severity >= minimum_importance:
+                    formatted_result += f"Severity {severity} finding (out of 5):\n\n"
+                    formatted_result += f"{result_to_format['Explanations'][i]}\n\n"
+                    formatted_result += f"Recommend replacing: {result_to_format['Phrases'][i]}\n"
+                    formatted_result += f"          With this: {result_to_format['Recommendations'][i]}\n\n"
         except Exception as e:
             # include exception in returned results, with raw JSON results
             formatted_result = (f"Error occurred formatting result: {str(e)}\n\n"
                                 f"Raw JSON: {json.dumps(result_to_format, indent=4)}")
             self.evaluation_engine.logger.error(formatted_result)
         return formatted_result
```

### Comparing `surveyeval-0.1.8/src/surveyeval/evaluation_engine.py` & `surveyeval-0.1.9/src/surveyeval/evaluation_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,30 +579,36 @@
         # call evaluation engine to run evaluation chain
         self.evaluation_result = await self.evaluation_engine.a_run_evaluation_chain(
             task_system_prompt=self.task_system_prompt_template.format(**kwargs),
             question=self.question_template.format(**kwargs),
             followups=self.followups, chat_history=chat_history)
         return self.evaluation_result
 
-    def format_result(self, result: dict | None = None) -> str:
+    def format_result(self, result: dict | None = None, minimum_importance: int = 0) -> str:
         """
         Format the evaluation result as a human-readable string.
 
         :param result: Evaluation result to format (or None to use the evaluation_result attribute).
         :type result: dict | None
+        :param minimum_importance: Minimum importance score for filtering results (defaults to 0, which doesn't filter).
+        :type minimum_importance: int
         :return: Formatted evaluation result.
         :rtype: str
         """
 
         # use evaluation_result attribute if no result is passed
         if result is not None:
             result_to_format = result
         else:
             result_to_format = self.evaluation_result[0]
 
+        # raise error if asked to filter for importance
+        if minimum_importance > 0:
+            raise NotImplementedError("No base class implementation for filtering by importance.")
+
         # return empty string if no result is available to format
         if result_to_format is None:
             return ""
 
         # format result as a list of key-value pairs
         formatted_results = []
         for key, value in result_to_format.items():
@@ -617,14 +623,27 @@
                 formatted_results.append(f"{key}: {value_str}")
             else:
                 formatted_results.append(f"{key}: {value}")
 
         # return the formatted result with each key-value pair on its own line
         return '\n'.join(formatted_results)
 
+    def standardize_result(self, result: dict | None = None) -> list[dict]:
+        """
+        Reorganize the evaluation result into a list of recommendations in a standardized format.
+
+        :param result: Evaluation result to format (or None to use the evaluation_result attribute).
+        :type result: dict | None
+        :return: List of recommendations, each of which is a dict with the following keys: importance (int 1-5),
+            replacement_original (str), replacement_suggested (str), explanation (str).
+        :rtype: list[dict]
+        """
+
+        raise NotImplementedError("No base class implementation for standardize_result().")
+
     @staticmethod
     def condition_is_value(response_dict: dict, condition_key: str, condition_value: str) -> bool:
         """
         Check if a condition is met in a given response dictionary: "is value" (string match).
 
         :param response_dict: Response dictionary to check.
         :type response_dict: dict
```

### Comparing `surveyeval-0.1.8/src/surveyeval/html_tools.py` & `surveyeval-0.1.9/src/surveyeval/html_tools.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.8/src/surveyeval/resources/EmptyForm.xlsx` & `surveyeval-0.1.9/src/surveyeval/resources/EmptyForm.xlsx`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.8/src/surveyeval/survey_parser.py` & `surveyeval-0.1.9/src/surveyeval/survey_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1790,21 +1790,21 @@
                 if translation['language'] and translation['language'] != primary_language:
                     language_suffix = f":{translation['language']}"
                     label_column = 'label' + language_suffix
                     hint_column = 'hint' + language_suffix
                     # also add translation columns as necessary
                     if label_column not in survey_columns:
                         _add_header_to_first_empty_cell(survey_ws, label_column)
-                        survey_columns = _get_columns_from_headers(survey_ws)
+                        survey_columns = _get_columns_from_headers(survey_ws, 1)
                     if translation['options'] and label_column not in choices_columns:
                         _add_header_to_first_empty_cell(choices_ws, label_column)
-                        choices_columns = _get_columns_from_headers(choices_ws)
+                        choices_columns = _get_columns_from_headers(choices_ws, 1)
                     if hint_column not in survey_columns:
                         _add_header_to_first_empty_cell(survey_ws, hint_column)
-                        survey_columns = _get_columns_from_headers(survey_ws)
+                        survey_columns = _get_columns_from_headers(survey_ws, 1)
                 else:
                     label_column = 'label'
                     hint_column = 'hint'
 
                 # add the question to the survey sheet
                 survey_ws.cell(row=survey_row_counter, column=survey_columns['type'],
                                value='text' if not translation['options'] else 'select_one ' + safe_question_id)
```

### Comparing `surveyeval-0.1.8/src/surveyeval.egg-info/PKG-INFO` & `surveyeval-0.1.9/src/surveyeval.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
@@ -83,29 +83,30 @@
 1. ``.docx``: Word files are read in the ``read_docx()`` function, using LangChain's ``UnstructuredFileLoader()`` function.
    Note that text within "content controls" is effectively invisible, so you might need to open your file, select all, 
    and select "Remove content controls" to render the text visible 
    (`see here for more on content controls <https://learn.microsoft.com/en-us/office/client-developer/word/content-controls-in-word>`_).
 2. ``.pdf``: PDF files are read in the ``read_pdf_combined()`` function, which tries to read the text and tables in a PDF
    (separately), combine them together, and then fall back to using an OCR reader if that process didn't find much 
    text. There is a ton of room for improvement here.
-3. ``.xlsx``: Excel files are read in the ``parse_xlsx()`` function, in two stages. First, it assumes that the file is in
-   `XLSForm format <https://xlsform.org/en/>`_ and uses `the pyxform library <https://github.com/XLSForm/pyxform>`_ to
-   read the survey. If it encounters an error, it falls back to using LangChain's ``UnstructuredExcelLoader()`` to load
-   the workbook in HTML format, then uses that HTML as the raw text for parsing. There is much that can be improved,
-   particularly in how XLSForms are handled (e.g., the current approach doesn't handle translations well).
-4. ``.csv``: CSV files are read in the ``parse_csv()`` function, also using two stages. First, it assumes that the file
-   is a REDCap data dictionary and parses the columns accordingly. If it encounters an error, it falls back to just
-   reading the file as raw text. There is much that can be improved here, particularly in how REDCap data 
-   dictionaries are handled (e.g., the current approach doesn't handle modules or translations).
+3. ``.xlsx``: Excel files are read in the ``parse_xlsx()`` function, in two ways. If the file looks like it's in
+   `XLSForm format <https://xlsform.org/en/>`_, it parses it accordingly; this parsing should be completely lossless
+   and requires no additional parsing at later stages. If the file does not appear to be an XLSForm, the reader falls
+   back to using LangChain's ``UnstructuredExcelLoader()`` to load the workbook in HTML format, then uses that HTML as
+   the raw text for parsing. XLSForm handling should be robust, but there is much that can be improved in how other
+   formats are handled.
+4. ``.csv``: CSV files are read in the ``parse_csv()`` function, also in two ways. If the file looks like a REDCap
+   data dictionary, it will parse the columns accordingly (requiring little to no later processing). Otherwise, it
+   falls back to just reading the file as raw text. There is much that can be improved here, particularly in how
+   REDCap data dictionaries are handled (e.g., the current approach doesn't handle modules or translations).
 5. ``.html``: HTML files are read in the ``read_html()`` function, then converted into markdown for parsing.
 
-All of the raw content is split into 6,000-character chunks with 500 characters of overlap, before being passed on
-for parsing. This is necessary to both (a) avoid overflowing LLM context windows, and (b) allow the LLM to focus on
-a tractable amount of text in any given request (with the latter becoming more important as the constraints on context
-windows are relaxed).
+All of the raw content is split into 3,000-character chunks with 500 characters of overlap, before being passed on
+for parsing. This is necessary to (a) avoid overflowing LLM context windows, (b) avoid overflowing output token
+limits, and (c) allow the LLM to focus on a tractable amount of text in any given request (with the latter becoming
+more important as the constraints on context windows are relaxed).
 
 Overall, the code for reading files performs pretty poorly for all but the simplest formats. There's much work to do
 here to improve quality.
 
 Parsing input files
 ^^^^^^^^^^^^^^^^^^^
 
@@ -126,15 +127,15 @@
 Roadmap
 -------
 
 There's much that can be improved here. For example:
 
 * We should track and report costs for the evaluation stage of the process.
 * We should generally overhaul the ``survey_parser`` module to better ingest different file formats into
-  raw text that works consistently well for parsing. Better PDF, XLSForm, and REDCap support, in particular, would be
+  raw text that works consistently well for parsing. Better PDF and REDCap support, in particular, would be
   nice.
 * We should add an LLM cache that avoids calling out to the LLM for responses that it already has from prior requests.
   After all, it's common to evaluate the same instrument multiple times, and it's incredibly wasteful to 
   keep going back to the LLM for the same responses every time (for requests that haven't changed in any way).
 * We should improve how findings are scored and filtered, to avoid giving overwhelming numbers of minor 
   recommendations.
 * We should improve the output format to be more user-friendly. (For example, a direct Word output with comments and
```

