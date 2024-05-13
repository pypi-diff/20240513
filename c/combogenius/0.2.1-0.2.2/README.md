# Comparing `tmp/combogenius-0.2.1.tar.gz` & `tmp/combogenius-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combogenius-0.2.1.tar", last modified: Sat May 11 18:12:18 2024, max compression
+gzip compressed data, was "combogenius-0.2.2.tar", last modified: Mon May 13 17:39:00 2024, max compression
```

## Comparing `combogenius-0.2.1.tar` & `combogenius-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 18:12:18.778872 combogenius-0.2.1/
--rw-rw-rw-   0        0        0     1086 2024-04-28 15:40:17.000000 combogenius-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       36 2024-04-28 15:40:17.000000 combogenius-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4368 2024-05-11 18:12:18.778872 combogenius-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3977 2024-05-11 18:09:35.000000 combogenius-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 18:12:18.778872 combogenius-0.2.1/combogenius.egg-info/
--rw-rw-rw-   0        0        0     4368 2024-05-11 18:12:18.000000 combogenius-0.2.1/combogenius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-11 18:12:18.000000 combogenius-0.2.1/combogenius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 18:12:18.000000 combogenius-0.2.1/combogenius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 18:12:18.000000 combogenius-0.2.1/combogenius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 18:12:18.778872 combogenius-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-05-11 18:12:03.000000 combogenius-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 18:12:18.778872 combogenius-0.2.1/tests/
--rw-rw-rw-   0        0        0      472 2024-05-10 17:29:35.000000 combogenius-0.2.1/tests/test_api.py
--rw-rw-rw-   0        0        0     1447 2024-05-10 17:31:41.000000 combogenius-0.2.1/tests/test_database.py
--rw-rw-rw-   0        0        0     1748 2024-05-10 17:31:40.000000 combogenius-0.2.1/tests/test_make_combos.py
+drwxrwxrwx   0        0        0        0 2024-05-13 17:39:00.253302 combogenius-0.2.2/
+-rw-rw-rw-   0        0        0     1086 2024-04-28 15:40:17.000000 combogenius-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-04-28 15:40:17.000000 combogenius-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5490 2024-05-13 17:39:00.251183 combogenius-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4710 2024-05-12 20:09:46.000000 combogenius-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 17:39:00.251183 combogenius-0.2.2/combogenius.egg-info/
+-rw-rw-rw-   0        0        0     5490 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 17:39:00.000000 combogenius-0.2.2/combogenius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 17:39:00.253302 combogenius-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2024-05-13 17:35:57.000000 combogenius-0.2.2/setup.py
```

### Comparing `combogenius-0.2.1/LICENSE` & `combogenius-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `combogenius-0.2.1/PKG-INFO` & `combogenius-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: combogenius
-Version: 0.2.1
-Summary: A package designed to efficiently generate new product combinations using check information, and deliver combo suggestions to business partners via email.
-Author: Anna Movsisyan, Lusine Aghinyan, Ararat Kazarian, Hovhannes Hovhannisyan, Eduard Petrosyan
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ComboGenius 
 ## Problem
 
 Many restaurants and food courts face challenges when it comes to expanding their corporate lunch service market through B2B websites. Despite offering great value and quality products, these businesses struggle with visibility among potential clients. The main issue lies in the lack of effective engagement strategies, making it difficult to showcase their benefits and attract new customers.
 
 ## Solution
 
@@ -40,14 +32,41 @@
 from combogenius.database.sql_interactions import SqlHandler
 from combogenius.logger.logger import CustomFormatter
 from combogenius.models.make_combos import combos
 import pandas as pd
 ```
 
 ### Create and Load Data into Database
+Before using ComboGenius, ensure your database tables follow this structure:
+```python
+class checks(Base):
+    __tablename__ = "checks"
+
+    check_number = Column(Integer, primary_key=True)
+    products = Column(String)
+
+class companies(Base):
+    __tablename__ = "companies"
+
+    company_id = Column(Integer, primary_key=True)
+    link = Column(String)
+    title = Column(String)
+    phone = Column(String)
+    address = Column(String)
+    district = Column(String)
+    email = Column(String)
+    clicked = Column(Integer, default=0)
+
+class price_list(Base):
+    __tablename__ = "price_list"
+
+    product_id = Column(Integer, primary_key=True)
+    product = Column(String)
+    price = Column(Integer)
+```
 Instantiate SqlHandler objects for each database table ('checks', 'companies', 'price_list'), and load the respective data into the database.
 ```python
 Inst  = SqlHandler('database', 'checks')
 Inst1 = SqlHandler('database', 'companies')
 Inst2 = SqlHandler('database', 'price_list')
 
 data = pd.read_csv('sample_data/data.csv')
@@ -72,8 +91,8 @@
 ### Visualize Combos
 Utilize the visualization methods provided by the combos class to visualize the generated combos. You can visualize the most frequent combos, expensive combos, and cheap combos.
 ```python 
 m.visualize_most_frequent_combos()
 m.visualize_expensive_combos()
 m.visualize_cheap_combos()
 ```
-This guideline provides a basic framework for using the ComboGenius package, covering data loading, combo generation, and visualization of the results. Make sure to adjust paths and database configurations according to your specific setup.
+This guideline provides a basic framework for using the ComboGenius package, covering data loading, combo generation, and visualization of the results. Make sure to adjust paths and database configurations according to your specific setup.
```

