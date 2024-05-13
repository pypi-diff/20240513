# Comparing `tmp/sqldatamodel-0.5.1.tar.gz` & `tmp/sqldatamodel-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldatamodel-0.5.1.tar", last modified: Fri May 10 18:10:15 2024, max compression
+gzip compressed data, was "sqldatamodel-0.5.2.tar", last modified: Mon May 13 20:02:20 2024, max compression
```

## Comparing `sqldatamodel-0.5.1.tar` & `sqldatamodel-0.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 18:10:15.831051 sqldatamodel-0.5.1/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    29557 2024-05-10 18:10:15.819404 sqldatamodel-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    27665 2024-05-07 00:24:25.000000 sqldatamodel-0.5.1/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 18:10:15.832054 sqldatamodel-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2424 2024-05-10 18:08:01.000000 sqldatamodel-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 18:10:14.364711 sqldatamodel-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 18:10:15.564811 sqldatamodel-0.5.1/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.5.1/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.5.1/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.5.1/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   613810 2024-05-10 18:09:36.000000 sqldatamodel-0.5.1/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.5.1/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.5.1/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.5.1/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.5.1/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.5.1/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-10 18:10:15.740831 sqldatamodel-0.5.1/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.5.1/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.5.1/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-05-10 18:10:15.815609 sqldatamodel-0.5.1/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    29557 2024-05-10 18:10:14.000000 sqldatamodel-0.5.1/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-05-10 18:10:14.000000 sqldatamodel-0.5.1/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 18:10:14.000000 sqldatamodel-0.5.1/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-10 18:10:14.000000 sqldatamodel-0.5.1/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 18:10:15.758642 sqldatamodel-0.5.1/tests/
--rw-rw-rw-   0        0        0    65741 2024-05-10 18:08:03.000000 sqldatamodel-0.5.1/tests/test_Future.py
--rw-rw-rw-   0        0        0    65744 2024-05-10 18:08:02.000000 sqldatamodel-0.5.1/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.331551 sqldatamodel-0.5.2/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 sqldatamodel-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    29574 2024-05-13 20:02:20.320546 sqldatamodel-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27682 2024-05-13 19:59:36.000000 sqldatamodel-0.5.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 sqldatamodel-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 20:02:20.332550 sqldatamodel-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     2424 2024-05-13 19:59:51.000000 sqldatamodel-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:02:18.364786 sqldatamodel-0.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 20:02:19.562318 sqldatamodel-0.5.2/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6644 2024-05-03 15:03:44.000000 sqldatamodel-0.5.2/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 sqldatamodel-0.5.2/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 sqldatamodel-0.5.2/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   621050 2024-05-13 20:01:36.000000 sqldatamodel-0.5.2/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 sqldatamodel-0.5.2/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 sqldatamodel-0.5.2/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 sqldatamodel-0.5.2/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 sqldatamodel-0.5.2/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 sqldatamodel-0.5.2/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.222090 sqldatamodel-0.5.2/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 sqldatamodel-0.5.2/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 sqldatamodel-0.5.2/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.313154 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    29574 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-13 20:02:18.000000 sqldatamodel-0.5.2/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 20:02:20.242314 sqldatamodel-0.5.2/tests/
+-rw-rw-rw-   0        0        0    66698 2024-05-13 17:45:04.000000 sqldatamodel-0.5.2/tests/test_Future.py
+-rw-rw-rw-   0        0        0    66701 2024-05-13 17:46:25.000000 sqldatamodel-0.5.2/tests/test_SQLDataModel.py
```

### Comparing `sqldatamodel-0.5.1/LICENSE` & `sqldatamodel-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/PKG-INFO` & `sqldatamodel-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.5.1
+Version: 0.5.2
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
@@ -581,12 +581,12 @@
 
 Please make sure to update tests as appropriate.
 
 ---
 
 ### License
 
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://github.com/AnteT/SQLDataModel/blob/master/LICENSE)
 
 
 Thank you!  
 Ante Tonkovic-Capin
```

### Comparing `sqldatamodel-0.5.1/README.md` & `sqldatamodel-0.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -556,12 +556,12 @@
 
 Please make sure to update tests as appropriate.
 
 ---
 
 ### License
 
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://github.com/AnteT/SQLDataModel/blob/master/LICENSE)
 
 
 Thank you!  
 Ante Tonkovic-Capin
