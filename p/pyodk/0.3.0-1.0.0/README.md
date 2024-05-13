# Comparing `tmp/pyodk-0.3.0.tar.gz` & `tmp/pyodk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodk-0.3.0.tar", last modified: Wed Apr  5 05:44:14 2023, max compression
+gzip compressed data, was "pyodk-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyodk-0.3.0.tar` & `pyodk-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:44:14.608410 pyodk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-04-05 05:43:46.000000 pyodk-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-05 05:44:14.608410 pyodk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-05 05:43:46.000000 pyodk-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:44:14.608410 pyodk-0.3.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 05:43:46.000000 pyodk-0.3.0/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-05 05:43:46.000000 pyodk-0.3.0/bin/clean_for_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-05 05:43:46.000000 pyodk-0.3.0/bin/pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:44:14.608410 pyodk-0.3.0/pyodk/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:44:14.608410 pyodk-0.3.0/pyodk/_endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/form_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/form_draft_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/form_drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/project_app_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_endpoints/submissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:44:14.608410 pyodk-0.3.0/pyodk/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/_utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyodk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 05:44:14.608410 pyodk-0.3.0/pyodk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-05 05:44:14.000000 pyodk-0.3.0/pyodk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-05 05:44:14.000000 pyodk-0.3.0/pyodk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 05:44:14.000000 pyodk-0.3.0/pyodk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 05:44:14.000000 pyodk-0.3.0/pyodk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-05 05:44:14.000000 pyodk-0.3.0/pyodk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-05 05:43:46.000000 pyodk-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-05 05:44:14.608410 pyodk-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-05 05:43:46.000000 pyodk-0.3.0/setup.py
+-rw-r--r--   0        0        0    10301 2024-05-13 18:46:13.493784 pyodk-1.0.0/README.md
+-rw-r--r--   0        0        0      180 2024-05-13 18:46:13.497784 pyodk-1.0.0/pyodk/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-13 18:46:13.497784 pyodk-1.0.0/pyodk/__version__.py
+-rw-r--r--   0        0        0       13 2024-05-13 18:46:13.497784 pyodk-1.0.0/pyodk/_endpoints/__init__.py
+-rw-r--r--   0        0        0     3208 2024-05-13 18:46:13.497784 pyodk-1.0.0/pyodk/_endpoints/auth.py
+-rw-r--r--   0        0        0      608 2024-05-13 18:46:13.497784 pyodk-1.0.0/pyodk/_endpoints/bases.py
+-rw-r--r--   0        0        0     3716 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/comments.py
+-rw-r--r--   0        0        0     9274 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/entities.py
+-rw-r--r--   0        0        0     1963 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/entity_lists.py
+-rw-r--r--   0        0        0     2119 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/form_assignments.py
+-rw-r--r--   0        0        0     2316 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/form_draft_attachments.py
+-rw-r--r--   0        0        0     7937 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/form_drafts.py
+-rw-r--r--   0        0        0     8292 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/forms.py
+-rw-r--r--   0        0        0     2800 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/project_app_users.py
+-rw-r--r--   0        0        0     4596 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/projects.py
+-rw-r--r--   0        0        0    15258 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_endpoints/submissions.py
+-rw-r--r--   0        0        0       13 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_utils/__init__.py
+-rw-r--r--   0        0        0     3432 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_utils/config.py
+-rw-r--r--   0        0        0     6468 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_utils/session.py
+-rw-r--r--   0        0        0       79 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_utils/utils.py
+-rw-r--r--   0        0        0     2547 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/_utils/validators.py
+-rw-r--r--   0        0        0     3937 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/client.py
+-rw-r--r--   0        0        0       65 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyodk/errors.py
+-rw-r--r--   0        0        0     3042 2024-05-13 18:46:13.501784 pyodk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11123 1970-01-01 00:00:00.000000 pyodk-1.0.0/PKG-INFO
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/auth.py` & `pyodk-1.0.0/pyodk/_endpoints/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from pyodk._utils import config
 from pyodk.errors import PyODKError
 
 if TYPE_CHECKING:
     from pyodk._utils.session import Session
 
 log = logging.getLogger(__name__)
 
 
 class AuthService:
-    def __init__(self, session: "Session", cache_path: Optional[str] = None) -> None:
+    def __init__(self, session: "Session", cache_path: str | None = None) -> None:
         self.session: "Session" = session
         self.cache_path: str = cache_path
 
     def verify_token(self, token: str) -> str:
         """
         Check with Central that a token is valid.
 
@@ -40,15 +40,15 @@
             log.error(err, exc_info=True)
             raise err
 
     def get_new_token(self, username: str, password: str) -> str:
         """
         Get a new token from Central by creating a new session.
 