### Comparing `combogenius-0.2.1/README.md` & `combogenius-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: combogenius
+Version: 0.2.2
+Summary: A package designed to efficiently generate new product combinations using check information, and deliver combo suggestions to business partners via email.
+Author: Anna Movsisyan, Lusine Aghinyan, Ararat Kazarian, Hovhannes Hovhannisyan, Eduard Petrosyan
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ComboGenius 
 ## Problem
 
 Many restaurants and food courts face challenges when it comes to expanding their corporate lunch service market through B2B websites. Despite offering great value and quality products, these businesses struggle with visibility among potential clients. The main issue lies in the lack of effective engagement strategies, making it difficult to showcase their benefits and attract new customers.
 
 ## Solution
 
@@ -32,14 +48,41 @@
 from combogenius.database.sql_interactions import SqlHandler
 from combogenius.logger.logger import CustomFormatter
 from combogenius.models.make_combos import combos
 import pandas as pd
 ```
 
 ### Create and Load Data into Database
+Before using ComboGenius, ensure your database tables follow this structure:
+```python
+class checks(Base):
+    __tablename__ = "checks"
+
+    check_number = Column(Integer, primary_key=True)
+    products = Column(String)
+
+class companies(Base):
+    __tablename__ = "companies"
+
+    company_id = Column(Integer, primary_key=True)
+    link = Column(String)
+    title = Column(String)
+    phone = Column(String)
+    address = Column(String)
+    district = Column(String)
+    email = Column(String)
+    clicked = Column(Integer, default=0)
+
+class price_list(Base):
+    __tablename__ = "price_list"
+
+    product_id = Column(Integer, primary_key=True)
+    product = Column(String)
+    price = Column(Integer)
+```
 Instantiate SqlHandler objects for each database table ('checks', 'companies', 'price_list'), and load the respective data into the database.
 ```python
 Inst  = SqlHandler('database', 'checks')
 Inst1 = SqlHandler('database', 'companies')
 Inst2 = SqlHandler('database', 'price_list')
 
 data = pd.read_csv('sample_data/data.csv')
@@ -64,8 +107,8 @@
 ### Visualize Combos
 Utilize the visualization methods provided by the combos class to visualize the generated combos. You can visualize the most frequent combos, expensive combos, and cheap combos.
 ```python 
 m.visualize_most_frequent_combos()
 m.visualize_expensive_combos()
 m.visualize_cheap_combos()
 ```
-This guideline provides a basic framework for using the ComboGenius package, covering data loading, combo generation, and visualization of the results. Make sure to adjust paths and database configurations according to your specific setup.
+This guideline provides a basic framework for using the ComboGenius package, covering data loading, combo generation, and visualization of the results. Make sure to adjust paths and database configurations according to your specific setup.
```

### Comparing `combogenius-0.2.1/combogenius.egg-info/PKG-INFO` & `combogenius-0.2.2/combogenius.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Metadata-Version: 2.1
 Name: combogenius
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package designed to efficiently generate new product combinations using check information, and deliver combo suggestions to business partners via email.
 Author: Anna Movsisyan, Lusine Aghinyan, Ararat Kazarian, Hovhannes Hovhannisyan, Eduard Petrosyan
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ComboGenius 
 ## Problem
 
 Many restaurants and food courts face challenges when it comes to expanding their corporate lunch service market through B2B websites. Despite offering great value and quality products, these businesses struggle with visibility among potential clients. The main issue lies in the lack of effective engagement strategies, making it difficult to showcase their benefits and attract new customers.
@@ -40,14 +48,41 @@
 from combogenius.database.sql_interactions import SqlHandler
 from combogenius.logger.logger import CustomFormatter
 from combogenius.models.make_combos import combos
 import pandas as pd
 ```
 
 ### Create and Load Data into Database
+Before using ComboGenius, ensure your database tables follow this structure:
+```python
+class checks(Base):
+    __tablename__ = "checks"
+
+    check_number = Column(Integer, primary_key=True)
+    products = Column(String)
+
+class companies(Base):
+    __tablename__ = "companies"
+
+    company_id = Column(Integer, primary_key=True)
+    link = Column(String)
+    title = Column(String)
+    phone = Column(String)
+    address = Column(String)
+    district = Column(String)
+    email = Column(String)
+    clicked = Column(Integer, default=0)
+
+class price_list(Base):
+    __tablename__ = "price_list"
+
+    product_id = Column(Integer, primary_key=True)
+    product = Column(String)
+    price = Column(Integer)
+```
 Instantiate SqlHandler objects for each database table ('checks', 'companies', 'price_list'), and load the respective data into the database.
 ```python
 Inst  = SqlHandler('database', 'checks')
 Inst1 = SqlHandler('database', 'companies')
 Inst2 = SqlHandler('database', 'price_list')
 
 data = pd.read_csv('sample_data/data.csv')
```

