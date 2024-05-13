# Comparing `tmp/pyaqueduct-0.0.7.tar.gz` & `tmp/pyaqueduct-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaqueduct-0.0.7.tar", max compression
+gzip compressed data, was "pyaqueduct-0.0.8.tar", max compression
```

## Comparing `pyaqueduct-0.0.7.tar` & `pyaqueduct-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-04-29 12:31:10.214111 pyaqueduct-0.0.7/LICENSE
--rw-r--r--   0        0        0     2331 2024-04-29 12:31:10.214111 pyaqueduct-0.0.7/README.md
--rw-r--r--   0        0        0      145 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/__init__.py
--rw-r--r--   0        0        0     3312 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/api.py
--rw-r--r--   0        0        0      292 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/client/__init__.py
--rw-r--r--   0        0        0    16160 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/client/client.py
--rw-r--r--   0        0        0     2176 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/client/types.py
--rw-r--r--   0        0        0      591 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/exceptions.py
--rw-r--r--   0        0        0     3493 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/experiment.py
--rw-r--r--   0        0        0        0 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/schemas/__init__.py
--rw-r--r--   0        0        0     2463 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/schemas/mutations.py
--rw-r--r--   0        0        0     1696 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/schemas/queries.py
--rw-r--r--   0        0        0      237 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyaqueduct/settings.py
--rw-r--r--   0        0        0     1144 2024-04-29 12:31:10.218111 pyaqueduct-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3397 1970-01-01 00:00:00.000000 pyaqueduct-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2331 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/README.md
+-rw-r--r--   0        0        0      145 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/__init__.py
+-rw-r--r--   0        0        0     4495 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/api.py
+-rw-r--r--   0        0        0      292 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/client/__init__.py
+-rw-r--r--   0        0        0    16755 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/client/client.py
+-rw-r--r--   0        0        0     2176 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/client/types.py
+-rw-r--r--   0        0        0      591 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/exceptions.py
+-rw-r--r--   0        0        0     3622 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/experiment.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/schemas/__init__.py
+-rw-r--r--   0        0        0     2682 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/schemas/mutations.py
+-rw-r--r--   0        0        0     1767 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/schemas/queries.py
+-rw-r--r--   0        0        0      237 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyaqueduct/settings.py
+-rw-r--r--   0        0        0     1144 2024-05-13 12:59:47.236085 pyaqueduct-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3397 1970-01-01 00:00:00.000000 pyaqueduct-0.0.8/PKG-INFO
```

### Comparing `pyaqueduct-0.0.7/LICENSE` & `pyaqueduct-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.7/README.md` & `pyaqueduct-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.7/pyaqueduct/client/client.py` & `pyaqueduct-0.0.8/pyaqueduct/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Aqueduct client class to enable experiment based operations."""
 
 import logging
 import os
-from datetime import date
+from datetime import datetime
 from typing import Dict, List, Optional
 from uuid import UUID
 
 from gql import Client
 from gql.client import SyncClientSession
 from gql.transport import exceptions as gql_exceptions
 from gql.transport.httpx import HTTPXTransport
@@ -21,14 +21,15 @@
     ForbiddenError,
     RemoteOperationError,
     UnAuthorizedError,
 )
 from pyaqueduct.schemas.mutations import (
     add_tag_to_experiment_mutation,
     create_experiment_mutation,
+    remove_experiment_mutation,
     remove_tag_from_experiment_mutation,
     update_experiment_mutation,
 )
 from pyaqueduct.schemas.queries import (
     get_all_tags_query,
     get_experiment_query,
     get_experiments_query,
@@ -80,23 +81,23 @@
             )
         )
 
     def create_experiment(
         self, title: str, description: str, tags: Optional[List[str]] = None
     ) -> ExperimentData:
         """
-        Create an experiment with title, description and list of tags
+        Create an experiment with title, description and list of tags.
 
         Args:
-        - title (str): Title of experiment
-        - description (str): Description of experiment
-        - tags (List[str]): List of tags to be assigned to experiment
+            title: Title of experiment.
+            description: Description of experiment.
+            tags: List of tags to be assigned to experiment.
 
         Returns:
-        Experiment: Experiment objects having all fields
+            Experiment object.
         """
         try:
             experiment = self._gql_client.execute(
                 create_experiment_mutation,
                 variable_values={"title": title, "description": description, "tags": tags or []},
             )
         except gql_exceptions.TransportServerError as error:
@@ -114,23 +115,24 @@
         logging.info("Created experiment - %s - %s", experiment_obj.id, experiment_obj.title)
         return experiment_obj
 
     def update_experiment(
         self, experiment_uuid: UUID, title: Optional[str] = None, description: Optional[str] = None
     ) -> ExperimentData:
         """
-        Update title or description or both for experiment
+        Update title or description or both for experiment.
 
         Args:
-        - experiment_uuid (UUID): UUID of experiment to be updated
-        - title (str): New title of experiment
-        - description (str): New description of experiment
+            experiment_uuid: UUID of experiment.
+            title: New title of experiment.
+            description: New description of experiment.
 
         Returns:
-        Experiment: Experiment object with updated fields
+            Experiment object.
+
         """
         if title and title == "":
             raise ValueError("Title cannot be an empty string")
 
         if description and description == "":
             raise ValueError("Description cannot be an empty string")
 
@@ -160,44 +162,45 @@
 
     def get_experiments(
         self,
         limit: int,
         offset: int,
         title: Optional[str] = None,
         tags: Optional[List[str]] = None,
-        start_date: Optional[date] = None,
-        end_date: Optional[date] = None,
+        start_datetime: Optional[datetime] = None,
+        end_datetime: Optional[datetime] = None,
     ) -> ExperimentsInfo:
         """
         Get a list of experiments
 
         Args:
-        - limit (int): Number of experiments to be fetched
-        - offset (offset): Number of experiments to skip
-        - title (str): Perform search on experiments through title
-        - tags (List[str]): Get experiments having these tags
-        - start_date (date): Start date to filter experiments
-        - end_date (date): End date to filter experiments to
+            limit: Pagination field, number of experiments to be fetched.
+            offset: Pagination field, number of experiments to skip.
+            title: Perform search on experiments through their title and alias.
+            tags: Get experiments that have these tags.
+            start_date: Start datetime to filter experiments (timezone aware).
+            end_date: End datetime to filter experiments to (timezone aware).
 
         Returns:
-        List[Experiment]: A list of experiments with filters applied
+            List of experiments with filters applied.
+
         """
         if limit <= 0:
             raise ValueError("Limit should be a positive number")
 
         try:
             experiments = self._gql_client.execute(
                 get_experiments_query,
                 variable_values={
                     "limit": limit,
                     "offset": offset,
                     "title": title,
-                    "start_date": start_date,
-                    "end_date": end_date,
-                    "tags": tags or [],
+                    "startDate": start_datetime.isoformat() if start_datetime else None,
+                    "endDate": end_datetime.isoformat() if end_datetime else None,
+                    "tags": tags,
                 },
             )
         except gql_exceptions.TransportServerError as error:
             if error.code:
                 process_response_common(codes(error.code))
             raise
         except gql_exceptions.TransportQueryError as error:
@@ -213,22 +216,22 @@
             len(experiments_obj.experiments),
             experiments_obj.total_count,
         )
         return experiments_obj
 
     def get_experiment(self, experiment_uuid: UUID) -> ExperimentData:
         """
-        Get an Experiment by ID or Alias
+        Get an Experiment by UUID.
 
         Args:
-        - id_ (str): "UUID | ALIAS" Unique identifier to be used
-        - value (str): Value of unique identifier to use for fetching experiment
+            experiment_uuid: UUID of experiment.
 
         Returns:
-        Experiment: Experiment object having all fields
+            Experiment object.
+
         """
         try:
             experiment = self._gql_client.execute(
                 get_experiment_query,
                 variable_values={"type": "UUID", "value": str(experiment_uuid)},
             )
         except gql_exceptions.TransportServerError as error:
@@ -244,22 +247,22 @@
             experiment["experiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Fetched experiment - %s", experiment_obj.title)
         return experiment_obj
 
     def get_experiment_by_alias(self, alias: str) -> ExperimentData:
         """