-        https://odkcentral.docs.apiary.io/#reference/authentication/session-authentication/logging-in
+        https://docs.getodk.org/central-api-authentication/#logging-in
 
         :param username: The username of the Web User to auth with.
         :param password: The Web User's password.
         :return: The session token.
         """
         response = self.session.post(
             url="sessions",
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/bases.py` & `pyodk-1.0.0/pyodk/_endpoints/bases.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict
-
 from pydantic import BaseModel
 
 from pyodk._utils.session import Session
 
 
 class Model(BaseModel):
     """Base configuration for data model classes."""
@@ -13,19 +11,17 @@
         validate_assignment = True
 
 
 class Manager:
     """Base for managers of data model classes."""
 
     __slots__ = ("__weakref__",)
-    pass
 
     @classmethod
-    def from_dict(cls, session: Session, project_id: int, data: Dict) -> Model:
+    def from_dict(cls, session: Session, project_id: int, data: dict) -> Model:
         raise NotImplementedError()
 
 
 class Service:
     """Base for services interacting with the ODK Central API over HTTP."""
 
     __slots__ = ("__weakref__",)
-    pass
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/comments.py` & `pyodk-1.0.0/pyodk/_endpoints/comments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from datetime import datetime
-from typing import List, Optional
 
 from pyodk._endpoints import bases
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
@@ -32,60 +31,62 @@
         "default_form_id",
         "default_instance_id",
     )
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
-        default_form_id: Optional[str] = None,
-        default_instance_id: Optional[str] = None,
+        default_project_id: int | None = None,
+        default_form_id: str | None = None,
+        default_instance_id: str | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
-        self.default_form_id: Optional[str] = default_form_id
-        self.default_instance_id: Optional[str] = default_instance_id
+        self.default_project_id: int | None = default_project_id
+        self.default_form_id: str | None = default_form_id
+        self.default_instance_id: str | None = default_instance_id
 
     def list(
         self,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-        instance_id: Optional[str] = None,
-    ) -> List[Comment]:
+        form_id: str | None = None,
+        project_id: int | None = None,
+        instance_id: str | None = None,
+    ) -> list[Comment]:
         """
         Read all Comment details.
 
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project the Submissions belong to.
         :param instance_id: The instanceId of the Submission being referenced.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
             iid = pv.validate_instance_id(instance_id, self.default_instance_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="GET",
-            url=self.urls.list.format(project_id=pid, form_id=fid, instance_id=iid),
+            url=self.session.urlformat(
+                self.urls.list, project_id=pid, form_id=fid, instance_id=iid
+            ),
             logger=log,
         )
         data = response.json()
         return [Comment(**r) for r in data]
 
     def post(
         self,
         comment: str,
-        project_id: Optional[int] = None,
-        form_id: Optional[str] = None,
-        instance_id: Optional[str] = None,
+        project_id: int | None = None,
+        form_id: str | None = None,
+        instance_id: str | None = None,
     ) -> Comment:
         """
         Create a Comment.
 
         :param comment: The text of the comment.
         :param project_id: The id of the project this form belongs to.
         :param form_id: The xmlFormId of the Form being referenced.
@@ -97,17 +98,19 @@
             iid = pv.validate_instance_id(instance_id, self.default_instance_id)
             comment = pv.wrap_error(
                 validator=pv.v.str_validator, key="comment", value=comment
             )
             json = {"body": comment}
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="POST",
-            url=self.urls.post.format(project_id=pid, form_id=fid, instance_id=iid),
+            url=self.session.urlformat(
+                self.urls.post, project_id=pid, form_id=fid, instance_id=iid
+            ),
             logger=log,
             json=json,
         )
         data = response.json()
         return Comment(**data)
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/form_assignments.py` & `pyodk-1.0.0/pyodk/_endpoints/form_assignments.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 from pyodk._endpoints import bases
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
@@ -19,29 +18,29 @@
 
 class FormAssignmentService(bases.Service):
     __slots__ = ("urls", "session", "default_project_id", "default_form_id")
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
-        default_form_id: Optional[str] = None,
+        default_project_id: int | None = None,
+        default_form_id: str | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
-        self.default_form_id: Optional[str] = default_form_id
+        self.default_project_id: int | None = default_project_id
+        self.default_form_id: str | None = default_form_id
 
     def assign(
         self,
         role_id: int,
         user_id: int,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
     ) -> bool:
         """
         Assign a user to a role for a form.
 
         :param role_id: The id of the role to assign the user to.
         :param user_id: The id of the user to assign to the role.
         :param form_id: The xmlFormId of the Form being referenced.
@@ -50,19 +49,19 @@
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
             rid = pv.validate_int(role_id, key="role_id")
             uid = pv.validate_int(user_id, key="user_id")
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="POST",
-            url=self.urls.post.format(
-                project_id=pid, form_id=fid, role_id=rid, user_id=uid
+            url=self.session.urlformat(
+                self.urls.post, project_id=pid, form_id=fid, role_id=rid, user_id=uid
             ),
             logger=log,
         )
 
         data = response.json()
         return data["success"]
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/form_draft_attachments.py` & `pyodk-1.0.0/pyodk/_endpoints/form_draft_attachments.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
-from pathlib import Path
-from typing import Optional
+from os import PathLike
 
 from pyodk._endpoints import bases
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
@@ -20,50 +19,52 @@
 
 class FormDraftAttachmentService(bases.Service):
     __slots__ = ("urls", "session", "default_project_id", "default_form_id")
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
-        default_form_id: Optional[str] = None,
+        default_project_id: int | None = None,
+        default_form_id: str | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
-        self.default_form_id: Optional[str] = default_form_id
+        self.default_project_id: int | None = default_project_id
+        self.default_form_id: str | None = default_form_id
 
     def upload(
         self,
-        file_path: str,
-        file_name: Optional[str] = None,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
+        file_path: PathLike | str,
+        file_name: str | None = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
     ) -> bool:
         """
         Upload a Form Draft Attachment.
 
         :param file_path: The path to the file to upload.
         :param file_name: A name for the file, otherwise the name in file_path is used.
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
-            file_path = Path(pv.validate_file_path(file_path))
+            file_path = pv.validate_file_path(file_path)
             if file_name is None:
                 file_name = pv.validate_str(file_path.name, key="file_name")
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         with open(file_path, "rb") as fd:
             response = self.session.response_or_error(
                 method="POST",
-                url=self.urls.post.format(project_id=pid, form_id=fid, fname=file_name),
+                url=self.session.urlformat(
+                    self.urls.post, project_id=pid, form_id=fid, fname=file_name
+                ),
                 logger=log,
                 data=fd,
             )
         data = response.json()
         return data["success"]
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/form_drafts.py` & `pyodk-1.0.0/pyodk/_endpoints/projects.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,138 @@
 import logging
-from contextlib import nullcontext
-from pathlib import Path
-from typing import Optional
+from collections.abc import Iterable
+from datetime import datetime
+from typing import Any
 
 from pyodk._endpoints import bases
+from pyodk._endpoints.form_assignments import FormAssignmentService
+from pyodk._endpoints.project_app_users import ProjectAppUser, ProjectAppUserService
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
 
 
+class Project(bases.Model):
+    id: int
+    name: str
+    createdAt: datetime
+    description: str | None = None
+    archived: bool | None = None
+    keyId: int | None = None
+    appUsers: int | None = None
+    forms: int | None = None
+    lastSubmission: str | None = None
+    updatedAt: datetime | None = None
+    deletedAt: datetime | None = None
+
+
 class URLs(bases.Model):
     class Config:
         frozen = True
 
-    _form: str = "projects/{project_id}/forms/{form_id}"
-    post: str = f"{_form}/draft"
-    post_publish: str = f"{_form}/draft/publish"
+    list: str = "projects"
+    get: str = "projects/{project_id}"
+    get_data: str = "projects/{project_id}/forms/{form_id}.svc/{table_name}"
+    post_app_users: str = "projects/{project_id}/app-users"
+
+
+class ProjectService(bases.Service):
+    """
+    Project-related functionality is accessed through `client.projects`. For example:
 
