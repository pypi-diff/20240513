# Comparing `tmp/kinde-python-sdk-1.2.3.tar.gz` & `tmp/kinde_python_sdk-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinde-python-sdk-1.2.3.tar", last modified: Wed Feb 28 09:21:15 2024, max compression
+gzip compressed data, was "kinde_python_sdk-1.2.4.tar", last modified: Sun May 12 23:30:48 2024, max compression
```

## Comparing `kinde-python-sdk-1.2.3.tar` & `kinde_python_sdk-1.2.4.tar`

### file list

```diff
@@ -1,494 +1,494 @@
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.149286 kinde-python-sdk-1.2.3/
--rw-r--r--   0 rai        (501) staff       (20)     1385 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/LICENSE
--rw-r--r--   0 rai        (501) staff       (20)     1997 2024-02-28 09:21:15.149028 kinde-python-sdk-1.2.3/PKG-INFO
--rw-r--r--   0 rai        (501) staff       (20)     1075 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/README.md
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.148596 kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/
--rw-r--r--   0 rai        (501) staff       (20)     1997 2024-02-28 09:21:14.000000 kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 rai        (501) staff       (20)    22181 2024-02-28 09:21:15.000000 kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 rai        (501) staff       (20)        1 2024-02-28 09:21:14.000000 kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 rai        (501) staff       (20)      145 2024-02-28 09:21:14.000000 kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/requires.txt
--rw-r--r--   0 rai        (501) staff       (20)       10 2024-02-28 09:21:14.000000 kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.021626 kinde-python-sdk-1.2.3/kinde_sdk/
--rw-r--r--   0 rai        (501) staff       (20)      726 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    58495 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/api_client.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.024189 kinde-python-sdk-1.2.3/kinde_sdk/apis/
--rw-r--r--   0 rai        (501) staff       (20)      214 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11191 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/path_to_api.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.036377 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/
--rw-r--r--   0 rai        (501) staff       (20)      236 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)      172 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_apis.py
--rw-r--r--   0 rai        (501) staff       (20)      197 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_apis_api_id.py
--rw-r--r--   0 rai        (501) staff       (20)      143 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_apis_api_id_applications.py
--rw-r--r--   0 rai        (501) staff       (20)      196 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_applications.py
--rw-r--r--   0 rai        (501) staff       (20)      474 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_applications_app_id_auth_logout_urls.py
--rw-r--r--   0 rai        (501) staff       (20)      484 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_applications_app_id_auth_redirect_urls.py
--rw-r--r--   0 rai        (501) staff       (20)      343 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_applications_application_id.py
--rw-r--r--   0 rai        (501) staff       (20)      187 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_business.py
--rw-r--r--   0 rai        (501) staff       (20)      135 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_connected_apps_auth_url.py
--rw-r--r--   0 rai        (501) staff       (20)      135 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_connected_apps_revoke.py
--rw-r--r--   0 rai        (501) staff       (20)      130 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_connected_apps_token.py
--rw-r--r--   0 rai        (501) staff       (20)      239 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_environment_feature_flags.py
--rw-r--r--   0 rai        (501) staff       (20)      293 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_environment_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      120 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_feature_flags.py
--rw-r--r--   0 rai        (501) staff       (20)      252 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      112 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_industries.py
--rw-r--r--   0 rai        (501) staff       (20)      196 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organization.py
--rw-r--r--   0 rai        (501) staff       (20)      233 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organization_org_code.py
--rw-r--r--   0 rai        (501) staff       (20)      118 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations.py
--rw-r--r--   0 rai        (501) staff       (20)      270 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags.py
--rw-r--r--   0 rai        (501) staff       (20)      324 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      340 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_users.py
--rw-r--r--   0 rai        (501) staff       (20)      168 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id.py
--rw-r--r--   0 rai        (501) staff       (20)      298 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_permissions.py
--rw-r--r--   0 rai        (501) staff       (20)      217 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id.py
--rw-r--r--   0 rai        (501) staff       (20)      280 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_roles.py
--rw-r--r--   0 rai        (501) staff       (20)      193 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_roles_role_id.py
--rw-r--r--   0 rai        (501) staff       (20)      193 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_permissions.py
--rw-r--r--   0 rai        (501) staff       (20)      245 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_permissions_permission_id.py
--rw-r--r--   0 rai        (501) staff       (20)      175 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_roles.py
--rw-r--r--   0 rai        (501) staff       (20)      209 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_roles_role_id.py
--rw-r--r--   0 rai        (501) staff       (20)      235 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_roles_role_id_permissions.py
--rw-r--r--   0 rai        (501) staff       (20)      174 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_roles_role_id_permissions_permission_id.py
--rw-r--r--   0 rai        (501) staff       (20)      193 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_subscribers.py
--rw-r--r--   0 rai        (501) staff       (20)      140 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_subscribers_subscriber_id.py
--rw-r--r--   0 rai        (501) staff       (20)      110 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_timezones.py
--rw-r--r--   0 rai        (501) staff       (20)      325 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_user.py
--rw-r--r--   0 rai        (501) staff       (20)      102 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_users.py
--rw-r--r--   0 rai        (501) staff       (20)      179 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_users_user_id_feature_flags_feature_flag_key.py
--rw-r--r--   0 rai        (501) staff       (20)      147 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/api_v1_users_user_id_refresh_claims.py
--rw-r--r--   0 rai        (501) staff       (20)      116 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/oauth2_introspect.py
--rw-r--r--   0 rai        (501) staff       (20)      108 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/oauth2_revoke.py
--rw-r--r--   0 rai        (501) staff       (20)      116 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/oauth2_user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)      121 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/paths/oauth2_v2_user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)     2383 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tag_to_api.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.039658 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/
--rw-r--r--   0 rai        (501) staff       (20)      714 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)      817 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/apis_api.py
--rw-r--r--   0 rai        (501) staff       (20)      936 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/applications_api.py
--rw-r--r--   0 rai        (501) staff       (20)      588 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/business_api.py
--rw-r--r--   0 rai        (501) staff       (20)     1423 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/callbacks_api.py
--rw-r--r--   0 rai        (501) staff       (20)      767 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/connected_apps_api.py
--rw-r--r--   0 rai        (501) staff       (20)     1038 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/environments_api.py
--rw-r--r--   0 rai        (501) staff       (20)      750 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/feature_flags_api.py
--rw-r--r--   0 rai        (501) staff       (20)      511 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/industries_api.py
--rw-r--r--   0 rai        (501) staff       (20)      768 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/o_auth_api.py
--rw-r--r--   0 rai        (501) staff       (20)     2979 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/organizations_api.py
--rw-r--r--   0 rai        (501) staff       (20)      821 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/permissions_api.py
--rw-r--r--   0 rai        (501) staff       (20)     1082 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/roles_api.py
--rw-r--r--   0 rai        (501) staff       (20)      704 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/subscribers_api.py
--rw-r--r--   0 rai        (501) staff       (20)      507 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/timezones_api.py
--rw-r--r--   0 rai        (501) staff       (20)     1044 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/users_api.py
--rw-r--r--   0 rai        (501) staff       (20)    15765 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/configuration.py
--rw-r--r--   0 rai        (501) staff       (20)     4736 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/exceptions.py
--rw-r--r--   0 rai        (501) staff       (20)    11493 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/kinde_api_client.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.068033 kinde-python-sdk-1.2.3/kinde_sdk/model/
--rw-r--r--   0 rai        (501) staff       (20)      343 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     4320 2024-02-28 08:24:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/add_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4320 2024-02-28 08:24:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/add_organization_users_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)    10480 2024-02-28 08:24:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/api.py
--rw-r--r--   0 rai        (501) staff       (20)    10480 2024-02-28 08:24:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/api.pyi
--rw-r--r--   0 rai        (501) staff       (20)     2410 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/api_result.py
--rw-r--r--   0 rai        (501) staff       (20)     2410 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/api_result.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4008 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/apis.py
--rw-r--r--   0 rai        (501) staff       (20)     4008 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/apis.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3322 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/applications.py
--rw-r--r--   0 rai        (501) staff       (20)     3322 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/applications.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3192 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_access_token.py
--rw-r--r--   0 rai        (501) staff       (20)     3192 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_access_token.pyi
--rw-r--r--   0 rai        (501) staff       (20)     2950 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_auth_url.py
--rw-r--r--   0 rai        (501) staff       (20)     2950 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_auth_url.pyi
--rw-r--r--   0 rai        (501) staff       (20)     7103 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_application_response.py
--rw-r--r--   0 rai        (501) staff       (20)     7103 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_application_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5765 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_organization_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5765 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_organization_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4867 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_subscriber_success_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4867 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_subscriber_success_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4393 2024-02-28 08:24:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_user_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4393 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/create_user_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     2894 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/error.py
--rw-r--r--   0 rai        (501) staff       (20)     2894 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/error.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3304 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/error_response.py
--rw-r--r--   0 rai        (501) staff       (20)     3304 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/error_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     8295 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_application_response.py
--rw-r--r--   0 rai        (501) staff       (20)     8295 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_application_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5011 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_applications_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5011 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_applications_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     9815 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_environment_feature_flags_response.py
--rw-r--r--   0 rai        (501) staff       (20)     9416 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_environment_feature_flags_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     9260 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_feature_flags_response.py
--rw-r--r--   0 rai        (501) staff       (20)     8861 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_feature_flags_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5134 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5134 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_users_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5027 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5027 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4572 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_permissions_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4572 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_permissions_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4991 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_roles_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4991 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_roles_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4988 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_permissions_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4988 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_permissions_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3545 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_redirect_callback_urls_response.py
--rw-r--r--   0 rai        (501) staff       (20)     3545 2024-02-28 08:24:35.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_redirect_callback_urls_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4850 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_roles_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4850 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_roles_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4422 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscriber_response.py
--rw-r--r--   0 rai        (501) staff       (20)     4422 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscriber_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5059 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscribers_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5059 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscribers_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3331 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/logout_redirect_urls.py
--rw-r--r--   0 rai        (501) staff       (20)     3331 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/logout_redirect_urls.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3998 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization.py
--rw-r--r--   0 rai        (501) staff       (20)     3998 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5805 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user.py
--rw-r--r--   0 rai        (501) staff       (20)     5805 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user.pyi
--rw-r--r--   0 rai        (501) staff       (20)     8498 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_permission.py
--rw-r--r--   0 rai        (501) staff       (20)     8498 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_permission.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3325 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role.py
--rw-r--r--   0 rai        (501) staff       (20)     3325 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5683 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role_permissions.py
--rw-r--r--   0 rai        (501) staff       (20)     5683 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role_permissions.pyi
--rw-r--r--   0 rai        (501) staff       (20)     1428 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_users.py
--rw-r--r--   0 rai        (501) staff       (20)     1428 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/organization_users.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3877 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/permissions.py
--rw-r--r--   0 rai        (501) staff       (20)     3877 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/permissions.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3335 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/redirect_callback_urls.py
--rw-r--r--   0 rai        (501) staff       (20)     3335 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/redirect_callback_urls.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3863 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/role.py
--rw-r--r--   0 rai        (501) staff       (20)     3863 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/role.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3865 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/roles.py
--rw-r--r--   0 rai        (501) staff       (20)     3865 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/roles.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5113 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/roles_permission_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5113 2024-02-28 08:24:36.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/roles_permission_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4083 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/subscriber.py
--rw-r--r--   0 rai        (501) staff       (20)     4083 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/subscriber.pyi
--rw-r--r--   0 rai        (501) staff       (20)     4519 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/subscribers_subscriber.py
--rw-r--r--   0 rai        (501) staff       (20)     4519 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/subscribers_subscriber.pyi
--rw-r--r--   0 rai        (501) staff       (20)     2914 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/success_response.py
--rw-r--r--   0 rai        (501) staff       (20)     2914 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/success_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     3063 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/token_error_response.py
--rw-r--r--   0 rai        (501) staff       (20)     3063 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/token_error_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5168 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/token_introspect.py
--rw-r--r--   0 rai        (501) staff       (20)     5168 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/token_introspect.pyi
--rw-r--r--   0 rai        (501) staff       (20)     6663 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/update_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)     6663 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/update_organization_users_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5898 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/update_role_permissions_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5898 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/update_role_permissions_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5878 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/update_user_response.py
--rw-r--r--   0 rai        (501) staff       (20)     5878 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/update_user_response.pyi
--rw-r--r--   0 rai        (501) staff       (20)    16810 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user.py
--rw-r--r--   0 rai        (501) staff       (20)    16810 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5176 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user_identity.py
--rw-r--r--   0 rai        (501) staff       (20)     5176 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user_identity.pyi
--rw-r--r--   0 rai        (501) staff       (20)     5779 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)     5779 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile.pyi
--rw-r--r--   0 rai        (501) staff       (20)     7198 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile_v2.py
--rw-r--r--   0 rai        (501) staff       (20)     7198 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile_v2.pyi
--rw-r--r--   0 rai        (501) staff       (20)     1340 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/users.py
--rw-r--r--   0 rai        (501) staff       (20)     1340 2024-02-28 08:24:37.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/users.pyi
--rw-r--r--   0 rai        (501) staff       (20)    27704 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/users_response.py
--rw-r--r--   0 rai        (501) staff       (20)    27704 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/model/users_response.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.070499 kinde-python-sdk-1.2.3/kinde_sdk/models/
--rw-r--r--   0 rai        (501) staff       (20)     4005 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/models/__init__.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.070677 kinde-python-sdk-1.2.3/kinde_sdk/paths/
--rw-r--r--   0 rai        (501) staff       (20)     3515 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/__init__.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.072005 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/
--rw-r--r--   0 rai        (501) staff       (20)      299 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     9822 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/get.py
--rw-r--r--   0 rai        (501) staff       (20)     9616 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    16268 2024-02-28 08:24:38.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/post.py
--rw-r--r--   0 rai        (501) staff       (20)    16062 2024-02-28 08:24:38.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.073269 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/
--rw-r--r--   0 rai        (501) staff       (20)      313 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11883 2024-02-28 08:24:38.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11677 2024-02-28 08:24:38.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    11789 2024-02-28 08:24:38.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11583 2024-02-28 08:24:38.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.074206 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id_applications/
--rw-r--r--   0 rai        (501) staff       (20)      339 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id_applications/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    22556 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    22350 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.075503 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/
--rw-r--r--   0 rai        (501) staff       (20)      315 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12885 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/get.py
--rw-r--r--   0 rai        (501) staff       (20)    12709 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    16879 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/post.py
--rw-r--r--   0 rai        (501) staff       (20)    16436 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.078311 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/
--rw-r--r--   0 rai        (501) staff       (20)      363 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13921 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    13715 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    11447 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11241 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    18219 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.py
--rw-r--r--   0 rai        (501) staff       (20)    18013 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.pyi
--rw-r--r--   0 rai        (501) staff       (20)    17993 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.py
--rw-r--r--   0 rai        (501) staff       (20)    17787 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.081586 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/
--rw-r--r--   0 rai        (501) staff       (20)      367 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13945 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    13739 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    11479 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11273 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    18247 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.py
--rw-r--r--   0 rai        (501) staff       (20)    18041 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.pyi
--rw-r--r--   0 rai        (501) staff       (20)    18021 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.py
--rw-r--r--   0 rai        (501) staff       (20)    17815 2024-02-28 08:24:41.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.083809 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/
--rw-r--r--   0 rai        (501) staff       (20)      345 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11819 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11613 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    11519 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11313 2024-02-28 08:24:39.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    20705 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    20499 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.085136 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/
--rw-r--r--   0 rai        (501) staff       (20)      307 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13665 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13489 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    16454 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    16248 2024-02-28 08:24:40.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.085982 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_auth_url/
--rw-r--r--   0 rai        (501) staff       (20)      337 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_auth_url/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13545 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13309 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.086917 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_revoke/
--rw-r--r--   0 rai        (501) staff       (20)      333 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_revoke/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12582 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py
--rw-r--r--   0 rai        (501) staff       (20)    12346 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_revoke/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.088022 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_token/
--rw-r--r--   0 rai        (501) staff       (20)      331 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_token/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12280 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_token/get.py
--rw-r--r--   0 rai        (501) staff       (20)    12074 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_token/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.089677 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/
--rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     9797 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/delete.py
--rw-r--r--   0 rai        (501) staff       (20)     9591 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)     9716 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/get.py
--rw-r--r--   0 rai        (501) staff       (20)     9510 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.091693 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      375 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11827 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11621 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    17958 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    17752 2024-02-28 08:24:42.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.092602 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags/
--rw-r--r--   0 rai        (501) staff       (20)      317 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    19617 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags/post.py
--rw-r--r--   0 rai        (501) staff       (20)    18935 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.094010 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      351 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11566 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11360 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    15759 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py
--rw-r--r--   0 rai        (501) staff       (20)    15295 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.094927 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_industries/
--rw-r--r--   0 rai        (501) staff       (20)      311 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_industries/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    10834 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_industries/get.py
--rw-r--r--   0 rai        (501) staff       (20)    10658 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_industries/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.096495 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/
--rw-r--r--   0 rai        (501) staff       (20)      315 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11598 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11392 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    25577 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/post.py
--rw-r--r--   0 rai        (501) staff       (20)    25038 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.099474 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/
--rw-r--r--   0 rai        (501) staff       (20)      333 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    10958 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    10752 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    25315 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    25109 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.100257 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations/
--rw-r--r--   0 rai        (501) staff       (20)      317 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13177 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13001 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.101763 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/
--rw-r--r--   0 rai        (501) staff       (20)      363 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11787 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11581 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    11710 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11504 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.103007 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      397 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12115 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11909 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    14275 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    14069 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.105085 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/
--rw-r--r--   0 rai        (501) staff       (20)      347 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    16668 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/get.py
--rw-r--r--   0 rai        (501) staff       (20)    16462 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    26157 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    25951 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.pyi
--rw-r--r--   0 rai        (501) staff       (20)    25893 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/post.py
--rw-r--r--   0 rai        (501) staff       (20)    25657 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.105787 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/
--rw-r--r--   0 rai        (501) staff       (20)      363 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11853 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11647 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.107202 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/
--rw-r--r--   0 rai        (501) staff       (20)      387 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13729 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13553 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    17315 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.py
--rw-r--r--   0 rai        (501) staff       (20)    17139 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.107809 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/
--rw-r--r--   0 rai        (501) staff       (20)      415 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12306 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    12100 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.109388 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/
--rw-r--r--   0 rai        (501) staff       (20)      375 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11100 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.py
--rw-r--r--   0 rai        (501) staff       (20)    10924 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    17153 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.py
--rw-r--r--   0 rai        (501) staff       (20)    16977 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.110176 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/
--rw-r--r--   0 rai        (501) staff       (20)      391 2024-02-28 08:24:46.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12192 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11986 2024-02-28 08:24:45.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.111714 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/
--rw-r--r--   0 rai        (501) staff       (20)      313 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13669 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13493 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    16493 2024-02-28 08:24:47.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/post.py
--rw-r--r--   0 rai        (501) staff       (20)    16287 2024-02-28 08:24:47.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.112771 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/
--rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11525 2024-02-28 08:24:47.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11319 2024-02-28 08:24:47.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    18752 2024-02-28 08:24:47.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    18546 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.113944 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/
--rw-r--r--   0 rai        (501) staff       (20)      301 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13573 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13397 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    17409 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/post.py
--rw-r--r--   0 rai        (501) staff       (20)    17233 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.115254 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/
--rw-r--r--   0 rai        (501) staff       (20)      317 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11411 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11205 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    19260 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    19054 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.116483 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/
--rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    16000 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.py
--rw-r--r--   0 rai        (501) staff       (20)    15794 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    21634 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    21458 2024-02-28 08:24:48.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.117200 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/
--rw-r--r--   0 rai        (501) staff       (20)      369 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11864 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11658 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.120558 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/
--rw-r--r--   0 rai        (501) staff       (20)      313 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13228 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13052 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    12914 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/post.py
--rw-r--r--   0 rai        (501) staff       (20)    12708 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.121843 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers_subscriber_id/
--rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers_subscriber_id/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11307 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11101 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.122959 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_timezones/
--rw-r--r--   0 rai        (501) staff       (20)      309 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_timezones/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    10821 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_timezones/get.py
--rw-r--r--   0 rai        (501) staff       (20)    10645 2024-02-28 08:24:49.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_timezones/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.125627 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/
--rw-r--r--   0 rai        (501) staff       (20)      299 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    11923 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/delete.py
--rw-r--r--   0 rai        (501) staff       (20)    11717 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/delete.pyi
--rw-r--r--   0 rai        (501) staff       (20)    12184 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/get.py
--rw-r--r--   0 rai        (501) staff       (20)    11978 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    19628 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    19422 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/patch.pyi
--rw-r--r--   0 rai        (501) staff       (20)    27927 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/post.py
--rw-r--r--   0 rai        (501) staff       (20)    27436 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.126390 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users/
--rw-r--r--   0 rai        (501) staff       (20)      301 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    13769 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users/get.py
--rw-r--r--   0 rai        (501) staff       (20)    13593 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.127232 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/
--rw-r--r--   0 rai        (501) staff       (20)      379 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    14172 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.py
--rw-r--r--   0 rai        (501) staff       (20)    13966 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.127984 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/
--rw-r--r--   0 rai        (501) staff       (20)      347 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    12006 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.py
--rw-r--r--   0 rai        (501) staff       (20)    11800 2024-02-28 08:24:50.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.129093 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_introspect/
--rw-r--r--   0 rai        (501) staff       (20)      311 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_introspect/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    16620 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_introspect/post.py
--rw-r--r--   0 rai        (501) staff       (20)    16414 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_introspect/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.130084 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_revoke/
--rw-r--r--   0 rai        (501) staff       (20)      303 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_revoke/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    16603 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_revoke/post.py
--rw-r--r--   0 rai        (501) staff       (20)    16397 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_revoke/post.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.133224 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_user_profile/
--rw-r--r--   0 rai        (501) staff       (20)      315 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_user_profile/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     7922 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_user_profile/get.py
--rw-r--r--   0 rai        (501) staff       (20)     7776 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_user_profile/get.pyi
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.134291 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_v2_user_profile/
--rw-r--r--   0 rai        (501) staff       (20)      321 2024-02-28 08:24:44.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_v2_user_profile/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     8381 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_v2_user_profile/get.py
--rw-r--r--   0 rai        (501) staff       (20)     8205 2024-02-28 08:24:43.000000 kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_v2_user_profile/get.pyi
--rw-r--r--   0 rai        (501) staff       (20)    10552 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/rest.py
--rw-r--r--   0 rai        (501) staff       (20)    97655 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/schemas.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.134769 kinde-python-sdk-1.2.3/kinde_sdk/test/
--rw-r--r--   0 rai        (501) staff       (20)        0 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)    61679 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_kinde_api_client.py
-drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-02-28 09:21:15.148210 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/
--rw-r--r--   0 rai        (501) staff       (20)        0 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/__init__.py
--rw-r--r--   0 rai        (501) staff       (20)     1017 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_add_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      517 2024-02-28 07:27:30.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_api.py
--rw-r--r--   0 rai        (501) staff       (20)      844 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_api_result.py
--rw-r--r--   0 rai        (501) staff       (20)      521 2024-02-28 07:27:30.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_apis.py
--rw-r--r--   0 rai        (501) staff       (20)      553 2024-02-28 07:27:30.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_applications.py
--rw-r--r--   0 rai        (501) staff       (20)      995 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_connected_apps_access_token.py
--rw-r--r--   0 rai        (501) staff       (20)      905 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_connected_apps_auth_url.py
--rw-r--r--   0 rai        (501) staff       (20)      607 2024-02-28 07:27:31.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_application_response.py
--rw-r--r--   0 rai        (501) staff       (20)      611 2024-02-28 07:27:31.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_organization_response.py
--rw-r--r--   0 rai        (501) staff       (20)      632 2024-02-28 07:27:31.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_subscriber_success_response.py
--rw-r--r--   0 rai        (501) staff       (20)      886 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_user_response.py
--rw-r--r--   0 rai        (501) staff       (20)      801 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_error.py
--rw-r--r--   0 rai        (501) staff       (20)      943 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_error_response.py
--rw-r--r--   0 rai        (501) staff       (20)      595 2024-02-28 07:27:31.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_application_response.py
--rw-r--r--   0 rai        (501) staff       (20)      599 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_applications_response.py
--rw-r--r--   0 rai        (501) staff       (20)      645 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_environment_feature_flags_response.py
--rw-r--r--   0 rai        (501) staff       (20)      649 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organization_feature_flags_response.py
--rw-r--r--   0 rai        (501) staff       (20)      620 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      942 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organizations_response.py
--rw-r--r--   0 rai        (501) staff       (20)      665 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organizations_user_permissions_response.py
--rw-r--r--   0 rai        (501) staff       (20)      641 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organizations_user_roles_response.py
--rw-r--r--   0 rai        (501) staff       (20)      595 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_permissions_response.py
--rw-r--r--   0 rai        (501) staff       (20)      633 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_redirect_callback_urls_response.py
--rw-r--r--   0 rai        (501) staff       (20)      571 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_roles_response.py
--rw-r--r--   0 rai        (501) staff       (20)      591 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_subscriber_response.py
--rw-r--r--   0 rai        (501) staff       (20)      595 2024-02-28 07:27:32.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_subscribers_response.py
--rw-r--r--   0 rai        (501) staff       (20)      579 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_logout_redirect_urls.py
--rw-r--r--   0 rai        (501) staff       (20)      850 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization.py
--rw-r--r--   0 rai        (501) staff       (20)      866 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user.py
--rw-r--r--   0 rai        (501) staff       (20)      611 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user_permission.py
--rw-r--r--   0 rai        (501) staff       (20)      587 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user_role.py
--rw-r--r--   0 rai        (501) staff       (20)      632 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user_role_permissions.py
--rw-r--r--   0 rai        (501) staff       (20)      575 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_users.py
--rw-r--r--   0 rai        (501) staff       (20)      549 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_permissions.py
--rw-r--r--   0 rai        (501) staff       (20)      587 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_redirect_callback_urls.py
--rw-r--r--   0 rai        (501) staff       (20)      521 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_role.py
--rw-r--r--   0 rai        (501) staff       (20)      525 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_roles.py
--rw-r--r--   0 rai        (501) staff       (20)      599 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_roles_permission_response.py
--rw-r--r--   0 rai        (501) staff       (20)      545 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_subscriber.py
--rw-r--r--   0 rai        (501) staff       (20)      590 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_subscribers_subscriber.py
--rw-r--r--   0 rai        (501) staff       (20)      907 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_success_response.py
--rw-r--r--   0 rai        (501) staff       (20)      579 2024-02-28 07:27:33.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_token_error_response.py
--rw-r--r--   0 rai        (501) staff       (20)      566 2024-02-28 07:27:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_token_introspect.py
--rw-r--r--   0 rai        (501) staff       (20)      632 2024-02-28 07:27:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_update_organization_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      624 2024-02-28 07:27:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_update_role_permissions_response.py
--rw-r--r--   0 rai        (501) staff       (20)      579 2024-02-28 07:27:34.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_update_user_response.py
--rw-r--r--   0 rai        (501) staff       (20)      780 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user.py
--rw-r--r--   0 rai        (501) staff       (20)      852 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user_identity.py
--rw-r--r--   0 rai        (501) staff       (20)      831 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user_profile.py
--rw-r--r--   0 rai        (501) staff       (20)      847 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user_profile_v2.py
--rw-r--r--   0 rai        (501) staff       (20)      526 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_users.py
--rw-r--r--   0 rai        (501) staff       (20)      858 2024-02-28 08:24:51.000000 kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_users_response.py
--rw-r--r--   0 rai        (501) staff       (20)      953 2024-02-28 09:18:20.000000 kinde-python-sdk-1.2.3/pyproject.toml
--rw-r--r--   0 rai        (501) staff       (20)       38 2024-02-28 09:21:15.149331 kinde-python-sdk-1.2.3/setup.cfg
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.462052 kinde_python_sdk-1.2.4/
+-rw-r--r--   0 rai        (501) staff       (20)     1385 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/LICENSE
+-rw-r--r--   0 rai        (501) staff       (20)     2003 2024-05-12 23:30:48.461772 kinde_python_sdk-1.2.4/PKG-INFO
+-rw-r--r--   0 rai        (501) staff       (20)     1075 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/README.md
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.461264 kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/
+-rw-r--r--   0 rai        (501) staff       (20)     2003 2024-05-12 23:30:48.000000 kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 rai        (501) staff       (20)    22181 2024-05-12 23:30:48.000000 kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 rai        (501) staff       (20)        1 2024-05-12 23:30:48.000000 kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 rai        (501) staff       (20)      151 2024-05-12 23:30:48.000000 kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 rai        (501) staff       (20)       10 2024-05-12 23:30:48.000000 kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.324702 kinde_python_sdk-1.2.4/kinde_sdk/
+-rw-r--r--   0 rai        (501) staff       (20)      726 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    58495 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/api_client.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.326008 kinde_python_sdk-1.2.4/kinde_sdk/apis/
+-rw-r--r--   0 rai        (501) staff       (20)      214 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11191 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/path_to_api.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.338139 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/
+-rw-r--r--   0 rai        (501) staff       (20)      236 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)      172 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_apis.py
+-rw-r--r--   0 rai        (501) staff       (20)      197 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_apis_api_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      143 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_apis_api_id_applications.py
+-rw-r--r--   0 rai        (501) staff       (20)      196 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_applications.py
+-rw-r--r--   0 rai        (501) staff       (20)      474 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_applications_app_id_auth_logout_urls.py
+-rw-r--r--   0 rai        (501) staff       (20)      484 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_applications_app_id_auth_redirect_urls.py
+-rw-r--r--   0 rai        (501) staff       (20)      343 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_applications_application_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      187 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_business.py
+-rw-r--r--   0 rai        (501) staff       (20)      135 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_connected_apps_auth_url.py
+-rw-r--r--   0 rai        (501) staff       (20)      135 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_connected_apps_revoke.py
+-rw-r--r--   0 rai        (501) staff       (20)      130 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_connected_apps_token.py
+-rw-r--r--   0 rai        (501) staff       (20)      239 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_environment_feature_flags.py
+-rw-r--r--   0 rai        (501) staff       (20)      293 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_environment_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      120 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_feature_flags.py
+-rw-r--r--   0 rai        (501) staff       (20)      252 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      112 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_industries.py
+-rw-r--r--   0 rai        (501) staff       (20)      196 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organization.py
+-rw-r--r--   0 rai        (501) staff       (20)      233 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organization_org_code.py
+-rw-r--r--   0 rai        (501) staff       (20)      118 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations.py
+-rw-r--r--   0 rai        (501) staff       (20)      270 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags.py
+-rw-r--r--   0 rai        (501) staff       (20)      324 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      340 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      168 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      298 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)      217 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      280 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_roles.py
+-rw-r--r--   0 rai        (501) staff       (20)      193 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_organizations_org_code_users_user_id_roles_role_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      193 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)      245 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_permissions_permission_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      175 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_roles.py
+-rw-r--r--   0 rai        (501) staff       (20)      209 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_roles_role_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      235 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_roles_role_id_permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)      174 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_roles_role_id_permissions_permission_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      193 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_subscribers.py
+-rw-r--r--   0 rai        (501) staff       (20)      140 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_subscribers_subscriber_id.py
+-rw-r--r--   0 rai        (501) staff       (20)      110 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_timezones.py
+-rw-r--r--   0 rai        (501) staff       (20)      325 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_user.py
+-rw-r--r--   0 rai        (501) staff       (20)      102 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      179 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_users_user_id_feature_flags_feature_flag_key.py
+-rw-r--r--   0 rai        (501) staff       (20)      147 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/api_v1_users_user_id_refresh_claims.py
+-rw-r--r--   0 rai        (501) staff       (20)      116 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/oauth2_introspect.py
+-rw-r--r--   0 rai        (501) staff       (20)      108 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/oauth2_revoke.py
+-rw-r--r--   0 rai        (501) staff       (20)      116 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/oauth2_user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)      121 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/paths/oauth2_v2_user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)     2383 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tag_to_api.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.341989 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/
+-rw-r--r--   0 rai        (501) staff       (20)      714 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)      817 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/apis_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      936 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/applications_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      588 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/business_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     1423 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/callbacks_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      767 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/connected_apps_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     1038 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/environments_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      750 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/feature_flags_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      511 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/industries_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      768 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/o_auth_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     2979 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/organizations_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      821 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/permissions_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     1082 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/roles_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      704 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/subscribers_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      507 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/timezones_api.py
+-rw-r--r--   0 rai        (501) staff       (20)     1044 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/users_api.py
+-rw-r--r--   0 rai        (501) staff       (20)    15765 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/configuration.py
+-rw-r--r--   0 rai        (501) staff       (20)     4736 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/exceptions.py
+-rw-r--r--   0 rai        (501) staff       (20)    11722 2024-05-12 23:29:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/kinde_api_client.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.374391 kinde_python_sdk-1.2.4/kinde_sdk/model/
+-rw-r--r--   0 rai        (501) staff       (20)      343 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     4320 2024-02-28 08:24:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/add_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4320 2024-02-28 08:24:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/add_organization_users_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    10480 2024-02-28 08:24:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/api.py
+-rw-r--r--   0 rai        (501) staff       (20)    10480 2024-02-28 08:24:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/api.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     2410 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/api_result.py
+-rw-r--r--   0 rai        (501) staff       (20)     2410 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/api_result.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4008 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/apis.py
+-rw-r--r--   0 rai        (501) staff       (20)     4008 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/apis.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3322 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/applications.py
+-rw-r--r--   0 rai        (501) staff       (20)     3322 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/applications.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3192 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_access_token.py
+-rw-r--r--   0 rai        (501) staff       (20)     3192 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_access_token.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     2950 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_auth_url.py
+-rw-r--r--   0 rai        (501) staff       (20)     2950 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_auth_url.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     7103 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_application_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     7103 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_application_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5765 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_organization_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5765 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_organization_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4867 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_subscriber_success_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4867 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_subscriber_success_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4393 2024-02-28 08:24:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_user_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4393 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/create_user_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     2894 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/error.py
+-rw-r--r--   0 rai        (501) staff       (20)     2894 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/error.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3304 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/error_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     3304 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/error_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     8295 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_application_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     8295 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_application_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5011 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_applications_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5011 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_applications_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     9815 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_environment_feature_flags_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     9416 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_environment_feature_flags_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     9260 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_feature_flags_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     8861 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_feature_flags_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5134 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5134 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_users_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5027 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5027 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4572 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_permissions_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4572 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_permissions_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4991 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_roles_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4991 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_roles_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4988 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_permissions_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4988 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_permissions_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3545 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_redirect_callback_urls_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     3545 2024-02-28 08:24:35.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_redirect_callback_urls_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4850 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_roles_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4850 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_roles_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4422 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscriber_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     4422 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscriber_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5059 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscribers_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5059 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscribers_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3331 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/logout_redirect_urls.py
+-rw-r--r--   0 rai        (501) staff       (20)     3331 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/logout_redirect_urls.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3998 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization.py
+-rw-r--r--   0 rai        (501) staff       (20)     3998 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5805 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user.py
+-rw-r--r--   0 rai        (501) staff       (20)     5805 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     8498 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_permission.py
+-rw-r--r--   0 rai        (501) staff       (20)     8498 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_permission.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3325 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role.py
+-rw-r--r--   0 rai        (501) staff       (20)     3325 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5683 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role_permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)     5683 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role_permissions.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     1428 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_users.py
+-rw-r--r--   0 rai        (501) staff       (20)     1428 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/organization_users.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3877 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)     3877 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/permissions.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3335 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/redirect_callback_urls.py
+-rw-r--r--   0 rai        (501) staff       (20)     3335 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/redirect_callback_urls.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3863 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/role.py
+-rw-r--r--   0 rai        (501) staff       (20)     3863 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/role.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3865 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/roles.py
+-rw-r--r--   0 rai        (501) staff       (20)     3865 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/roles.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5113 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/roles_permission_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5113 2024-02-28 08:24:36.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/roles_permission_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4083 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/subscriber.py
+-rw-r--r--   0 rai        (501) staff       (20)     4083 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/subscriber.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     4519 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/subscribers_subscriber.py
+-rw-r--r--   0 rai        (501) staff       (20)     4519 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/subscribers_subscriber.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     2914 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/success_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     2914 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/success_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     3063 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/token_error_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     3063 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/token_error_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5168 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/token_introspect.py
+-rw-r--r--   0 rai        (501) staff       (20)     5168 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/token_introspect.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     6663 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/update_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     6663 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/update_organization_users_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5898 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/update_role_permissions_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5898 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/update_role_permissions_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5878 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/update_user_response.py
+-rw-r--r--   0 rai        (501) staff       (20)     5878 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/update_user_response.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    16810 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user.py
+-rw-r--r--   0 rai        (501) staff       (20)    16810 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5176 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user_identity.py
+-rw-r--r--   0 rai        (501) staff       (20)     5176 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user_identity.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     5779 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)     5779 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     7198 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile_v2.py
+-rw-r--r--   0 rai        (501) staff       (20)     7198 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile_v2.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     1340 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/users.py
+-rw-r--r--   0 rai        (501) staff       (20)     1340 2024-02-28 08:24:37.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/users.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    27704 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)    27704 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/model/users_response.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.374624 kinde_python_sdk-1.2.4/kinde_sdk/models/
+-rw-r--r--   0 rai        (501) staff       (20)     4005 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/models/__init__.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.374892 kinde_python_sdk-1.2.4/kinde_sdk/paths/
+-rw-r--r--   0 rai        (501) staff       (20)     3515 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/__init__.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.378457 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/
+-rw-r--r--   0 rai        (501) staff       (20)      299 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     9822 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/get.py
+-rw-r--r--   0 rai        (501) staff       (20)     9616 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    16268 2024-02-28 08:24:38.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    16062 2024-02-28 08:24:38.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.379633 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/
+-rw-r--r--   0 rai        (501) staff       (20)      313 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11883 2024-02-28 08:24:38.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11677 2024-02-28 08:24:38.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    11789 2024-02-28 08:24:38.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11583 2024-02-28 08:24:38.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.380505 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id_applications/
+-rw-r--r--   0 rai        (501) staff       (20)      339 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id_applications/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    22556 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    22350 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.381772 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/
+-rw-r--r--   0 rai        (501) staff       (20)      315 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12885 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    12709 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    16879 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    16436 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.384280 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/
+-rw-r--r--   0 rai        (501) staff       (20)      363 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13921 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    13715 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    11447 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11241 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    18219 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    18013 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    17993 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.py
+-rw-r--r--   0 rai        (501) staff       (20)    17787 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.386670 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/
+-rw-r--r--   0 rai        (501) staff       (20)      367 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13945 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    13739 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    11479 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11273 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    18247 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    18041 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    18021 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.py
+-rw-r--r--   0 rai        (501) staff       (20)    17815 2024-02-28 08:24:41.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.388674 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/
+-rw-r--r--   0 rai        (501) staff       (20)      345 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11819 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11613 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    11519 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11313 2024-02-28 08:24:39.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    20705 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    20499 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.390084 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/
+-rw-r--r--   0 rai        (501) staff       (20)      307 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13665 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13489 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    16454 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    16248 2024-02-28 08:24:40.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.391025 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_auth_url/
+-rw-r--r--   0 rai        (501) staff       (20)      337 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_auth_url/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13545 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13309 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.391884 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_revoke/
+-rw-r--r--   0 rai        (501) staff       (20)      333 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_revoke/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12582 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    12346 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_revoke/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.392799 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_token/
+-rw-r--r--   0 rai        (501) staff       (20)      331 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_token/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12280 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_token/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    12074 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_token/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.394257 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/
+-rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     9797 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)     9591 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)     9716 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/get.py
+-rw-r--r--   0 rai        (501) staff       (20)     9510 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.395653 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      375 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11827 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11621 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    17958 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    17752 2024-02-28 08:24:42.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.396494 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags/
+-rw-r--r--   0 rai        (501) staff       (20)      317 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    19617 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    18935 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.400331 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      351 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11566 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11360 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    15759 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py
+-rw-r--r--   0 rai        (501) staff       (20)    15295 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.403473 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_industries/
+-rw-r--r--   0 rai        (501) staff       (20)      311 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_industries/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    10834 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_industries/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    10658 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_industries/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.406355 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/
+-rw-r--r--   0 rai        (501) staff       (20)      315 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11598 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11392 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    25577 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    25038 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.408954 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/
+-rw-r--r--   0 rai        (501) staff       (20)      333 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    10958 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    10752 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    25315 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    25109 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.411239 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations/
+-rw-r--r--   0 rai        (501) staff       (20)      317 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13177 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13001 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.413412 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/
+-rw-r--r--   0 rai        (501) staff       (20)      363 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11787 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11581 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    11710 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11504 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.416075 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      397 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12115 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11909 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    14275 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    14069 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.418530 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/
+-rw-r--r--   0 rai        (501) staff       (20)      347 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    16668 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    16462 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    26157 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    25951 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    25893 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    25657 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.419491 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/
+-rw-r--r--   0 rai        (501) staff       (20)      363 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11853 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11647 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.421009 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/
+-rw-r--r--   0 rai        (501) staff       (20)      387 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13729 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13553 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    17315 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    17139 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.421830 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/
+-rw-r--r--   0 rai        (501) staff       (20)      415 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12306 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    12100 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.423066 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/
+-rw-r--r--   0 rai        (501) staff       (20)      375 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11100 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    10924 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    17153 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    16977 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.423882 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/
+-rw-r--r--   0 rai        (501) staff       (20)      391 2024-02-28 08:24:46.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12192 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11986 2024-02-28 08:24:45.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.425218 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/
+-rw-r--r--   0 rai        (501) staff       (20)      313 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13669 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13493 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    16493 2024-02-28 08:24:47.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    16287 2024-02-28 08:24:47.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.426703 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/
+-rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11525 2024-02-28 08:24:47.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11319 2024-02-28 08:24:47.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    18752 2024-02-28 08:24:47.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    18546 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.428053 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/
+-rw-r--r--   0 rai        (501) staff       (20)      301 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13573 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13397 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    17409 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    17233 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.429730 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/
+-rw-r--r--   0 rai        (501) staff       (20)      317 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11411 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11205 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    19260 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    19054 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.431028 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/
+-rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    16000 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    15794 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    21634 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    21458 2024-02-28 08:24:48.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.431858 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/
+-rw-r--r--   0 rai        (501) staff       (20)      369 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11864 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11658 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.433600 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/
+-rw-r--r--   0 rai        (501) staff       (20)      313 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13228 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13052 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    12914 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    12708 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.434443 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers_subscriber_id/
+-rw-r--r--   0 rai        (501) staff       (20)      341 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers_subscriber_id/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11307 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11101 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.435863 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_timezones/
+-rw-r--r--   0 rai        (501) staff       (20)      309 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_timezones/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    10821 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_timezones/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    10645 2024-02-28 08:24:49.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_timezones/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.438871 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/
+-rw-r--r--   0 rai        (501) staff       (20)      299 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    11923 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/delete.py
+-rw-r--r--   0 rai        (501) staff       (20)    11717 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/delete.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    12184 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    11978 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    19628 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    19422 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/patch.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    27927 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    27436 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.439677 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users/
+-rw-r--r--   0 rai        (501) staff       (20)      301 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    13769 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users/get.py
+-rw-r--r--   0 rai        (501) staff       (20)    13593 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.440763 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/
+-rw-r--r--   0 rai        (501) staff       (20)      379 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    14172 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.py
+-rw-r--r--   0 rai        (501) staff       (20)    13966 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.441546 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/
+-rw-r--r--   0 rai        (501) staff       (20)      347 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    12006 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    11800 2024-02-28 08:24:50.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.442629 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_introspect/
+-rw-r--r--   0 rai        (501) staff       (20)      311 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_introspect/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    16620 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_introspect/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    16414 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_introspect/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.445216 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_revoke/
+-rw-r--r--   0 rai        (501) staff       (20)      303 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_revoke/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    16603 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_revoke/post.py
+-rw-r--r--   0 rai        (501) staff       (20)    16397 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_revoke/post.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.446018 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_user_profile/
+-rw-r--r--   0 rai        (501) staff       (20)      315 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_user_profile/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     7922 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_user_profile/get.py
+-rw-r--r--   0 rai        (501) staff       (20)     7776 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_user_profile/get.pyi
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.446945 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_v2_user_profile/
+-rw-r--r--   0 rai        (501) staff       (20)      321 2024-02-28 08:24:44.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_v2_user_profile/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     8381 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_v2_user_profile/get.py
+-rw-r--r--   0 rai        (501) staff       (20)     8205 2024-02-28 08:24:43.000000 kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_v2_user_profile/get.pyi
+-rw-r--r--   0 rai        (501) staff       (20)    10552 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/rest.py
+-rw-r--r--   0 rai        (501) staff       (20)    97655 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/schemas.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.447432 kinde_python_sdk-1.2.4/kinde_sdk/test/
+-rw-r--r--   0 rai        (501) staff       (20)        0 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)    61679 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_kinde_api_client.py
+drwxr-xr-x   0 rai        (501) staff       (20)        0 2024-05-12 23:30:48.460877 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/
+-rw-r--r--   0 rai        (501) staff       (20)        0 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/__init__.py
+-rw-r--r--   0 rai        (501) staff       (20)     1017 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_add_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      517 2024-02-28 07:27:30.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_api.py
+-rw-r--r--   0 rai        (501) staff       (20)      844 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_api_result.py
+-rw-r--r--   0 rai        (501) staff       (20)      521 2024-02-28 07:27:30.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_apis.py
+-rw-r--r--   0 rai        (501) staff       (20)      553 2024-02-28 07:27:30.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_applications.py
+-rw-r--r--   0 rai        (501) staff       (20)      995 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_connected_apps_access_token.py
+-rw-r--r--   0 rai        (501) staff       (20)      905 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_connected_apps_auth_url.py
+-rw-r--r--   0 rai        (501) staff       (20)      607 2024-02-28 07:27:31.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_application_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      611 2024-02-28 07:27:31.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_organization_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      632 2024-02-28 07:27:31.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_subscriber_success_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      886 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_user_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      801 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_error.py
+-rw-r--r--   0 rai        (501) staff       (20)      943 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_error_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      595 2024-02-28 07:27:31.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_application_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      599 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_applications_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      645 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_environment_feature_flags_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      649 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organization_feature_flags_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      620 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      942 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organizations_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      665 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organizations_user_permissions_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      641 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organizations_user_roles_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      595 2024-02-28 09:18:20.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_permissions_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      633 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_redirect_callback_urls_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      571 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_roles_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      591 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_subscriber_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      595 2024-02-28 07:27:32.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_subscribers_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      579 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_logout_redirect_urls.py
+-rw-r--r--   0 rai        (501) staff       (20)      850 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization.py
+-rw-r--r--   0 rai        (501) staff       (20)      866 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user.py
+-rw-r--r--   0 rai        (501) staff       (20)      611 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user_permission.py
+-rw-r--r--   0 rai        (501) staff       (20)      587 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user_role.py
+-rw-r--r--   0 rai        (501) staff       (20)      632 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user_role_permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)      575 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      549 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_permissions.py
+-rw-r--r--   0 rai        (501) staff       (20)      587 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_redirect_callback_urls.py
+-rw-r--r--   0 rai        (501) staff       (20)      521 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_role.py
+-rw-r--r--   0 rai        (501) staff       (20)      525 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_roles.py
+-rw-r--r--   0 rai        (501) staff       (20)      599 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_roles_permission_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      545 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_subscriber.py
+-rw-r--r--   0 rai        (501) staff       (20)      590 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_subscribers_subscriber.py
+-rw-r--r--   0 rai        (501) staff       (20)      907 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_success_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      579 2024-02-28 07:27:33.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_token_error_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      566 2024-02-28 07:27:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_token_introspect.py
+-rw-r--r--   0 rai        (501) staff       (20)      632 2024-02-28 07:27:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_update_organization_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      624 2024-02-28 07:27:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_update_role_permissions_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      579 2024-02-28 07:27:34.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_update_user_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      780 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user.py
+-rw-r--r--   0 rai        (501) staff       (20)      852 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user_identity.py
+-rw-r--r--   0 rai        (501) staff       (20)      831 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user_profile.py
+-rw-r--r--   0 rai        (501) staff       (20)      847 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user_profile_v2.py
+-rw-r--r--   0 rai        (501) staff       (20)      526 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_users.py
+-rw-r--r--   0 rai        (501) staff       (20)      858 2024-02-28 08:24:51.000000 kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_users_response.py
+-rw-r--r--   0 rai        (501) staff       (20)      958 2024-05-12 23:29:48.000000 kinde_python_sdk-1.2.4/pyproject.toml
+-rw-r--r--   0 rai        (501) staff       (20)       38 2024-05-12 23:30:48.462099 kinde_python_sdk-1.2.4/setup.cfg
```

### Comparing `kinde-python-sdk-1.2.3/LICENSE` & `kinde_python_sdk-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/PKG-INFO` & `kinde_python_sdk-1.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kinde-python-sdk
-Version: 1.2.3
+Version: 1.2.4
 Summary: Connect your app to the Kinde platform
 Author-email: Kinde Engineering <engineering@kinde.com>
 Project-URL: Homepage, https://github.com/kinde-oss/kinde-python-sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: urllib3~=2.0.3
