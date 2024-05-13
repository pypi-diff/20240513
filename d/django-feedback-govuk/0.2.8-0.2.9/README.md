# Comparing `tmp/django_feedback_govuk-0.2.8.tar.gz` & `tmp/django_feedback_govuk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feedback_govuk-0.2.8.tar", max compression
+gzip compressed data, was "django_feedback_govuk-0.2.9.tar", max compression
```

## Comparing `django_feedback_govuk-0.2.8.tar` & `django_feedback_govuk-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.2.8/LICENSE
--rw-r--r--   0        0        0     8244 2023-08-22 10:39:21.456724 django_feedback_govuk-0.2.8/README.md
--rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.2.8/django_feedback_govuk/__init__.py
--rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.2.8/django_feedback_govuk/admin.py
--rw-r--r--   0        0        0      172 2023-08-09 13:00:16.881231 django_feedback_govuk-0.2.8/django_feedback_govuk/apps.py
--rw-r--r--   0        0        0     2226 2023-08-09 15:37:32.470389 django_feedback_govuk-0.2.8/django_feedback_govuk/forms.py
--rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0001_initial.py
--rw-r--r--   0        0        0      661 2023-08-22 10:39:21.451783 django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
--rw-r--r--   0        0        0     4404 2023-08-11 13:33:58.339102 django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0003_restructure_feedback.py
--rw-r--r--   0        0        0      495 2023-08-22 10:39:21.451846 django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0004_alter_basefeedback_id.py
--rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/__init__.py
--rw-r--r--   0        0        0      967 2023-08-04 15:03:25.339404 django_feedback_govuk-0.2.8/django_feedback_govuk/models.py
--rw-r--r--   0        0        0     2709 2023-08-22 10:39:21.455044 django_feedback_govuk-0.2.8/django_feedback_govuk/settings.py
--rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.2.8/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
--rw-r--r--   0        0        0     2808 2023-08-22 10:39:21.452728 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
--rw-r--r--   0        0        0      245 2023-08-10 10:57:30.145939 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
--rw-r--r--   0        0        0     1262 2023-08-07 14:54:31.051907 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
--rw-r--r--   0        0        0      434 2023-08-10 10:56:56.527121 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
--rw-r--r--   0        0        0      656 2023-08-08 13:19:15.633440 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html
--rw-r--r--   0        0        0       64 2023-08-22 10:39:21.452297 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
--rw-r--r--   0        0        0      170 2023-08-07 14:19:10.227646 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
--rw-r--r--   0        0        0       63 2023-08-07 09:56:47.682637 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
--rw-r--r--   0        0        0       50 2023-08-07 14:57:13.037656 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/templates/submitted.html
--rw-r--r--   0        0        0     1955 2023-08-22 10:39:21.453515 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
--rw-r--r--   0        0        0     1811 2023-08-22 10:39:21.453515 django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
--rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.2.8/django_feedback_govuk/templatetags/__init__.py
--rw-r--r--   0        0        0     2467 2023-08-10 10:57:41.165716 django_feedback_govuk-0.2.8/django_feedback_govuk/templatetags/feedback_tags.py
--rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.2.8/django_feedback_govuk/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.2.8/django_feedback_govuk/tests/factories.py
--rw-r--r--   0        0        0     1923 2023-08-07 15:42:14.291502 django_feedback_govuk-0.2.8/django_feedback_govuk/tests/settings.py
--rw-r--r--   0        0        0     1964 2023-08-08 12:54:38.518706 django_feedback_govuk-0.2.8/django_feedback_govuk/tests/test_views.py
--rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.2.8/django_feedback_govuk/tests/urls.py
--rw-r--r--   0        0        0      742 2023-08-09 15:34:49.961645 django_feedback_govuk-0.2.8/django_feedback_govuk/urls.py
--rw-r--r--   0        0        0     5297 2023-08-22 10:39:21.454988 django_feedback_govuk-0.2.8/django_feedback_govuk/views.py
--rw-r--r--   0        0        0     1850 2023-08-22 10:39:44.825546 django_feedback_govuk-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     9381 1970-01-01 00:00:00.000000 django_feedback_govuk-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.2.9/LICENSE
+-rw-r--r--   0        0        0     8244 2023-08-22 10:39:21.456724 django_feedback_govuk-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.2.9/django_feedback_govuk/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.2.9/django_feedback_govuk/admin.py
+-rw-r--r--   0        0        0      172 2023-08-09 13:00:16.881231 django_feedback_govuk-0.2.9/django_feedback_govuk/apps.py
+-rw-r--r--   0        0        0     2226 2023-08-09 15:37:32.470389 django_feedback_govuk-0.2.9/django_feedback_govuk/forms.py
+-rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0001_initial.py
+-rw-r--r--   0        0        0      661 2023-08-22 10:39:21.451783 django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
+-rw-r--r--   0        0        0     4404 2023-08-11 13:33:58.339102 django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0003_restructure_feedback.py
+-rw-r--r--   0        0        0      495 2023-08-22 10:39:21.451846 django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0004_alter_basefeedback_id.py
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/__init__.py
+-rw-r--r--   0        0        0      967 2023-08-04 15:03:25.339404 django_feedback_govuk-0.2.9/django_feedback_govuk/models.py
+-rw-r--r--   0        0        0     2709 2023-08-22 10:39:21.455044 django_feedback_govuk-0.2.9/django_feedback_govuk/settings.py
+-rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.2.9/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
+-rw-r--r--   0        0        0     2808 2023-08-22 10:39:21.452728 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
+-rw-r--r--   0        0        0      245 2023-08-10 10:57:30.145939 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
+-rw-r--r--   0        0        0     1262 2023-08-07 14:54:31.051907 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
+-rw-r--r--   0        0        0      434 2023-08-10 10:56:56.527121 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
+-rw-r--r--   0        0        0      656 2023-08-08 13:19:15.633440 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html
+-rw-r--r--   0        0        0       64 2023-08-22 10:39:21.452297 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
+-rw-r--r--   0        0        0      170 2023-08-07 14:19:10.227646 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
+-rw-r--r--   0        0        0       63 2023-08-07 09:56:47.682637 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
+-rw-r--r--   0        0        0       50 2023-08-07 14:57:13.037656 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/templates/submitted.html
+-rw-r--r--   0        0        0     1955 2023-08-22 10:39:21.453515 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
+-rw-r--r--   0        0        0     1811 2023-08-22 10:39:21.453515 django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
+-rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.2.9/django_feedback_govuk/templatetags/__init__.py
+-rw-r--r--   0        0        0     2470 2024-05-13 09:32:04.858877 django_feedback_govuk-0.2.9/django_feedback_govuk/templatetags/feedback_tags.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.2.9/django_feedback_govuk/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.2.9/django_feedback_govuk/tests/factories.py
+-rw-r--r--   0        0        0     1923 2023-08-07 15:42:14.291502 django_feedback_govuk-0.2.9/django_feedback_govuk/tests/settings.py
+-rw-r--r--   0        0        0     1964 2023-08-08 12:54:38.518706 django_feedback_govuk-0.2.9/django_feedback_govuk/tests/test_views.py
+-rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.2.9/django_feedback_govuk/tests/urls.py
+-rw-r--r--   0        0        0      742 2023-08-09 15:34:49.961645 django_feedback_govuk-0.2.9/django_feedback_govuk/urls.py
+-rw-r--r--   0        0        0     5297 2023-08-22 10:39:21.454988 django_feedback_govuk-0.2.9/django_feedback_govuk/views.py
+-rw-r--r--   0        0        0     1850 2024-05-13 09:32:04.863484 django_feedback_govuk-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     9432 1970-01-01 00:00:00.000000 django_feedback_govuk-0.2.9/PKG-INFO
```

### Comparing `django_feedback_govuk-0.2.8/LICENSE` & `django_feedback_govuk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/README.md` & `django_feedback_govuk-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/forms.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/forms.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0001_initial.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/migrations/0003_restructure_feedback.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/migrations/0003_restructure_feedback.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/models.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/models.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/settings.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/static/django_feedback_govuk/star-rating.css` & `django_feedback_govuk-0.2.9/django_feedback_govuk/static/django_feedback_govuk/star-rating.css`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html` & `django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html` & `django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html` & `django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html` & `django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html` & `django_feedback_govuk-0.2.9/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/templatetags/feedback_tags.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/templatetags/feedback_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     feedback_config = dfg_settings.FEEDBACK_FORMS[form_id]
     feedback_form = import_string(feedback_config["form"])
     if "form" in context:
         form = context["form"]
     else:
         if not initial:
             initial = {}
-        initial.update(submitter=context.request.user)
+        initial.update(submitter=context["request"].user)
 
         form = feedback_form(initial=initial)
 
     new_context = {
         "form": form,
         "form_id": form_id,
         "service_name": dfg_settings.SERVICE_NAME,
```

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/tests/settings.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/tests/test_views.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/urls.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/urls.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/django_feedback_govuk/views.py` & `django_feedback_govuk-0.2.9/django_feedback_govuk/views.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.8/pyproject.toml` & `django_feedback_govuk-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-feedback-govuk"
-version = "0.2.8"
+version = "0.2.9"
 description = "A Django app to gather and send internal Government staff feedback"
 authors = [
     "jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>",
     "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `django_feedback_govuk-0.2.8/PKG-INFO` & `django_feedback_govuk-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-feedback-govuk
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Django app to gather and send internal Government staff feedback
 License: MIT
 Author: jafacakes2011
 Author-email: cameron.lamb@digitial.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (>=3.2,<4.3)
 Requires-Dist: crispy-forms-gds (>=0.2.4,<0.3.0)
 Requires-Dist: django-crispy-forms (>=1.9,<2.0)
```