+    ```python
+    from pyodk.client import Client
 
-class FormDraftService(bases.Service):
-    __slots__ = ("urls", "session", "default_project_id", "default_form_id")
+    client = Client()
+    projects = client.projects.list()
+    ```
+    """
+
+    __slots__ = ("urls", "session", "default_project_id")
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
-        default_form_id: Optional[str] = None,
+        default_project_id: int | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
-        self.default_form_id: Optional[str] = default_form_id
+        self.default_project_id: int | None = default_project_id
 
-    def create(
-        self,
-        file_path: Optional[str] = None,
-        ignore_warnings: Optional[bool] = True,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-    ) -> bool:
+    def _default_kw(self) -> dict[str, Any]:
+        return {
+            "default_project_id": self.default_project_id,
+        }
+
+    def list(self) -> list[Project]:
         """
-        Create a Form Draft.
+        Read Project details.
 
-        :param file_path: The path to the file to upload.
-        :param form_id: The xmlFormId of the Form being referenced.
-        :param project_id: The id of the project this form belongs to.
-        :param ignore_warnings: If True, create the form if there are XLSForm warnings.
+        :return: An list of object representations of the Projects' metadata.
+        """
+        response = self.session.response_or_error(
+            method="GET",
+            url=self.urls.list,
+            logger=log,
+        )
+        data = response.json()
+        return [Project(**r) for r in data]
+
+    def get(self, project_id: int | None = None) -> Project:
+        """
+        Read all Project details.
+
+        :param project_id: The id of the project to read.
+
+        :return: An object representation of the Project's metadata.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
-            fid = pv.validate_form_id(form_id, self.default_form_id)
-            headers = {}
-            params = {}
-            if file_path is not None:
-                if ignore_warnings is not None:
-                    key = "ignore_warnings"
-                    params["ignoreWarnings"] = pv.validate_bool(ignore_warnings, key=key)
-                file_path = Path(pv.validate_file_path(file_path))
-                if file_path.suffix == ".xlsx":
-                    content_type = (
-                        "application/vnd.openxmlformats-"
-                        "officedocument.spreadsheetml.sheet"
-                    )
-                elif file_path.suffix == ".xls":
-                    content_type = "application/vnd.ms-excel"
-                elif file_path.suffix == ".xml":
-                    content_type = "application/xml"
-                else:
-                    raise PyODKError(
-                        "Parameter 'file_path' file name has an unexpected extension, "
-                        "expected one of '.xlsx', '.xls', '.xml'."
-                    )
-                headers = {
-                    "Content-Type": content_type,
-                    "X-XlsForm-FormId-Fallback": file_path.stem,
-                }
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
-
-        with open(file_path, "rb") if file_path is not None else nullcontext() as fd:
+            raise
+        else:
             response = self.session.response_or_error(
-                method="POST",
-                url=self.urls.post.format(project_id=pid, form_id=fid),
+                method="GET",
+                url=self.session.urlformat(self.urls.get, project_id=pid),
                 logger=log,
-                headers=headers,
-                params=params,
-                data=fd,
             )
+            data = response.json()
+            return Project(**data)
 
-        data = response.json()
-        return data["success"]
-
-    def publish(
+    def create_app_users(
         self,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-        version: Optional[str] = None,
-    ) -> bool:
+        display_names: Iterable[str],
+        forms: Iterable[str] | None = None,
+        project_id: int | None = None,
+    ) -> Iterable[ProjectAppUser]:
         """
-        Publish a Form Draft.
+        Create new project app users and optionally assign forms to them.
 
-        :param form_id: The xmlFormId of the Form being referenced.
+        :param display_names: The friendly nicknames of the app users to be created.
+        :param forms: The xmlFormIds of the forms to assign the app users to.
         :param project_id: The id of the project this form belongs to.
-        :param version: The version to be associated with the Draft once it's published.
         """
-        try:
-            pid = pv.validate_project_id(project_id, self.default_project_id)
-            fid = pv.validate_form_id(form_id, self.default_form_id)
-            params = {}
-            if version is not None:
-                key = "version"
-                params[key] = pv.validate_str(version, key=key)
-        except PyODKError as err:
-            log.error(err, exc_info=True)
-            raise err
+        if display_names is None:
+            raise PyODKError("Must specify display_names.")
 
-        response = self.session.response_or_error(
-            method="POST",
-            url=self.urls.post_publish.format(project_id=pid, form_id=fid),
-            logger=log,
-            params=params,
-        )
-        data = response.json()
-        return data["success"]
+        pid = {"project_id": project_id}
+        pau = ProjectAppUserService(session=self.session, **self._default_kw())
+        fa = FormAssignmentService(session=self.session, **self._default_kw())
+
+        current = {u.displayName for u in pau.list(**pid) if u.token is not None}
+        to_create = (user for user in display_names if user not in current)
+        users = [pau.create(display_name=n, **pid) for n in to_create]
+        # The "App User" role_id should always be "2", so no need to look it up by name.
+        # Ref: "https://github.com/getodk/central-backend/blob/9db0d792cf4640ec7329722984
+        #   cebdee3687e479/lib/model/migrations/20181212-01-add-roles.js"
+        # See also roles data in `tests/resources/projects_data.py`.
+        if forms is not None:
+            for user in users:
+                for form_id in forms:
+                    if not fa.assign(role_id=2, user_id=user.id, form_id=form_id, **pid):
+                        raise PyODKError("Role assignment failed.")
+
+        return users
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/forms.py` & `pyodk-1.0.0/pyodk/_endpoints/forms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
+from collections.abc import Callable, Iterable
 from datetime import datetime
