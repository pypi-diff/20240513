# Comparing `tmp/annonition-0.0.3.tar.gz` & `tmp/annonition-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.0.3.tar", last modified: Sun May 12 22:41:56 2024, max compression
+gzip compressed data, was "annonition-0.0.4.tar", last modified: Sun May 12 23:12:02 2024, max compression
```

## Comparing `annonition-0.0.3.tar` & `annonition-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 22:41:54.410000 annonition-0.0.3/
--rw-rw-rw-   0        0        0      452 2024-05-12 22:41:58.000000 annonition-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 22:41:54.820000 annonition-0.0.3/annonition/
--rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.3/annonition/__init__.py
--rw-rw-rw-   0        0        0     2524 2024-05-12 22:39:52.000000 annonition-0.0.3/annonition/logger.py
--rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.3/annonition/main.py
-drwxrwxrwx   0        0        0        0 2024-05-12 22:41:55.270000 annonition-0.0.3/annonition.egg-info/
--rw-rw-rw-   0        0        0      452 2024-05-12 22:41:54.000000 annonition-0.0.3/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 22:41:58.000000 annonition-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      843 2024-05-12 22:41:44.000000 annonition-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:12:00.490000 annonition-0.0.4/
+-rw-rw-rw-   0        0        0      452 2024-05-12 23:12:04.000000 annonition-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 23:12:00.830000 annonition-0.0.4/annonition/
+-rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.4/annonition/__init__.py
+-rw-rw-rw-   0        0        0     3222 2024-05-12 23:10:30.000000 annonition-0.0.4/annonition/logger.py
+-rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.4/annonition/main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 23:12:01.180000 annonition-0.0.4/annonition.egg-info/
+-rw-rw-rw-   0        0        0      452 2024-05-12 23:12:02.000000 annonition-0.0.4/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-12 23:12:02.000000 annonition-0.0.4/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 23:12:02.000000 annonition-0.0.4/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-12 23:12:02.000000 annonition-0.0.4/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 23:12:02.000000 annonition-0.0.4/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 23:12:04.000000 annonition-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-12 23:11:36.000000 annonition-0.0.4/setup.py
```

### Comparing `annonition-0.0.3/annonition/logger.py` & `annonition-0.0.4/annonition/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,26 +38,41 @@
     """
     A factory for creating pre-configured logger instances with enhanced capabilities such as verbose logging levels and colored output, ignoring specified endpoints.
     
     Example:
         # Create a logger instance ignoring logs containing "/health" and "Press CTRL+C to quit"
         logger = CustomLogger(ignore=["/health", "Press CTRL+C to quit"])
     """
-    def __new__(cls, name='werkzeug', ignore=None):
+    def __new__(cls, level="INFO", name='werkzeug', ignore=None, include_date=True, include_level=True):
         """
         Creates and returns a new logger instance with specified configurations.
 
         Parameters:
             name (str): The name of the logger. Default is 'werkzeug'.
             ignore (list of str, optional): A list of message substrings to ignore in the logs.
+            include_date (bool, optional): Whether to include the date in the log messages. Default is True.
+            include_level (bool, optional): Whether to include the log level in the log messages. Default is True.
 
         Returns:
             logging.Logger: A configured logger instance with colored logs and endpoint filtering.
         """
         if ignore is None:
             ignore = []
         verboselogs.install()
+
         logger = logging.getLogger(name)
+        logger.addHandler(logging.StreamHandler())
+        logger.setLevel(level.upper())
         logger.addFilter(EndpointFilter(ignore))
-        coloredlogs.install(logger=logger, isatty=True)
+
+        format_elements = []
+        if include_date:
+            format_elements.append('%(asctime)s')
+        if include_level:
+            format_elements.append('%(levelname)s')
+        format_elements.append('%(message)s')
+        log_format = ' '.join(format_elements)
+
+
+        coloredlogs.install(logger=logger, isatty=True, fmt=log_format, level=level.upper())
         return logger
```

### Comparing `annonition-0.0.3/setup.py` & `annonition-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="annonition",
-    version="0.0.3",
+    version="0.0.4",
     author="Abtin Turing",
     author_email="abtinturing@gmail.com",
     description="Beginning of a new era in annotation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/abtinturing/anno",
     packages=find_packages(),
```