-        Get an Experiment by ID or Alias
+        Get an Experiment by Alias.
 
         Args:
-        - id_ (str): "UUID | ALIAS" Unique identifier to be used
-        - value (str): Value of unique identifier to use for fetching experiment
+            alias: Experiment's alias.
 
         Returns:
-        Experiment: Experiment object having all fields
+            Updated experiment.
+
         """
         try:
             experiment = self._gql_client.execute(
                 get_experiment_query, variable_values={"type": "ALIAS", "value": alias}
             )
         except gql_exceptions.TransportServerError as error:
             if error.code:
@@ -277,19 +280,20 @@
         return experiment_obj
 
     def add_tag_to_experiment(self, experiment_uuid: UUID, tag: str) -> ExperimentData:
         """
         Add a tag to an experiment
 
         Args:
-        - experiment_uuid (UUID): UUID of experiment to which tag is to be added
-        - tag (str): Tag to be added to experiment
+            experiment_uuid: UUID of experiment.
+            tag: Tag to be added to experiment.
 
         Returns:
-        Experiment: Experiment having tag added
+            Updated experiment.
+
         """
         try:
             experiment = self._gql_client.execute(
                 add_tag_to_experiment_mutation,
                 variable_values={"experimentId": str(experiment_uuid), "tag": tag},
             )
         except gql_exceptions.TransportServerError as error:
@@ -303,14 +307,36 @@
 
         experiment_obj = ExperimentData.from_dict(
             experiment["addTagToExperiment"]  # pylint: disable=unsubscriptable-object
         )
         logging.info("Added tag %s to experiment <%s>", tag, experiment_obj.title)
         return experiment_obj
 
+    def remove_experiment(self, experiment_uuid: UUID) -> None:
+        """
+        Remove experiment from the database. It removes the experiments files as well.
+
+        Args:
+            experiment_uuid: UUID of experiment.
+
+        """
+        try:
+            self._gql_client.execute(
+                remove_experiment_mutation,
+                variable_values={"experimentId": str(experiment_uuid)},
+            )
+        except gql_exceptions.TransportServerError as error:
+            if error.code:
+                process_response_common(codes(error.code))
+            raise
+        except gql_exceptions.TransportQueryError as error:
+            raise RemoteOperationError(
+                error.errors if error.errors else "Unknown error occurred in the remote operation."
+            ) from error
+
     def remove_tag_from_experiment(self, experiment_uuid: UUID, tag: str) -> ExperimentData:
         """
         Remove a tag from an experiment
 
         Args:
         - experiment_uuid (UUID): UUID of experiment frin which tag has to be removed
         - tag (str): Tag to be removed from experiment
```

### Comparing `pyaqueduct-0.0.7/pyaqueduct/client/types.py` & `pyaqueduct-0.0.8/pyaqueduct/client/types.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.7/pyaqueduct/exceptions.py` & `pyaqueduct-0.0.8/pyaqueduct/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyaqueduct-0.0.7/pyaqueduct/experiment.py` & `pyaqueduct-0.0.8/pyaqueduct/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from datetime import datetime
 from re import compile as recompile
 from typing import List, Tuple
 from uuid import UUID
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, validate_call
 
 from pyaqueduct.client import AqueductClient
 
 _MAX_TITLE_LENGTH = 100
 _MAX_DESCRIPTION_LENGTH = 2000
 _MAX_TAG_LENGTH = 50
 
@@ -43,14 +43,15 @@
 
     @property
     def title(self) -> str:
         """Get title of experiment."""
         return self._client.get_experiment(experiment_uuid=self.id).title
 
     @title.setter
+    @validate_call
     def title(self, value: str = Field(..., max_length=_MAX_TITLE_LENGTH)) -> None:
         """Set title of experiment.
 
         Args:
             value: New title.
 
         """
@@ -58,52 +59,57 @@
 
     @property
     def description(self) -> str:
         """Get description of experiment."""
         return self._client.get_experiment(self.id).description
 
     @description.setter