-from typing import Any, Callable, Dict, Iterable, List, Optional
+from os import PathLike
+from typing import Any
 
 from pyodk._endpoints import bases
 from pyodk._endpoints.form_draft_attachments import FormDraftAttachmentService
 from pyodk._endpoints.form_drafts import FormDraftService
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
@@ -20,25 +22,25 @@
     xmlFormId: str
     name: str
     version: str
     enketoId: str
     hash: str
     state: str  # open, closing, closed
     createdAt: datetime
-    keyId: Optional[int]
-    updatedAt: Optional[datetime]
-    publishedAt: Optional[datetime]
+    keyId: int | None
+    updatedAt: datetime | None
+    publishedAt: datetime | None
 
 
 class URLs(bases.Model):
     class Config:
         frozen = True
 
-    list: str = "projects/{project_id}/forms"
-    get: str = "projects/{project_id}/forms/{form_id}"
+    forms: str = "projects/{project_id}/forms"
+    get: str = f"{forms}/{{form_id}}"
 
 
 class FormService(bases.Service):
     """
     Form-related functionality is accessed through `client.forms`. For example:
 
     ```python
@@ -50,121 +52,164 @@
     """
 
     __slots__ = ("urls", "session", "default_project_id", "default_form_id")
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
-        default_form_id: Optional[str] = None,
+        default_project_id: int | None = None,
+        default_form_id: str | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
-        self.default_form_id: Optional[str] = default_form_id
+        self.default_project_id: int | None = default_project_id
+        self.default_form_id: str | None = default_form_id
 
-    def _default_kw(self) -> Dict[str, Any]:
+    def _default_kw(self) -> dict[str, Any]:
         return {
             "default_project_id": self.default_project_id,
             "default_form_id": self.default_form_id,
         }
 
-    def list(self, project_id: Optional[int] = None) -> List[Form]:
+    def list(self, project_id: int | None = None) -> list[Form]:
         """
         Read all Form details.
 
         :param project_id: The id of the project the forms belong to.
 
         :return: A list of object representations of all Forms' metadata.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
         else:
             response = self.session.response_or_error(
                 method="GET",
-                url=self.urls.list.format(project_id=pid),
+                url=self.session.urlformat(self.urls.forms, project_id=pid),
                 logger=log,
             )
             data = response.json()
             return [Form(**r) for r in data]
 
     def get(
         self,
         form_id: str,
-        project_id: Optional[int] = None,
+        project_id: int | None = None,
     ) -> Form:
         """
         Read Form details.
 
         :param form_id: The id of this form as given in its XForms XML definition.
         :param project_id: The id of the project this form belongs to.
 
         :return: An object representation of the Form's metadata.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
         else:
             response = self.session.response_or_error(
                 method="GET",
-                url=self.urls.get.format(project_id=pid, form_id=fid),
+                url=self.session.urlformat(self.urls.get, project_id=pid, form_id=fid),
                 logger=log,
             )
             data = response.json()
             return Form(**data)
 
+    def create(
+        self,
+        definition: PathLike | str | bytes,
+        ignore_warnings: bool | None = True,
+        form_id: str | None = None,
+        project_id: int | None = None,
+    ) -> Form:
+        """
+        Create a form.
+
+        :param definition: The path to the file to upload (string or PathLike), or the
+          form definition in memory (string (XML) or bytes (XLS/XLSX)).
+        :param ignore_warnings: If True, create the form if there are XLSForm warnings.
+        :param form_id: The xmlFormId of the Form being referenced.
+        :param project_id: The id of the project this form belongs to.
+        :return: An object representation of the Form's metadata.
+        """
+        fd = FormDraftService(session=self.session, **self._default_kw())
+        pid, fid, headers, params, form_def = fd._prep_form_post(
+            definition=definition,
+            ignore_warnings=ignore_warnings,
+            form_id=form_id,
+            project_id=project_id,
+        )
+        params["publish"] = True
+        response = self.session.response_or_error(
+            method="POST",
+            url=self.session.urlformat(self.urls.forms, project_id=pid),
+            logger=log,
+            headers=headers,
+            params=params,
+            data=form_def,
+        )
+        data = response.json()
+        return Form(**data)
+
     def update(
         self,
         form_id: str,
-        project_id: Optional[int] = None,
-        definition: Optional[str] = None,
-        attachments: Optional[Iterable[str]] = None,
-        version_updater: Optional[Callable[[str], str]] = None,
+        project_id: int | None = None,
+        definition: PathLike | str | bytes | None = None,
+        attachments: Iterable[PathLike | str] | None = None,
+        version_updater: Callable[[str], str] | None = None,
     ) -> None:
         """
         Update an existing Form. Must specify definition, attachments or both.
 
         Accepted call patterns:
-        - definition +/- attachments
-        - attachments +/- version_updater
 
-        If a definition is provided, the new version name is presumed to be specified in
-        the definition. If no definition is provided, a default version will be set using
+        * form definition only
+        * form definition with attachments
+        * form attachments only
+        * form attachments with `version_updater`
+
+        If a definition is provided, the new version name must be specified in the
+        definition. If no definition is provided, a default version will be set using
         the current datetime is ISO format.
 
-        The default datetime version can be overridden by providing a version_updater
+        The default datetime version can be overridden by providing a `version_updater`
         function. The function will be passed the current version name as a string, and
-        must return a string with the new version name. For example the function could
-        parse then increment a version number. Or the function could disregard the input
-        and return a string e.g. `version_updater=lambda x: "v2.0"`.
+        must return a string with the new version name. For example:
+
+        * Parse then increment a version number: `version_updater=lambda v: int(v) + 1`
+        * Disregard the input and return a string: `version_updater=lambda v: "v2.0"`.
 
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
-        :param definition: The path to a form definition file to upload.
+        :param definition: The path to the file to upload (string or PathLike), or the
+          form definition in memory (string (XML) or bytes (XLS/XLSX)). The form
+          definition must include an updated version string.
         :param attachments: The paths of the form attachment file(s) to upload.
         :param version_updater: A function that accepts a version name string and returns
-          a version name string, which is used for the new form version.
+          a version name string, which is used for the new form version. Not allowed if a
+          form definition is specified.
         """
         if definition is None and attachments is None:
             raise PyODKError("Must specify a form definition and/or attachments.")
 
         if definition is not None and version_updater is not None:
             raise PyODKError("Must not specify both a definition and version_updater.")
 
         # Start a new draft - with a new definition, if provided.
         fp_ids = {"form_id": form_id, "project_id": project_id}
         fd = FormDraftService(session=self.session, **self._default_kw())