```

### Comparing `sqldatamodel-0.5.1/setup.py` & `sqldatamodel-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.5.1',
+     version='0.5.2',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords=['SQL','ETL','dataframe','terminal-tables','pretty-print-tables','sql2sql','data-analysis','data-science','datamodel','extract','transform','load','web-scraping-tables','data-mining','html','html-table-parsing','apache-arrow','pyarrow','pyarrow-conversion','pyarrow-to-table','pyarrow-to-sql','pyarrow-to-csv','parquet-file-parsing','csv','csv-parsing','markdown','markdown-table-parsing','latex','latex-table-parsing','delimited','delimited-data-parsing','file-conversion','format-conversion','terminal-styling','table-styling','from-sqlite','to-sqlite','from-postgresql','to-postgresql','sql-to-sql','excel','xlsx-file','excel-to-sql','DataFrames','polars2pandas','pandas2polars'],
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/ANSIColor.py` & `sqldatamodel-0.5.2/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/HTMLParser.py` & `sqldatamodel-0.5.2/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/JSONEncoder.py` & `sqldatamodel-0.5.2/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/SQLDataModel.py` & `sqldatamodel-0.5.2/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,18 +614,18 @@
 
             # Generate and view the returned table chunks
             for chunk in SQLDataModel.generate_html_table_chunks(html_source):
                 print('Chunk:', chunk)
             
         This will output:
 
-            ```text
+        ```text
             Chunk: <table><tr><td>Table 1</td></tr></table>
             Chunk: <table><tr><td>Table 2</td></tr></table>
-            ```
+        ```
         
         Note:
             - HTML content before the first ``<table>`` element and after the last ``</table>`` element is ignored and not yielded.
             - See :meth:`SQLDataModel.from_html()` for full implementation and how this function is used for HTML parsing.
         """
         start_index, table_found = 0, False
         while True:
@@ -1408,15 +1408,15 @@
             display_max_rows = sdm.get_display_max_rows()
 
             # By default rows will be limited by current terminal height
             print(display_max_rows) # None
         
         Note:
             - This does not affect the actual number of rows in the model, only the maximum **displayed**.
-            - Use :meth:`SQLDataModel.set_display_max_rows()` to explicitely set a max row limit instead of using terminal height.
+            - Use :meth:`SQLDataModel.set_display_max_rows()` to explicitly set a max row limit instead of using terminal height.
         """
         return self.display_max_rows
     
     def set_display_max_rows(self, rows:int|None) -> None:
         """
         Sets value at :py:attr:`SQLDataModel.display_max_rows` to limit maximum rows displayed when ``repr`` or ``print`` is called. Use ``rows = None`` to derive max number to display from the current terminal height.
 
@@ -2248,81 +2248,144 @@
                 self.set_column_dtypes(column=col, dtype=dtype)
 
 #############################################################################################################
 ############################################ class constructors #############################################
 #############################################################################################################
 
     @classmethod
-    def from_shape(cls, n_rows:int, n_cols:int, dtype:Literal['bytes','datetime','float','int','str']=None) -> SQLDataModel:
+    def from_shape(cls, shape:tuple[int, int], fill:Any=None, headers:list[str]=None, dtype:Literal['bytes','date','datetime','float','int','str']=None, **kwargs) -> SQLDataModel:
         """
-        Returns an empty SQLDataModel of shape (`n_rows`, ``n_cols``) as a convenience method to quickly build a model through an iterative approach. 
-        By default, no particular ``dtype`` is assigned given the flexibility of sqlite3 when it comes to column datatypes, however one can be enforced in the schema be providing a valid datatype identifier to the ``dtype`` keyword argument.
+        Returns a SQLDataModel from shape ``(N rows, M columns)`` as a convenience method to quickly build a model through an iterative approach. 
+        By default, no particular data type is assigned given the flexibility of ``sqlite3``, however one can be inferred by providing an initial ``fill`` value or explicitly by providing the ``dtype`` argument.
 
         Parameters:
-            ``n_rows`` (int): The number of rows for the new SQLDataModel.
-            ``n_cols`` (int): The number of columns for the new SQLDataModel.
-            ``dtype`` (str) (optional): A valid python or SQL datatype to initialize the n-dimensional model with
+            ``shape`` (tuple[int, int]): The shape to initialize the SQLDataModel with as ``(M, N)`` where ``M`` is the number of rows and ``N`` is the number of columns.
+            ``fill`` (Any, optional): The scalar fill value to populate the new SQLDataModel with. Default is None, using SQL null values or deriving from ``dype`` if provided.
+            ``headers`` (list[str], optional): The headers to use for the model. Default is None, incrementing headers ``0, 1, ..., N`` where ``N`` is the number of columns.
+            ``dtype`` (str, optional): A valid python or SQL datatype to initialize the n-dimensional model with. Default is None, using the SQL text type.
+            ``**kwargs``: Additional keyword arguments to pass to the ``SQLDataModel`` constructor.            
 
         Raises:
-            ``TypeError``: If ``n_rows`` is not of type 'int' or if ``n_cols`` is not of type 'int'.
+            ``TypeError``: If ``M`` or ``N`` are not of type 'int' representing a valid shape to initialize a SQLDataModel with.
+            ``ValueError``: If ``M`` or ``N`` are not positive integer values representing valid nonzero row and column dimensions.
             ``ValueError``: If ``dtype`` is not a valid python or SQL convertible datatype to initialize the model with.
 
         Returns:
             ``SQLDataModel``: Instance with the specified number of rows and columns, initialized with by ``dtype`` fill values or with ``None`` values (default).
 
         Example::
         
             from SQLDataModel import SQLDataModel
 
-            # Define shape
-            n_rows, n_cols = 10, 3
+            # Create a 3x3 model filled by 'X'
+            sdm = SQLDataModel.from_shape((3,3), fill='X')            
 
-            # Create an empty SQLDataModel with 10 rows and 3 columns
-            sdm = SQLDataModel.from_shape(n_rows, n_cols)
+            # View it
+            print(sdm)
+            
+        This will output a 3x3 grid of 'X' characters:
 
-            # Assign rows
-            for row in range(n_rows):
-                sdm[row] = ('john', 'smith', 29)
-            
-            # Assign specific cells
-            for row in range(n_rows):
-                for col in range(n_cols):
-                    sdm[row, col] = f"cell at index {row}, {col}"
+        ```text
+            ┌───┬─────┬─────┬─────┐
+            │   │ 0   │ 1   │ 2   │
+            ├───┼─────┼─────┼─────┤
+            │ 0 │ X   │ X   │ X   │
+            │ 1 │ X   │ X   │ X   │
+            │ 2 │ X   │ X   │ X   │
+            └───┴─────┴─────┴─────┘
+            [3 rows x 3 columns]
+        ```
+
+        We can iteratively build the model from the shape dimensions:
+
+        ```python
+            from SQLDataModel import SQLDataModel
+
+            # Define shape
+            shape = (6,6)
             
-            # Assign headers if needed
-            sdm.set_headers(['first', 'last', 'age'])
+            # Initialize the multiplcation table with integer dtypes
+            mult_table = SQLDataModel.from_shape(shape=shape, dtype='int')
+
+            # Construct the table values
+            for x in range(shape[0]):
+                for y in range(shape[1]):
+                    mult_table[x, y] = x * y
+            
+            # View the multiplcation table
+            print(mult_table)
+        ```
         