+    @validate_call
     def description(self, value: str = Field(..., max_length=_MAX_DESCRIPTION_LENGTH)) -> None:
         """Set description of experiment.
 
         Args:
             value: New description.
 
         """
         self._client.update_experiment(experiment_uuid=self.id, description=value)
 
     @property
     def tags(self) -> List[str]:
         """Gets tags of experiment."""
         return self._client.get_experiment(self.id).tags
 
+    @validate_call
     def add_tag(self, tag: str = Field(..., max_length=_MAX_TAG_LENGTH)) -> None:
         """Add new tag to experiment."""
         if not is_valid_tag(tag):
             raise ValueError(
                 f"Tag {tag} should only contain alphanumeric characters, underscores or hyphens"
             )
 
         self._client.add_tag_to_experiment(experiment_uuid=self.id, tag=tag)
 
+    @validate_call
     def remove_tag(self, tag: str = Field(..., max_length=_MAX_TAG_LENGTH)) -> None:
         """Remove tag from experiment."""
         self._client.remove_tag_from_experiment(experiment_uuid=self.id, tag=tag)
 
     @property
     def files(self) -> List[Tuple[str, datetime]]:
         """Get file names of expriment."""
         return [
             (item.name, item.modified_at) for item in self._client.get_experiment(self.id).files
         ]
 
+    @validate_call
     def download_file(self, file_name: str, destination_dir: str) -> None:
         """Download the specified file of experiment."""
         self._client.download_file(self.id, file_name=file_name, destination_dir=destination_dir)
 
+    @validate_call
     def upload_file(self, file: str) -> None:
         """Upload the specified file to experiment."""
         self._client.upload_file(self.id, file=file)
 
     @property
     def updated_at(self) -> datetime:
         """Get last updated datetime of the experiment."""
```

### Comparing `pyaqueduct-0.0.7/pyaqueduct/schemas/mutations.py` & `pyaqueduct-0.0.8/pyaqueduct/schemas/mutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Aqueduct GraphQL Mutation schemas"""
+
 from gql import gql
 
 create_experiment_mutation = gql(
     """
     mutation CreateExperiment (
         $title: String!,
         $description: String!,
@@ -116,7 +117,17 @@
                 path
                 modifiedAt
             }
         }
     }
     """
 )
+
+remove_experiment_mutation = gql(
+    """
+    mutation RemoveTagFromExperiment (
+        $experimentId: UUID!
+        ) {
+        removeExperiment(experimentRemoveInput: {experimentId: $experimentId})
+    }
+    """
+)
```

### Comparing `pyaqueduct-0.0.7/pyaqueduct/schemas/queries.py` & `pyaqueduct-0.0.8/pyaqueduct/schemas/queries.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Aqueduct GraphQL Query schemas"""
+
 from gql import gql
 
 get_experiments_query = gql(
     """
     query GetExperiments (
         $limit: Int!,
         $offset: Int!,
-        $title: String = "",
-        $startDate: Date = null,
-        $endDate: Date = null,
+        $title: String = null,
+        $startDate: DateTime = null,
+        $endDate: DateTime = null,
+        $tags: [String!] = null
     ) {
         experiments (
             filters: {
                 title: $title,
                 startDate: $startDate,
                 endDate: $endDate,
+                tags: $tags
             }
             limit: $limit,
             offset: $offset,
         ) {
             experimentsData {
                 id
                 title
```

### Comparing `pyaqueduct-0.0.7/pyproject.toml` & `pyaqueduct-0.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyaqueduct"
-version = "0.0.7"
+version = "0.0.8"
 description = "Aqueduct Python Client Library"
 authors = ["Aqueduct Team <aqueduct@riverlane.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://aqueducthub.github.io/pyaqueduct"
 documentation = "https://aqueducthub.github.io/pyaqueduct"
 repository = "https://github.com/AqueductHub/pyaqueduct"
```

### Comparing `pyaqueduct-0.0.7/PKG-INFO` & `pyaqueduct-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaqueduct
-Version: 0.0.7
+Version: 0.0.8
 Summary: Aqueduct Python Client Library
 Home-page: https://aqueducthub.github.io/pyaqueduct
 License: MIT
 Author: Aqueduct Team
 Author-email: aqueduct@riverlane.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