-        if not fd.create(file_path=definition, **fp_ids):
+        if not fd.create(definition=definition, **fp_ids):
             raise PyODKError("Form update (form draft create) failed.")
 
         # Upload the attachments, if any.
         if attachments is not None:
             fda = FormDraftAttachmentService(session=self.session, **self._default_kw())
             for attach in attachments:
                 if not fda.upload(file_path=attach, **fp_ids):
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/project_app_users.py` & `pyodk-1.0.0/pyodk/_endpoints/project_app_users.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import logging
 from datetime import datetime
-from typing import List, Optional
 
 from pyodk._endpoints import bases
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
 
 
 class ProjectAppUser(bases.Model):
     projectId: int
     id: int
     displayName: str
     createdAt: datetime
-    type: Optional[str]  # user, field_key, public_link, singleUse
-    token: Optional[str]
-    updatedAt: Optional[datetime]
-    deletedAt: Optional[datetime]
+    type: str | None  # user, field_key, public_link, singleUse
+    token: str | None
+    updatedAt: datetime | None
+    deletedAt: datetime | None
 
 
 class URLs(bases.Model):
     class Config:
         frozen = True
 
     list: str = "projects/{project_id}/app-users"
@@ -35,48 +34,48 @@
         "session",
         "default_project_id",
     )
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
+        default_project_id: int | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
+        self.default_project_id: int | None = default_project_id
 
     def list(
         self,
-        project_id: Optional[int] = None,
-    ) -> List[ProjectAppUser]:
+        project_id: int | None = None,
+    ) -> list[ProjectAppUser]:
         """
         Read all ProjectAppUser details.
 
         :param project_id: The project_id the ProjectAppUsers are assigned to.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="GET",
-            url=self.urls.list.format(project_id=pid),
+            url=self.session.urlformat(self.urls.list, project_id=pid),
             logger=log,
         )
         data = response.json()
         return [ProjectAppUser(**r) for r in data]
 
     def create(
         self,
         display_name: str,
-        project_id: Optional[int] = None,
+        project_id: int | None = None,
     ) -> ProjectAppUser:
         """
         Create a ProjectAppUser.
 
         :param display_name: The friendly nickname of the App User to be created.
         :param project_id: The project_id the ProjectAppUser should be assigned to.
         """
@@ -84,17 +83,17 @@
             pid = pv.validate_project_id(project_id, self.default_project_id)
             display_name = pv.wrap_error(
                 validator=pv.v.str_validator, key="display_name", value=display_name
             )
             json = {"displayName": display_name}
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="POST",
-            url=self.urls.post.format(project_id=pid),
+            url=self.session.urlformat(self.urls.post, project_id=pid),
             logger=log,
             json=json,
         )
         data = response.json()
         return ProjectAppUser(**data)
```

### Comparing `pyodk-0.3.0/pyodk/_endpoints/submissions.py` & `pyodk-1.0.0/pyodk/_endpoints/submissions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import logging
+from collections.abc import Iterable
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 from pyodk._endpoints import bases
 from pyodk._endpoints.comments import Comment, CommentService
 from pyodk._utils import validators as pv
 from pyodk._utils.session import Session
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
 
 
 class Submission(bases.Model):
     instanceId: str
     submitterId: int
     createdAt: datetime
-    deviceId: Optional[str]
+    deviceId: str | None = None
     # null, edited, hasIssues, rejected, approved
-    reviewState: Optional[str]
-    userAgent: Optional[str]
-    instanceName: Optional[str]
-    updatedAt: Optional[datetime]
+    reviewState: str | None = None
+    userAgent: str | None = None
+    instanceName: str | None = None
+    updatedAt: datetime | None = None
 
 
 class URLs(bases.Model):
     class Config:
         frozen = True
 
     _form: str = "projects/{project_id}/forms/{form_id}"
@@ -49,60 +50,60 @@
     """
 
     __slots__ = ("urls", "session", "default_project_id", "default_form_id")
 
     def __init__(
         self,
         session: Session,
-        default_project_id: Optional[int] = None,
-        default_form_id: Optional[str] = None,
+        default_project_id: int | None = None,
+        default_form_id: str | None = None,
         urls: URLs = None,
     ):
         self.urls: URLs = urls if urls is not None else URLs()
         self.session: Session = session
-        self.default_project_id: Optional[int] = default_project_id
-        self.default_form_id: Optional[str] = default_form_id
+        self.default_project_id: int | None = default_project_id
+        self.default_form_id: str | None = default_form_id
 