-Requires-Dist: python-dateutil~=2.8.2
-Requires-Dist: Authlib~=1.2.0
+Requires-Dist: urllib3~=2.2.1
+Requires-Dist: python-dateutil~=2.9.0.post0
+Requires-Dist: Authlib~=1.3.0
 Requires-Dist: pyjwt~=2.8.0
 Requires-Dist: requests~=2.31.0
-Requires-Dist: typing-extensions~=4.8.0
-Requires-Dist: frozendict~=2.3.8
-Requires-Dist: certifi~=2022.12.7
+Requires-Dist: typing-extensions~=4.11.0
+Requires-Dist: frozendict~=2.4.3
+Requires-Dist: certifi~=2024.2.2
 
 # Kinde Python SDK
 
 The Kinde SDK for Python.
 
 You can also use the [Python starter kit here](https://github.com/kinde-starter-kits/python-starter-kit).
```

### Comparing `kinde-python-sdk-1.2.3/README.md` & `kinde_python_sdk-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/PKG-INFO` & `kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kinde-python-sdk
-Version: 1.2.3
+Version: 1.2.4
 Summary: Connect your app to the Kinde platform
 Author-email: Kinde Engineering <engineering@kinde.com>
 Project-URL: Homepage, https://github.com/kinde-oss/kinde-python-sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: urllib3~=2.0.3
-Requires-Dist: python-dateutil~=2.8.2
-Requires-Dist: Authlib~=1.2.0
+Requires-Dist: urllib3~=2.2.1
+Requires-Dist: python-dateutil~=2.9.0.post0
+Requires-Dist: Authlib~=1.3.0
 Requires-Dist: pyjwt~=2.8.0
 Requires-Dist: requests~=2.31.0
-Requires-Dist: typing-extensions~=4.8.0
-Requires-Dist: frozendict~=2.3.8
-Requires-Dist: certifi~=2022.12.7
+Requires-Dist: typing-extensions~=4.11.0
+Requires-Dist: frozendict~=2.4.3
+Requires-Dist: certifi~=2024.2.2
 
 # Kinde Python SDK
 
 The Kinde SDK for Python.
 
 You can also use the [Python starter kit here](https://github.com/kinde-starter-kits/python-starter-kit).
```

### Comparing `kinde-python-sdk-1.2.3/kinde_python_sdk.egg-info/SOURCES.txt` & `kinde_python_sdk-1.2.4/kinde_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/__init__.py` & `kinde_python_sdk-1.2.4/kinde_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/api_client.py` & `kinde_python_sdk-1.2.4/kinde_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/path_to_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tag_to_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/__init__.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/apis_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/apis_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/applications_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/applications_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/business_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/business_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/callbacks_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/callbacks_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/connected_apps_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/connected_apps_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/environments_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/environments_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/feature_flags_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/feature_flags_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/o_auth_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/o_auth_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/organizations_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/organizations_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/permissions_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/permissions_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/roles_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/roles_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/subscribers_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/subscribers_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/apis/tags/users_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/apis/tags/users_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/configuration.py` & `kinde_python_sdk-1.2.4/kinde_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/exceptions.py` & `kinde_python_sdk-1.2.4/kinde_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/kinde_api_client.py` & `kinde_python_sdk-1.2.4/kinde_sdk/kinde_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 from kinde_sdk.exceptions import (
     KindeConfigurationException,
     KindeLoginException,
     KindeTokenException,
     KindeRetrieveException,
 )
 from kinde_sdk import __version__ as kinde_sdk_version
+import logging
 
+def debug(msg):
+    if logging.getLogger().getEffectiveLevel() == logging.DEBUG:
+        logging.debug(msg)
 
 class FlagType(Enum):
     s = "string"
     i = "integer"
     b = "boolean"
 
 
@@ -128,14 +132,16 @@
     def get_claim(self, key: str, token_name: str = "access_token") -> Any:
         if token_name not in self.TOKEN_NAMES:
             raise KindeTokenException(
                 f"Please use only tokens from the list: {self.TOKEN_NAMES}"
             )
         self._decode_token_if_needed(token_name)
         value = self.__decoded_tokens[token_name].get(key)
+        if value is None:
+            debug(f"The claimed value of '{key}' does not exist in your token")
         return {"name": key, "value": value}
 
     def get_permission(self, permission: str) -> Dict[str, Any]:
         return {
             "org_code": self.get_claim("org_code")["value"],
             "is_granted": permission in self.get_claim("permissions")["value"],
         }
```

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/add_organization_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/add_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/add_organization_users_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/add_organization_users_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/api.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/api.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/api_result.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/api_result.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/api_result.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/api_result.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/apis.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/apis.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/apis.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/apis.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/applications.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/applications.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/applications.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/applications.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_access_token.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_access_token.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_access_token.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_access_token.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_auth_url.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_auth_url.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/connected_apps_auth_url.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/connected_apps_auth_url.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_application_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_application_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_application_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_application_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_organization_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_organization_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_organization_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_subscriber_success_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_subscriber_success_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_subscriber_success_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_subscriber_success_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_user_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_user_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/create_user_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/create_user_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/error.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/error.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/error.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/error.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/error_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/error_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/error_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/error_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_application_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_application_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_application_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_application_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_applications_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_applications_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_applications_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_applications_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_environment_feature_flags_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_environment_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_environment_feature_flags_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_environment_feature_flags_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_feature_flags_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_feature_flags_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_feature_flags_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organization_users_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organization_users_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_permissions_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_permissions_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_permissions_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_permissions_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_roles_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_organizations_user_roles_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_organizations_user_roles_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_permissions_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_permissions_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_permissions_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_permissions_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_redirect_callback_urls_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_redirect_callback_urls_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_redirect_callback_urls_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_redirect_callback_urls_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_roles_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_roles_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_roles_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_roles_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscriber_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscriber_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscriber_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscriber_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscribers_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscribers_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/get_subscribers_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/get_subscribers_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/logout_redirect_urls.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/logout_redirect_urls.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/logout_redirect_urls.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/logout_redirect_urls.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_permission.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_permission.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_permission.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_permission.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role_permissions.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role_permissions.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_user_role_permissions.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_user_role_permissions.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_users.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_users.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/organization_users.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/organization_users.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/permissions.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/permissions.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/permissions.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/permissions.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/redirect_callback_urls.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/redirect_callback_urls.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/redirect_callback_urls.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/redirect_callback_urls.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/role.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/role.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/role.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/role.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/roles.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/roles.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/roles.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/roles.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/roles_permission_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/roles_permission_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/roles_permission_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/roles_permission_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/subscriber.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/subscriber.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/subscriber.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/subscriber.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/subscribers_subscriber.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/subscribers_subscriber.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/subscribers_subscriber.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/subscribers_subscriber.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/success_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/success_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/success_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/success_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/token_error_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/token_error_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/token_error_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/token_error_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/token_introspect.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/token_introspect.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/token_introspect.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/token_introspect.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/update_organization_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/update_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/update_organization_users_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/update_organization_users_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/update_role_permissions_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/update_role_permissions_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/update_role_permissions_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/update_role_permissions_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/update_user_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/update_user_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/update_user_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/update_user_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user_identity.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user_identity.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user_identity.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user_identity.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile_v2.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile_v2.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/user_profile_v2.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/user_profile_v2.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/users.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/users.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/users.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/users.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/model/users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/model/users_response.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/model/users_response.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/models/__init__.py` & `kinde_python_sdk-1.2.4/kinde_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/__init__.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_apis_api_id_applications/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_logout_urls/put.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_app_id_auth_redirect_urls/put.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_applications_application_id/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_applications_application_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_business/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_business/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_auth_url/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_revoke/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_revoke/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_revoke/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_token/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_token/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_connected_apps_token/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_connected_apps_token/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_environment_feature_flags_feature_flag_key/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_feature_flags_feature_flag_key/put.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_industries/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_industries/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_industries/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_industries/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organization_org_code/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organization_org_code/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_feature_flags_feature_flag_key/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_permissions_permission_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_organizations_org_code_users_user_id_roles_role_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_permissions_permission_id/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_permissions_permission_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_roles_role_id_permissions_permission_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_subscribers_subscriber_id/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_timezones/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_timezones/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_timezones/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_timezones/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/delete.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/delete.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/delete.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/delete.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_user/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_user/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_feature_flags_feature_flag_key/patch.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/api_v1_users_user_id_refresh_claims/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_introspect/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_introspect/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_introspect/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_introspect/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_revoke/post.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_revoke/post.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_revoke/post.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_revoke/post.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_user_profile/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_user_profile/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_user_profile/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_user_profile/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_v2_user_profile/get.py` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_v2_user_profile/get.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/paths/oauth2_v2_user_profile/get.pyi` & `kinde_python_sdk-1.2.4/kinde_sdk/paths/oauth2_v2_user_profile/get.pyi`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/rest.py` & `kinde_python_sdk-1.2.4/kinde_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/schemas.py` & `kinde_python_sdk-1.2.4/kinde_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_kinde_api_client.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_kinde_api_client.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_add_organization_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_add_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_api.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_api.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_api_result.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_api_result.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_apis.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_apis.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_applications.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_applications.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_connected_apps_access_token.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_connected_apps_access_token.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_connected_apps_auth_url.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_connected_apps_auth_url.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_application_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_application_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_organization_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_organization_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_subscriber_success_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_subscriber_success_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_create_user_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_create_user_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_error.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_error.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_error_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_application_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_application_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_applications_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_applications_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_environment_feature_flags_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_environment_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organization_feature_flags_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organization_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organization_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organizations_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organizations_user_permissions_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organizations_user_permissions_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_organizations_user_roles_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_organizations_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_permissions_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_permissions_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_redirect_callback_urls_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_redirect_callback_urls_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_roles_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_roles_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_subscriber_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_subscriber_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_get_subscribers_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_get_subscribers_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_logout_redirect_urls.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_logout_redirect_urls.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user_permission.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user_permission.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user_role.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user_role.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_user_role_permissions.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_user_role_permissions.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_organization_users.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_organization_users.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_permissions.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_permissions.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_redirect_callback_urls.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_redirect_callback_urls.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_role.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_role.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_roles.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_roles.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_roles_permission_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_roles_permission_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_subscriber.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_subscribers_subscriber.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_subscribers_subscriber.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_success_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_success_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_token_error_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_token_error_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_token_introspect.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_token_introspect.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_update_organization_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_update_organization_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_update_role_permissions_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_update_role_permissions_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_update_user_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_update_user_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user_identity.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user_identity.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user_profile.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_user_profile_v2.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_user_profile_v2.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_users.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_users.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/kinde_sdk/test/test_models/test_users_response.py` & `kinde_python_sdk-1.2.4/kinde_sdk/test/test_models/test_users_response.py`

 * *Files identical despite different names*

### Comparing `kinde-python-sdk-1.2.3/pyproject.toml` & `kinde_python_sdk-1.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kinde-python-sdk"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
     { name = "Kinde Engineering", email = "engineering@kinde.com" },
 ]
 description = "Connect your app to the Kinde platform"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -13,21 +13,21 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "urllib3 ~=2.0.3",
-    "python-dateutil ~=2.8.2",
-    "Authlib ~=1.2.0",
+    "urllib3 ~=2.2.1",
+    "python-dateutil ~=2.9.0.post0",
+    "Authlib ~=1.3.0",
     "pyjwt ~=2.8.0",
     "requests ~=2.31.0",
-    "typing-extensions ~=4.8.0",
-    "frozendict ~=2.3.8",
-    "certifi ~=2022.12.7",
+    "typing-extensions ~=4.11.0",
+    "frozendict ~=2.4.3",
+    "certifi ~=2024.2.2",
 ]
 [project.urls]
 "Homepage" = "https://github.com/kinde-oss/kinde-python-sdk"
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
```

