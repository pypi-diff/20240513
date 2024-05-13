# Comparing `tmp/airflow-metaplane-0.0.3.tar.gz` & `tmp/airflow_metaplane-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-metaplane-0.0.3.tar", last modified: Tue Feb 20 21:32:24 2024, max compression
+gzip compressed data, was "airflow_metaplane-0.0.4.tar", last modified: Mon May 13 20:30:55 2024, max compression
```

## Comparing `airflow-metaplane-0.0.3.tar` & `airflow_metaplane-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-02-20 21:32:24.043160 airflow-metaplane-0.0.3/
--rw-r--r--   0 jenhuang   (501) staff       (20)    11357 2024-01-16 17:52:37.000000 airflow-metaplane-0.0.3/LICENSE
--rw-r--r--   0 jenhuang   (501) staff       (20)    13874 2024-02-20 21:32:24.042816 airflow-metaplane-0.0.3/PKG-INFO
--rw-r--r--   0 jenhuang   (501) staff       (20)      109 2024-01-24 20:03:28.000000 airflow-metaplane-0.0.3/README.md
-drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-02-20 21:32:24.040384 airflow-metaplane-0.0.3/airflow_metaplane/
--rw-r--r--   0 jenhuang   (501) staff       (20)      799 2024-01-24 20:03:28.000000 airflow-metaplane-0.0.3/airflow_metaplane/get_provider_info.py
-drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-02-20 21:32:24.041673 airflow-metaplane-0.0.3/airflow_metaplane/hooks/
--rw-r--r--   0 jenhuang   (501) staff       (20)        0 2024-01-24 20:03:28.000000 airflow-metaplane-0.0.3/airflow_metaplane/hooks/__init__.py
--rw-r--r--   0 jenhuang   (501) staff       (20)     6495 2024-02-20 18:39:15.000000 airflow-metaplane-0.0.3/airflow_metaplane/hooks/metaplane_hook.py
--rw-r--r--   0 jenhuang   (501) staff       (20)     1546 2024-02-20 18:39:15.000000 airflow-metaplane-0.0.3/airflow_metaplane/hooks/models.py
--rw-r--r--   0 jenhuang   (501) staff       (20)     2390 2024-01-24 20:03:28.000000 airflow-metaplane-0.0.3/airflow_metaplane/mp_callbacks.py
-drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-02-20 21:32:24.042034 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/
--rw-r--r--   0 jenhuang   (501) staff       (20)    13874 2024-02-20 21:32:24.000000 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/PKG-INFO
--rw-r--r--   0 jenhuang   (501) staff       (20)      465 2024-02-20 21:32:24.000000 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/SOURCES.txt
--rw-r--r--   0 jenhuang   (501) staff       (20)        1 2024-02-20 21:32:24.000000 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/dependency_links.txt
--rw-r--r--   0 jenhuang   (501) staff       (20)       96 2024-02-20 21:32:24.000000 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/entry_points.txt
--rw-r--r--   0 jenhuang   (501) staff       (20)      150 2024-02-20 21:32:24.000000 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/requires.txt
--rw-r--r--   0 jenhuang   (501) staff       (20)       18 2024-02-20 21:32:24.000000 airflow-metaplane-0.0.3/airflow_metaplane.egg-info/top_level.txt
--rw-r--r--   0 jenhuang   (501) staff       (20)      912 2024-02-20 21:31:58.000000 airflow-metaplane-0.0.3/pyproject.toml
--rw-r--r--   0 jenhuang   (501) staff       (20)       38 2024-02-20 21:32:24.043237 airflow-metaplane-0.0.3/setup.cfg
+drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-05-13 20:30:55.151435 airflow_metaplane-0.0.4/
+-rw-r--r--   0 jenhuang   (501) staff       (20)    11357 2024-01-16 17:52:37.000000 airflow_metaplane-0.0.4/LICENSE
+-rw-r--r--   0 jenhuang   (501) staff       (20)    13874 2024-05-13 20:30:55.151108 airflow_metaplane-0.0.4/PKG-INFO
+-rw-r--r--   0 jenhuang   (501) staff       (20)      109 2024-01-24 20:03:28.000000 airflow_metaplane-0.0.4/README.md
+drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-05-13 20:30:55.148819 airflow_metaplane-0.0.4/airflow_metaplane/
+-rw-r--r--   0 jenhuang   (501) staff       (20)      799 2024-01-24 20:03:28.000000 airflow_metaplane-0.0.4/airflow_metaplane/get_provider_info.py
+drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-05-13 20:30:55.150234 airflow_metaplane-0.0.4/airflow_metaplane/hooks/
+-rw-r--r--   0 jenhuang   (501) staff       (20)        0 2024-01-24 20:03:28.000000 airflow_metaplane-0.0.4/airflow_metaplane/hooks/__init__.py
+-rw-r--r--   0 jenhuang   (501) staff       (20)     6364 2024-05-13 20:17:11.000000 airflow_metaplane-0.0.4/airflow_metaplane/hooks/metaplane_hook.py
+-rw-r--r--   0 jenhuang   (501) staff       (20)     1502 2024-05-13 20:17:06.000000 airflow_metaplane-0.0.4/airflow_metaplane/hooks/models.py
+-rw-r--r--   0 jenhuang   (501) staff       (20)     2390 2024-01-24 20:03:28.000000 airflow_metaplane-0.0.4/airflow_metaplane/mp_callbacks.py
+drwxr-xr-x   0 jenhuang   (501) staff       (20)        0 2024-05-13 20:30:55.150416 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/
+-rw-r--r--   0 jenhuang   (501) staff       (20)    13874 2024-05-13 20:30:55.000000 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/PKG-INFO
+-rw-r--r--   0 jenhuang   (501) staff       (20)      465 2024-05-13 20:30:55.000000 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/SOURCES.txt
+-rw-r--r--   0 jenhuang   (501) staff       (20)        1 2024-05-13 20:30:55.000000 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/dependency_links.txt
+-rw-r--r--   0 jenhuang   (501) staff       (20)       96 2024-05-13 20:30:55.000000 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/entry_points.txt
+-rw-r--r--   0 jenhuang   (501) staff       (20)      150 2024-05-13 20:30:55.000000 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/requires.txt
+-rw-r--r--   0 jenhuang   (501) staff       (20)       18 2024-05-13 20:30:55.000000 airflow_metaplane-0.0.4/airflow_metaplane.egg-info/top_level.txt
+-rw-r--r--   0 jenhuang   (501) staff       (20)      912 2024-05-13 20:30:31.000000 airflow_metaplane-0.0.4/pyproject.toml
+-rw-r--r--   0 jenhuang   (501) staff       (20)       38 2024-05-13 20:30:55.151503 airflow_metaplane-0.0.4/setup.cfg
```

### Comparing `airflow-metaplane-0.0.3/LICENSE` & `airflow_metaplane-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-metaplane-0.0.3/PKG-INFO` & `airflow_metaplane-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metaplane
-Version: 0.0.3
+Version: 0.0.4
 Summary: Metaplane Airflow Provider
 Author-email: Metaplane <engineering@metaplane.dev>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `airflow-metaplane-0.0.3/airflow_metaplane/get_provider_info.py` & `airflow_metaplane-0.0.4/airflow_metaplane/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `airflow-metaplane-0.0.3/airflow_metaplane/hooks/metaplane_hook.py` & `airflow_metaplane-0.0.4/airflow_metaplane/hooks/metaplane_hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,17 +53,14 @@
         return MPTaskInstance(
             task_id=ti.task_id,
             dag_id=ti.dag_id,
             run_id=ti.run_id,
             start_date=ti.start_date,
             end_date=ti.end_date,
             execution_date=ti.execution_date,
-            next_retry_datetime=ti.next_retry_datetime()
-            if hasattr(ti, "task") and ti.end_date
-            else None,
             duration=ti.duration,
             state=ti.state,
             try_number=ti.try_number,
             max_tries=ti.max_tries,
             job_id=ti.job_id,
             operator=ti.operator,
             queued_dttm=ti.queued_dttm,
```

### Comparing `airflow-metaplane-0.0.3/airflow_metaplane/hooks/models.py` & `airflow_metaplane-0.0.4/airflow_metaplane/hooks/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 class MPTaskInstance:
     task_id: str
     dag_id: str
     run_id: str
     start_date: Optional[datetime]
     end_date: Optional[datetime]
     execution_date: Optional[datetime]
-    next_retry_datetime: Optional[datetime]
     duration: Optional[float]
     state: Optional[str]
     try_number: int
     max_tries: int
     job_id: Optional[int]
     operator: str
     queued_dttm: Optional[datetime]
```

### Comparing `airflow-metaplane-0.0.3/airflow_metaplane/mp_callbacks.py` & `airflow_metaplane-0.0.4/airflow_metaplane/mp_callbacks.py`

 * *Files identical despite different names*

### Comparing `airflow-metaplane-0.0.3/airflow_metaplane.egg-info/PKG-INFO` & `airflow_metaplane-0.0.4/airflow_metaplane.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-metaplane
-Version: 0.0.3
+Version: 0.0.4
 Summary: Metaplane Airflow Provider
 Author-email: Metaplane <engineering@metaplane.dev>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `airflow-metaplane-0.0.3/pyproject.toml` & `airflow_metaplane-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airflow-metaplane"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Metaplane", email="engineering@metaplane.dev" },
 ]
 description = "Metaplane Airflow Provider"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = [ "airflow-provider", "metaplane", "airflow", "integration" ]
```