-    def _default_kw(self) -> Dict[str, Any]:
+    def _default_kw(self) -> dict[str, Any]:
         return {
             "default_project_id": self.default_project_id,
             "default_form_id": self.default_form_id,
         }
 
     def list(
-        self, form_id: Optional[str] = None, project_id: Optional[int] = None
-    ) -> List[Submission]:
+        self, form_id: str | None = None, project_id: int | None = None
+    ) -> list[Submission]:
         """
         Read all Submission metadata.
 
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project the Submissions belong to.
 
         :return: A list of the object representation of all Submissions' metadata.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="GET",
-            url=self.urls.list.format(project_id=pid, form_id=fid),
+            url=self.session.urlformat(self.urls.list, project_id=pid, form_id=fid),
             logger=log,
         )
         data = response.json()
         return [Submission(**r) for r in data]
 
     def get(
         self,
         instance_id: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
     ) -> Submission:
         """
         Read Submission metadata.
 
         :param instance_id: The instanceId of the Submission being referenced.
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
@@ -111,36 +112,39 @@
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
             iid = pv.validate_instance_id(instance_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="GET",
-            url=self.urls.get.format(project_id=pid, form_id=fid, instance_id=iid),
+            url=self.session.urlformat(
+                self.urls.get, project_id=pid, form_id=fid, instance_id=iid
+            ),
             logger=log,
         )
         data = response.json()
         return Submission(**data)
 
     def get_table(
         self,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-        table_name: Optional[str] = "Submissions",
-        skip: Optional[int] = None,
-        top: Optional[int] = None,
-        count: Optional[bool] = None,
-        wkt: Optional[bool] = None,
-        filter: Optional[str] = None,
-        expand: Optional[str] = None,
-    ) -> Dict:
+        form_id: str | None = None,
+        project_id: int | None = None,
+        table_name: str | None = "Submissions",
+        skip: int | None = None,
+        top: int | None = None,
+        count: bool | None = None,
+        wkt: bool | None = None,
+        filter: str | None = None,
+        expand: str | None = None,
+        select: str | None = None,
+    ) -> dict:
         """
         Read Submission data.
 
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
         :param table_name: The name of the table to be returned.
         :param skip: The first n rows will be omitted from the results.
@@ -151,14 +155,15 @@
           strings rather than GeoJSON structures.
         :param filter: Filter responses to those matching the query. Only certain fields
           are available to reference (submitterId, createdAt, updatedAt, reviewState).
           The operators lt, le, eq, neq, ge, gt, not, and, and or are supported, and the
           built-in functions now, year, month, day, hour, minute, second.
         :param expand: Repetitions, which should get expanded. Currently, only `*` (star)
           is implemented, which expands all repetitions.
+        :param select: If provided, will return only the selected fields.
 
         :return: A dictionary representation of the OData JSON document.
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
             table = pv.validate_table_name(table_name)
@@ -167,35 +172,39 @@
                 for k, v in {
                     "$skip": skip,
                     "$top": top,
                     "$count": count,
                     "$wkt": wkt,
                     "$filter": filter,
                     "$expand": expand,
+                    "$select": select,
                 }.items()
                 if v is not None
             }
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="GET",
-            url=self.urls.get_table.format(project_id=pid, form_id=fid, table_name=table),
+            url=self.session.urlformat(
+                self.urls.get_table, project_id=pid, form_id=fid, table_name=table
+            ),
             logger=log,
             params=params,
         )
         return response.json()
 
     def create(
         self,
         xml: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-        device_id: Optional[str] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
+        device_id: str | None = None,
+        encoding: str = "utf-8",
     ) -> Submission:
         """
         Create a Submission.
 
         Example submission XML structure:
 
         ```
@@ -208,88 +217,80 @@
         </data>
         ```
 
         :param xml: The submission XML.
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
         :param device_id: An optional deviceID associated with the submission.
+        :param encoding: The encoding of the submission XML, default "utf-8".
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
             params = {}
             if device_id is not None:
                 params["deviceID"] = pv.validate_str(device_id, key="device_id")
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="POST",
-            url=self.urls.post.format(project_id=pid, form_id=fid),
+            url=self.session.urlformat(self.urls.post, project_id=pid, form_id=fid),
             logger=log,
             headers={"Content-Type": "application/xml"},
             params=params,
-            data=xml,
+            data=xml.encode(encoding=encoding),
         )
         data = response.json()
         return Submission(**data)
 
     def _put(
         self,
         instance_id: str,
         xml: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
+        encoding: str = "utf-8",
     ) -> Submission:
         """
         Update Submission data.
 
-        Example submission XML structure:
-
-        ```
-        <data id="my_form" version="v1">
-          <meta>
-            <deprecatedID>uuid:85cb9aff-005e-4edd-9739-dc9c1a829c44</deprecatedID>
-            <instanceID>uuid:315c2f74-c8fc-4606-ae3f-22f8983e441e</instanceID>
-          </meta>
-          <name>Alice</name>
-          <age>36</age>
-        </data>
-        ```
-
         :param instance_id: The instanceId of the Submission being referenced.
         :param xml: The submission XML.
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
+        :param encoding: The encoding of the submission XML, default "utf-8".
         """
         try:
             pid = pv.validate_project_id(project_id, self.default_project_id)
             fid = pv.validate_form_id(form_id, self.default_form_id)
             iid = pv.validate_instance_id(instance_id)
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="PUT",
-            url=self.urls.put.format(project_id=pid, form_id=fid, instance_id=iid),
+            url=self.session.urlformat(
+                self.urls.put, project_id=pid, form_id=fid, instance_id=iid
+            ),
             logger=log,
             headers={"Content-Type": "application/xml"},
-            data=xml,
+            data=xml.encode(encoding=encoding),
         )
         data = response.json()
         return Submission(**data)
 
     def _patch(
         self,
         instance_id: str,
         review_state: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
     ) -> Submission:
         """
         Update Submission metadata.
 
         :param instance_id: The instanceId of the Submission being referenced.
         :param review_state: The current review state of the submission.
         :param form_id: The xmlFormId of the Form being referenced.
@@ -300,54 +301,75 @@
             fid = pv.validate_form_id(form_id, self.default_form_id)
             iid = pv.validate_instance_id(instance_id)
             json = {}
             if review_state is not None:
                 json["reviewState"] = review_state
         except PyODKError as err:
             log.error(err, exc_info=True)
-            raise err
+            raise
 
         response = self.session.response_or_error(
             method="PATCH",
-            url=self.urls.patch.format(project_id=pid, form_id=fid, instance_id=iid),
+            url=self.session.urlformat(
+                self.urls.patch, project_id=pid, form_id=fid, instance_id=iid
+            ),
             logger=log,
             json=json,
         )
         data = response.json()
         return Submission(**data)
 
     def edit(
         self,
         instance_id: str,
         xml: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-        comment: Optional[str] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
+        comment: str | None = None,
+        encoding: str = "utf-8",
     ) -> None:
         """
         Edit a submission and optionally comment on it.
 