+        This will output our 6x6 multiplication table:
+
+        ```text
+            ┌───┬─────┬─────┬─────┬─────┬─────┬─────┐
+            │   │   0 │   1 │   2 │   3 │   4 │   5 │
+            ├───┼─────┼─────┼─────┼─────┼─────┼─────┤
+            │ 0 │   0 │   0 │   0 │   0 │   0 │   0 │
+            │ 1 │   0 │   1 │   2 │   3 │   4 │   5 │
+            │ 2 │   0 │   2 │   4 │   6 │   8 │  10 │
+            │ 3 │   0 │   3 │   6 │   9 │  12 │  15 │
+            │ 4 │   0 │   4 │   8 │  12 │  16 │  20 │
+            │ 5 │   0 │   5 │  10 │  15 │  20 │  25 │
+            └───┴─────┴─────┴─────┴─────┴─────┴─────┘
+            [6 rows x 6 columns]
+        ```
+
+        Change Log:
+            - Version 0.5.2 (2024-05-13):
+                - Added ``shape`` parameter in lieu of separate ``n_rows`` and ``n_cols`` arguments.
+                - Added ``fill`` parameter to populate resulting SQLDataModel with values to override type-specific initialization defaults.
+                - Added ``headers`` parameter to explicitly set column names when creating the SQLDataModel.
+                - Added ``**kwargs`` parameter to align more closely with usage patterns of other model initializing constructor methods.
+
+        Note:
+            - If both ``fill`` and ``dtype`` are provided, the data type will be derived from ``type(fill)`` overriding or ignoring the specified ``dtype``.
+            - If only ``dtype`` is provided, sensible default initialization fill values will be used to populate the model such as 0 or 0.0 for numeric and empty string or null for others.
+            - For those data types not natively implemented by ``sqlite3`` such as ``date`` and ``datetime``, today's date and now's datetime will be used respectively for initialization values.
         """
+        try:
+            n_rows, n_cols = shape
+        except ValueError:
+            raise ValueError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid length '{len(shape)}', argument for `shape` must be a tuple or list with 2 elements of type 'int' representing `(n_rows, n_cols)`")
+            ) from None            
+        except TypeError:
+            raise TypeError(
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(shape).__name__}', argument for `shape` must be a tuple or list with 2 elements of type 'int' representing `(n_rows, n_cols)`")
+            ) from None
         if not isinstance(n_rows, int):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(n_rows).__name__}', argument of type 'int' expected for `n_rows` parameter")
             )
         if not isinstance(n_cols, int):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(n_cols).__name__}', argument of type 'int' expected for `n_cols` parameter")
             )
-        if dtype is not None:
-            if dtype not in ('bytes','datetime','float','int','str'):
+        if fill is None and dtype is not None:
+            if dtype not in ('bytes','date','datetime','float','int','str'):
                 raise ValueError(
                     SQLDataModel.ErrorFormat(f"ValueError: invalid argument '{dtype}', `dtype` must be one of 'bytes','datetime','float','int','str'")
                 )
             else:
                 if dtype == 'bytes':
                     fill_value = b''
+                elif dtype == 'date':
+                    fill_value = datetime.date.today()
                 elif dtype == 'datetime':
                     fill_value = datetime.datetime.now()
                 elif dtype == 'float':
                     fill_value = 0.0
                 elif dtype == 'int':
                     fill_value = 0
                 else:
                     fill_value = ''
         else:
-            fill_value = None
-        return cls([[fill_value for _ in range(n_cols)] for _ in range(n_rows)])
+            fill_value = fill
+        return cls(data=[[fill_value for _ in range(n_cols)] for _ in range(n_rows)], headers=headers, **kwargs)
         
     @classmethod
     def from_csv(cls, csv_source:str, infer_types:bool=True, encoding:str = 'Latin1', delimiter:str = ',', quotechar:str = '"', headers:list[str] = None, **kwargs) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` generated from the provided CSV source, which can be either a file path or a raw delimited string.
 
         Parameters:
@@ -6320,55 +6383,79 @@
             except Exception as e:
                 raise Exception (
                     SQLDataModel.ErrorFormat(f"{type(e).__name__}: {e} encountered when trying to open and write text to '{filename}'")
                 ) from None
         else:
             return table_repr 
 
-    def to_local_db(self, db:str=None) -> None:
+    def to_local_db(self, filename:str) -> None:
         """
-        Stores the ``SQLDataModel`` internal in-memory database to a local disk database.
+        Writes the ``SQLDataModel`` in-memory database to disk as a SQLite database file using the specified filename.
 
         Parameters:
-            ``db`` (str, optional): The filename or path of the target local disk database. If ``None``, the current filename will be used as a default target.
+            ``filename`` (str): The filename or filepath to use when writing the model to disk.
 
         Raises:
-            ``TypeError``: If ``db`` is provided and is not of type 'str' representing a valid sqlite database save path.
+            ``TypeError``: If ``filename`` is provided and is not of type 'str' representing a valid sqlite database save path.
             ``sqlite3.Error``: If there is an issue with the SQLite database operations during backup.
 
         Returns:
             ``None``
             
         Example::
 
             import sqlite3
             from SQLDataModel import SQLDataModel
 
-            # Example 1: Store the in-memory database to a local disk database with a specific filename
-            sdm.to_local_db("local_database.db")
+            # Sample data
+            data = [('Alice', 20, 'F'), ('Billy', 25, 'M'), ('Chris', 30, 'M')]
+
+            # Create the model
+            sdm = SQLDataModel(data, headers=['Name','Age','Sex'])
+
+            # Filename to use for database
+            db_file = "model.db"
 
-            # Example 2: Store the in-memory database to a local disk database using the default filename
-            sdm.to_local_db()
+            # Write the in-memory database model to disk
+            sdm.to_local_db(db_file)
 
-            # Reload model from local db using default path 'sdm_local_db.db'
-            sdm_loaded = SQLDataModel.from_sql("sdm", sqlite3.connect("sdm_local_db.db"))
+            # Loading the model back from disk can now be done at anytime
+            sdm = SQLDataModel.from_sql("sdm", sqlite3.connect(db_file))
+
+            # View restored model
+            print(sdm)
+
+        This will output the model we originally created:
+
+        ```text
+            ┌───┬───────┬─────┬─────┐
+            │   │ Name  │ Age │ Sex │
+            ├───┼───────┼─────┼─────┤
+            │ 0 │ Alice │  20 │ F   │
+            │ 1 │ Billy │  25 │ M   │
+            │ 2 │ Chris │  30 │ M   │
+            └───┴───────┴─────┴─────┘
+            [3 rows x 3 columns]
+        ```
+
+        Change Log:
+            - Version 0.5.2 (2024-05-13):
+                - Renamed ``db`` parameter to ``filename`` for package consistency and to avoid confusion between similarily named database objects.
+                - Changed ``filename`` from keyword to positional argument making it a required parameter to avoid accidental overwriting.
 
         Note:
-            - The method connects to the specified local disk database using ``sqlite3``.
-            - It performs a backup of the in-memory database to the local disk database.
-            - If ``db=None``, the current filename is used as the default target.
-            - After successful backup, it prints a success message indicating the creation of the local database.
+            - Use any compatible SQL API to load the resulting database file or use :meth:`SQLDataModel.from_sql()` to reload it back into a ``SQLDataModel``.
+            - Table name is determined by value at :py:attr:`SQLDataModel.sql_model` which is set to ``'sdm'`` by default, use :meth:`SQLDataModel.set_model_name()` to modify.
         """
-        if not isinstance(db, str) and db is not None:
+        if not isinstance(filename, str):
             raise TypeError(
-                SQLDataModel.ErrorFormat(f"invalid type '{type(db).__name__}', argument for `db` must be of type 'str' representing a valid sqlite database save path")
+                SQLDataModel.ErrorFormat(f"TypeError: invalid type '{type(filename).__name__}', argument for `filename` must be of type 'str' representing a valid sqlite database save path")
             )
-        if db is None:
-            db = "sdm_local_db.db"
-        with sqlite3.connect(db) as target:
+        self.sql_db_conn.commit()
+        with sqlite3.connect(filename) as target:
             self.sql_db_conn.backup(target)
 
 ####################################################################################################################
 ############################################## dunder special methods ##############################################
 ####################################################################################################################
 
     def __lt__(self, other) -> SQLDataModel:
@@ -10755,70 +10842,91 @@
         except Exception as e:
             self.sql_db_conn.rollback()
             raise SQLProgrammingError(
                 SQLDataModel.ErrorFormat(f'SQLProgrammingError: unable to update values, SQL execution failed with: "{e}"')
             ) from None
         self._update_model_metadata(update_row_meta=True)        
 
-    def update_index_at(self, row_index:int, column_index:int|str, value=None) -> None:
+    def update_index_at(self, row_index:int, column_index:int|str, value:Any=None) -> None:
         """
         Updates a specific cell in the ``SQLDataModel`` at the given row and column indices with the provided value.
 
         Parameters:
             ``row_index`` (int): The index of the row to be updated.
             ``column_index`` (int or str): The index or name of the column to be updated.
-            ``value``: The new value to be assigned to the specified cell.
+            ``value (Any, optional)``: The new value to be assigned to the specified cell.
 
         Raises:
             ``TypeError``: If ``row_index`` is not of type 'int' or if ``column_index`` is not of type 'int' or 'str'.
-            ``ValueError``: If the provided row index is outside the current model range.
-            ``IndexError``: If the provided column index (when specified as an integer) is outside of the current model range.
+            ``IndexError``: If row or column provided as an 'int' but is outside of the current model row or column range.
+            ``ValueError``: If column provided as a 'str' but is not found in the current model headers.
             ``SQLProgrammingError``: If there is an issue with the SQL execution during the update.
         
         Returns:
             ``None``
 
         Example::
 
             from SQLDataModel import SQLDataModel
 
-            headers = ['idx', 'first', 'last', 'age']
-            data = [
-                (0, 'john', 'smith', 27)
-                ,(1, 'sarah', 'west', 29)
-                ,(2, 'mike', 'harlin', 36)
-                ,(3, 'pat', 'douglas', 42)
-            ]
+            # Create an initial 3x3 model filled with dashes
+            sdm = SQLDataModel.from_shape((3,3), fill='---', headers=['A', 'B', 'C'])
 
-            # Create the model with sample data
-            sdm = SQLDataModel(data,headers)
+            # Update cell based on integer indicies
+            sdm.update_index_at(0, 0, 'Top Left')
+            sdm.update_index_at(0, 2, 'Top Right')
+
+            # Update cell based on row index and column name
+            sdm.update_index_at(2, 'A', 'Bottom Left')
+            sdm.update_index_at(2, 'C', 'Bottom Right')
+
+            # Update based on negative row and column indexing
+            sdm.update_index_at(-2, -2, 'Center')
+
+            # View result
+            print(sdm)
 
