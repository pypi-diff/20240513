# Comparing `tmp/django_allianceutils-3.0.0.tar.gz` & `tmp/django_allianceutils-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allianceutils-3.0.0.tar", max compression
+gzip compressed data, was "django_allianceutils-4.0.0.tar", max compression
```

## Comparing `django_allianceutils-3.0.0.tar` & `django_allianceutils-4.0.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0     3628 2023-06-08 00:59:23.897567 django_allianceutils-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1541 2020-09-13 18:13:00.145577 django_allianceutils-3.0.0/LICENSE
--rw-r--r--   0        0        0    38610 2023-06-08 00:58:48.623754 django_allianceutils-3.0.0/README.md
--rw-r--r--   0        0        0     5972 2023-06-08 00:59:36.341485 django_allianceutils-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1000 2023-06-08 00:59:35.523430 django_allianceutils-3.0.0/src/allianceutils/__init__.py
--rw-r--r--   0        0        0       22 2023-06-05 01:24:04.281525 django_allianceutils-3.0.0/src/allianceutils/api/__init__.py
--rw-r--r--   0        0        0     4154 2023-06-05 01:24:04.281720 django_allianceutils-3.0.0/src/allianceutils/api/mixins.py
--rw-r--r--   0        0        0     4380 2023-06-05 01:24:04.281911 django_allianceutils-3.0.0/src/allianceutils/api/parsers.py
--rw-r--r--   0        0        0     7935 2023-06-05 01:24:04.282167 django_allianceutils-3.0.0/src/allianceutils/api/permissions.py
--rw-r--r--   0        0        0      568 2023-06-05 01:24:04.282357 django_allianceutils-3.0.0/src/allianceutils/api/renderers.py
--rw-r--r--   0        0        0      192 2023-06-05 01:24:04.282852 django_allianceutils-3.0.0/src/allianceutils/apps.py
--rw-r--r--   0        0        0        0 2023-06-05 01:24:04.282975 django_allianceutils-3.0.0/src/allianceutils/auth/__init__.py
--rw-r--r--   0        0        0     2056 2023-06-05 01:24:04.283129 django_allianceutils-3.0.0/src/allianceutils/auth/backends.py
--rw-r--r--   0        0        0    13890 2023-06-08 00:58:45.062512 django_allianceutils-3.0.0/src/allianceutils/auth/models.py
--rwxr-xr-x   0        0        0      590 2023-06-05 01:24:04.283948 django_allianceutils-3.0.0/src/allianceutils/bin/internaldeps.sh
--rw-r--r--   0        0        0    15004 2023-06-05 01:24:04.284300 django_allianceutils-3.0.0/src/allianceutils/checks.py
--rw-r--r--   0        0        0     3118 2023-06-08 00:58:45.063255 django_allianceutils-3.0.0/src/allianceutils/decorators.py
--rw-r--r--   0        0        0        0 2023-06-05 01:24:04.284626 django_allianceutils-3.0.0/src/allianceutils/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 01:24:04.284767 django_allianceutils-3.0.0/src/allianceutils/management/commands/__init__.py
--rw-r--r--   0        0        0     1829 2023-06-05 01:24:04.284986 django_allianceutils-3.0.0/src/allianceutils/management/commands/base.py
--rw-r--r--   0        0        0     6991 2023-06-05 01:24:04.285225 django_allianceutils-3.0.0/src/allianceutils/management/commands/document_reverse_accessors.py
--rw-r--r--   0        0        0     1600 2023-06-05 01:24:04.285405 django_allianceutils-3.0.0/src/allianceutils/management/commands/print_logging.py
--rw-r--r--   0        0        0      234 2023-06-05 01:24:04.285610 django_allianceutils-3.0.0/src/allianceutils/middleware/__init__.py
--rw-r--r--   0        0        0     1899 2023-06-05 01:24:04.285819 django_allianceutils-3.0.0/src/allianceutils/middleware/current_user.py
--rw-r--r--   0        0        0     1216 2023-06-05 01:24:04.285981 django_allianceutils-3.0.0/src/allianceutils/middleware/http_auth.py
--rw-r--r--   0        0        0     2643 2023-06-05 01:24:04.286203 django_allianceutils-3.0.0/src/allianceutils/middleware/query_count.py
--rw-r--r--   0        0        0     1705 2023-06-05 01:24:04.286378 django_allianceutils-3.0.0/src/allianceutils/migrations.py
--rw-r--r--   0        0        0    11164 2023-06-05 01:24:04.286743 django_allianceutils-3.0.0/src/allianceutils/models.py
--rw-r--r--   0        0        0        0 2023-06-08 00:58:45.063336 django_allianceutils-3.0.0/src/allianceutils/py.typed
--rw-r--r--   0        0        0     1325 2023-06-05 01:24:04.286949 django_allianceutils-3.0.0/src/allianceutils/rules.py
--rw-r--r--   0        0        0        0 2023-06-05 01:24:04.287065 django_allianceutils-3.0.0/src/allianceutils/serializers/__init__.py
--rw-r--r--   0        0        0      640 2023-06-05 01:24:04.287268 django_allianceutils-3.0.0/src/allianceutils/serializers/json_ordered.py
--rw-r--r--   0        0        0        0 2023-06-05 01:24:04.287375 django_allianceutils-3.0.0/src/allianceutils/templatetags/__init__.py
--rw-r--r--   0        0        0     2054 2023-06-05 01:24:04.287568 django_allianceutils-3.0.0/src/allianceutils/templatetags/alliance_webpack.py
--rw-r--r--   0        0        0     1345 2023-06-05 01:24:04.287736 django_allianceutils-3.0.0/src/allianceutils/templatetags/default_value.py
--rw-r--r--   0        0        0     2217 2023-06-05 01:24:04.287963 django_allianceutils-3.0.0/src/allianceutils/util/__init__.py
--rw-r--r--   0        0        0     9530 2023-06-05 01:24:04.288588 django_allianceutils-3.0.0/src/allianceutils/util/camel_case.py
--rw-r--r--   0        0        0     1238 2023-06-05 01:24:04.288782 django_allianceutils-3.0.0/src/allianceutils/util/date.py
--rw-r--r--   0        0        0     1278 2023-06-08 00:33:28.380905 django_allianceutils-3.0.0/src/allianceutils/util/get_firstparty_apps.py
--rw-r--r--   0        0        0        0 2023-06-05 01:24:04.289603 django_allianceutils-3.0.0/src/allianceutils/views/__init__.py
--rw-r--r--   0        0        0      788 2023-06-05 01:24:04.289806 django_allianceutils-3.0.0/src/allianceutils/views/decorators.py
--rw-r--r--   0        0        0     7186 2023-06-05 01:24:04.290003 django_allianceutils-3.0.0/src/allianceutils/webpack.py
--rw-r--r--   0        0        0    40536 1970-01-01 00:00:00.000000 django_allianceutils-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4701 2024-04-04 04:26:16.768353 django_allianceutils-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1541 2021-02-21 23:36:59.889372 django_allianceutils-4.0.0/LICENSE
+-rw-r--r--   0        0        0    44959 2024-04-04 04:26:16.768651 django_allianceutils-4.0.0/README.md
+-rw-r--r--   0        0        0     5862 2024-04-04 04:26:16.769884 django_allianceutils-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1000 2024-04-04 04:26:16.770083 django_allianceutils-4.0.0/src/allianceutils/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-04 04:26:16.770395 django_allianceutils-4.0.0/src/allianceutils/api/__init__.py
+-rw-r--r--   0        0        0     4202 2024-04-04 04:26:16.770518 django_allianceutils-4.0.0/src/allianceutils/api/mixins.py
+-rw-r--r--   0        0        0     4380 2024-04-04 04:26:16.770635 django_allianceutils-4.0.0/src/allianceutils/api/parsers.py
+-rw-r--r--   0        0        0     7935 2024-04-04 04:26:16.770750 django_allianceutils-4.0.0/src/allianceutils/api/permissions.py
+-rw-r--r--   0        0        0      568 2024-04-04 04:26:16.770992 django_allianceutils-4.0.0/src/allianceutils/api/renderers.py
+-rw-r--r--   0        0        0      192 2024-04-04 04:26:16.771251 django_allianceutils-4.0.0/src/allianceutils/apps.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.771358 django_allianceutils-4.0.0/src/allianceutils/auth/__init__.py
+-rw-r--r--   0        0        0     2060 2024-04-04 04:26:16.771663 django_allianceutils-4.0.0/src/allianceutils/auth/backends.py
+-rw-r--r--   0        0        0    14006 2024-04-04 04:26:16.771856 django_allianceutils-4.0.0/src/allianceutils/auth/models.py
+-rw-r--r--   0        0        0     7997 2024-04-04 04:26:16.771994 django_allianceutils-4.0.0/src/allianceutils/auth/permission.py
+-rwxr-xr-x   0        0        0      590 2024-04-04 04:26:16.772150 django_allianceutils-4.0.0/src/allianceutils/bin/internaldeps.sh
+-rw-r--r--   0        0        0    15032 2024-04-04 04:26:16.772356 django_allianceutils-4.0.0/src/allianceutils/checks.py
+-rw-r--r--   0        0        0     3118 2024-04-04 04:26:16.772496 django_allianceutils-4.0.0/src/allianceutils/decorators.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.772594 django_allianceutils-4.0.0/src/allianceutils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.772736 django_allianceutils-4.0.0/src/allianceutils/management/commands/__init__.py
+-rw-r--r--   0        0        0     1829 2024-04-04 04:26:16.772867 django_allianceutils-4.0.0/src/allianceutils/management/commands/base.py
+-rw-r--r--   0        0        0     6991 2024-04-04 04:26:16.773001 django_allianceutils-4.0.0/src/allianceutils/management/commands/document_reverse_accessors.py
+-rw-r--r--   0        0        0     1600 2024-04-04 04:26:16.773517 django_allianceutils-4.0.0/src/allianceutils/management/commands/print_logging.py
+-rw-r--r--   0        0        0      320 2024-04-04 04:26:16.773658 django_allianceutils-4.0.0/src/allianceutils/middleware/__init__.py
+-rw-r--r--   0        0        0     1149 2024-04-04 04:26:16.773758 django_allianceutils-4.0.0/src/allianceutils/middleware/current_request.py
+-rw-r--r--   0        0        0     1899 2024-04-04 04:26:16.773857 django_allianceutils-4.0.0/src/allianceutils/middleware/current_user.py
+-rw-r--r--   0        0        0     1216 2024-04-04 04:26:16.774116 django_allianceutils-4.0.0/src/allianceutils/middleware/http_auth.py
+-rw-r--r--   0        0        0     2643 2024-04-04 04:26:16.774240 django_allianceutils-4.0.0/src/allianceutils/middleware/query_count.py
+-rw-r--r--   0        0        0     1761 2024-04-04 04:26:16.774339 django_allianceutils-4.0.0/src/allianceutils/migrations.py
+-rw-r--r--   0        0        0    11173 2024-04-04 04:26:16.774495 django_allianceutils-4.0.0/src/allianceutils/models.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.774528 django_allianceutils-4.0.0/src/allianceutils/py.typed
+-rw-r--r--   0        0        0     1325 2024-04-04 04:26:16.774636 django_allianceutils-4.0.0/src/allianceutils/rules.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.774714 django_allianceutils-4.0.0/src/allianceutils/serializers/__init__.py
+-rw-r--r--   0        0        0      640 2024-04-04 04:26:16.774817 django_allianceutils-4.0.0/src/allianceutils/serializers/json_ordered.py
+-rw-r--r--   0        0        0     7590 2024-04-04 04:26:16.774936 django_allianceutils-4.0.0/src/allianceutils/template.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.775017 django_allianceutils-4.0.0/src/allianceutils/templatetags/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-04 04:26:16.775115 django_allianceutils-4.0.0/src/allianceutils/templatetags/alliance_webpack.py
+-rw-r--r--   0        0        0     1345 2024-04-04 04:26:16.775200 django_allianceutils-4.0.0/src/allianceutils/templatetags/default_value.py
+-rw-r--r--   0        0        0     3656 2024-04-04 04:26:16.775369 django_allianceutils-4.0.0/src/allianceutils/tests/util.py
+-rw-r--r--   0        0        0     2248 2024-04-04 04:26:16.775513 django_allianceutils-4.0.0/src/allianceutils/util/__init__.py
+-rw-r--r--   0        0        0     9559 2024-04-04 04:26:16.775618 django_allianceutils-4.0.0/src/allianceutils/util/camel_case.py
+-rw-r--r--   0        0        0     1238 2024-04-04 04:26:16.775719 django_allianceutils-4.0.0/src/allianceutils/util/date.py
+-rw-r--r--   0        0        0     1278 2024-04-04 04:26:16.775822 django_allianceutils-4.0.0/src/allianceutils/util/get_firstparty_apps.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:26:16.775909 django_allianceutils-4.0.0/src/allianceutils/views/__init__.py
+-rw-r--r--   0        0        0      788 2024-04-04 04:26:16.776008 django_allianceutils-4.0.0/src/allianceutils/views/decorators.py
+-rw-r--r--   0        0        0     7186 2024-04-04 04:26:16.776122 django_allianceutils-4.0.0/src/allianceutils/webpack.py
+-rw-r--r--   0        0        0    46751 1970-01-01 00:00:00.000000 django_allianceutils-4.0.0/PKG-INFO
```

### Comparing `django_allianceutils-3.0.0/CHANGELOG.md` & `django_allianceutils-4.0.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -22,14 +22,48 @@
 
 ### Fixed
 
 * An Item
 
 -->
 
+## 4.0.0 2024-03-18
+
+### Breaking Changes
+* Dropped support for django 3.2
+
+### Added
+
+* Add support for django 5.0
+* Add `CurrentRequestMiddleware`
+* Add `tox-poetry-installer` middleware to allow better management of tox dependencies in poetry
+
+* Migrate `common_lib.templatetags.common` from template project to `template.py` with the following functions:
+    * `resolve`
+    * `token_kwargs`
+    * `parse_tag_arguments`
+    * `build_html_attrs`
+    * `is_static_expression`
+
+* Migrate `common_lib.tests.util` from template project to `tests/util.py` with the following decorators:
+    * `suppress_silk`
+    * `logging_filter`
+    * `warning_filter`
+
+* Migrate `permission` from template project with:
+    * `class NoDefaultPermissionsMeta`
+    * `class PermissionNotImplementedError`
+    * `class AmbiguousGlobalPermissionWarning`
+    * `def identify_global_perms`
+    * `def reverse_if_probably_allowed`
+
+### Fixed
+
+* CI now properly tests for all Django versions, whereas previously Poetry would install the latest Django version and overwrite the tox-managed dependencies
+
 ## 3.0.0 2023-06-08
 
 ### Breaking changes
 * Dropped support for django 2.2
 * Dropped support for python 3.7, 3.6
 * Dropped support for django-db-constraints validation (`check_db_constraints()` constraint length & collisions); should use django native constraints instead
 * `ProfileModelBackend` has been removed. You should use `ProfileModelBackendMixin` instead, and implement a case