-        :param instance_id: The instanceId of the Submission being referenced.
+        Example edited submission XML structure:
+
+        ```
+        <data id="my_form" version="v1">
+          <meta>
+            <deprecatedID>uuid:85cb9aff-005e-4edd-9739-dc9c1a829c44</deprecatedID>
+            <instanceID>uuid:315c2f74-c8fc-4606-ae3f-22f8983e441e</instanceID>
+          </meta>
+          <name>Alice</name>
+          <age>36</age>
+        </data>
+        ```
+
+        :param instance_id: The instanceId of the Submission being referenced. The
+          `instance_id` each Submission is first submitted with will always represent
+          that Submission as a whole. Each version of the Submission, though, has its own
+          `instance_id`. So `instance_id` will not necessarily match the values in
+           the XML elements named `instanceID` and `deprecatedID`.
         :param xml: The submission XML.
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project this form belongs to.
         :param comment: The text of the comment.
+        :param encoding: The encoding of the submission XML, default "utf-8".
         """
         fp_ids = {"form_id": form_id, "project_id": project_id}
-        self._put(instance_id=instance_id, xml=xml, **fp_ids)
+        self._put(instance_id=instance_id, xml=xml, encoding=encoding, **fp_ids)
         if comment is not None:
             self.add_comment(instance_id=instance_id, comment=comment, **fp_ids)
 
     def review(
         self,
         instance_id: str,
         review_state: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-        comment: Optional[str] = None,
+        form_id: str | None = None,
+        project_id: int | None = None,
+        comment: str | None = None,
     ) -> None:
         """
         Update Submission metadata and optionally comment on it.
 
         :param instance_id: The instanceId of the Submission being referenced.
         :param review_state: The current review state of the submission.
         :param form_id: The xmlFormId of the Form being referenced.
@@ -358,17 +380,17 @@
         self._patch(instance_id=instance_id, review_state=review_state, **fp_ids)
         if comment is not None:
             self.add_comment(instance_id=instance_id, comment=comment, **fp_ids)
 
     def list_comments(
         self,
         instance_id: str,
-        form_id: Optional[str] = None,
-        project_id: Optional[int] = None,
-    ) -> List[Comment]:
+        form_id: str | None = None,
+        project_id: int | None = None,
+    ) -> Iterable[Comment]:
         """
         Read all Comment details.
 
         :param instance_id: The instanceId of the Submission being referenced.
         :param form_id: The xmlFormId of the Form being referenced.
         :param project_id: The id of the project the Submissions belong to.
 
@@ -378,16 +400,16 @@
         comment_svc = CommentService(session=self.session, **self._default_kw())
         return comment_svc.list(instance_id=instance_id, **fp_ids)
 
     def add_comment(
         self,
         instance_id: str,
         comment: str,
-        project_id: Optional[int] = None,
-        form_id: Optional[str] = None,
+        project_id: int | None = None,
+        form_id: str | None = None,
     ) -> Comment:
         """
         Create a Comment.
 
         :param instance_id: The instanceId of the Submission being referenced.
         :param comment: The text of the comment.
         :param project_id: The id of the project this form belongs to.
```

### Comparing `pyodk-0.3.0/pyodk/_utils/config.py` & `pyodk-1.0.0/pyodk/_utils/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Dict, Optional
 
 import toml
 
 from pyodk.errors import PyODKError
 
 log = logging.getLogger(__name__)
 
@@ -14,19 +13,18 @@
     "PYODK_CONFIG_FILE": Path.home() / ".pyodk_config.toml",
     "PYODK_CACHE_FILE": Path.home() / ".pyodk_cache.toml",
 }
 
 
 @dataclass
 class CentralConfig:
-
     base_url: str
     username: str
     password: str = field(repr=False)
-    default_project_id: Optional[int] = None
+    default_project_id: int | None = None
 
     def validate(self):
         for key in ["base_url", "username", "password"]:  # Mandatory keys.
             if getattr(self, key) is None or getattr(self, key) == "":
                 err = PyODKError(f"Config value '{key}' must not be empty.")
                 log.error(err, exc_info=True)
                 raise err
@@ -36,15 +34,15 @@
 
 
 @dataclass
 class Config:
     central: CentralConfig
 
 
-def objectify_config(config_data: Dict) -> Config:
+def objectify_config(config_data: dict) -> Config:
     """
     Convert a config dict into objects to validate the data.
     """
     central = CentralConfig(**config_data["central"])
     config = Config(central=central)
     return config
 
@@ -57,70 +55,70 @@
         return Path(path)
     env_file_path = os.environ.get(env_key)
     if env_file_path is not None:
         return Path(env_file_path)
     return defaults[env_key]
 
 
-def get_config_path(config_path: Optional[str] = None) -> Path:
+def get_config_path(config_path: str | None = None) -> Path:
     return get_path(path=config_path, env_key="PYODK_CONFIG_FILE")
 
 
-def get_cache_path(cache_path: Optional[str] = None) -> Path:
+def get_cache_path(cache_path: str | None = None) -> Path:
     return get_path(path=cache_path, env_key="PYODK_CACHE_FILE")
 
 
-def read_toml(path: Path) -> Dict:
+def read_toml(path: Path) -> dict:
     """
     Read a toml file.
     """
     try:
-        with open(path, "r") as f:
+        with open(path) as f:
             return toml.load(f)
     except (FileNotFoundError, PermissionError) as err:
-        err = PyODKError(f"Could not read file at: {path}. {repr(err)}.")
-        log.error(err, exc_info=True)
-        raise err
+        pyodk_err = PyODKError(f"Could not read file at: {path}. {err!r}.")
+        log.error(pyodk_err, exc_info=True)
+        raise pyodk_err from err
 
 
-def read_config(config_path: Optional[str] = None) -> Config:
+def read_config(config_path: str | None = None) -> Config:
     """
     Read the config file.
     """
     file_path = get_path(path=config_path, env_key="PYODK_CONFIG_FILE")
     file_data = read_toml(path=file_path)
     return objectify_config(config_data=file_data)
 
 