-            # Example 1: Update a cell in the first row and second column
-            sdm.update_index_at(0, 1, 'NewValue')
+        This will output cumulative result of our updates:
+
+        ```text
+            ┌───┬─────────────┬────────┬──────────────┐
+            │   │ A           │ B      │ C            │
+            ├───┼─────────────┼────────┼──────────────┤
+            │ 0 │ Top Left    │ ---    │ Top Right    │
+            │ 1 │ ---         │ Center │ ---          │
+            │ 2 │ Bottom Left │ ---    │ Bottom Right │
+            └───┴─────────────┴────────┴──────────────┘
+            [3 rows x 3 columns]
+        ```
 
-            # Example 2: Update a cell in the 'Name' column of the third row
-            sdm.update_index_at(2, 'Name', 'John Doe')
+        Change Log:
+            - Version 0.5.2 (2024-05-13):
+                - Modified ``row_index`` parameter to use :py:attr:`SQLDataModel.indicies` to index into rows in lieu of row index value equality.
 
+        Important:
+            - Indexing is done using zero-based integers and not done by index value. Most of the time this distinction is irrelevant as the row index at position '0' will have an index value of '0', however this can change after transformation operations like filter or sort. To reset and realign the index value use :meth:`SQLDataModel.reset_index()` or use :py:attr:`SQLDataModel.indicies` to view the current row indicies.
+        
         Note:
-            - If an error occurs during SQL execution, it rolls back the changes and raises a ``SQLProgrammingError``.
+            - This method only updates individual cells in the current model based on integer indexing for both rows and columns using their (row, column) position.
+            - To broadcast updates across row and column dimensions use the syntax of ``sdm[row, column] = value`` or see :meth:`SQLDataModel.__setitem__()` for more details.
         """        
         if not isinstance(row_index, int):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid row index type '{type(row_index).__name__}', rows must be indexed by type 'int'")
             )
         if not isinstance(column_index, (int,str)):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid column index type '{type(row_index).__name__}', columns must be indexed by type 'int' or 'str', use `.get_headers()` to view current model headers")
             )
-        if row_index < 0:
-            row_index = self.row_count + row_index
-        if row_index < 0 or row_index > self.row_count:
-            raise ValueError(
-                SQLDataModel.ErrorFormat(f"ValueError: invalid row index '{row_index}', provided row index is outisde of current model range '0:{self.row_count}'")
-            )
+        try:
+            row_index = self.indicies[row_index]
+        except IndexError:
+            raise IndexError(
+                SQLDataModel.ErrorFormat(f"IndexError: invalid row index '{row_index}', provided row index is outisde of current model range '0:{self.row_count}'")
+            ) from None
         if isinstance(column_index, int):
             try:
                 column_index = self.headers[column_index]
             except IndexError:
                 raise IndexError(
                     SQLDataModel.ErrorFormat(f"IndexError: invalid column index '{column_index}', provided column index is outside of current model range '0:{self.column_count}'")
                 ) from None
@@ -11148,14 +11256,15 @@
             # Create a new column named "new_column" with default values
             sdm._update_rows_and_columns_with_values(
                 columns_to_update=["new_column"],
                 values_to_update=[(None,)] * sdm.row_count
             )
 
         Note:
+            - Used by :meth:`SQLDataModel.__setitem__()` to broadcast updates across row and column index ranges.
             - To create a new column, pass a single header item in a list to the ``columns_to_update`` parameter.
             - To copy an existing column, pass the corresponding data is a list of tuples to the ``values_to_update`` parameter.        
         """
         update_sql_script = None
         # this is the problem, even if the indicies are 2-7, this will generate 0:5 since the rowcount is 5 regardless of min and max indicies
         rows_to_update = rows_to_update if rows_to_update is not None else self.indicies # use all rows if none specified, courtesy of new `indicies` property
         columns_to_update = columns_to_update if columns_to_update is not None else self.headers