@@ -45,40 +79,40 @@
 * Add support for django 4.2
 * Add support for python 3.10, 3.11
 * New `QueryCountMiddleware` methods `set_threshold` and `increase_threshold`
   * `request.QUERY_COUNT_WARNING_THRESHOLD` is still supported but will be removed in future versions
 
 ### Fixed
 
-* Resolve bug in `CamelCaseMultiPartJSONParser.parse` where if the `HTTP_X_MULTIPART_JSON` header is not set it tries to parse the stream a second time, which returns no data 
+* Resolve bug in `CamelCaseMultiPartJSONParser.parse` where if the `HTTP_X_MULTIPART_JSON` header is not set it tries to parse the stream a second time, which returns no data
 
 ## 2.2.0 2022-03-28
 
 ### Fixed
 
 * `CheckExplicitTableNames` will now skip unmanaged models to allow for cases where there is no table
 
 ## 2.1.0 2021-12-17
 
 ### Fixed
-* Support new URL pattern adopted by django to resolve [CVE-2021-44420] (https://www.djangoproject.com/weblog/2021/dec/07/security-releases/) 
-* Add check class for configurable git path, update to handle hooksPath config for newer husky  
+* Support new URL pattern adopted by django to resolve [CVE-2021-44420] (https://www.djangoproject.com/weblog/2021/dec/07/security-releases/)
+* Add check class for configurable git path, update to handle hooksPath config for newer husky
 
 ## 2.0.0 2021-07-22
 
 ### Added
 
 * Add support for django 3.2
 * `auth/backends` now works without `authtools`
     * `ProfileModelBackend` will not be available if `authtools` is not able to be imported (`authtools` does not currently work with django 3.2)
 * ````
 * Add `add_autoreload_extra_files()`
-* Add ability for checks to ignore apps/models using a regex instead of just a static string 
+* Add ability for checks to ignore apps/models using a regex instead of just a static string
+
 
-  
 ### Fixed
 * `GenericUserProfile.normalize_email` can now be overridden on child classes and will work as expected
 
 ### Breaking Changes
 * Drop support for django 1.11
 * Drop support for isort 4
```

### Comparing `django_allianceutils-3.0.0/LICENSE` & `django_allianceutils-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/README.md` & `django_allianceutils-4.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,27 @@
         * [Commands](#commands)
         * [Checks](#checks)
     * [Middleware](#middleware)
     * [Migrations](#migrations)
     * [Models](#models)
     * [Rules](#rules)
     * [Serializers](#serializers)
+    * [Template](#template)
     * [Template Tags](#template-tags)
+    * [Tests](#tests)
     * [Util](#util)
 * [Changelog](#changelog)
 
 ## Installation
 
 `pip install django-allianceutils`
 
 ## System Requirements
 
-* Tested with django 3.2 and 4.2
+* Tested with django 4.2 and 5.0
   * Pull requests accepted for other versions, but at minimum we test against current LTS versions
 * Python >=3.8
 
 ## Usage
 
 ### API
 
@@ -77,61 +79,61 @@
 
 * Creates permissions that have no model by linking them to an empty content type
 * Django creates permissions as part of
   the [`post_migrate` signal](https://docs.djangoproject.com/en/stable/ref/signals/#post-migrate)
 
 Usage
 
-```py
+```python
 def on_post_migrate(sender, **kwargs):
     register_custom_permissions("myapp", ("my_perm", "My Permission"))
 ```
 
 ##### SimpleDjangoObjectPermissions
 
 Permission class for Django Rest Framework that adds support for object level permissions.
 
 Differs from just DRF's [DjangoObjectPermissions](https://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions) because it
 * does not require a queryset
-* uses the same permission for every request http method and ViewSet method 
+* uses the same permission for every request http method and ViewSet method
 
 Notes
 * The default django permissions system will [always return False](https://docs.djangoproject.com/en/stable/topics/auth/customizing/#handling-object-permissions) if given an object; you must be using another permissions backend
 * As per [DRF documentation](http://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions): get_object() is only required if you want to implement object-level permissions
 * **WARNING** If you override `get_object()` then you need to *manually* invoke `self.check_object_permissions(self.request, obj)`
 * Will attempt to check permission both globally and on a per-object basis but considers it an error if the check returns True for both
-*   
+*
 
 Usage
 * See [DRF permissions policy](https://www.django-rest-framework.org/api-guide/permissions/#setting-the-permission-policy) for details on apply Permissions policies globally
 
 * To apply to a specific view you need to set `permission_required`
 ```python
 class MyAPIView(SimpleDjangoObjectPermissions, APIView):
         permission_required = 'my_module.my_permission'
-        permission_classes = [allianceutils.api.permissions.SimpleDjangoObjectPermissions] 
+        permission_classes = [allianceutils.api.permissions.SimpleDjangoObjectPermissions]
 ```
 
 If you have no object level permissions (eg. from rules) then it will just do a static permission check.
 
 ##### GenericDjangoViewsetPermissions
 
 * Map viewset actions to Django permissions.
   * The model used for permission is extracted from the ViewSet
     * If you implement `get_permission_model` on the ViewSet that will be used
-    * Otherwise it will call `get_queryset` on the ViewSet and extract the model from the returned queryset 
- * To alter this behaviour extends `GenericDjangoViewsetPermissions` and implement `get_model` 
+    * Otherwise it will call `get_queryset` on the ViewSet and extract the model from the returned queryset
+ * To alter this behaviour extends `GenericDjangoViewsetPermissions` and implement `get_model`
 * Usage example:
-```
+```python
 class MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):
     queryset = MyModel.objects.all()
     serializer_class = MySerializer
 ```
 * `GenericDjangoViewsetPermissions.default_actions_to_perms_map` defines the default set of permissions. These can be extended or overridden using `actions_to_perms_map`:
-```
+```python
 class MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):
 
     # ...
 
     actions_to_perms_map = {
         'create': []
     }
@@ -220,107 +222,137 @@
 ### Auth
 
 #### MinimalModelBackend
 
 * `allianceutils.auth.backends.MinimalModelBackend`
     * Replaces the built-in django [ModelBackend](https://docs.djangoproject.com/en/stable/ref/contrib/auth/#django.contrib.auth.backends.ModelBackend)
     * Provides django model-based authentication
-    * Removes the default authorization (permissions checks) except for checking `is_superuser` 
+    * Removes the default authorization (permissions checks) except for checking `is_superuser`
 
 #### ProfileModelBackend
 
 * Backends for use with [GenericUserProfile](#GenericUserProfile); see code examples there
 * `allianceutils.auth.backends.ProfileModelBackendMixin` - in combo with [AuthenticationMiddleware](https://docs.djangoproject.com/en/stable/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) will set user profiles on `request.user`
-  * If you want  
+  * If you want
       * ~`allianceutils.auth.backends.ProfileModelBackend`~ - convenience class combined with case insensitive username & default django permissions backend
           * this depended on [`authtools`](https://django-authtools.readthedocs.io/en/latest/) which appears to have been
             abandoned and does not work with django >= 3.
             If using django 3 then we recommended that you create your own backend in your app:
             ```python
               class ProfileModelBackend(ProfileModelBackendMixin, MinimalModelBackend):
-                  # you'll need to implement case insensitivity either here or in the User Model  
+                  # you'll need to implement case insensitivity either here or in the User Model
                   pass
             ```
 
+#### Permissions
+
+##### NoDefaultPermissionsMeta
+
+- Define a `Meta` class with empty default permissions so Django doesn't create any
+- Usage example:
+
+```python
+class User(GenericUserProfile):
+
+    class Meta(NoDefaultPermissionsMeta):
+        pass
+```
+
+##### PermissionNotImplementedError
+
+- Subclass of `NotImplementedError` specific to permissions
+
+##### identify_global_perms
+
+- Takes a permission or list of permissions and splits them into global and object permissions, returning a tuple of (global permission list, object permission list). If the type can't be determined, the permission is returned in the global permission list.
+
+##### AmbiguousGlobalPermissionWarning
+
+- Raised if a permission cannot be classified as either global or per-object
+
+##### reverse_if_probably_allowed
+
+- Attempts to guess whether a user has permission to access a view to determine whether a URL should be displayed. Only for display purposes, not actual security, as it is not 100% reliable: can be used to, for example, hide the edit link in a CRUD view where the user does not have edit access. Takes the current request and the requested viewname, and optionally the specific object to be accessed.
+
 ### Decorators
 
 #### gzip_page_ajax
 
 * Smarter version of django's [gzip_page](https://docs.djangoproject.com/en/stable/topics/http/decorators/#django.views.decorators.gzip.gzip_page):
     * If settings.DEBUG not set, will always gzip
     * If settings.DEBUG set, will gzip only if request is an ajax request
 * This allows you to use django-debug-toolbar in DEBUG mode (if you gzip a response then the debug toolbar middleware won't run)
 
 Example
 
-```
+```python
 
 @allianceutils.views.decorators.gzip_page_ajax
 def my_view(request: HttpRequest) -> httpResponse:
     data = {
         "message": "Hello World",
     }
-    return django.http.JsonResponse(data) 
+    return django.http.JsonResponse(data)
 
 ```
 
 #### method_cache
 
 * Caches the results of a method on the object instance
-* There is no thread synchronization so in some circumstances the method may be called multiple times if multiple threads share the object 
+* There is no thread synchronization so in some circumstances the method may be called multiple times if multiple threads share the object
 * Only works for regular object methods with no arguments other than `self`.
     * Does not support `@classmethod` or `@staticmethod`
     * If you want more powerful caching behaviour then you can
       * use [`methodtools`](https://pypi.org/project/methodtools/)
       * wrap `cachetools` (examples [here](https://github.com/tkem/cachetools/issues/107#issuecomment-436274285))
 * Similar to [`@cached_property`](https://docs.python.org/3/library/functools.html#functools.cached_property) except that it works on methods instead of properties
 * Differs from [`@lru_cache()`](https://docs.python.org/3/library/functools.html#functools.lru_cache) in that
     * `lru_cache` uses a single cache for each decorated function
-    * `lru_cache` will block garbage collection of values in the cache 
-    * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance   
+    * `lru_cache` will block garbage collection of values in the cache
+    * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance
 
 Usage
 ```python
 class MyViewSet(ViewSet):
 
     # ...
 
     @method_cache
     def get_object(self):
         return super().get_object()
 
 obj = MyViewSet()
 obj.get_object() is obj.get_object()
-obj.get_object.cache_clear()   
+obj.get_object.cache_clear()
 ```
 
 ### Management
 
 #### Commands
 
 ##### OptionalAppCommand
 
 * A utility class that extends `django.core.management.base.BaseCommand` and adds optional argument(s) for django apps
 * If app names are passed on the command line `handle_app_config()` will be called with the `AppConfig` for each app otherwise it will be called with every first-party app (as determined by `isort`)
 
 
 Example:
 
-```
+```python
 class Command(allianceutils.management.commands.base.OptionalAppCommand):
     def add_arguments(self, parser):
         super().add_arguments(parser)
         parser.add_argument('--type', choices=('name', 'label'), default='name')
 
     def handle_app_config(self, app_config: AppConfig, **options):
         if options['type'] == 'name':
             print(f"Called with {app_config.name}")
         if options['type'] == 'label':
             print(f"Called with {app_config.label}")
-```  
+```
 
 ##### print_logging
 
 * Displays the current logging configuration in a hierarchical fashion
 * Requires [`logging_tree`](https://pypi.python.org/pypi/logging_tree) to be installed
 
 #### Checks
@@ -347,31 +379,31 @@
 
     def ready(self):
         register(check=check_admins, tags=Tags.admin, deploy=True)
         register(check=check_db_constraints, tags=Tags.database)
         register(check=CheckExplicitTableNames(), tags=Tags.models)
         register(check=check_git_hooks, tags=Tags.admin)
         register(check=CheckReversibleFieldNames(), tags=Tags.models)
-        register(check=CheckUrlTrailingSlash(expect_trailing_slash=True), tags=Tags.url)        
+        register(check=CheckUrlTrailingSlash(expect_trailing_slash=True), tags=Tags.url)
 ```
 
 ##### CheckUrlTrailingSlash
 
-* Checks that your URLs are consistent with the `settings.APPEND_SLASH`  
+* Checks that your URLs are consistent with the `settings.APPEND_SLASH`
 * Arguments:
     * `ignore_attrs` - skip checks on url patterns where an attribute of the pattern matches something in here (see example above)
         * Most relevant attributes of a `RegexURLResolver`:
             * `_regex` - string used for regex matching. Defaults to `[r'^$']`
             * `app_name` - app name (only works for `include()` patterns). Defaults to `['djdt']` (django debug toolbar)
             * `namespace` - pattern defines a namespace
             * `lookup_str` - string defining view to use. Defaults to `['django.views.static.serve']`
         * Note that if you skip a resolver it will also skip checks on everything inside that resolver
 * Note: If using Django REST Framework's [`DefaultRouter`](http://www.django-rest-framework.org/api-guide/routers/#defaultrouter) then you need to turn off `include_format_suffixes`:
 
-```
+```python
 router = routers.DefaultRouter(trailing_slash=True)
 router.include_format_suffixes = False
 router.register(r'myurl', MyViewSet)
 urlpatterns += router.urls
 ```
 
 
@@ -379,30 +411,30 @@
 
 * Checks that `settings.ADMINS` has been properly set in settings files.
 
 ##### check\_git\_hooks
 
 * Checks that git hookshave been set up, one of:
   * `.git/hooks` directory has been symlinked to the project's `git-hooks`
-  * [`husky`](https://github.com/typicode/husky) hooks have been installed 
-* 
+  * [`husky`](https://github.com/typicode/husky) hooks have been installed
+*
 
 ##### check\_db\_constraints
 
 * Checks that all models that specify `db_constraints` in their Meta will generate unique constraint names when truncated by the database.
 
 ##### CheckExplicitTableNames
 
 * Checks that all first-party models have `db_table` explicitly defined on their Meta class, and the table name is in lowercase
 * Arguments:
     * `enforce_lowercase` - check that there are no uppercase characters in the table name
     * `ignore_labels` - if an app label (eg `silk`) or app_label + model labels (eg `silk.request`)
         matches something in `ignore_labels` then it will be ignored.
         * `allianceutils.checks.DEFAULT_TABLE_NAME_CHECK_IGNORE` contains a default list of apps/models to ignore
-        * Can be either a `str` or a regex (anything that contains a `.match()` method) 
+        * Can be either a `str` or a regex (anything that contains a `.match()` method)
 
 ##### CheckReversibleFieldNames
 
 * Checks that all models have fields names that are reversible with `underscorize`/`camelize`/`camel_to_underscore`/`underscore_to_camel`
 * Arguments:
     * `ignore_labels` - ignore these apps/models: see `CheckExplicitTableNames`
 
@@ -418,15 +450,15 @@
     * Add `allianceutils.middleware.HttpAuthMiddleware` to `MIDDLEWARE`.
     * Add `HTTP_AUTH_USERNAME` and `HTTP_AUTH_PASSWORD` to appropriate setting file, e.g. `settings/production_staging.py`
         * Remember that you shouldn't be hardcoding credentials in code: read content from env vars or file
 
 #### CurrentUserMiddleware
 
 * Middleware to enable accessing the currently logged-in user without a request object.
-    * Assumes that `threading.local` is not shared between requests (an assumption also made by django internationalisation) 
+    * Assumes that `threading.local` is not shared between requests (an assumption also made by django internationalisation)
 
 * Setup
     * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.
 
 * Usage
 
 ```python
@@ -439,33 +471,33 @@
 
 * Warns if query count reaches a given threshold
     * Threshold can be changed by setting `settings.QUERY_COUNT_WARNING_THRESHOLD`
 
 * Usage
     * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.
     * Uses the `warnings` module to raise a warning; by default this is suppressed by django
-        * To ensure `QueryCountWarning` is never suppressed  
+        * To ensure `QueryCountWarning` is never suppressed
 
 ```python
 warnings.simplefilter('always', allianceutils.middleware.QueryCountWarning)
 ```
 
-* To increase the query count limit for one request, you can call `QueryCountMiddleware.increase_threshold(request, increment)` 
+* To increase the query count limit for one request, you can call `QueryCountMiddleware.increase_threshold(request, increment)`
 * To set the query count limit for one request you can call `QueryCountMiddleware.set_threshold(request, threshold)`
   * Rather than hardcode a new limit, `increase_threshold()` is generally preferable
   * This can be useful to disable checks entirely (pass `0` as the new limit)
 
 
 ```python
 def my_view(request, *args, **kwargs):
     request.QUERY_COUNT_WARNING_THRESHOLD += 10
     ...
 
 ```
- 
+
 
 ### Migrations
 
 #### Run SQL function
 * Wrapper to `RunSQL` that reads SQL from a file instead of inline in python
 * The reason you would do this as an external file & function is so that squashed migrations don't become unwieldy (django will inline and strip whitespace in the SQL)
 
@@ -493,48 +525,48 @@
     * Can still be deleted with manual queries
 * Read django docs about [manager inheritance](https://docs.djangoproject.com/en/stable/topics/db/managers/#custom-managers-and-model-inheritance)
     * If you wish add your own manager, you need to combine the querysets:
 
 ```python
 class MyModel(NoDeleteModel):
         objects = combine_querysets_as_manager(NoDeleteQuerySet, MyQuerySet)
-```  
+```
 
 #### GenericUserProfile
 Allows you to iterate over a `User` table and have it return a corresponding `Profile` record without generating extra queries
 
 Minimal example:
 
 ```python
 # ------------------------------------------------------------------
-# base User model 
+# base User model
 
 # If you're using django auth instead of authtools, you can just use
 # GenericUserProfileManager instead of having to make your own manager class
 class UserManager(GenericUserProfileManagerMixin, authtools.models.UserManager):
     pass
 
 class User(GenericUserProfile, authtools.models.AbstractEmailUser):
     objects = UserManager()
     profiles = UserManager(select_related_profiles=True)
-    
+
     # these are the tables that should be select_related()/prefetch_related()
     # to minimise queries
     related_profile_tables = [
         'customerprofile',
         'adminprofile',
     ]
-    
+
     # the default implementation will iterate through the related profile tables
     # and return the first profile it can find. If you have custom logic for
     # choosing the profile for a user then you can do that here
     #
     # You would normally not access this directly but instead use the`.profile`
     # property that caches the return value of `get_profile()` and works
-    # correctly for both user and profile records  
+    # correctly for both user and profile records
     def get_profile(self) -> Model:
         # custom logic
         if datetime.now() > datetime.date(2000,1,1):
             return self
         return super().get_profile()
 
 
@@ -559,15 +591,15 @@
 
 # we can explicitly perform the transform on the queryset
 profiles = list(User.objects.select_related_profiles().all())
 
 # joining to profile tables: 1 query
 # This assumes that RetailLocation.company.manager is a FK ref to the user table
 # The syntax is a bit different because we can't modify the query generation
-# in an unrelated table 
+# in an unrelated table
 qs = RetailLocation.objects.all()
 qs = User.objects.select_related_profiles(qs, 'company__manager')
 location_managers = list((loc, loc.company.manager.profile) for loc in qs.all())
 ```
 
 * There is also an authentication backend that will load profiles instead of just User records
 * If the `User` model has no `get_profile()` method then this backend is equivalent to the built-in django `django.contrib.auth.backends.ModelBackend`
@@ -579,60 +611,60 @@
 AUTHENTICATION_BACKENDS = [
     'allianceutils.auth.backends.ProfileModelBackend',
 ]
 
 
 def my_view(request):
     # standard django AuthenticationMiddleware will call the authentication backend
-    profile = request.user  
+    profile = request.user
     return HttpResponse('Current user is ' + profile.username)
 
 ```
 
 * Limitations:
     * Profile iteration does not work with `.values()` or `.values_list()`
-    
+
 #### raise_validation_errors
 
 * The `raise_validation_errors` context manager enables cleaner code for constructing validation
     * [Django documentation](https://docs.djangoproject.com/en/stable/ref/models/instances/#django.db.models.Model.clean) recommends raising a `ValidationError` when you encounter a problem
     * This creates a poor user experience if there are multiple errors: the user only sees the first error and has to resubmit a form multiple times to fix problems
 * `raise_validation_errors` accepts an (optional) function to wrap
     * The context manager returns a `ValidationError` subclass with an `add_error` function that follows the same rules as `django.forms.forms.BaseForm.add_error`
     * If the wrapped function raises a `ValidationError` then this will be merged into the `ValidationError` returned by the context manager
-    * If the wrapped function raises any other exception then this will not be intercepted and the context block will not be executed 
+    * If the wrapped function raises any other exception then this will not be intercepted and the context block will not be executed
     * At the end of a block,
         * If code in the context block raised an exception (including a `ValidationError`) then this will not be caught
-        * If `ValidationError` the context manager returned has any errors (either from `ve.add_error()` or from the wrapped function) then this will be raised 
+        * If `ValidationError` the context manager returned has any errors (either from `ve.add_error()` or from the wrapped function) then this will be raised
 
-```
+```python
     def clean(self):
         with allianceutils.models.raise_validation_errors(super().clean) as ve:
             if some_condition:
                 ve.add_error(None, 'model error message')
             if other_condition:
                 ve.add_error('fieldname', 'field-specific error message')
             if other_condition:
                 ve.add_error(None, {
                     'fieldname1': field-specific error message',
                     'fieldname2': field-specific error message',
                 })
             if something_bad:
-                raise RuntimeError('Oh no!') 
-            
+                raise RuntimeError('Oh no!')
+
             # at the end of the context, ve will be raised if it contains any errors
             #   - unless an exception was raised in the block (RuntimeError example above) in which case
             #     the raised exception will take precedence
 ```
 
 * Sometimes you already have functions that may raise a `ValidationError` and `add_error()` will not help
     * The `capture_validation_error()` context manager solves this problem
-    * Note that due to the way context managers work, each potential `ValidationError` needs its own with `capture_validation_error` context 
+    * Note that due to the way context managers work, each potential `ValidationError` needs its own with `capture_validation_error` context
 
-```
+```python
     def clean(self):
         with allianceutils.models.raise_validation_errors() as ve:
              with ve.capture_validation_error():
                  self.func1()
              with ve.capture_validation_error():
                  self.func2()
              with ve.capture_validation_error():
@@ -640,27 +672,27 @@
             # all raised ValidationErrors will be collected, merged and raised at the end of this block
 ```
 
 ### Rules
 
 * Utility functions that return predicates for use with [django-rules](https://github.com/dfunckt/django-rules)
 
-```
+```python
 from allianceutils.rules import has_any_perms, has_perms, has_perm
 
 # requires at least 1 listed permission
 rules.add_perm('northwind.publish_book', has_any_perms('northwind.is_book_author', 'northwind.is_book_editor'))
 
 # requires listed permission
 rules.add_perm('northwind.unpublish_book', has_perm('northwind.is_book_editor'))
 
 # requires all listed permissions
 rules.add_perm('northwind.sublicense_book', has_perms('northwind.is_book_editor', 'northwind.can_sign_contracts'))
 
-```  
+```
 
 ### Serializers
 
 #### JSON Ordered
 
 * A version of django's core json serializer that outputs field in sorted order
 * The built-in one uses a standard `dict` with completely unpredictable order which causes json diffs to show spurious changes
@@ -672,14 +704,127 @@
 
 ```python
 SERIALIZATION_MODULES = {
     'json_ordered': 'allianceutils.serializers.json_ordered',
 }
 ```
 
+### Template
+
+##### resolve
+
+* Resolves different types of kwarg values consistently.
+  * If value is a NodeList then it is rendered
+  * If value is a FilterExpression then it is resolved
+  * If value is a dict then each element is resolved if it is a FilterExpression, or else returned as is
+  * Otherwise value is returned as is
+
+
+* Example Usage
+```python
+    def resolved_kwargs(self, context: Context):
+        pk = resolve(self.pk, context)
+        model = resolve(self.model_name, context)
+        object = resolve(self.object, context)
+```
+
+##### token_kwargs
+
+* Re-implements the `token_kwargs` function from the Django base template library. This allows expanding the range of possible keywords to include '-' for aria attributes (e.g. `aria-label="My Label"`), and ':' for namespaced attributes (e.g. `xlink:href="foo"`). Used internally in [parse_tag_arguments](#parse_tag_arguments) - see that section for usage
+
+##### parse_tag_arguments
+
+* Implements a stripped-down version of `django.template.library.parse_bits()` to parse tokens passed to tags in Django templates.
+  * Takes the parser to process the tag, the token passed to the tag, and the kwarg `supports_as`
+  * Returns a tuple of `(args: list, kwargs: dict, target_var: str)`:
+    * args: a list of args as FilterExpressions
+    * kwargs: a dict of kwargs
+    * target_var: if `supports_as` is `True` and `as <variable>` is specified, returns the string reference for the tag. Otherwise returns `None`
+
+
+* Example Usage
+
+```python
+class StylesheetNode(template.Node, BundlerAsset):
+    def __init__(self, filename: Path, origin: Origin | None, attrs=None, target_var=None):
+        self.filename = filename
+        self.attrs = attrs
+        self.target_var = target_var
+        super().__init__(origin or Origin(UNKNOWN_SOURCE))
+
+    def render(self, context: Context):
+        if self.target_var:
+            context[self.target_var] = get_classes(self.filename)
+
+@register.tag("stylesheet")
+def stylesheet(parser: template.base.Parser, token: template.base.Token):
+    args, kwargs, target_var = parse_tag_arguments(parser, token, supports_as=True)
+    filename = args[0]
+    return StylesheetNode(filename, parser.origin, kwargs, target_var=target_var)
+```
+
+```html
+    {% stylesheet "./theme.css" as styles %}
+
+    <div class="{{ styles.section }}">
+        <h1 class="{{ styles.heading }}">My View</h1>
+        ...
+    </div>
+```
+
+##### build_html_attrs
+
+* Takes a dict of HTML tag attributes and transforms values into escaped strings suitable for use as HTML tag attributes. Can also pass a list of `prohibited_attrs` to prevent passing attributes which should not be passed to template tags.
+
+* Example Usage
+```python
+from django.utils.html import format_html
+...
+class LinkNode(template.Node):
+    def __init__(
+        self,
+        *,
+        href: FilterExpression | str | None = None,
+        **extra_kwargs,
+    ) -> None:
+        self.href = href
+
+    ...
+
+    def render(self, context: Context) -> SafeString:
+        href = resolve(self.href, context)
+        html_kwargs = { "href": href }
+        html_attrs = build_html_attrs(html_kwargs)
+        return format_html(
+            "<a {}>{}</a>",
+            html_attrs,
+        )
+```
+
+```html
+    {% link "/home" %}
+```
+
+##### is_static_expression
+
+* Checks if a given FilterExpression is static using the same method as Django's `resolve` implementation for the `Variable` class
+
+* Example Usage
+```python
+def validate_tag(parser, token):
+    tag_name = token.split_contents()[0]
+    args, _, _ = parse_tag_arguments(parser, token)
+
+    for arg in args:
+        if not is_static_expression(arg):
+            raise TemplateSyntaxError(
+                f"{tag_name} must be passed static strings for its arguments (encountered variable '{arg.var}')"
+            )
+```
+
 ### Template Tags
 
 #### render_entry_point
 
 * Replaces old usage of [django-webpack-loader](https://github.com/ezhome/django-webpack-loader)
    * At time of writing django-webpack-loader does not have a stable release that [works with webpack 4](https://github.com/owais/django-webpack-loader/issues/218)
    * Worked at bundle level rather than entry point. See below for how we embed tags based on entry point.
@@ -707,23 +852,23 @@
             "contentHash": "c78fb252d4e00207afef"
           }
         ]
       },
       "publicPath": "/assets/"
     }
    ```
-   
+
    Output for `{% render_entry_point 'admin' 'js' %}`:
 
    ```html
    <script type="text/javascript" src="/assets/runtime.bundle.js?e2b781da02d36dad3aff"></script>
    <script type="text/javascript" src="/assets/common.bundle.js?639269b921c8cf869c5f"></script>
    <script type="text/javascript" src="/assets/admin.bundle.js?c78fb252d4e00207afef"></script>
    ```
-   
+
    Output for `{% render_entry_point 'admin' 'css' %}`:
 
    ```html
    <link type="text/css" href="/assets/common.bundle.css?d60a0fa36613ea58a23d" rel="stylesheet" />
    ```
 * As an entry point maps to a single HTML file it's expected you would only use this tag for a single entry point on a page but generally would call it for both `js` and `css`
 * Arguments
@@ -744,51 +889,105 @@
 ```html
 {% load alliance_webpack %}
 <html>
 <head>
   {% render_entry_point 'app' 'css' %}
 </head>
 <body>
-  
+
   ...
-  
+
   {% if DEBUG %}
     {# See https://reactjs.org/docs/cross-origin-errors.html #}
     {% render_entry_point entry_point 'js' attrs="crossorigin" %}
   {% else %}
     {% render_entry_point entry_point 'js' %}
   {% endif %}
 </body>
 </html>
 ```
 
 #### default_value
 
 * Sets default value(s) on the context in a template
 * This is useful because some built-in django templates raise warnings about unset variables (eg `is_popup` in the django admin template)
-* Note that some tags (eg `with`) save & restore the context state; if done inside such a template tag `default_value` will not persist when the state is restored 
+* Note that some tags (eg `with`) save & restore the context state; if done inside such a template tag `default_value` will not persist when the state is restored
 
 ```html
 {% load default_value %}
 {{ default_value myvar1=99 myvar2=myvar1|upper }}
 {{ myvar1 }} {{ myvar2 }}
 ```
 
+### Tests
+
+##### suppress_silk
+
+* Decorator to disable silk SQL query logging.
+* This is needed for tests that use `assertNumQueries()` since otherwise the query count may include silk's `EXPLAIN`
+
+* Example Usage
+
+```python
+    @suppress_silk()
+    def test_lookup_object(self):
+        """Test that a query is run if object is not provided in template"""
+        user = self.get_privileged_user()
+        viewname = self.VIEW_KWARGS
+        view_kwargs = {"pk": user.pk}
+
+        request = HttpRequest()
+
+        # Without suppress_silk, an EXPLAIN query will be added
+        with self.assertNumQueries(1):
+            tpl = Template('{% load link %}{% link "' + viewname + '" pk=pk %}foo{% endlink %}')
+            tpl.render(Context({"request": request, "user": user, **view_kwargs}))
+```
+
+##### logging_filter
+
+* Decorator to disable logging for specified log names
+* This is useful because using `override_settings(LOGGING=...)` triggers an update to the python logging settings
+
+* Example Usage
+```python
+    @logging_filter(["django.request"])
+    def test_django_validation_errors(self):
+        url = reverse("django-validation-test-url")
+        for key, expect in EXPECTED_RESPONSES.items():
+            with self.subTest(key=key):
+                response = self.client.post(url, data={"error_key": key}, format="json")
+                self.assertEqual(400, response.status_code)
+                self.assertEqual(expect, response.json())
+```
+
+##### warning_filter
+
+* Apply a `warning.simplefilter()` for the specified warnings
+
+* Example Usage
+```python
+    @warning_filter("ignore", category=DeprecationWarning)
+    def test_relying_on_deprecated_feature(self):
+        instance = MyModel.objects.filter(deprecated_filter=True)
+        assertIsInstance(instance, MyModel)
+```
+
 ### Util
 
 #### add_autoreload_extra_files
 
 * Adds files to the autoreloader watch list
     * Works with both the built-in [`runserver`](https://docs.djangoproject.com/en/stable/ref/django-admin/#runserver)
       and [`runserver_plus`](https://django-extensions.readthedocs.io/en/latest/runserver_plus.html) from `django-extensions`
     * If `DEBUG` is not enabled then this will do nothing
     * This should be called from inside the
       [`ready()`](https://docs.djangoproject.com/en/stable/ref/applications/#django.apps.AppConfig.ready) method of
-      an [`AppConfig`](https://docs.djangoproject.com/en/stable/ref/applications/#configuring-applications) 
-  
+      an [`AppConfig`](https://docs.djangoproject.com/en/stable/ref/applications/#configuring-applications)
+
 ```python
 class MyAppConfig(AppConfig):
     def ready(self):
         extra_files = [
           "/data/file.csv",
         ]
         add_autoreload_extra_files(extra_files)
@@ -835,15 +1034,15 @@
 
 * `allianceutils.util.camelize(data, ignores)` - underscore case => camel case a json tree of data
 * `allianceutils.util.underscorize(data, ignores)` - camel case => underscore case a json tree of data
 * `allianceutils.util.camel_to_underscore(str)` - underscore case => camel case a string
 * `allianceutils.util.underscore_to_camel(str)` - camel case => underscore case a string
 * It is assumed that words will not begin with numbers:
     * `zoo_foo99_bar` is okay
-    * `zoo_foo_99bar` will result in an irreversible transformation (`zooFoo99bar` => `zoo_foo99_bar`) 
+    * `zoo_foo_99bar` will result in an irreversible transformation (`zooFoo99bar` => `zoo_foo99_bar`)
 
 #### get_firstparty_apps
 
 `util.get_firstparty_apps` can be used to retrieve app_configs considered to be first party, ie, all that does not come from a third party package.
 This is beneficial when you want to write your own checks by excluding things you dont really care - a sample usage can be found inside 'checks.py', or
 used as such:
 
@@ -891,27 +1090,27 @@
     super().save(*args, **kwargs)
 retry_fn(generate_number, (IntegrityError, ), 10)
 ```
 
 ## Experimental
 
 * These are experimental and may change without notice
-    * `document_reverse_accessors` management command  
+    * `document_reverse_accessors` management command
 
 ## Changelog
 
 See [CHANGELOG.md](CHANGELOG.md)
 
 ## Development
 
 * To create a clean local environment
-  * `python3 -m venv venv && source venv/bin/activate && pip install --upgrade pip` 
+  * `python3 -m venv venv && source venv/bin/activate && pip install --upgrade pip`
   * `poetry install --no-root --sync --only=main --extras=""`
   * Note that due to [a poetry bug](https://github.com/python-poetry/poetry/issues/7364) extras are currently not removed
-  * This will install the latest django version; if you want to test a specific django version you need to `pip install` it manually 
+  * This will install the latest django version; if you want to test a specific django version you need to `pip install` it manually
 * Dev dependencies
   * `poetry install --no-root --sync --with=dev --extras "extras mysql postgres"`
 
 ### Release Process
 
 #### Poetry Config
 * Add test repository
@@ -923,47 +1122,32 @@
     * Generate an account API token at https://pypi.org/manage/account/token/
     * `poetry config pypi-token.pypi ${TOKEN}`
         * On macs this will be stored in the `login` keychain at `poetry-repository-pypi`
 
 #### Publishing a New Release
     * Update CHANGELOG.md with details of changes and new version
     * Run `bin/build.py`. This will extract version from CHANGELOG.md, bump version in `pyproject.toml` and generate a build for publishing
+    * Commit version bumps
     * Tag with new version and update the version branch:
         * `ver=$( poetry version --short ) && echo "Version: $ver"`
         * `git tag v/$ver`
         * `git push --tags`
     * To publish to test.pypi.org
         * `poetry publish --repository testpypi`
     * To publish to pypi.org
         * `poetry publish`
 
 
 ### Testing
 * To run test cases
   * The django settings module is `test_allianceutils/settings.py`
-    * The following env vars are optional but you may want to set them if the default don't match your local setup: 
+    * The following env vars are optional but you may want to set them if the default don't match your local setup:
       * `DB_NAME`
       * `DB_HOST`
       * `DB_PORT`
       * `DB_USER`
       * `DB_PASSWORD`
 * [tox](https://tox.wiki/en/latest/)
   * used to run tests against different django/python/database versions
   * `tox` to run all tests. Will require that you have a postgres & mysql server running.
-    * `tox -f django42` will run the subset of tests that cover django 4.2. Check `tox.ini` for the list of tested environments. 
-* When you push to github a [github Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python) workflow will be triggered (see `.github/workflows/django.yml`)  
-
-
-
-TODO:
-- [x] mypy checks all pass
-- [x] github actions pass
-- [] stricter mypy settings?
-- [] flake8, black, isort
-- [x] can cachetools replace @method_cache?
-  - No; can use methodtools but is another dependency. just documented the alternative 
-- [x] Use collections.abc:
-  - no, doesn't work with 3.8
-- [x] Use | instead of Optional, Union
-  - no, doesn't work with 3.8
-- [] Remove legacy build settings (poetry shouldn't need setup.cfg, MANIFEST.in so can we remove them?)
- 
+    * `tox -f django42` will run the subset of tests that cover django 4.2. Check `tox.ini` for the list of tested environments.
+* When you push to github a [github Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python) workflow will be triggered (see `.github/workflows/django.yml`)
```

### Comparing `django_allianceutils-3.0.0/pyproject.toml` & `django_allianceutils-4.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "django-allianceutils"
-version = "3.0.0"
+version = "4.0.0"
 description = "Alliance Software common utilities for Django"
 repository = "https://github.com/AllianceSoftware/django-allianceutils/"
 homepage = "https://github.com/AllianceSoftware/django-allianceutils/"
 documentation = "https://github.com/AllianceSoftware/django-allianceutils/blob/master/README.md"
 authors = ["Alliance Software <support@alliancesoftware.com.au>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 packages = [
     { include = "allianceutils", from = "src" },
 ]
 include = [
     "CHANGELOG.md",
-	"LICENSE",
+    "LICENSE",
     "src/allianceutils/py.typed",
 ]
 keywords = [
     "django",
     'alliance',
     'alliancesoftware',
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -46,57 +46,53 @@
 # you need the <4.0 for cachetools which is a tox dependency
 python = ">=3.8,<4.0"
 
 # the only hard dependency is django; everything else is only required
 # if you use functions/classes that require them
 #
 # IMPORTANT
-# We need to specify a minimum django version that this package requires, but
-#   this means that when poetry creates a lock file that it will pick the latest
-#   version available
-# For development purposes we will override this in tox to install a specific
-#   version
+# We test multiple django versions, so these appear under `deps` in tox.ini
+# and aren't listed here at all. Other deps are installed from the poetry
+# lockfile based on what is listed here.
+
 # It's not possible to natively get poetry to use a different version for dev
 #   via groups or extras because it only resolves dependencies once (globally)
 #   see https://github.com/python-poetry/poetry/issues/6611
-Django = ">=3.2"
+
 typing_extensions = "^4.5.0"
 
 # optional extras
-django-filter = { version = "*", optional = true }
-django-storages = { version = "*", optional = true }
-djangorestframework = { version = "*", optional = true }
 isort = { version = ">=5", optional = true }
 logging_tree = { version = "*", optional = true }
 rules = { version = "*", optional = true }
 
 # optional databases
 mysqlclient = { version = "*", optional = true }
 psycopg2 = { version = "*", optional = true }
 
-
 [tool.poetry.extras]
 extras = [
-	"django-filter",
-	"django-storages",
-	"djangorestframework",
-	"isort",
-	"logging_tree",
-	"rules",
+    "isort",
+    "logging_tree",
+    "rules",
 ]
 mysql = ["mysqlclient"]
 postgres = ["psycopg2"]
 
+[tool.poetry.group.databases.dependencies]
+mysqlclient = "*"
+psycopg2 = "*"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 isort = ">=5"
 tox = ">=4"
+tox-poetry-installer = {extras = ["poetry"], version = "^1.0.0b1", allow-prereleases = true}
 
 mypy = ">=1.3"
 django-filter-stubs = "*"
 django-stubs = "*"
 djangorestframework-stubs = "*"
 types-mysqlclient = "*"
 types-psycopg2 = "*"
@@ -112,38 +108,38 @@
 # ===================================================================================================================
 [tool.isort]
 force_single_line = true
 force_sort_within_sections = true
 line_length = 110
 order_by_type = false
 skip_glob = [
-	"*/.tox/*",
-	"*/node_modules/*.py",
-	"*/migrations/0*.py",
-	"*/settings/*.py",
+    "*/.tox/*",
+    "*/node_modules/*.py",
+    "*/migrations/0*.py",
+    "*/settings/*.py",
 ]
 # stdlib that may be backported or not always there
 extra_standard_library=[
-	"pkg_resources",
-	"setuptools",
-	"typing",
+    "pkg_resources",
+    "setuptools",
+    "typing",
 ]
 
 # packages that we may have made local modifications to or are checked out from github
 # IsortTestCase has expectations about what is set here:
 known_third_party=["test_allianceutils.tests.isort_force_thirdparty"]
 #known_first_party=["allianceutils"]
 
 # ===================================================================================================================
 
 [tool.mypy]
 python_version = "3.8"
 plugins = [
-	"mypy_django_plugin.main",
-	"mypy_drf_plugin.main",
+    "mypy_django_plugin.main",
+    "mypy_drf_plugin.main",
 ]
 #exclude = ['/migrations/', 'bin/', 'venv/', '/tests/']
 # mypy_path is needed because mypy won't look for config in ancestor dirs:
 #  https://github.com/python/mypy/issues/3377#issuecomment-302308046
 mypy_path = '$MYPY_CONFIG_FILE_DIR/src'
 # default files to check if none given on command line
 files = '$MYPY_CONFIG_FILE_DIR/src/**/*.py'
@@ -200,8 +196,8 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "rules"
 ignore_missing_imports = true
 
 [tool.django-stubs]
-django_settings_module = "test_allianceutils.settings"
+django_settings_module = "test_allianceutils.settings"
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/__init__.py` & `django_allianceutils-4.0.0/src/allianceutils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import _ProtocolMeta
 from typing import TYPE_CHECKING
 import unittest
 
 from django.db.models.base import ModelBase
 
-__version__ = "3.0.0"
+__version__ = "4.0.0"
 
 
 # All the tests are in test_allianceutils
 # Django's test autodiscovery will try to recursively import everything which causes asynctask to fail if we're running
 # mysql tests
 def load_tests(*args, **kwargs):
     empty_suite = unittest.TestSuite()
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/api/mixins.py` & `django_allianceutils-4.0.0/src/allianceutils/api/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 from typing import Collection
+from typing import Dict
+from typing import List
 from typing import Protocol
 from typing import TYPE_CHECKING
 
 from django.db.models import Field as ModelField
 from django.db.models.options import Options
 from rest_framework.fields import Field
 from rest_framework.serializers import ModelSerializer
 
 if TYPE_CHECKING:
     # ModelSerializer.Meta is only available in DRF stubs
     class DRFSerializerProtocol(Protocol):
         Meta: ModelSerializer.Meta
-        fields: dict[str, Field]
+        fields: Dict[str, Field]
 
         # this is provided by SerializerOptInFieldsMixin
         def get_pinned_fields(self: DRFSerializerProtocol) -> Collection[str]:
             ...
 
 else:
     class DRFSerializerProtocol:
@@ -83,15 +85,15 @@
             or ("include_fields" in self.context and self.context["include_fields"])
             or set(self.Meta.fields).difference(set(fields_to_exclude))
         )
 
         if isinstance(fields_to_include, str):
             fields_to_include = [fields_to_include]
 
-        fields_to_include_list: list[str] = []
+        fields_to_include_list: List[str] = []
         for f in fields_to_include:
             if f.find(",") != -1:
                 fields_to_include_list += f.split(",")
             else:
                 fields_to_include_list.append(f)
 
         opt_in_fields_to_include = (
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/api/parsers.py` & `django_allianceutils-4.0.0/src/allianceutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/api/permissions.py` & `django_allianceutils-4.0.0/src/allianceutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/api/renderers.py` & `django_allianceutils-4.0.0/src/allianceutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/auth/backends.py` & `django_allianceutils-4.0.0/src/allianceutils/auth/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class ProfileModelBackendMixin:
     """
     Backend that provides authentication using User.profiles & get_profile().
     Will fall back to default get_user() behaviour if no profiles manager available
     """
 
-    def get_user(self: _BaseUserModelBackend, user_id) -> GenericUserProfile | None:
+    def get_user(self: _BaseUserModelBackend, user_id) -> Optional[GenericUserProfile]:
         try:
             manager = UserModel.profiles
         except AttributeError:
             return super().get_user(user_id)
 
         try:
             user = manager.get(pk=user_id)
@@ -68,8 +68,8 @@
 
     def has_perm(self, user: _BaseUserModel, perm: str, obj: Optional[Model] = None) -> bool:
         """
         We defer to other backends for the real logic
         """
         if user.is_superuser:
             return True
-        return False
+        return False
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/auth/models.py` & `django_allianceutils-4.0.0/src/allianceutils/auth/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 from typing import cast
 from typing import Iterable
+from typing import List
+from typing import Optional
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
+from typing import Union
 
 from django.contrib.auth.models import BaseUserManager
 from django.contrib.auth.models import UserManager
 from django.core import checks
 from django.core.exceptions import ValidationError
 from django.db.models import EmailField
 from django.db.models import Field
@@ -26,15 +29,15 @@
 class GenericUserProfileIterable(ModelIterable):
     """
     The iterator that transforms user records into profiles
     """
 
     queryset: GenericUserProfileQuerySet  # this is coupled to this QuerySet
 
-    def __iter__(self) -> Iterable[GenericUserProfile | _ModelT]:  # type:ignore[override]  # specialised return
+    def __iter__(self) -> Iterable[Union[GenericUserProfile, _ModelT]]:  # type:ignore[override]  # specialised return
         if self.queryset._do_iterate_profiles:
             for user in super().__iter__():
                 yield user.profile
         else:
             yield from super().__iter__()
 
 
@@ -87,15 +90,15 @@
             raise ValueError('Bad _iterable_class. (Trying to use values()/values_list() with profiles()? This has not been implemented yet)')
 
     def _clone(self, **kwargs):
         qs = super()._clone(**kwargs)  # type:ignore[misc]  # not in django stubs
         qs._do_iterate_profiles = self._do_iterate_profiles
         return qs
 
-    def _get_related_profile_tables(self) -> list[str]:
+    def _get_related_profile_tables(self) -> List[str]:
         """
         See GenericUserProfile.related_profile_tables
         """
         if _is_profile(self.model):
             return []
         else:
             return self.model.related_profile_tables
@@ -229,29 +232,29 @@
     # unfortunately the code to do the joins is baked into SQLCompiler.get_related_selections() and is not really
     # extensible without being very invasive
     #
     # Instead we have to call select_related_profiles on an unrelated queryset with a prefix
 
     def select_related_profiles(
         self,
-        queryset: GenericUserProfileQuerySet | GenericUserProfileManagerMixin | None = None,
+        queryset: Optional[Union[GenericUserProfileQuerySet, GenericUserProfileManagerMixin]] = None,
         prefix: str = ""
     ) -> GenericUserProfileQuerySet:
         if bool(queryset) != bool(prefix):
             raise ValueError('Either none or both of queryset and prefix must be specified')
 
         if queryset is None:
             return self.get_queryset().select_related_profiles()
         else:
             filters = [prefix + '__' + profile for profile in self.model.related_profile_tables]
             return cast(GenericUserProfileQuerySet, queryset.select_related(*filters))
 
     def prefetch_related_profiles(
         self,
-        queryset: GenericUserProfileQuerySet | GenericUserProfileManagerMixin | None = None,
+        queryset: Optional[Union[GenericUserProfileQuerySet, GenericUserProfileManagerMixin]] = None,
         prefix: str = ""
     ) -> GenericUserProfileQuerySet:
         if bool(queryset) != bool(prefix):
             raise ValueError('Either none or both of queryset and prefix must be specified')
 
         if queryset is None:
             return self.get_queryset().prefetch_related_profiles()
@@ -273,15 +276,15 @@
     You should override related_profile_tables
     """
     objects = GenericUserProfileManager()
     profiles = GenericUserProfileManager(select_related_profiles=True)
 
     # This should be overridden to include a list of the FKs to the tables
     # to join to in order to fetch profiles [will be passed to select_related()]
-    related_profile_tables: list[str]
+    related_profile_tables: List[str]
 
     class Meta:
         abstract = True
 
     def get_profile(self) -> Self:
         # We're already a profile
         if _is_profile(type(self)):
@@ -301,25 +304,25 @@
     class _CachedProfileDescriptor:
         """
         Evaluates and caches the result of get_profile()
         Caches the result on all records in the multi-table inheritance chain
         """
         def __get__(
             self,
-            obj: GenericUserProfile | None,
-            cls: type[GenericUserProfile] | None = None
-        ) -> Self | GenericUserProfile:
+            obj: Optional[GenericUserProfile],
+            cls: Optional[type[GenericUserProfile]] = None
+        ) -> Union[Self, GenericUserProfile]:
             if obj is None:
                 # class invocation
                 return self
 
             user_profile = obj.get_profile()
 
             # cache the result on all records in the multi-table inheritance chain
-            record: GenericUserProfile | None = user_profile
+            record: Optional[GenericUserProfile] = user_profile
             while isinstance(record, Model):
                 record.__dict__['profile'] = user_profile
 
                 # note that record.pk will always return the underlying pk id, not the user_ptr record
                 # so we have to access it via the pk field's name and not the 'pk' alias
                 pk = cast(Field, record._meta.pk)
                 record = getattr(record, pk.name)
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/bin/internaldeps.sh` & `django_allianceutils-4.0.0/src/allianceutils/bin/internaldeps.sh`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/checks.py` & `django_allianceutils-4.0.0/src/allianceutils/checks.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import defaultdict
 import inspect
 from pathlib import Path
 import re
 import subprocess
 from typing import cast
 from typing import Collection
+from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Mapping
 from typing import Optional
 from typing import Type
 from typing import Union
 
@@ -47,15 +48,15 @@
 ID_INFO_EXPLICIT_TABLE_NAME_LOWERCASE = 'allianceutils.I010'
 ID_ERROR_FIELD_NAME_NOT_CAMEL_FRIENDLY = 'allianceutils.E011'
 
 
 def find_candidate_models(
     app_configs: Optional[Iterable[AppConfig]],
     ignore_labels: Optional[Iterable[Union[str, re.Pattern]]] = None
-) -> dict[str, Type[Model]]:
+) -> Dict[str, Type[Model]]:
     """
     Given a list of labels to ignore, return models whose app_label or label is NOT in ignore_labels.
     :return: dict which is a mapping of candidate models in the format of { model_label: Model }
     """
     if app_configs is None:
         app_configs = get_firstparty_apps()
 
@@ -67,54 +68,54 @@
         return (
             # string match
             any(s == label for s in ignore_labels) or
             # regex pattern match
             any(p.match(label) for p in ignore_labels if hasattr(p, "match"))
         )
 
-    candidate_models: dict[str, Type[Model]] = {}
+    candidate_models: Dict[str, Type[Model]] = {}
 
     for app_config in app_configs:
         candidate_models.update({
             model._meta.label: model
             for model
             in app_config.get_models()
             if not should_ignore(model._meta.app_label) and not should_ignore(model._meta.label)
         })
 
     return candidate_models
 
 
 class CheckUrlTrailingSlash:
     expect_trailing_slash: bool
-    ignore_attrs: dict[str, Collection[str]]
+    ignore_attrs: Dict[str, Collection[str]]
 
     def __init__(self, expect_trailing_slash: bool, ignore_attrs: Mapping[str, Collection[str]] = {}):
         self.expect_trailing_slash = expect_trailing_slash
         self.ignore_attrs = dict(ignore_attrs.items())
 
-    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> list[CheckMessage]:
+    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
         # We ignore app_configs; so does django core check_url_settings()
         # Consider where ROOT_URLCONF points app A urlpatterns which include() app B urlpatterns
         # which define a URL to view in app C -- which app was the one that owned the URL?
-        _ignore_attrs: dict[str, Collection[str]] = {
+        _ignore_attrs: Dict[str, Collection[str]] = {
             '_regex': [
                 '^$',
             ],
             'lookup_str': [
                 'django.views.static.serve',
             ],
             'app_name': [
                 'admin',
                 'djdt',
             ],
         }
         _ignore_attrs.update(self.ignore_attrs)
 
-        def check_resolver(resolver: URLResolver, depth: int = 0) -> list[CheckMessage]:
+        def check_resolver(resolver: URLResolver, depth: int = 0) -> List[CheckMessage]:
             messages = []
             for url_pattern in resolver.url_patterns:
 
                 if any(
                     getattr(url_pattern, attr, None) in vals
                         or getattr(getattr(url_pattern, 'pattern', {}), attr, None) in vals
                     for attr, vals
@@ -160,28 +161,28 @@
 
 def get_default_git_path() -> Path:
     assert hasattr(settings, "PROJECT_DIR")
     project_dir = settings.PROJECT_DIR  # type:ignore[misc]  # we already checked that this is present
     return Path(project_dir, '.git')
 
 
-def check_git_hooks(app_configs: Iterable[AppConfig], **kwargs) -> list[CheckMessage]:
+def check_git_hooks(app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
     return _check_git_hooks(app_configs, git_path=get_default_git_path(), **kwargs)
 
 
-def _check_git_hooks(app_configs: Iterable[AppConfig], git_path: Path, **kwargs) -> list[CheckMessage]:
+def _check_git_hooks(app_configs: Iterable[AppConfig], git_path: Path, **kwargs) -> List[CheckMessage]:
 
     # handle the case where .git is a file rather than a directory
     try:
         with git_path.open() as f:
             git_path = Path(f.readline())
     except OSError:
         pass
 
-    messages: list[CheckMessage] = []
+    messages: List[CheckMessage] = []
 
     if not git_path.exists():
         if settings.DEBUG:
             # If in dev mode then there should be a .git dir
             messages.append(
                 Warning(
                     "DEBUG is true but can't find a .git dir; are you trying to use DEBUG in production?",
@@ -236,35 +237,35 @@
                     id=warning_id,
                 )
             )
 
     return messages
 
 
-def check_admins(app_configs: Iterable[AppConfig] | None, **kwargs) -> list[CheckMessage]:
-    messages: list[CheckMessage] = []
+def check_admins(app_configs: Optional[Iterable[AppConfig]], **kwargs) -> List[CheckMessage]:
+    messages: List[CheckMessage] = []
     if not getattr(settings, "AUTOMATED_TESTS", False) and not settings.DEBUG:
         if len(settings.ADMINS) == 0:
             messages.append(
                 Error(
                     "settings.ADMINS should not be empty",
                     obj='settings',
                     id=ID_ERROR_ADMINS,
                 )
             )
     return messages
 
 
-def _check_explicit_table_names_on_model(model: Type[Model], enforce_lowercase: bool) -> list[CheckMessage]:
+def _check_explicit_table_names_on_model(model: Type[Model], enforce_lowercase: bool) -> List[CheckMessage]:
     """
     Use an ast to check if a model has the db_table meta option set.
     This is done this way because a model instance's db_table is always
     populated even if with that of the default.
     """
-    messages: list[CheckMessage] = []
+    messages: List[CheckMessage] = []
     found = None
     try:
         source = inspect.getsource(model)
     except OSError:
         # if a model class is dynamically created then we can't inspect the source code
         # (eg this happens with audit models)
         message = f"Can't get source for {model.__name__}"
@@ -338,15 +339,15 @@
         """
         ignore_labels: ignore apps or models matching supplied labels
         enforce_lowercase: applies rule E010 which enforces table name to be all lowercase; defaults to True
         """
         self.ignore_labels = ignore_labels
         self.enforce_lowercase = enforce_lowercase
 
-    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> list[CheckMessage]:
+    def __call__(self, app_configs: Iterable[AppConfig], **kwargs) -> List[CheckMessage]:
         """
         Warn when models don't have Meta's db_table_name set in apps that require it.
         """
         candidate_models = find_candidate_models(app_configs, self.ignore_labels)
 
         messages = []
         for model in candidate_models.values():
@@ -363,25 +364,25 @@
     def __call__(self, app_configs: Iterable[AppConfig], ** kwargs):
         candidate_models = find_candidate_models(app_configs, self.ignore_labels)
         errors = []
         for model in candidate_models.values():
             errors += self._check_field_names_on_model(model)
         return errors
 
-    def _check_field_names_on_model(self, model: Type[Model]) -> list[CheckMessage]:
+    def _check_field_names_on_model(self, model: Type[Model]) -> List[CheckMessage]:
         """
         check whether field names on model are legit
 
         currently contains only one check:
         1. checks whether field name contains any number preceded by an underscore. the underscore will be lost when
            camelized then de-camelized again. Since camelize is performed automatically to/from frontend it leads to bugs.
 
         """
 
-        messages: list[CheckMessage] = []
+        messages: List[CheckMessage] = []
 
         for field in model._meta.fields:
             if camel_to_underscore(underscore_to_camel(field.name)) != field.name:
                 hint = None
                 if re.search(r'_[0-9]', field.name):
                     hint = f'Underscore before a number in {model._meta.label}.{field.name}'
                 messages.append(
@@ -389,8 +390,8 @@
                         "Field name is not reversible with underscore_to_camel()/camel_to_underscore()",
                         hint=hint,
                         obj=model,
                         id=ID_ERROR_FIELD_NAME_NOT_CAMEL_FRIENDLY,
                     )
                 )
 
-        return messages
+        return messages
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/decorators.py` & `django_allianceutils-4.0.0/src/allianceutils/decorators.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/management/commands/base.py` & `django_allianceutils-4.0.0/src/allianceutils/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/management/commands/document_reverse_accessors.py` & `django_allianceutils-4.0.0/src/allianceutils/management/commands/document_reverse_accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         output = self.generate_comments(source_file_model_fields)
 
         if options['preview']:
             self.preview_output(output)
         else:
             self.apply_output(output)
 
-    def determine_fields_by_model_by_file(self, models: Iterable[type[Model]]) -> Dict[str, Dict[type[Model], list[ForeignObjectRel]]]:
+    def determine_fields_by_model_by_file(self, models: Iterable[type[Model]]) -> Dict[str, Dict[type[Model], List[ForeignObjectRel]]]:
         """
         Takes a list of models and returns the models & fields for each source file
         :param: models[] - look up the source file & fields for these models
         :returns: { source_file: { Model: [ Field ] } }
         """
         related_fields = [
             field
@@ -56,15 +56,15 @@
             model: list(model_fields)
             for model, model_fields
             in groupby(sorted(related_fields, key=lambda f: f.model.__name__), key=lambda f: f.model)
         }
 
         get_model_source = cast(Callable[[type], str], inspect.getsourcefile)
         models_sorted_by_source = sorted(model_fields.keys(), key=get_model_source)
-        source_file_models: dict[str, list[type[Model]]] = {
+        source_file_models: Dict[str, List[type[Model]]] = {
             source_file: list(models)
             for source_file, models
             in groupby(models_sorted_by_source, key=get_model_source)
         }
 
         source_file_model_fields = {
             source_file: {
@@ -73,15 +73,15 @@
                 in models
             }
             for source_file, models
             in source_file_models.items()
         }
         return source_file_model_fields
 
-    def generate_comments(self, fields_by_model_by_source_file: Dict[str, Dict[type[Model], list[ForeignObjectRel]]]) -> Dict[str, List[str]]:
+    def generate_comments(self, fields_by_model_by_source_file: Dict[str, Dict[type[Model], List[ForeignObjectRel]]]) -> Dict[str, List[str]]:
         """
         takes in a dict of fields in the format returned by determine_fields_by_model_by_file
         spits out { source_file: [ lines_with_comments ] }, where lines_with_comments are consisted of
         original code (without any reverse accessor comments) + added reverse accessor comments.
         """
         output = {}
         for source_file, fields_by_model in fields_by_model_by_source_file.items():
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/management/commands/print_logging.py` & `django_allianceutils-4.0.0/src/allianceutils/management/commands/print_logging.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/middleware/current_user.py` & `django_allianceutils-4.0.0/src/allianceutils/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/middleware/http_auth.py` & `django_allianceutils-4.0.0/src/allianceutils/middleware/http_auth.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/middleware/query_count.py` & `django_allianceutils-4.0.0/src/allianceutils/middleware/query_count.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/migrations.py` & `django_allianceutils-4.0.0/src/allianceutils/migrations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any
+from typing import Dict
 from typing import Sequence
+from typing import Tuple
 from typing import Union
 
 from django.apps import apps
 from django.db.migrations import RunSQL
 
 
 class RunSQLFromFile(RunSQL):
@@ -18,26 +20,26 @@
     The reason you would do this as an external file & function is so that squashed migrations don't become
     unreadable (the squash process will inline and strip whitespace in the SQL even for large data files)
     """
 
     app_name: str
     filename: Path
 
-    def __init__(self, *, app_name: str, filename: str | Path, **kwargs):
+    def __init__(self, *, app_name: str, filename: Union[str, Path], **kwargs):
         self.app_name = app_name
         self.filename = Path(filename)
         if self.filename.is_absolute():
             raise ValueError("filename should be relative to app's migrations directory")
 
         super().__init__(
             sql="",
             reverse_sql=None,
             **kwargs)
 
-    def deconstruct(self) -> tuple[str, Sequence[Any], dict[str, Any]]:
+    def deconstruct(self) -> Tuple[str, Sequence[Any], Dict[str, Any]]:
         path, args, kwargs = super().deconstruct()
         del kwargs["sql"]
         del kwargs["reverse_sql"]
         kwargs["app_name"] = self.app_name
         kwargs["filename"] = str(self.filename)
         return path, args, kwargs
 
@@ -46,8 +48,8 @@
 
     def _run_sql(self, schema_editor, sqls):
         path = Path(apps.get_app_config(self.app_name).path, 'migrations', self.filename)
         sql = path.read_text()
         super()._run_sql(schema_editor, sqls)  # type:ignore[misc] # underscore methods are hidden
 
 
-# TODO: add test cases for this
+# TODO: add test cases for this
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/models.py` & `django_allianceutils-4.0.0/src/allianceutils/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     def __init__(self, message: ExtendedErrorT, *args, **kwargs):
         if message is None:
             message = []
         super().__init__(message, *args, *kwargs)
 
     def add_error(
         self,
-        field: str | None,
+        field: Optional[str],
         error: ExtendedErrorT,
     ):
         """
         This has the same behaviour as BaseForm.add_error()
         """
         if error is None:
             return
@@ -168,15 +168,15 @@
         # [3] scalar: self.message is a single message & self.error_list == [self]
 
         # list of validation errors to merge
         to_merge = [self, errors]
 
         # we need to promote one or more both to a dict-type ValidationError
         if any(hasattr(ve, 'error_dict') for ve in to_merge):
-            to_merge_dicts: list[ErrorDictT] = []
+            to_merge_dicts: List[ErrorDictT] = []
             for ve in to_merge:
                 if not hasattr(ve, 'error_dict'):
                     ve_list: ErrorListT = [x for x in ve.error_list if not is_empty(x)]
                     if ve_list:
                         to_merge_dicts.append({NON_FIELD_ERRORS: ve_list})
                 else:
                     # cast() needed because list is invariant
@@ -191,15 +191,15 @@
                     error_list = cast(list, merged_dict[key])
                     copied_value: ErrorT
                     # there's an assumption here that a promise is only wrapping a str and
                     # not a mutable structure like a dict or list
                     if isinstance(value, (str, Promise)):
                         copied_value = value
                     else:
-                        copied_value = value.copy() # cast(ErrorListT | ErrorDictT, value).copy()
+                        copied_value = value.copy() # cast(Union[ErrorListT, ErrorDictT], value).copy()
                     error_list.extend(copied_value)
 
             new_ve = _ExtendedValidationError(merged_dict)
         else:
             codes = []
             params = []
             to_merge_messages = []
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/rules.py` & `django_allianceutils-4.0.0/src/allianceutils/rules.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/serializers/json_ordered.py` & `django_allianceutils-4.0.0/src/allianceutils/serializers/json_ordered.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/templatetags/alliance_webpack.py` & `django_allianceutils-4.0.0/src/allianceutils/templatetags/alliance_webpack.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/templatetags/default_value.py` & `django_allianceutils-4.0.0/src/allianceutils/templatetags/default_value.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/util/__init__.py` & `django_allianceutils-4.0.0/src/allianceutils/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Callable
 from typing import Iterable
+from typing import Optional
 from typing import Tuple
 from typing import Union
 
 from django.conf import settings
 from django.utils.autoreload import autoreload_started
 from django.utils.autoreload import StatReloader
 
@@ -42,15 +43,15 @@
                 raise
 
 
 def add_autoreload_extra_files(extra_files: Iterable[Union[str, Path]]):
     if not settings.DEBUG:
         return
 
-    is_running_from_reloader: Callable[[], bool] | None
+    is_running_from_reloader: Optional[Callable[[], bool]]
     try:
        from werkzeug.serving import is_running_from_reloader
     except ImportError:
         is_running_from_reloader = None
 
     if is_running_from_reloader and is_running_from_reloader():
         # we're running from the main runserver_plus process
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/util/camel_case.py` & `django_allianceutils-4.0.0/src/allianceutils/util/camel_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import OrderedDict
 import re
 from typing import Any
 from typing import Callable
 from typing import cast
 from typing import Dict
 from typing import Iterable
+from typing import List
 from typing import Literal
 from typing import Mapping
 from typing import Sequence
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
 
@@ -22,30 +23,30 @@
 
 _first_cap_re = re.compile('(.)([A-Z][a-z]+)')
 _all_cap_re = re.compile('([a-z0-9])([A-Z])')
 _re_underscore = re.compile(r'(?!^)(?<!_)_([^_])')
 
 """
 a sequence of fields to ignore when camelizing
-# see camelize()/underscorize() 
+# see camelize()/underscorize()
 """
 IgnoreSpecifier = Iterable[str]
 
 # Internal structure: see _create_ignore_lookup() for usage
 # Exposed only for typing purposes; treat this as an opaque type
 IgnoreDict: TypeAlias = Dict[Union[str, None], Union["IgnoreDict", Literal[True]]]
 
 _empty_dict: IgnoreDict = {} # we use this a lot in here
 
 
 # a generic type that can be camelized/underscorized
 CamelizeT = TypeVar('CamelizeT')
 
 
-def _debug_lookup(ignore_tree: IgnoreDict, indent: int = 0) -> list[str]:
+def _debug_lookup(ignore_tree: IgnoreDict, indent: int = 0) -> List[str]:
     """
     Format a tree processed by _transform_ignore() into something human-readable (for debugging/testing purposes)
     """
     x = []
     for sort_key, key, children in sorted([(key or '', key, val) for key, val in ignore_tree.items()]):
         if key is None:
             continue
@@ -103,26 +104,26 @@
         - * is a wildcard indicator
     TODO: In future if we allow pre-split paths then we might relax some of these constraints
 
     :param ignore: list of field paths to ignore
     :return: See above
     """
 
-    def process_path(parts: Sequence[str], candidates: list[IgnoreDict]):
+    def process_path(parts: Sequence[str], candidates: List[IgnoreDict]):
         """
         Breadth-first transform of the tree; will merge `parts` into the sub-tree(s) specified by `candidates`
 
         :param parts: list of field path parts (ie already split on '.') relative to candidates
         :param candidates: list of current candidate sub-trees to process
         """
         while len(parts):
             part = parts[0]
             assert part != ''
 
-            new_candidates: list[IgnoreDict] = []
+            new_candidates: List[IgnoreDict] = []
 
             for candidate in candidates:
                 if part not in candidate:
                     candidate[part] = {}
 
                 if len(parts) > 1:
                     if part == '*':
@@ -149,15 +150,15 @@
     data: IgnoreDict = {}
     for parts in ignore_parts:
         process_path(parts, [data])
     return data
 
 
 def _transform_key_val(
-    key: str | Promise,
+    key: Union[str, Promise],
     value: CamelizeT,
     transform_key: Callable,
     ignore_lookup: Dict
 ) -> Tuple[str, CamelizeT]:
     """
     Transform a particular key/value pair
     - Will rename the key if it's not in the ignore_lookup
```

### Comparing `django_allianceutils-3.0.0/src/allianceutils/util/date.py` & `django_allianceutils-4.0.0/src/allianceutils/util/date.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/util/get_firstparty_apps.py` & `django_allianceutils-4.0.0/src/allianceutils/util/get_firstparty_apps.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/views/decorators.py` & `django_allianceutils-4.0.0/src/allianceutils/views/decorators.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/src/allianceutils/webpack.py` & `django_allianceutils-4.0.0/src/allianceutils/webpack.py`

 * *Files identical despite different names*

### Comparing `django_allianceutils-3.0.0/PKG-INFO` & `django_allianceutils-4.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 Metadata-Version: 2.1
 Name: django-allianceutils
-Version: 3.0.0
+Version: 4.0.0
 Summary: Alliance Software common utilities for Django
 Home-page: https://github.com/AllianceSoftware/django-allianceutils/
 License: BSD-2-Clause
 Keywords: django,alliance,alliancesoftware
 Author: Alliance Software
 Author-email: support@alliancesoftware.com.au
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Provides-Extra: extras
 Provides-Extra: mysql
 Provides-Extra: postgres
-Requires-Dist: Django (>=3.2)
-Requires-Dist: django-filter ; extra == "extras"
-Requires-Dist: django-storages ; extra == "extras"
-Requires-Dist: djangorestframework ; extra == "extras"
 Requires-Dist: isort (>=5) ; extra == "extras"
 Requires-Dist: logging_tree ; extra == "extras"
 Requires-Dist: mysqlclient ; extra == "mysql"
 Requires-Dist: psycopg2 ; extra == "postgres"
 Requires-Dist: rules ; extra == "extras"
 Requires-Dist: typing_extensions (>=4.5.0,<5.0.0)
 Project-URL: Documentation, https://github.com/AllianceSoftware/django-allianceutils/blob/master/README.md
@@ -57,25 +54,27 @@
         * [Commands](#commands)
         * [Checks](#checks)
     * [Middleware](#middleware)
     * [Migrations](#migrations)
     * [Models](#models)
     * [Rules](#rules)
     * [Serializers](#serializers)
+    * [Template](#template)
     * [Template Tags](#template-tags)
+    * [Tests](#tests)
     * [Util](#util)
 * [Changelog](#changelog)
 
 ## Installation
 
 `pip install django-allianceutils`
 
 ## System Requirements
 
-* Tested with django 3.2 and 4.2
+* Tested with django 4.2 and 5.0
   * Pull requests accepted for other versions, but at minimum we test against current LTS versions
 * Python >=3.8
 
 ## Usage
 
 ### API
 
@@ -121,61 +120,61 @@
 
 * Creates permissions that have no model by linking them to an empty content type
 * Django creates permissions as part of
   the [`post_migrate` signal](https://docs.djangoproject.com/en/stable/ref/signals/#post-migrate)
 
 Usage
 
-```py
+```python
 def on_post_migrate(sender, **kwargs):
     register_custom_permissions("myapp", ("my_perm", "My Permission"))
 ```
 
 ##### SimpleDjangoObjectPermissions
 
 Permission class for Django Rest Framework that adds support for object level permissions.
 
 Differs from just DRF's [DjangoObjectPermissions](https://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions) because it
 * does not require a queryset
-* uses the same permission for every request http method and ViewSet method 
+* uses the same permission for every request http method and ViewSet method
 
 Notes
 * The default django permissions system will [always return False](https://docs.djangoproject.com/en/stable/topics/auth/customizing/#handling-object-permissions) if given an object; you must be using another permissions backend
 * As per [DRF documentation](http://www.django-rest-framework.org/api-guide/permissions/#object-level-permissions): get_object() is only required if you want to implement object-level permissions
 * **WARNING** If you override `get_object()` then you need to *manually* invoke `self.check_object_permissions(self.request, obj)`
 * Will attempt to check permission both globally and on a per-object basis but considers it an error if the check returns True for both
-*   
+*
 
 Usage
 * See [DRF permissions policy](https://www.django-rest-framework.org/api-guide/permissions/#setting-the-permission-policy) for details on apply Permissions policies globally
 
 * To apply to a specific view you need to set `permission_required`
 ```python
 class MyAPIView(SimpleDjangoObjectPermissions, APIView):
         permission_required = 'my_module.my_permission'
-        permission_classes = [allianceutils.api.permissions.SimpleDjangoObjectPermissions] 
+        permission_classes = [allianceutils.api.permissions.SimpleDjangoObjectPermissions]
 ```
 
 If you have no object level permissions (eg. from rules) then it will just do a static permission check.
 
 ##### GenericDjangoViewsetPermissions
 
 * Map viewset actions to Django permissions.
   * The model used for permission is extracted from the ViewSet
     * If you implement `get_permission_model` on the ViewSet that will be used
-    * Otherwise it will call `get_queryset` on the ViewSet and extract the model from the returned queryset 
- * To alter this behaviour extends `GenericDjangoViewsetPermissions` and implement `get_model` 
+    * Otherwise it will call `get_queryset` on the ViewSet and extract the model from the returned queryset
+ * To alter this behaviour extends `GenericDjangoViewsetPermissions` and implement `get_model`
 * Usage example:
-```
+```python
 class MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):
     queryset = MyModel.objects.all()
     serializer_class = MySerializer
 ```
 * `GenericDjangoViewsetPermissions.default_actions_to_perms_map` defines the default set of permissions. These can be extended or overridden using `actions_to_perms_map`:
-```
+```python
 class MyViewSet(GenericDjangoViewsetPermissions, viewsets.ModelViewSet):
 
     # ...
 
     actions_to_perms_map = {
         'create': []
     }
@@ -264,107 +263,137 @@
 ### Auth
 
 #### MinimalModelBackend
 
 * `allianceutils.auth.backends.MinimalModelBackend`
     * Replaces the built-in django [ModelBackend](https://docs.djangoproject.com/en/stable/ref/contrib/auth/#django.contrib.auth.backends.ModelBackend)
     * Provides django model-based authentication
-    * Removes the default authorization (permissions checks) except for checking `is_superuser` 
+    * Removes the default authorization (permissions checks) except for checking `is_superuser`
 
 #### ProfileModelBackend
 
 * Backends for use with [GenericUserProfile](#GenericUserProfile); see code examples there
 * `allianceutils.auth.backends.ProfileModelBackendMixin` - in combo with [AuthenticationMiddleware](https://docs.djangoproject.com/en/stable/ref/middleware/#django.contrib.auth.middleware.AuthenticationMiddleware) will set user profiles on `request.user`
-  * If you want  
+  * If you want
       * ~`allianceutils.auth.backends.ProfileModelBackend`~ - convenience class combined with case insensitive username & default django permissions backend
           * this depended on [`authtools`](https://django-authtools.readthedocs.io/en/latest/) which appears to have been
             abandoned and does not work with django >= 3.
             If using django 3 then we recommended that you create your own backend in your app:
             ```python
               class ProfileModelBackend(ProfileModelBackendMixin, MinimalModelBackend):
-                  # you'll need to implement case insensitivity either here or in the User Model  
+                  # you'll need to implement case insensitivity either here or in the User Model
                   pass
             ```
 
+#### Permissions
+
+##### NoDefaultPermissionsMeta
+
+- Define a `Meta` class with empty default permissions so Django doesn't create any
+- Usage example:
+
+```python
+class User(GenericUserProfile):
+
+    class Meta(NoDefaultPermissionsMeta):
+        pass
+```
+
+##### PermissionNotImplementedError
+
+- Subclass of `NotImplementedError` specific to permissions
+
+##### identify_global_perms
+
+- Takes a permission or list of permissions and splits them into global and object permissions, returning a tuple of (global permission list, object permission list). If the type can't be determined, the permission is returned in the global permission list.
+
+##### AmbiguousGlobalPermissionWarning
+
+- Raised if a permission cannot be classified as either global or per-object
+
+##### reverse_if_probably_allowed
+
+- Attempts to guess whether a user has permission to access a view to determine whether a URL should be displayed. Only for display purposes, not actual security, as it is not 100% reliable: can be used to, for example, hide the edit link in a CRUD view where the user does not have edit access. Takes the current request and the requested viewname, and optionally the specific object to be accessed.
+
 ### Decorators
 
 #### gzip_page_ajax
 
 * Smarter version of django's [gzip_page](https://docs.djangoproject.com/en/stable/topics/http/decorators/#django.views.decorators.gzip.gzip_page):
     * If settings.DEBUG not set, will always gzip
     * If settings.DEBUG set, will gzip only if request is an ajax request
 * This allows you to use django-debug-toolbar in DEBUG mode (if you gzip a response then the debug toolbar middleware won't run)
 
 Example
 
-```
+```python
 
 @allianceutils.views.decorators.gzip_page_ajax
 def my_view(request: HttpRequest) -> httpResponse:
     data = {
         "message": "Hello World",
     }
-    return django.http.JsonResponse(data) 
+    return django.http.JsonResponse(data)
 
 ```
 
 #### method_cache
 
 * Caches the results of a method on the object instance
-* There is no thread synchronization so in some circumstances the method may be called multiple times if multiple threads share the object 
+* There is no thread synchronization so in some circumstances the method may be called multiple times if multiple threads share the object
 * Only works for regular object methods with no arguments other than `self`.
     * Does not support `@classmethod` or `@staticmethod`
     * If you want more powerful caching behaviour then you can
       * use [`methodtools`](https://pypi.org/project/methodtools/)
       * wrap `cachetools` (examples [here](https://github.com/tkem/cachetools/issues/107#issuecomment-436274285))
 * Similar to [`@cached_property`](https://docs.python.org/3/library/functools.html#functools.cached_property) except that it works on methods instead of properties
 * Differs from [`@lru_cache()`](https://docs.python.org/3/library/functools.html#functools.lru_cache) in that
     * `lru_cache` uses a single cache for each decorated function
-    * `lru_cache` will block garbage collection of values in the cache 
-    * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance   
+    * `lru_cache` will block garbage collection of values in the cache
+    * A `cache_clear()` method is attached to the function but unlike `lru_cache` it is scoped to an object instance
 
 Usage
 ```python
 class MyViewSet(ViewSet):
 
     # ...
 
     @method_cache
     def get_object(self):
         return super().get_object()
 
 obj = MyViewSet()
 obj.get_object() is obj.get_object()
-obj.get_object.cache_clear()   
+obj.get_object.cache_clear()
 ```
 
 ### Management
 
 #### Commands
 
 ##### OptionalAppCommand
 
 * A utility class that extends `django.core.management.base.BaseCommand` and adds optional argument(s) for django apps
 * If app names are passed on the command line `handle_app_config()` will be called with the `AppConfig` for each app otherwise it will be called with every first-party app (as determined by `isort`)
 
 
 Example:
 
-```
+```python
 class Command(allianceutils.management.commands.base.OptionalAppCommand):
     def add_arguments(self, parser):
         super().add_arguments(parser)
         parser.add_argument('--type', choices=('name', 'label'), default='name')
 
     def handle_app_config(self, app_config: AppConfig, **options):
         if options['type'] == 'name':
             print(f"Called with {app_config.name}")
         if options['type'] == 'label':
             print(f"Called with {app_config.label}")
-```  
+```
 
 ##### print_logging
 
 * Displays the current logging configuration in a hierarchical fashion
 * Requires [`logging_tree`](https://pypi.python.org/pypi/logging_tree) to be installed
 
 #### Checks
@@ -391,31 +420,31 @@
 
     def ready(self):
         register(check=check_admins, tags=Tags.admin, deploy=True)
         register(check=check_db_constraints, tags=Tags.database)
         register(check=CheckExplicitTableNames(), tags=Tags.models)
         register(check=check_git_hooks, tags=Tags.admin)
         register(check=CheckReversibleFieldNames(), tags=Tags.models)
-        register(check=CheckUrlTrailingSlash(expect_trailing_slash=True), tags=Tags.url)        
+        register(check=CheckUrlTrailingSlash(expect_trailing_slash=True), tags=Tags.url)
 ```
 
 ##### CheckUrlTrailingSlash
 
-* Checks that your URLs are consistent with the `settings.APPEND_SLASH`  
+* Checks that your URLs are consistent with the `settings.APPEND_SLASH`
 * Arguments:
     * `ignore_attrs` - skip checks on url patterns where an attribute of the pattern matches something in here (see example above)
         * Most relevant attributes of a `RegexURLResolver`:
             * `_regex` - string used for regex matching. Defaults to `[r'^$']`
             * `app_name` - app name (only works for `include()` patterns). Defaults to `['djdt']` (django debug toolbar)
             * `namespace` - pattern defines a namespace
             * `lookup_str` - string defining view to use. Defaults to `['django.views.static.serve']`
         * Note that if you skip a resolver it will also skip checks on everything inside that resolver
 * Note: If using Django REST Framework's [`DefaultRouter`](http://www.django-rest-framework.org/api-guide/routers/#defaultrouter) then you need to turn off `include_format_suffixes`:
 
-```
+```python
 router = routers.DefaultRouter(trailing_slash=True)
 router.include_format_suffixes = False
 router.register(r'myurl', MyViewSet)
 urlpatterns += router.urls
 ```
 
 
@@ -423,30 +452,30 @@
 
 * Checks that `settings.ADMINS` has been properly set in settings files.
 
 ##### check\_git\_hooks
 
 * Checks that git hookshave been set up, one of:
   * `.git/hooks` directory has been symlinked to the project's `git-hooks`
-  * [`husky`](https://github.com/typicode/husky) hooks have been installed 
-* 
+  * [`husky`](https://github.com/typicode/husky) hooks have been installed
+*
 
 ##### check\_db\_constraints
 
 * Checks that all models that specify `db_constraints` in their Meta will generate unique constraint names when truncated by the database.
 
 ##### CheckExplicitTableNames
 
 * Checks that all first-party models have `db_table` explicitly defined on their Meta class, and the table name is in lowercase
 * Arguments:
     * `enforce_lowercase` - check that there are no uppercase characters in the table name
     * `ignore_labels` - if an app label (eg `silk`) or app_label + model labels (eg `silk.request`)
         matches something in `ignore_labels` then it will be ignored.
         * `allianceutils.checks.DEFAULT_TABLE_NAME_CHECK_IGNORE` contains a default list of apps/models to ignore
-        * Can be either a `str` or a regex (anything that contains a `.match()` method) 
+        * Can be either a `str` or a regex (anything that contains a `.match()` method)
 
 ##### CheckReversibleFieldNames
 
 * Checks that all models have fields names that are reversible with `underscorize`/`camelize`/`camel_to_underscore`/`underscore_to_camel`
 * Arguments:
     * `ignore_labels` - ignore these apps/models: see `CheckExplicitTableNames`
 
@@ -462,15 +491,15 @@
     * Add `allianceutils.middleware.HttpAuthMiddleware` to `MIDDLEWARE`.
     * Add `HTTP_AUTH_USERNAME` and `HTTP_AUTH_PASSWORD` to appropriate setting file, e.g. `settings/production_staging.py`
         * Remember that you shouldn't be hardcoding credentials in code: read content from env vars or file
 
 #### CurrentUserMiddleware
 
 * Middleware to enable accessing the currently logged-in user without a request object.
-    * Assumes that `threading.local` is not shared between requests (an assumption also made by django internationalisation) 
+    * Assumes that `threading.local` is not shared between requests (an assumption also made by django internationalisation)
 
 * Setup
     * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.
 
 * Usage
 
 ```python
@@ -483,33 +512,33 @@
 
 * Warns if query count reaches a given threshold
     * Threshold can be changed by setting `settings.QUERY_COUNT_WARNING_THRESHOLD`
 
 * Usage
     * Add `allianceutils.middleware.CurrentUserMiddleware` to `MIDDLEWARE`.
     * Uses the `warnings` module to raise a warning; by default this is suppressed by django
-        * To ensure `QueryCountWarning` is never suppressed  
+        * To ensure `QueryCountWarning` is never suppressed
 
 ```python
 warnings.simplefilter('always', allianceutils.middleware.QueryCountWarning)
 ```
 
-* To increase the query count limit for one request, you can call `QueryCountMiddleware.increase_threshold(request, increment)` 
+* To increase the query count limit for one request, you can call `QueryCountMiddleware.increase_threshold(request, increment)`
 * To set the query count limit for one request you can call `QueryCountMiddleware.set_threshold(request, threshold)`
   * Rather than hardcode a new limit, `increase_threshold()` is generally preferable
   * This can be useful to disable checks entirely (pass `0` as the new limit)
 
 
 ```python
 def my_view(request, *args, **kwargs):
     request.QUERY_COUNT_WARNING_THRESHOLD += 10
     ...
 
 ```
- 
+
 
 ### Migrations
 
 #### Run SQL function
 * Wrapper to `RunSQL` that reads SQL from a file instead of inline in python
 * The reason you would do this as an external file & function is so that squashed migrations don't become unwieldy (django will inline and strip whitespace in the SQL)
 
@@ -537,48 +566,48 @@
     * Can still be deleted with manual queries
 * Read django docs about [manager inheritance](https://docs.djangoproject.com/en/stable/topics/db/managers/#custom-managers-and-model-inheritance)
     * If you wish add your own manager, you need to combine the querysets:
 
 ```python
 class MyModel(NoDeleteModel):
         objects = combine_querysets_as_manager(NoDeleteQuerySet, MyQuerySet)
-```  
+```
 
 #### GenericUserProfile
 Allows you to iterate over a `User` table and have it return a corresponding `Profile` record without generating extra queries
 
 Minimal example:
 
 ```python
 # ------------------------------------------------------------------
-# base User model 
+# base User model
 
 # If you're using django auth instead of authtools, you can just use
 # GenericUserProfileManager instead of having to make your own manager class
 class UserManager(GenericUserProfileManagerMixin, authtools.models.UserManager):
     pass
 
 class User(GenericUserProfile, authtools.models.AbstractEmailUser):
     objects = UserManager()
     profiles = UserManager(select_related_profiles=True)
-    
+
     # these are the tables that should be select_related()/prefetch_related()
     # to minimise queries
     related_profile_tables = [
         'customerprofile',
         'adminprofile',
     ]
-    
+
     # the default implementation will iterate through the related profile tables
     # and return the first profile it can find. If you have custom logic for
     # choosing the profile for a user then you can do that here
     #
     # You would normally not access this directly but instead use the`.profile`
     # property that caches the return value of `get_profile()` and works
-    # correctly for both user and profile records  
+    # correctly for both user and profile records
     def get_profile(self) -> Model:
         # custom logic
         if datetime.now() > datetime.date(2000,1,1):
             return self
         return super().get_profile()
 
 
@@ -603,15 +632,15 @@
 
 # we can explicitly perform the transform on the queryset
 profiles = list(User.objects.select_related_profiles().all())
 
 # joining to profile tables: 1 query
 # This assumes that RetailLocation.company.manager is a FK ref to the user table
 # The syntax is a bit different because we can't modify the query generation
-# in an unrelated table 
+# in an unrelated table
 qs = RetailLocation.objects.all()
 qs = User.objects.select_related_profiles(qs, 'company__manager')
 location_managers = list((loc, loc.company.manager.profile) for loc in qs.all())
 ```
 
 * There is also an authentication backend that will load profiles instead of just User records
 * If the `User` model has no `get_profile()` method then this backend is equivalent to the built-in django `django.contrib.auth.backends.ModelBackend`
@@ -623,60 +652,60 @@
 AUTHENTICATION_BACKENDS = [
     'allianceutils.auth.backends.ProfileModelBackend',
 ]
 
 
 def my_view(request):
     # standard django AuthenticationMiddleware will call the authentication backend
-    profile = request.user  
+    profile = request.user
     return HttpResponse('Current user is ' + profile.username)
 
 ```
 
 * Limitations:
     * Profile iteration does not work with `.values()` or `.values_list()`
-    
+
 #### raise_validation_errors
 
 * The `raise_validation_errors` context manager enables cleaner code for constructing validation
     * [Django documentation](https://docs.djangoproject.com/en/stable/ref/models/instances/#django.db.models.Model.clean) recommends raising a `ValidationError` when you encounter a problem
     * This creates a poor user experience if there are multiple errors: the user only sees the first error and has to resubmit a form multiple times to fix problems
 * `raise_validation_errors` accepts an (optional) function to wrap
     * The context manager returns a `ValidationError` subclass with an `add_error` function that follows the same rules as `django.forms.forms.BaseForm.add_error`
     * If the wrapped function raises a `ValidationError` then this will be merged into the `ValidationError` returned by the context manager
-    * If the wrapped function raises any other exception then this will not be intercepted and the context block will not be executed 
+    * If the wrapped function raises any other exception then this will not be intercepted and the context block will not be executed
     * At the end of a block,
         * If code in the context block raised an exception (including a `ValidationError`) then this will not be caught
-        * If `ValidationError` the context manager returned has any errors (either from `ve.add_error()` or from the wrapped function) then this will be raised 
+        * If `ValidationError` the context manager returned has any errors (either from `ve.add_error()` or from the wrapped function) then this will be raised
 
-```
+```python
     def clean(self):
         with allianceutils.models.raise_validation_errors(super().clean) as ve:
             if some_condition:
                 ve.add_error(None, 'model error message')
             if other_condition:
                 ve.add_error('fieldname', 'field-specific error message')
             if other_condition:
                 ve.add_error(None, {
                     'fieldname1': field-specific error message',
                     'fieldname2': field-specific error message',
                 })
             if something_bad:
-                raise RuntimeError('Oh no!') 
-            
+                raise RuntimeError('Oh no!')
+
             # at the end of the context, ve will be raised if it contains any errors
             #   - unless an exception was raised in the block (RuntimeError example above) in which case
             #     the raised exception will take precedence
 ```
 
 * Sometimes you already have functions that may raise a `ValidationError` and `add_error()` will not help
     * The `capture_validation_error()` context manager solves this problem
-    * Note that due to the way context managers work, each potential `ValidationError` needs its own with `capture_validation_error` context 
+    * Note that due to the way context managers work, each potential `ValidationError` needs its own with `capture_validation_error` context
 
-```
+```python
     def clean(self):
         with allianceutils.models.raise_validation_errors() as ve:
              with ve.capture_validation_error():
                  self.func1()
              with ve.capture_validation_error():
                  self.func2()
              with ve.capture_validation_error():
@@ -684,27 +713,27 @@
             # all raised ValidationErrors will be collected, merged and raised at the end of this block
 ```
 
 ### Rules
 
 * Utility functions that return predicates for use with [django-rules](https://github.com/dfunckt/django-rules)
 
-```
+```python
 from allianceutils.rules import has_any_perms, has_perms, has_perm
 
 # requires at least 1 listed permission
 rules.add_perm('northwind.publish_book', has_any_perms('northwind.is_book_author', 'northwind.is_book_editor'))
 
 # requires listed permission
 rules.add_perm('northwind.unpublish_book', has_perm('northwind.is_book_editor'))
 
 # requires all listed permissions
 rules.add_perm('northwind.sublicense_book', has_perms('northwind.is_book_editor', 'northwind.can_sign_contracts'))
 
-```  
+```
 
 ### Serializers
 
 #### JSON Ordered
 
 * A version of django's core json serializer that outputs field in sorted order
 * The built-in one uses a standard `dict` with completely unpredictable order which causes json diffs to show spurious changes
@@ -716,14 +745,127 @@
 
 ```python
 SERIALIZATION_MODULES = {
     'json_ordered': 'allianceutils.serializers.json_ordered',
 }
 ```
 
+### Template
+
+##### resolve
+
+* Resolves different types of kwarg values consistently.
+  * If value is a NodeList then it is rendered
+  * If value is a FilterExpression then it is resolved
+  * If value is a dict then each element is resolved if it is a FilterExpression, or else returned as is
+  * Otherwise value is returned as is
+
+
+* Example Usage
+```python
+    def resolved_kwargs(self, context: Context):
+        pk = resolve(self.pk, context)
+        model = resolve(self.model_name, context)
+        object = resolve(self.object, context)
+```
+
+##### token_kwargs
+
+* Re-implements the `token_kwargs` function from the Django base template library. This allows expanding the range of possible keywords to include '-' for aria attributes (e.g. `aria-label="My Label"`), and ':' for namespaced attributes (e.g. `xlink:href="foo"`). Used internally in [parse_tag_arguments](#parse_tag_arguments) - see that section for usage
+
+##### parse_tag_arguments
+
+* Implements a stripped-down version of `django.template.library.parse_bits()` to parse tokens passed to tags in Django templates.
+  * Takes the parser to process the tag, the token passed to the tag, and the kwarg `supports_as`
+  * Returns a tuple of `(args: list, kwargs: dict, target_var: str)`:
+    * args: a list of args as FilterExpressions
+    * kwargs: a dict of kwargs
+    * target_var: if `supports_as` is `True` and `as <variable>` is specified, returns the string reference for the tag. Otherwise returns `None`
+
+
+* Example Usage
+
+```python
+class StylesheetNode(template.Node, BundlerAsset):
+    def __init__(self, filename: Path, origin: Origin | None, attrs=None, target_var=None):
+        self.filename = filename
+        self.attrs = attrs
+        self.target_var = target_var
+        super().__init__(origin or Origin(UNKNOWN_SOURCE))
+
+    def render(self, context: Context):
+        if self.target_var:
+            context[self.target_var] = get_classes(self.filename)
+
+@register.tag("stylesheet")
+def stylesheet(parser: template.base.Parser, token: template.base.Token):
+    args, kwargs, target_var = parse_tag_arguments(parser, token, supports_as=True)
+    filename = args[0]
+    return StylesheetNode(filename, parser.origin, kwargs, target_var=target_var)
+```
+
+```html
+    {% stylesheet "./theme.css" as styles %}
+
+    <div class="{{ styles.section }}">
+        <h1 class="{{ styles.heading }}">My View</h1>
+        ...
+    </div>
+```
+
+##### build_html_attrs
+
+* Takes a dict of HTML tag attributes and transforms values into escaped strings suitable for use as HTML tag attributes. Can also pass a list of `prohibited_attrs` to prevent passing attributes which should not be passed to template tags.
+
+* Example Usage
+```python
+from django.utils.html import format_html
+...
+class LinkNode(template.Node):
+    def __init__(
+        self,
+        *,
+        href: FilterExpression | str | None = None,
+        **extra_kwargs,
+    ) -> None:
+        self.href = href
+
+    ...
+
+    def render(self, context: Context) -> SafeString:
+        href = resolve(self.href, context)
+        html_kwargs = { "href": href }
+        html_attrs = build_html_attrs(html_kwargs)
+        return format_html(
+            "<a {}>{}</a>",
+            html_attrs,
+        )
+```
+
+```html
+    {% link "/home" %}
+```
+
+##### is_static_expression
+
+* Checks if a given FilterExpression is static using the same method as Django's `resolve` implementation for the `Variable` class
+
+* Example Usage
+```python
+def validate_tag(parser, token):
+    tag_name = token.split_contents()[0]
+    args, _, _ = parse_tag_arguments(parser, token)
+
+    for arg in args:
+        if not is_static_expression(arg):
+            raise TemplateSyntaxError(
+                f"{tag_name} must be passed static strings for its arguments (encountered variable '{arg.var}')"
+            )
+```
+
 ### Template Tags
 
 #### render_entry_point
 
 * Replaces old usage of [django-webpack-loader](https://github.com/ezhome/django-webpack-loader)
    * At time of writing django-webpack-loader does not have a stable release that [works with webpack 4](https://github.com/owais/django-webpack-loader/issues/218)
    * Worked at bundle level rather than entry point. See below for how we embed tags based on entry point.
@@ -751,23 +893,23 @@
             "contentHash": "c78fb252d4e00207afef"
           }
         ]
       },
       "publicPath": "/assets/"
     }
    ```
-   
+
    Output for `{% render_entry_point 'admin' 'js' %}`:
 
    ```html
    <script type="text/javascript" src="/assets/runtime.bundle.js?e2b781da02d36dad3aff"></script>
    <script type="text/javascript" src="/assets/common.bundle.js?639269b921c8cf869c5f"></script>
    <script type="text/javascript" src="/assets/admin.bundle.js?c78fb252d4e00207afef"></script>
    ```
-   
+
    Output for `{% render_entry_point 'admin' 'css' %}`:
 
    ```html
    <link type="text/css" href="/assets/common.bundle.css?d60a0fa36613ea58a23d" rel="stylesheet" />
    ```
 * As an entry point maps to a single HTML file it's expected you would only use this tag for a single entry point on a page but generally would call it for both `js` and `css`
 * Arguments
@@ -788,51 +930,105 @@
 ```html
 {% load alliance_webpack %}
 <html>
 <head>
   {% render_entry_point 'app' 'css' %}
 </head>
 <body>
-  
+
   ...
-  
+
   {% if DEBUG %}
     {# See https://reactjs.org/docs/cross-origin-errors.html #}
     {% render_entry_point entry_point 'js' attrs="crossorigin" %}
   {% else %}
     {% render_entry_point entry_point 'js' %}
   {% endif %}
 </body>
 </html>
 ```
 
 #### default_value
 
 * Sets default value(s) on the context in a template
 * This is useful because some built-in django templates raise warnings about unset variables (eg `is_popup` in the django admin template)
-* Note that some tags (eg `with`) save & restore the context state; if done inside such a template tag `default_value` will not persist when the state is restored 
+* Note that some tags (eg `with`) save & restore the context state; if done inside such a template tag `default_value` will not persist when the state is restored
 
 ```html
 {% load default_value %}
 {{ default_value myvar1=99 myvar2=myvar1|upper }}
 {{ myvar1 }} {{ myvar2 }}
 ```
 
+### Tests
+
+##### suppress_silk
+
+* Decorator to disable silk SQL query logging.
+* This is needed for tests that use `assertNumQueries()` since otherwise the query count may include silk's `EXPLAIN`
+
+* Example Usage
+
+```python
+    @suppress_silk()
+    def test_lookup_object(self):
+        """Test that a query is run if object is not provided in template"""
+        user = self.get_privileged_user()
+        viewname = self.VIEW_KWARGS
+        view_kwargs = {"pk": user.pk}
+
+        request = HttpRequest()
+
+        # Without suppress_silk, an EXPLAIN query will be added
+        with self.assertNumQueries(1):
+            tpl = Template('{% load link %}{% link "' + viewname + '" pk=pk %}foo{% endlink %}')
+            tpl.render(Context({"request": request, "user": user, **view_kwargs}))
+```
+
+##### logging_filter
+
+* Decorator to disable logging for specified log names
+* This is useful because using `override_settings(LOGGING=...)` triggers an update to the python logging settings
+
+* Example Usage
+```python
+    @logging_filter(["django.request"])
+    def test_django_validation_errors(self):
+        url = reverse("django-validation-test-url")
+        for key, expect in EXPECTED_RESPONSES.items():
+            with self.subTest(key=key):
+                response = self.client.post(url, data={"error_key": key}, format="json")
+                self.assertEqual(400, response.status_code)
+                self.assertEqual(expect, response.json())
+```
+
+##### warning_filter
+
+* Apply a `warning.simplefilter()` for the specified warnings
+
+* Example Usage
+```python
+    @warning_filter("ignore", category=DeprecationWarning)
+    def test_relying_on_deprecated_feature(self):
+        instance = MyModel.objects.filter(deprecated_filter=True)
+        assertIsInstance(instance, MyModel)
+```
+
 ### Util
 
 #### add_autoreload_extra_files
 
 * Adds files to the autoreloader watch list
     * Works with both the built-in [`runserver`](https://docs.djangoproject.com/en/stable/ref/django-admin/#runserver)
       and [`runserver_plus`](https://django-extensions.readthedocs.io/en/latest/runserver_plus.html) from `django-extensions`
     * If `DEBUG` is not enabled then this will do nothing
     * This should be called from inside the
       [`ready()`](https://docs.djangoproject.com/en/stable/ref/applications/#django.apps.AppConfig.ready) method of
-      an [`AppConfig`](https://docs.djangoproject.com/en/stable/ref/applications/#configuring-applications) 
-  
+      an [`AppConfig`](https://docs.djangoproject.com/en/stable/ref/applications/#configuring-applications)
+
 ```python
 class MyAppConfig(AppConfig):
     def ready(self):
         extra_files = [
           "/data/file.csv",
         ]
         add_autoreload_extra_files(extra_files)
@@ -879,15 +1075,15 @@
 
 * `allianceutils.util.camelize(data, ignores)` - underscore case => camel case a json tree of data
 * `allianceutils.util.underscorize(data, ignores)` - camel case => underscore case a json tree of data
 * `allianceutils.util.camel_to_underscore(str)` - underscore case => camel case a string
 * `allianceutils.util.underscore_to_camel(str)` - camel case => underscore case a string
 * It is assumed that words will not begin with numbers:
     * `zoo_foo99_bar` is okay
-    * `zoo_foo_99bar` will result in an irreversible transformation (`zooFoo99bar` => `zoo_foo99_bar`) 
+    * `zoo_foo_99bar` will result in an irreversible transformation (`zooFoo99bar` => `zoo_foo99_bar`)
 
 #### get_firstparty_apps
 
 `util.get_firstparty_apps` can be used to retrieve app_configs considered to be first party, ie, all that does not come from a third party package.
 This is beneficial when you want to write your own checks by excluding things you dont really care - a sample usage can be found inside 'checks.py', or
 used as such:
 
@@ -935,27 +1131,27 @@
     super().save(*args, **kwargs)
 retry_fn(generate_number, (IntegrityError, ), 10)
 ```
 
 ## Experimental
 
 * These are experimental and may change without notice
-    * `document_reverse_accessors` management command  
+    * `document_reverse_accessors` management command
 
 ## Changelog
 
 See [CHANGELOG.md](CHANGELOG.md)
 
 ## Development
 
 * To create a clean local environment
-  * `python3 -m venv venv && source venv/bin/activate && pip install --upgrade pip` 
+  * `python3 -m venv venv && source venv/bin/activate && pip install --upgrade pip`
   * `poetry install --no-root --sync --only=main --extras=""`
   * Note that due to [a poetry bug](https://github.com/python-poetry/poetry/issues/7364) extras are currently not removed
-  * This will install the latest django version; if you want to test a specific django version you need to `pip install` it manually 
+  * This will install the latest django version; if you want to test a specific django version you need to `pip install` it manually
 * Dev dependencies
   * `poetry install --no-root --sync --with=dev --extras "extras mysql postgres"`
 
 ### Release Process
 
 #### Poetry Config
 * Add test repository
@@ -967,47 +1163,33 @@
     * Generate an account API token at https://pypi.org/manage/account/token/
     * `poetry config pypi-token.pypi ${TOKEN}`
         * On macs this will be stored in the `login` keychain at `poetry-repository-pypi`
 
 #### Publishing a New Release
     * Update CHANGELOG.md with details of changes and new version
     * Run `bin/build.py`. This will extract version from CHANGELOG.md, bump version in `pyproject.toml` and generate a build for publishing
+    * Commit version bumps
     * Tag with new version and update the version branch:
         * `ver=$( poetry version --short ) && echo "Version: $ver"`
         * `git tag v/$ver`
         * `git push --tags`
     * To publish to test.pypi.org
         * `poetry publish --repository testpypi`
     * To publish to pypi.org
         * `poetry publish`
 
 
 ### Testing
 * To run test cases
   * The django settings module is `test_allianceutils/settings.py`
-    * The following env vars are optional but you may want to set them if the default don't match your local setup: 
+    * The following env vars are optional but you may want to set them if the default don't match your local setup:
       * `DB_NAME`
       * `DB_HOST`
       * `DB_PORT`
       * `DB_USER`
       * `DB_PASSWORD`
 * [tox](https://tox.wiki/en/latest/)
   * used to run tests against different django/python/database versions
   * `tox` to run all tests. Will require that you have a postgres & mysql server running.
-    * `tox -f django42` will run the subset of tests that cover django 4.2. Check `tox.ini` for the list of tested environments. 
-* When you push to github a [github Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python) workflow will be triggered (see `.github/workflows/django.yml`)  
-
-
+    * `tox -f django42` will run the subset of tests that cover django 4.2. Check `tox.ini` for the list of tested environments.
+* When you push to github a [github Actions](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python) workflow will be triggered (see `.github/workflows/django.yml`)
 
-TODO:
-- [x] mypy checks all pass
-- [x] github actions pass
-- [] stricter mypy settings?
-- [] flake8, black, isort
-- [x] can cachetools replace @method_cache?
-  - No; can use methodtools but is another dependency. just documented the alternative 
-- [x] Use collections.abc:
-  - no, doesn't work with 3.8
-- [x] Use | instead of Optional, Union
-  - no, doesn't work with 3.8
-- [] Remove legacy build settings (poetry shouldn't need setup.cfg, MANIFEST.in so can we remove them?)
-
```