-def read_cache_token(cache_path: Optional[str] = None) -> str:
+def read_cache_token(cache_path: str | None = None) -> str:
     """
     Read the "token" key from the cache file.
     """
     file_path = get_cache_path(cache_path=cache_path)
     file_data = read_toml(path=file_path)
     if "token" not in file_data:
         err = PyODKError(f"Cached token not found in file: {file_path}")
         log.error(err, exc_info=True)
         raise err
     return file_data["token"]
 
 
-def write_cache(key: str, value: str, cache_path: Optional[str] = None) -> None:
+def write_cache(key: str, value: str, cache_path: str | None = None) -> None:
     """
     Append or overwrite the given key/value pair to the cache file.
     """
     file_path = get_cache_path(cache_path=cache_path)
     if file_path.exists() and file_path.is_file():
         file_data = read_toml(path=file_path)
         file_data[key] = value
     else:
         file_data = {key: value}
     with open(file_path, "w") as outfile:
         toml.dump(file_data, outfile)
 
 
-def delete_cache(cache_path: Optional[str] = None) -> None:
+def delete_cache(cache_path: str | None = None) -> None:
     """
     Delete the cache file, if it exists.
     """
     file_path = get_cache_path(cache_path=cache_path)
     file_path.unlink(missing_ok=True)
```

### Comparing `pyodk-0.3.0/pyodk/_utils/validators.py` & `pyodk-1.0.0/pyodk/_utils/validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from collections.abc import Callable
+from os import PathLike
 from pathlib import Path
-from typing import Any, Callable
+from typing import Any
 
-from pydantic import validators as v
-from pydantic.errors import PydanticTypeError
+from pydantic.v1 import validators as v
+from pydantic.v1.errors import PydanticValueError
+from pydantic_core._pydantic_core import ValidationError
 
 from pyodk._utils.utils import coalesce
 from pyodk.errors import PyODKError
 
 
 def wrap_error(validator: Callable, key: str, value: Any) -> Any:
     """
@@ -15,16 +18,16 @@
     :param validator: A pydantic validator function.
     :param key: The variable name to use in the error message.
     :param value: The variable value.
     :return:
     """
     try:
         return validator(value)
-    except PydanticTypeError as err:
-        msg = f"{key}: {str(err)}"
+    except (ValidationError, PydanticValueError) as err:
+        msg = f"{key}: {err!s}"
         raise PyODKError(msg) from err
 
 
 def validate_project_id(*args: int) -> int:
     return wrap_error(
         validator=v.int_validator,
         key="project_id",
@@ -52,14 +55,22 @@
     return wrap_error(
         validator=v.str_validator,
         key="instance_id",
         value=coalesce(*args),
     )
 
 
+def validate_entity_list_name(*args: str) -> str:
+    return wrap_error(
+        validator=v.str_validator,
+        key="entity_list_name",
+        value=coalesce(*args),
+    )
+
+
 def validate_str(*args: str, key: str) -> str:
     return wrap_error(
         validator=v.str_validator,
         key=key,
         value=coalesce(*args),
     )
 
@@ -76,13 +87,21 @@
     return wrap_error(
         validator=v.int_validator,
         key=key,
         value=coalesce(*args),
     )
 
 
-def validate_file_path(*args: str) -> Path:
+def validate_dict(*args: dict, key: str) -> int:
+    return wrap_error(
+        validator=v.dict_validator,
+        key=key,
+        value=coalesce(*args),
+    )
+
+
+def validate_file_path(*args: PathLike | str) -> Path:
     def validate_fp(f):
         p = v.path_validator(f)
         return v.path_exists_validator(p)
 
     return wrap_error(validator=validate_fp, key="file_path", value=coalesce(*args))
```

### Comparing `pyodk-0.3.0/pyodk/client.py` & `pyodk-1.0.0/pyodk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Callable, Optional
+from collections.abc import Callable
 
 from pyodk._endpoints.comments import CommentService
+from pyodk._endpoints.entities import EntityService
+from pyodk._endpoints.entity_lists import EntityListService
 from pyodk._endpoints.forms import FormService
 from pyodk._endpoints.projects import ProjectService
 from pyodk._endpoints.submissions import SubmissionService
 from pyodk._utils import config
 from pyodk._utils.session import Session
 
 
@@ -24,22 +26,22 @@
         of a customised subclass.
     :param api_version: The ODK Central API version, which is used in the URL path
         e.g. 'v1' in 'https://www.example.com/v1/projects'.
     """
 
     def __init__(
         self,
-        config_path: Optional[str] = None,
-        cache_path: Optional[str] = None,
-        project_id: Optional[int] = None,
-        session: Optional[Session] = None,
-        api_version: Optional[str] = "v1",
+        config_path: str | None = None,
+        cache_path: str | None = None,
+        project_id: int | None = None,
+        session: Session | None = None,
+        api_version: str | None = "v1",
     ) -> None:
         self.config: config.Config = config.read_config(config_path=config_path)
-        self._project_id: Optional[int] = project_id
+        self._project_id: int | None = project_id
         if session is None:
             session = Session(
                 base_url=self.config.central.base_url,
                 api_version=api_version,
                 username=self.config.central.username,
                 password=self.config.central.password,
                 cache_path=cache_path,
@@ -63,17 +65,23 @@
         )
         self.submissions: SubmissionService = SubmissionService(
             session=self.session, default_project_id=self.project_id
         )
         self._comments: CommentService = CommentService(
             session=self.session, default_project_id=self.project_id
         )
+        self.entities: EntityService = EntityService(
+            session=self.session, default_project_id=self.project_id
+        )
+        self.entity_lists: EntityListService = EntityListService(
+            session=self.session, default_project_id=self.project_id
+        )
 
     @property
-    def project_id(self) -> Optional[int]:
+    def project_id(self) -> int | None:
         if self._project_id is None:
             return self.config.central.default_project_id
         else:
             return self._project_id
 
     @project_id.setter
     def project_id(self, v: str):
```