```

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/StandardDeviation.py` & `sqldatamodel-0.5.2/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/converters.py` & `sqldatamodel-0.5.2/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/demo.py` & `sqldatamodel-0.5.2/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/exceptions.py` & `sqldatamodel-0.5.2/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel/extensions/str_utils.c` & `sqldatamodel-0.5.2/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel.egg-info/PKG-INFO` & `sqldatamodel-0.5.2/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.5.1
+Version: 0.5.2
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal-tables,pretty-print-tables,sql2sql,data-analysis,data-science,datamodel,extract,transform,load,web-scraping-tables,data-mining,html,html-table-parsing,apache-arrow,pyarrow,pyarrow-conversion,pyarrow-to-table,pyarrow-to-sql,pyarrow-to-csv,parquet-file-parsing,csv,csv-parsing,markdown,markdown-table-parsing,latex,latex-table-parsing,delimited,delimited-data-parsing,file-conversion,format-conversion,terminal-styling,table-styling,from-sqlite,to-sqlite,from-postgresql,to-postgresql,sql-to-sql,excel,xlsx-file,excel-to-sql,DataFrames,polars2pandas,pandas2polars
@@ -581,12 +581,12 @@
 
 Please make sure to update tests as appropriate.
 
 ---
 
 ### License
 
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://github.com/AnteT/SQLDataModel/blob/master/LICENSE)
 
 
 Thank you!  
 Ante Tonkovic-Capin
```

### Comparing `sqldatamodel-0.5.1/src/SQLDataModel.egg-info/SOURCES.txt` & `sqldatamodel-0.5.2/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldatamodel-0.5.1/tests/test_Future.py` & `sqldatamodel-0.5.2/tests/test_Future.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,14 +446,31 @@
     inferred_output = sdm.data(include_headers=True)
     inferred_output, headers_output = inferred_output[1:], inferred_output[0]
     assert headers_input == headers_output
     for i in range(len(typed_input)):
         assert typed_input[i] == inferred_output[i]
 
 @pytest.mark.core
+def test_from_shape(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    row_lower, row_upper = 1, len(input_data)
+    col_lower, col_upper = 1, len(input_headers)
+    rand_row = random.randint(row_lower, row_upper)
+    rand_col = random.randint(col_lower, col_upper)
+    input_shape = (rand_row, rand_col)
+    sdm = SQLDataModel.from_shape(shape=input_shape, fill=None, dtype=None)
+    output_shape = sdm.shape
+    assert output_shape == input_shape
+    test_fills = (b'bytes', None, 'strings', 12, 3.14, datetime.date(1999,12,31), datetime.datetime(1999, 12, 31, 23, 59, 59), True)
+    for input_fill in test_fills:
+        expected_output = [tuple([input_fill for _ in range(rand_col)]) for _ in range(rand_row)]
+        output_data = SQLDataModel.from_shape(shape=input_shape, fill=input_fill, display_float_precision=2).data(strict_2d=True)
+        assert output_data == expected_output
+
+@pytest.mark.core
 def test_to_from_dict():
     input_dict = {0: ('hTpigTHKcfoK', 285, -497.17176, 0, datetime.date(1914, 6, 27), b'zPx3Bp', None, datetime.datetime(1985, 11, 10, 14, 20, 59)), 1: ('mNHnKXaXQv', -673, 106.451792, 1, datetime.date(2003, 5, 8), b'vKo', None, datetime.datetime(1996, 2, 1, 14, 39, 36)), 2: ('nVgx', 622, 884.861723, 1, datetime.date(1907, 4, 19), b'aRdeb', None, datetime.datetime(1912, 2, 18, 6, 32, 16)), 3: ('0LXSG8x', 393, 360.566821, 0, datetime.date(2021, 2, 3), b'eoPni5I', None, datetime.datetime(1916, 6, 3, 7, 23, 18)), 4: ('sM2wmeOV90', -136, -770.896514, 1, datetime.date(1993, 8, 27), b'pCzfOwz1d', None, datetime.datetime(1920, 8, 27, 17, 45, 19)), 5: ('xBZ', 221, 769.5769, 1, datetime.date(1908, 9, 25), b'9gzv1plB_rp5', None, datetime.datetime(1978, 11, 17, 0, 42, 52)), 6: ('xnq6', -870, 501.755599, 0, datetime.date(1916, 3, 22), b'X0gOHafUo', None, datetime.datetime(1970, 5, 22, 3, 56, 8)), 7: ('eNGpCr5QnuVd', -212, 537.197465, 1, datetime.date(1960, 9, 6), b'Dnzdx9qW', None, datetime.datetime(1933, 2, 4, 23, 35, 9)), 8: ('Xz', -219, -319.649054, 1, datetime.date(1933, 9, 28), b'rQTWODlnd', None, datetime.datetime(1934, 5, 20, 6, 45, 21)), 9: ('n62', 220, -412.999743, 0, datetime.date(1977, 7, 7), b'dtdD4GdE0e', None, datetime.datetime(1926, 11, 21, 8, 32, 31)), 10: ('nE2NjiT', -42, -683.684491, 0, datetime.date(2018, 9, 25), b'Poh', None, datetime.datetime(1932, 1, 3, 20, 27, 53)), 11: ('qJ3zn9Ffcg', 83, -993.509368, 1, datetime.date(1993, 12, 7), b'pKM_JF5mSpy', None, datetime.datetime(1935, 1, 1, 10, 49, 8))}
     output_dict = SQLDataModel.from_dict(input_dict).to_dict()
     for key in input_dict.keys():
         assert input_dict[key] == output_dict[key]
 
 @pytest.mark.core
```

### Comparing `sqldatamodel-0.5.1/tests/test_SQLDataModel.py` & `sqldatamodel-0.5.2/tests/test_SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,14 +446,31 @@
     inferred_output = sdm.data(include_headers=True)
     inferred_output, headers_output = inferred_output[1:], inferred_output[0]
     assert headers_input == headers_output
     for i in range(len(typed_input)):
         assert typed_input[i] == inferred_output[i]
 
 @pytest.mark.core
+def test_from_shape(sample_data):
+    input_data, input_headers = sample_data[1:], sample_data[0]
+    row_lower, row_upper = 1, len(input_data)
+    col_lower, col_upper = 1, len(input_headers)
+    rand_row = random.randint(row_lower, row_upper)
+    rand_col = random.randint(col_lower, col_upper)
+    input_shape = (rand_row, rand_col)
+    sdm = SQLDataModel.from_shape(shape=input_shape, fill=None, dtype=None)
+    output_shape = sdm.shape
+    assert output_shape == input_shape
+    test_fills = (b'bytes', None, 'strings', 12, 3.14, datetime.date(1999,12,31), datetime.datetime(1999, 12, 31, 23, 59, 59), True)
+    for input_fill in test_fills:
+        expected_output = [tuple([input_fill for _ in range(rand_col)]) for _ in range(rand_row)]
+        output_data = SQLDataModel.from_shape(shape=input_shape, fill=input_fill, display_float_precision=2).data(strict_2d=True)
+        assert output_data == expected_output
+
+@pytest.mark.core
 def test_to_from_dict():
     input_dict = {0: ('hTpigTHKcfoK', 285, -497.17176, 0, datetime.date(1914, 6, 27), b'zPx3Bp', None, datetime.datetime(1985, 11, 10, 14, 20, 59)), 1: ('mNHnKXaXQv', -673, 106.451792, 1, datetime.date(2003, 5, 8), b'vKo', None, datetime.datetime(1996, 2, 1, 14, 39, 36)), 2: ('nVgx', 622, 884.861723, 1, datetime.date(1907, 4, 19), b'aRdeb', None, datetime.datetime(1912, 2, 18, 6, 32, 16)), 3: ('0LXSG8x', 393, 360.566821, 0, datetime.date(2021, 2, 3), b'eoPni5I', None, datetime.datetime(1916, 6, 3, 7, 23, 18)), 4: ('sM2wmeOV90', -136, -770.896514, 1, datetime.date(1993, 8, 27), b'pCzfOwz1d', None, datetime.datetime(1920, 8, 27, 17, 45, 19)), 5: ('xBZ', 221, 769.5769, 1, datetime.date(1908, 9, 25), b'9gzv1plB_rp5', None, datetime.datetime(1978, 11, 17, 0, 42, 52)), 6: ('xnq6', -870, 501.755599, 0, datetime.date(1916, 3, 22), b'X0gOHafUo', None, datetime.datetime(1970, 5, 22, 3, 56, 8)), 7: ('eNGpCr5QnuVd', -212, 537.197465, 1, datetime.date(1960, 9, 6), b'Dnzdx9qW', None, datetime.datetime(1933, 2, 4, 23, 35, 9)), 8: ('Xz', -219, -319.649054, 1, datetime.date(1933, 9, 28), b'rQTWODlnd', None, datetime.datetime(1934, 5, 20, 6, 45, 21)), 9: ('n62', 220, -412.999743, 0, datetime.date(1977, 7, 7), b'dtdD4GdE0e', None, datetime.datetime(1926, 11, 21, 8, 32, 31)), 10: ('nE2NjiT', -42, -683.684491, 0, datetime.date(2018, 9, 25), b'Poh', None, datetime.datetime(1932, 1, 3, 20, 27, 53)), 11: ('qJ3zn9Ffcg', 83, -993.509368, 1, datetime.date(1993, 12, 7), b'pKM_JF5mSpy', None, datetime.datetime(1935, 1, 1, 10, 49, 8))}
     output_dict = SQLDataModel.from_dict(input_dict).to_dict()
     for key in input_dict.keys():
         assert input_dict[key] == output_dict[key]
 
 @pytest.mark.core
```

