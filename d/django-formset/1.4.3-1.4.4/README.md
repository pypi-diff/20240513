# Comparing `tmp/django_formset-1.4.3.tar.gz` & `tmp/django_formset-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_formset-1.4.3.tar", last modified: Wed May  8 15:18:58 2024, max compression
+gzip compressed data, was "django_formset-1.4.4.tar", last modified: Mon May 13 09:49:48 2024, max compression
```

## Comparing `django_formset-1.4.3.tar` & `django_formset-1.4.4.tar`

### file list

```diff
@@ -1,470 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 15:18:32.000000 django_formset-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 15:18:32.000000 django_formset-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-08 15:18:58.724098 django_formset-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-08 15:18:32.000000 django_formset-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 15:18:58.000000 django_formset-1.4.3/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.680098 django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/he_IL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.664098 django_formset-1.4.3/formset/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.684098 django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.688098 django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.668098 django_formset-1.4.3/formset/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/sr_Latn_BA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.692098 django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-08 15:18:54.000000 django_formset-1.4.3/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-08 15:18:55.000000 django_formset-1.4.3/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.696098 django_formset-1.4.3/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/Calendar-6GWQDXEH.js
--rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/CountrySelectize-SV3ETVIG.js
--rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DateTime-7RV5MOXB.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DjangoSelectize-FCAZIQIK.js
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DjangoSlug-SHZN726V.js
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/DualSelector-TFBRBEV6.js
--rw-r--r--   0 runner    (1001) docker     (127)   270424 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/PhoneNumber-XY2VHR24.js
--rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/RichtextArea-PVV6GJIQ.js
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/SortableSelect-3ABJOEP2.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-65OJRBX6.js
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-FDUUONAQ.js
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-IH7AT57W.js
--rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-NOGHTXP6.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-P2VM2T3G.js
--rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-R3EYKSPB.js
--rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-RLE6ONWJ.js
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-SERXULES.js
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-TRJBB73N.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-W5RPWA2M.js
--rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/chunk-YMY5H5XX.js
--rw-r--r--   0 runner    (1001) docker     (127)    64081 2024-05-08 15:18:56.000000 django_formset-1.4.3/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/static/formset/tiptap-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/footnote.js
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/procurator.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/simple_image.js
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/static/formset/tiptap-extensions/simple_link.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.676098 django_formset-1.4.3/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.672098 django_formset-1.4.3/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/range.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.704098 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.708098 django_formset-1.4.3/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/detached_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/calendar.html
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/country_selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.712098 django_formset-1.4.3/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/activator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/footnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/strike.svg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/align.html
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/color.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/control.html
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/dialog_control.html
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/richtext/separator.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.720098 django_formset-1.4.3/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/footnote.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/footnote_ref.html
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/footnotes_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/procurator.html
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/simple_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:58.724098 django_formset-1.4.3/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/phonenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-08 15:18:32.000000 django_formset-1.4.3/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:18:58.724098 django_formset-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-08 15:18:32.000000 django_formset-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.141835 django_formset-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-13 09:49:10.000000 django_formset-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 09:49:10.000000 django_formset-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-13 09:49:48.141835 django_formset-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-13 09:49:10.000000 django_formset-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.141835 django_formset-1.4.4/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-13 09:49:48.000000 django_formset-1.4.4/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-13 09:49:48.000000 django_formset-1.4.4/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:49:48.000000 django_formset-1.4.4/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:49:47.000000 django_formset-1.4.4/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 09:49:48.000000 django_formset-1.4.4/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 09:49:48.000000 django_formset-1.4.4/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.065835 django_formset-1.4.4/formset/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/af/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.065835 django_formset-1.4.4/formset/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.065835 django_formset-1.4.4/formset/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/bg/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.065835 django_formset-1.4.4/formset/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/ca/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.065835 django_formset-1.4.4/formset/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.085835 django_formset-1.4.4/formset/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/da/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/et/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/eu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/fi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.089835 django_formset-1.4.4/formset/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/he_IL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/he_IL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/hr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/hr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/hu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/hy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/hy/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.069835 django_formset-1.4.4/formset/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/ja/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/lt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.093834 django_formset-1.4.4/formset/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.097835 django_formset-1.4.4/formset/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/sr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/sr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/sr_Latn_BA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/sr_Latn_BA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.073835 django_formset-1.4.4/formset/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.101835 django_formset-1.4.4/formset/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-13 09:49:46.000000 django_formset-1.4.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.105835 django_formset-1.4.4/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.105835 django_formset-1.4.4/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.105835 django_formset-1.4.4/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-13 09:49:43.000000 django_formset-1.4.4/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 09:49:43.000000 django_formset-1.4.4/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-13 09:49:43.000000 django_formset-1.4.4/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-13 09:49:43.000000 django_formset-1.4.4/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-13 09:49:44.000000 django_formset-1.4.4/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.105835 django_formset-1.4.4/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.113834 django_formset-1.4.4/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/Calendar-TWTCQYBD.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/CountrySelectize-JKM7Q3A2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/DateTime-WWADX7D6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/DjangoSelectize-7RDFNLMN.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/DjangoSlug-SHZN726V.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/DualSelector-XUGCVBT5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   270325 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/PhoneNumber-FXLXZ74J.js
+-rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/RichtextArea-LQJSGPD7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/SortableSelect-UDJCCTN4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-3FM5H3DO.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-54ILQ33N.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-65OJRBX6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-FDUUONAQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-IUS6Z5AU.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-MC5NQ26F.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-NOGHTXP6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-P2VM2T3G.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-RLE6ONWJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-SERXULES.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/chunk-W5RPWA2M.js
+-rw-r--r--   0 runner    (1001) docker     (127)    64081 2024-05-13 09:49:45.000000 django_formset-1.4.4/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.113834 django_formset-1.4.4/formset/static/formset/tiptap-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/tiptap-extensions/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/tiptap-extensions/procurator.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/tiptap-extensions/simple_image.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/static/formset/tiptap-extensions/simple_link.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.081835 django_formset-1.4.4/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.077835 django_formset-1.4.4/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.113834 django_formset-1.4.4/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.113834 django_formset-1.4.4/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/calendar/range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.113834 django_formset-1.4.4/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.113834 django_formset-1.4.4/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.117835 django_formset-1.4.4/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.117835 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.117835 django_formset-1.4.4/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.117835 django_formset-1.4.4/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.117835 django_formset-1.4.4/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.117835 django_formset-1.4.4/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.121835 django_formset-1.4.4/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/detached_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.121835 django_formset-1.4.4/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/country_selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.121835 django_formset-1.4.4/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.121835 django_formset-1.4.4/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.125835 django_formset-1.4.4/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.133834 django_formset-1.4.4/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/activator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/footnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/strike.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.133834 django_formset-1.4.4/formset/templates/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/dialog_control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/richtext/separator.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.133834 django_formset-1.4.4/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.133834 django_formset-1.4.4/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.133834 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.133834 django_formset-1.4.4/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.137835 django_formset-1.4.4/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.137835 django_formset-1.4.4/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.137835 django_formset-1.4.4/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/footnote.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/footnote_ref.html
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/footnotes_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.141835 django_formset-1.4.4/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/procurator.html
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/simple_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:48.141835 django_formset-1.4.4/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templatetags/phonenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-13 09:49:10.000000 django_formset-1.4.4/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:49:48.141835 django_formset-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-13 09:49:10.000000 django_formset-1.4.4/setup.py
```

### Comparing `django_formset-1.4.3/LICENSE` & `django_formset-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/PKG-INFO` & `django_formset-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4.3
+Version: 1.4.4
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4.3/README.md` & `django_formset-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/django_formset.egg-info/PKG-INFO` & `django_formset-1.4.4/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4.3
+Version: 1.4.4
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4.3/django_formset.egg-info/SOURCES.txt` & `django_formset-1.4.4/django_formset.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -136,34 +136,34 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/Calendar-6GWQDXEH.js
-formset/static/formset/js/CountrySelectize-SV3ETVIG.js
-formset/static/formset/js/DateTime-7RV5MOXB.js
-formset/static/formset/js/DjangoSelectize-FCAZIQIK.js
+formset/static/formset/js/Calendar-TWTCQYBD.js
+formset/static/formset/js/CountrySelectize-JKM7Q3A2.js
+formset/static/formset/js/DateTime-WWADX7D6.js
+formset/static/formset/js/DjangoSelectize-7RDFNLMN.js
 formset/static/formset/js/DjangoSlug-SHZN726V.js
-formset/static/formset/js/DualSelector-TFBRBEV6.js
-formset/static/formset/js/PhoneNumber-XY2VHR24.js
-formset/static/formset/js/RichtextArea-PVV6GJIQ.js
-formset/static/formset/js/SortableSelect-3ABJOEP2.js
+formset/static/formset/js/DualSelector-XUGCVBT5.js
+formset/static/formset/js/PhoneNumber-FXLXZ74J.js
+formset/static/formset/js/RichtextArea-LQJSGPD7.js
+formset/static/formset/js/SortableSelect-UDJCCTN4.js
+formset/static/formset/js/chunk-3FM5H3DO.js
+formset/static/formset/js/chunk-54ILQ33N.js
 formset/static/formset/js/chunk-65OJRBX6.js
 formset/static/formset/js/chunk-FDUUONAQ.js
-formset/static/formset/js/chunk-IH7AT57W.js
+formset/static/formset/js/chunk-IUS6Z5AU.js
+formset/static/formset/js/chunk-MC5NQ26F.js
 formset/static/formset/js/chunk-NOGHTXP6.js
 formset/static/formset/js/chunk-P2VM2T3G.js
-formset/static/formset/js/chunk-R3EYKSPB.js
 formset/static/formset/js/chunk-RLE6ONWJ.js
 formset/static/formset/js/chunk-SERXULES.js
-formset/static/formset/js/chunk-TRJBB73N.js
 formset/static/formset/js/chunk-W5RPWA2M.js
-formset/static/formset/js/chunk-YMY5H5XX.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/tiptap-extensions/footnote.js
 formset/static/formset/tiptap-extensions/procurator.js
 formset/static/formset/tiptap-extensions/simple_image.js
 formset/static/formset/tiptap-extensions/simple_link.js
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
```

### Comparing `django_formset-1.4.3/formset/boundfield.py` & `django_formset-1.4.4/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/calendar.py` & `django_formset-1.4.4/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/collection.py` & `django_formset-1.4.4/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/dialog.py` & `django_formset-1.4.4/formset/dialog.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/fields.py` & `django_formset-1.4.4/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/fieldset.py` & `django_formset-1.4.4/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/af/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/af/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/af/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ar/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/bg/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ca/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/cs/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/da/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/da/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.mo` & `django_formset-1.4.4/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/django.po` & `django_formset-1.4.4/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/de/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/el/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/eo/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/es/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/et/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/et/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/eu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/eu_ES/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/fa/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/fi/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/fr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/he/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/he_IL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/he_IL/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/hr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/hr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/hr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/hu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/hy/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/hy/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/hy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/it/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/ja/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ja/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ko_KR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/lt/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/lv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/mn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/nb/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/nl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/pl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/pt_PT/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ro/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/ru/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/sr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/sr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/sv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/tr_TR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/uk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/zh_CN/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `django_formset-1.4.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/ranges.py` & `django_formset-1.4.4/formset/ranges.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/__init__.py` & `django_formset-1.4.4/formset/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/bootstrap.py` & `django_formset-1.4.4/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/bulma.py` & `django_formset-1.4.4/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/default.py` & `django_formset-1.4.4/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/foundation.py` & `django_formset-1.4.4/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/tailwind.py` & `django_formset-1.4.4/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/renderers/uikit.py` & `django_formset-1.4.4/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/richtext/controls.py` & `django_formset-1.4.4/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/richtext/dialogs.py` & `django_formset-1.4.4/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/richtext/widgets.py` & `django_formset-1.4.4/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css` & `django_formset-1.4.4/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/css/bootstrap5-extra.css.map` & `django_formset-1.4.4/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/css/collections.css` & `django_formset-1.4.4/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/css/tailwind.css` & `django_formset-1.4.4/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-audio.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-empty.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-font.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-missing.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-pdf.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-picture.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-unknown.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-video.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/icons/file-zip.svg` & `django_formset-1.4.4/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/CountrySelectize-SV3ETVIG.js` & `django_formset-1.4.4/formset/static/formset/js/CountrySelectize-JKM7Q3A2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as c
-} from "./chunk-R3EYKSPB.js";
+} from "./chunk-IUS6Z5AU.js";
 import "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as r
 } from "./chunk-FDUUONAQ.js";
 import "./chunk-65OJRBX6.js";
 import {
```

### Comparing `django_formset-1.4.3/formset/static/formset/js/DateTime-7RV5MOXB.js` & `django_formset-1.4.4/formset/static/formset/js/DateTime-WWADX7D6.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as v
-} from "./chunk-TRJBB73N.js";
+} from "./chunk-MC5NQ26F.js";
 import {
     b as m
 } from "./chunk-W5RPWA2M.js";
 import {
     a as x,
     c as f,
     d as g,
```

### Comparing `django_formset-1.4.3/formset/static/formset/js/DjangoSlug-SHZN726V.js` & `django_formset-1.4.4/formset/static/formset/js/DjangoSlug-SHZN726V.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/DualSelector-TFBRBEV6.js` & `django_formset-1.4.4/formset/static/formset/js/DualSelector-XUGCVBT5.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as p
-} from "./chunk-IH7AT57W.js";
+} from "./chunk-3FM5H3DO.js";
 import "./chunk-NOGHTXP6.js";
 import {
     a as v
 } from "./chunk-FDUUONAQ.js";
 import {
     a as r
 } from "./chunk-65OJRBX6.js";
```

### Comparing `django_formset-1.4.3/formset/static/formset/js/PhoneNumber-XY2VHR24.js` & `django_formset-1.4.4/formset/static/formset/js/PhoneNumber-FXLXZ74J.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2958,79 +2958,79 @@
             [
                 ["(\\d)(\\d{4})(\\d{4})", "$1 $2 $3", ["[1359]"]]
             ], 0, 0, 0, 0, 0, 0, [0, 0, 0, ["[1359]\\d{8}"]]
         ]
     }
 };
 
-function I(e, t) {
-    var d = Array.prototype.slice.call(t);
+function S(e, a) {
+    var d = Array.prototype.slice.call(a);
     return d.push(R), e.apply(this, d)
 }
 var bd = 3,
     k = "0-9\uFF10-\uFF19\u0660-\u0669\u06F0-\u06F9",
     f0 = "-\u2010-\u2015\u2212\u30FC\uFF0D",
     c0 = "\uFF0F/",
     $0 = "\uFF0E.",
     m0 = " \xA0\xAD\u200B\u2060\u3000",
     h0 = "()\uFF08\uFF09\uFF3B\uFF3D\\[\\]",
     b0 = "~\u2053\u223C\uFF5E",
     m = "".concat(f0).concat(c0).concat($0).concat(m0).concat(h0).concat(b0),
     vd = "+\uFF0B";
 
-function K(e, t) {
-    e = e.split("-"), t = t.split("-");
-    for (var d = e[0].split("."), a = t[0].split("."), i = 0; i < 3; i++) {
+function K(e, a) {
+    e = e.split("-"), a = a.split("-");
+    for (var d = e[0].split("."), t = a[0].split("."), i = 0; i < 3; i++) {
         var n = Number(d[i]),
-            r = Number(a[i]);
+            r = Number(t[i]);
         if (n > r) return 1;
         if (r > n) return -1;
         if (!isNaN(n) && isNaN(r)) return 1;
         if (isNaN(n) && !isNaN(r)) return -1
     }
-    return e[1] && t[1] ? e[1] > t[1] ? 1 : e[1] < t[1] ? -1 : 0 : !e[1] && t[1] ? 1 : e[1] && !t[1] ? -1 : 0
+    return e[1] && a[1] ? e[1] > a[1] ? 1 : e[1] < a[1] ? -1 : 0 : !e[1] && a[1] ? 1 : e[1] && !a[1] ? -1 : 0
 }
 var v0 = {}.constructor;
 
 function _(e) {
     return e != null && e.constructor === v0
 }
 
 function Y(e) {
     "@babel/helpers - typeof";
-    return Y = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
-        return typeof t
-    } : function(t) {
-        return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
+    return Y = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(a) {
+        return typeof a
+    } : function(a) {
+        return a && typeof Symbol == "function" && a.constructor === Symbol && a !== Symbol.prototype ? "symbol" : typeof a
     }, Y(e)
 }
 
-function D(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function D(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function xd(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function xd(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function G(e, t, d) {
-    return t && xd(e.prototype, t), d && xd(e, d), Object.defineProperty(e, "prototype", {
+function G(e, a, d) {
+    return a && xd(e.prototype, a), d && xd(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var x0 = "1.2.0",
     p0 = "1.7.35",
     pd = " ext. ",
     y0 = /^\d+$/,
     u = function() {
-        function e(t) {
-            D(this, e), N0(t), this.metadata = t, _d.call(this, t)
+        function e(a) {
+            D(this, e), N0(a), this.metadata = a, _d.call(this, a)
         }
         return G(e, [{
             key: "getCountries",
             value: function() {
                 return Object.keys(this.metadata.countries).filter(function(d) {
                     return d !== "001"
                 })
@@ -3053,57 +3053,57 @@
         }, {
             key: "hasCallingCode",
             value: function(d) {
                 if (this.getCountryCodesForCallingCode(d)) return !0;
                 if (this.nonGeographic()) {
                     if (this.nonGeographic()[d]) return !0
                 } else {
-                    var a = this.countryCallingCodes()[d];
-                    if (a && a.length === 1 && a[0] === "001") return !0
+                    var t = this.countryCallingCodes()[d];
+                    if (t && t.length === 1 && t[0] === "001") return !0
                 }
             }
         }, {
             key: "isNonGeographicCallingCode",
             value: function(d) {
                 return this.nonGeographic() ? !!this.nonGeographic()[d] : !this.getCountryCodesForCallingCode(d)
             }
         }, {
             key: "country",
             value: function(d) {
                 return this.selectNumberingPlan(d)
             }
         }, {
             key: "selectNumberingPlan",
-            value: function(d, a) {
-                if (d && y0.test(d) && (a = d, d = null), d && d !== "001") {
+            value: function(d, t) {
+                if (d && y0.test(d) && (t = d, d = null), d && d !== "001") {
                     if (!this.hasCountry(d)) throw new Error("Unknown country: ".concat(d));
                     this.numberingPlan = new yd(this.getCountryMetadata(d), this)
-                } else if (a) {
-                    if (!this.hasCallingCode(a)) throw new Error("Unknown calling code: ".concat(a));
-                    this.numberingPlan = new yd(this.getNumberingPlanMetadata(a), this)
+                } else if (t) {
+                    if (!this.hasCallingCode(t)) throw new Error("Unknown calling code: ".concat(t));
+                    this.numberingPlan = new yd(this.getNumberingPlanMetadata(t), this)
                 } else this.numberingPlan = void 0;
                 return this
             }
         }, {
             key: "getCountryCodesForCallingCode",
             value: function(d) {
-                var a = this.countryCallingCodes()[d];
-                if (a) return a.length === 1 && a[0].length === 3 ? void 0 : a
+                var t = this.countryCallingCodes()[d];
+                if (t) return t.length === 1 && t[0].length === 3 ? void 0 : t
             }
         }, {
             key: "getCountryCodeForCallingCode",
             value: function(d) {
-                var a = this.getCountryCodesForCallingCode(d);
-                if (a) return a[0]
+                var t = this.getCountryCodesForCallingCode(d);
+                if (t) return t[0]
             }
         }, {
             key: "getNumberingPlanMetadata",
             value: function(d) {
-                var a = this.getCountryCodeForCallingCode(d);
-                if (a) return this.getCountryMetadata(a);
+                var t = this.getCountryCodeForCallingCode(d);
+                if (t) return this.getCountryMetadata(t);
                 if (this.nonGeographic()) {
                     var i = this.nonGeographic()[d];
                     if (i) return i
                 } else {
                     var n = this.countryCallingCodes()[d];
                     if (n && n.length === 1 && n[0] === "001") return this.metadata.countries["001"]
                 }
@@ -3182,16 +3182,16 @@
             key: "hasSelectedNumberingPlan",
             value: function() {
                 return this.numberingPlan !== void 0
             }
         }]), e
     }();
 var yd = function() {
-        function e(t, d) {
-            D(this, e), this.globalMetadataObject = d, this.metadata = t, _d.call(this, d.metadata)
+        function e(a, d) {
+            D(this, e), this.globalMetadataObject = d, this.metadata = a, _d.call(this, d.metadata)
         }
         return G(e, [{
             key: "callingCode",
             value: function() {
                 return this.metadata[0]
             }
         }, {
@@ -3224,16 +3224,16 @@
             value: function(d) {
                 return d[this.v1 ? 2 : this.v2 ? 3 : 4]
             }
         }, {
             key: "formats",
             value: function() {
                 var d = this,
-                    a = this._getFormats(this.metadata) || this._getFormats(this.getDefaultCountryMetadataForRegion()) || [];
-                return a.map(function(i) {
+                    t = this._getFormats(this.metadata) || this._getFormats(this.getDefaultCountryMetadataForRegion()) || [];
+                return t.map(function(i) {
                     return new k0(i, d)
                 })
             }
         }, {
             key: "nationalPrefix",
             value: function() {
                 return this.metadata[this.v1 ? 3 : this.v2 ? 4 : 5]
@@ -3297,16 +3297,16 @@
             key: "ext",
             value: function() {
                 return this.v1 || this.v2 ? pd : this.metadata[13] || pd
             }
         }]), e
     }(),
     k0 = function() {
-        function e(t, d) {
-            D(this, e), this._format = t, this.metadata = d
+        function e(a, d) {
+            D(this, e), this._format = a, this.metadata = d
         }
         return G(e, [{
             key: "pattern",
             value: function() {
                 return this._format[0]
             }
         }, {
@@ -3344,32 +3344,32 @@
             value: function() {
                 return this._format[5] || this.format()
             }
         }]), e
     }(),
     _0 = /^\(?\$1\)?$/,
     C0 = function() {
-        function e(t, d) {
-            D(this, e), this.type = t, this.metadata = d
+        function e(a, d) {
+            D(this, e), this.type = a, this.metadata = d
         }
         return G(e, [{
             key: "pattern",
             value: function() {
                 return this.metadata.v1 ? this.type : this.type[0]
             }
         }, {
             key: "possibleLengths",
             value: function() {
                 if (!this.metadata.v1) return this.type[1] || this.metadata.possibleLengths()
             }
         }]), e
     }();
 
-function kd(e, t) {
-    switch (t) {
+function kd(e, a) {
+    switch (a) {
         case "FIXED_LINE":
             return e[0];
         case "MOBILE":
             return e[1];
         case "TOLL_FREE":
             return e[2];
         case "PREMIUM_RATE":
@@ -3389,60 +3389,60 @@
     }
 }
 
 function N0(e) {
     if (!e) throw new Error("[libphonenumber-js] `metadata` argument not passed. Check your arguments.");
     if (!_(e) || !_(e.countries)) throw new Error("[libphonenumber-js] `metadata` argument was passed but it's not a valid metadata. Must be an object having `.countries` child object property. Got ".concat(_(e) ? "an object of shape: { " + Object.keys(e).join(", ") + " }" : "a " + P0(e) + ": " + e, "."))
 }
-var P0 = function(t) {
-    return Y(t)
+var P0 = function(a) {
+    return Y(a)
 };
 
-function v(e, t) {
-    if (t = new u(t), t.hasCountry(e)) return t.country(e).countryCallingCode();
+function v(e, a) {
+    if (a = new u(a), a.hasCountry(e)) return a.country(e).countryCallingCode();
     throw new Error("Unknown country: ".concat(e))
 }
 
 function _d(e) {
-    var t = e.version;
-    typeof t == "number" ? (this.v1 = t === 1, this.v2 = t === 2, this.v3 = t === 3, this.v4 = t === 4) : t ? K(t, x0) === -1 ? this.v2 = !0 : K(t, p0) === -1 ? this.v3 = !0 : this.v4 = !0 : this.v1 = !0
+    var a = e.version;
+    typeof a == "number" ? (this.v1 = a === 1, this.v2 = a === 2, this.v3 = a === 3, this.v4 = a === 4) : a ? K(a, x0) === -1 ? this.v2 = !0 : K(a, p0) === -1 ? this.v3 = !0 : this.v4 = !0 : this.v1 = !0
 }
 
-function S0(e, t) {
+function I0(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = I0(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = S0(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function I0(e, t) {
+function S0(e, a) {
     if (e) {
-        if (typeof e == "string") return Cd(e, t);
+        if (typeof e == "string") return Cd(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Cd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Cd(e, a)
     }
 }
 
-function Cd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Cd(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 var T0 = {
     0: "0",
     1: "1",
     2: "2",
     3: "3",
     4: "4",
@@ -3484,86 +3484,86 @@
 };
 
 function E0(e) {
     return T0[e]
 }
 
 function x(e) {
-    for (var t = "", d = S0(e.split("")), a; !(a = d()).done;) {
-        var i = a.value,
+    for (var a = "", d = I0(e.split("")), t; !(t = d()).done;) {
+        var i = t.value,
             n = E0(i);
-        n && (t += n)
+        n && (a += n)
     }
-    return t
+    return a
 }
 
-function A0(e, t) {
+function A0(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = F0(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = F0(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function F0(e, t) {
+function F0(e, a) {
     if (e) {
-        if (typeof e == "string") return Nd(e, t);
+        if (typeof e == "string") return Nd(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Nd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Nd(e, a)
     }
 }
 
-function Nd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Nd(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function z(e, t) {
-    for (var d = e.slice(), a = A0(t), i; !(i = a()).done;) {
+function z(e, a) {
+    for (var d = e.slice(), t = A0(a), i; !(i = t()).done;) {
         var n = i.value;
         e.indexOf(n) < 0 && d.push(n)
     }
     return d.sort(function(r, o) {
         return r - o
     })
 }
 
-function b(e, t) {
-    return Pd(e, void 0, t)
+function b(e, a) {
+    return Pd(e, void 0, a)
 }
 
-function Pd(e, t, d) {
-    var a = d.type(t),
-        i = a && a.possibleLengths() || d.possibleLengths();
+function Pd(e, a, d) {
+    var t = d.type(a),
+        i = t && t.possibleLengths() || d.possibleLengths();
     if (!i) return "IS_POSSIBLE";
-    if (t === "FIXED_LINE_OR_MOBILE") {
+    if (a === "FIXED_LINE_OR_MOBILE") {
         if (!d.type("FIXED_LINE")) return Pd(e, "MOBILE", d);
         var n = d.type("MOBILE");
         n && (i = z(i, n.possibleLengths()))
-    } else if (t && !a) return "INVALID_LENGTH";
+    } else if (a && !t) return "INVALID_LENGTH";
     var r = e.length,
         o = i[0];
     return o === r ? "IS_POSSIBLE" : o > r ? "TOO_SHORT" : i[i.length - 1] < r ? "TOO_LONG" : i.indexOf(r, 1) >= 0 ? "IS_POSSIBLE" : "INVALID_LENGTH"
 }
 
-function q(e, t, d) {
-    if (t === void 0 && (t = {}), d = new u(d), t.v2) {
+function q(e, a, d) {
+    if (a === void 0 && (a = {}), d = new u(d), a.v2) {
         if (!e.countryCallingCode) throw new Error("Invalid phone number object passed");
         d.selectNumberingPlan(e.countryCallingCode)
     } else {
         if (!e.phone) return !1;
         if (e.country) {
             if (!d.hasCountry(e.country)) throw new Error("Unknown country: ".concat(e.country));
             d.country(e.country)
@@ -3573,323 +3573,323 @@
         }
     }
     if (d.possibleLengths()) return w0(e.phone || e.nationalNumber, d);
     if (e.countryCallingCode && d.isNonGeographicCallingCode(e.countryCallingCode)) return !0;
     throw new Error('Missing "possibleLengths" in metadata. Perhaps the metadata has been generated before v1.0.18.')
 }
 
-function w0(e, t) {
-    switch (b(e, t)) {
+function w0(e, a) {
+    switch (b(e, a)) {
         case "IS_POSSIBLE":
             return !0;
         default:
             return !1
     }
 }
 
-function f(e, t) {
-    return e = e || "", new RegExp("^(?:" + t + ")$").test(e)
+function f(e, a) {
+    return e = e || "", new RegExp("^(?:" + a + ")$").test(e)
 }
 
-function M0(e, t) {
+function M0(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = O0(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = O0(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function O0(e, t) {
+function O0(e, a) {
     if (e) {
-        if (typeof e == "string") return Sd(e, t);
+        if (typeof e == "string") return Id(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Sd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Id(e, a)
     }
 }
 
-function Sd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Id(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 var L0 = ["MOBILE", "PREMIUM_RATE", "TOLL_FREE", "SHARED_COST", "VOIP", "PERSONAL_NUMBER", "PAGER", "UAN", "VOICEMAIL"];
 
-function C(e, t, d) {
-    if (t = t || {}, !(!e.country && !e.countryCallingCode)) {
+function C(e, a, d) {
+    if (a = a || {}, !(!e.country && !e.countryCallingCode)) {
         d = new u(d), d.selectNumberingPlan(e.country, e.countryCallingCode);
-        var a = t.v2 ? e.nationalNumber : e.phone;
-        if (f(a, d.nationalNumberPattern())) {
-            if (Z(a, "FIXED_LINE", d)) return d.type("MOBILE") && d.type("MOBILE").pattern() === "" || !d.type("MOBILE") || Z(a, "MOBILE", d) ? "FIXED_LINE_OR_MOBILE" : "FIXED_LINE";
+        var t = a.v2 ? e.nationalNumber : e.phone;
+        if (f(t, d.nationalNumberPattern())) {
+            if (Z(t, "FIXED_LINE", d)) return d.type("MOBILE") && d.type("MOBILE").pattern() === "" || !d.type("MOBILE") || Z(t, "MOBILE", d) ? "FIXED_LINE_OR_MOBILE" : "FIXED_LINE";
             for (var i = M0(L0), n; !(n = i()).done;) {
                 var r = n.value;
-                if (Z(a, r, d)) return r
+                if (Z(t, r, d)) return r
             }
         }
     }
 }
 
-function Z(e, t, d) {
-    return t = d.type(t), !t || !t.pattern() || t.possibleLengths() && t.possibleLengths().indexOf(e.length) < 0 ? !1 : f(e, t.pattern())
+function Z(e, a, d) {
+    return a = d.type(a), !a || !a.pattern() || a.possibleLengths() && a.possibleLengths().indexOf(e.length) < 0 ? !1 : f(e, a.pattern())
 }
 
-function X(e, t, d) {
-    if (t = t || {}, d = new u(d), d.selectNumberingPlan(e.country, e.countryCallingCode), d.hasTypes()) return C(e, t, d.metadata) !== void 0;
-    var a = t.v2 ? e.nationalNumber : e.phone;
-    return f(a, d.nationalNumberPattern())
+function X(e, a, d) {
+    if (a = a || {}, d = new u(d), d.selectNumberingPlan(e.country, e.countryCallingCode), d.hasTypes()) return C(e, a, d.metadata) !== void 0;
+    var t = a.v2 ? e.nationalNumber : e.phone;
+    return f(t, d.nationalNumberPattern())
 }
 
-function J(e, t, d) {
-    var a = new u(d),
-        i = a.getCountryCodesForCallingCode(e);
+function J(e, a, d) {
+    var t = new u(d),
+        i = t.getCountryCodesForCallingCode(e);
     return i ? i.filter(function(n) {
-        return R0(t, n, d)
+        return R0(a, n, d)
     }) : []
 }
 
-function R0(e, t, d) {
-    var a = new u(d);
-    return a.selectNumberingPlan(t), a.numberingPlan.possibleLengths().indexOf(e.length) >= 0
+function R0(e, a, d) {
+    var t = new u(d);
+    return t.selectNumberingPlan(a), t.numberingPlan.possibleLengths().indexOf(e.length) >= 0
 }
 
 function T(e) {
     return e.replace(new RegExp("[".concat(m, "]+"), "g"), " ").trim()
 }
 var Q = /(\$\d)/;
 
-function E(e, t, d) {
-    var a = d.useInternationalFormat,
+function E(e, a, d) {
+    var t = d.useInternationalFormat,
         i = d.withNationalPrefix,
         n = d.carrierCode,
         r = d.metadata,
-        o = e.replace(new RegExp(t.pattern()), a ? t.internationalFormat() : i && t.nationalPrefixFormattingRule() ? t.format().replace(Q, t.nationalPrefixFormattingRule()) : t.format());
-    return a ? T(o) : o
+        o = e.replace(new RegExp(a.pattern()), t ? a.internationalFormat() : i && a.nationalPrefixFormattingRule() ? a.format().replace(Q, a.nationalPrefixFormattingRule()) : a.format());
+    return t ? T(o) : o
 }
 var D0 = /^[\d]+(?:[~\u2053\u223C\uFF5E][\d]+)?$/;
 
-function dd(e, t, d) {
-    var a = new u(d);
-    if (a.selectNumberingPlan(e, t), a.defaultIDDPrefix()) return a.defaultIDDPrefix();
-    if (D0.test(a.IDDPrefix())) return a.IDDPrefix()
+function dd(e, a, d) {
+    var t = new u(d);
+    if (t.selectNumberingPlan(e, a), t.defaultIDDPrefix()) return t.defaultIDDPrefix();
+    if (D0.test(t.IDDPrefix())) return t.IDDPrefix()
 }
 
-function Id(e) {
-    var t = e.number,
+function Sd(e) {
+    var a = e.number,
         d = e.ext;
-    if (!t) return "";
-    if (t[0] !== "+") throw new Error('"formatRFC3966()" expects "number" to be in E.164 format.');
-    return "tel:".concat(t).concat(d ? ";ext=" + d : "")
+    if (!a) return "";
+    if (a[0] !== "+") throw new Error('"formatRFC3966()" expects "number" to be in E.164 format.');
+    return "tel:".concat(a).concat(d ? ";ext=" + d : "")
 }
 
-function G0(e, t) {
+function G0(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = B0(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = B0(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function B0(e, t) {
+function B0(e, a) {
     if (e) {
-        if (typeof e == "string") return Td(e, t);
+        if (typeof e == "string") return Td(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Td(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Td(e, a)
     }
 }
 
-function Td(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Td(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function Ed(e, t) {
+function Ed(e, a) {
     var d = Object.keys(e);
     if (Object.getOwnPropertySymbols) {
-        var a = Object.getOwnPropertySymbols(e);
-        t && (a = a.filter(function(i) {
+        var t = Object.getOwnPropertySymbols(e);
+        a && (t = t.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
-        })), d.push.apply(d, a)
+        })), d.push.apply(d, t)
     }
     return d
 }
 
 function Ad(e) {
-    for (var t = 1; t < arguments.length; t++) {
-        var d = arguments[t] != null ? arguments[t] : {};
-        t % 2 ? Ed(Object(d), !0).forEach(function(a) {
-            j0(e, a, d[a])
-        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(d)) : Ed(Object(d)).forEach(function(a) {
-            Object.defineProperty(e, a, Object.getOwnPropertyDescriptor(d, a))
+    for (var a = 1; a < arguments.length; a++) {
+        var d = arguments[a] != null ? arguments[a] : {};
+        a % 2 ? Ed(Object(d), !0).forEach(function(t) {
+            j0(e, t, d[t])
+        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(d)) : Ed(Object(d)).forEach(function(t) {
+            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(d, t))
         })
     }
     return e
 }
 
-function j0(e, t, d) {
-    return t in e ? Object.defineProperty(e, t, {
+function j0(e, a, d) {
+    return a in e ? Object.defineProperty(e, a, {
         value: d,
         enumerable: !0,
         configurable: !0,
         writable: !0
-    }) : e[t] = d, e
+    }) : e[a] = d, e
 }
 var Fd = {
-    formatExtension: function(t, d, a) {
-        return "".concat(t).concat(a.ext()).concat(d)
+    formatExtension: function(a, d, t) {
+        return "".concat(a).concat(t.ext()).concat(d)
     }
 };
 
-function td(e, t, d, a) {
-    if (d ? d = Ad(Ad({}, Fd), d) : d = Fd, a = new u(a), e.country && e.country !== "001") {
-        if (!a.hasCountry(e.country)) throw new Error("Unknown country: ".concat(e.country));
-        a.country(e.country)
-    } else if (e.countryCallingCode) a.selectNumberingPlan(e.countryCallingCode);
+function ad(e, a, d, t) {
+    if (d ? d = Ad(Ad({}, Fd), d) : d = Fd, t = new u(t), e.country && e.country !== "001") {
+        if (!t.hasCountry(e.country)) throw new Error("Unknown country: ".concat(e.country));
+        t.country(e.country)
+    } else if (e.countryCallingCode) t.selectNumberingPlan(e.countryCallingCode);
     else return e.phone || "";
-    var i = a.countryCallingCode(),
+    var i = t.countryCallingCode(),
         n = d.v2 ? e.nationalNumber : e.phone,
         r;
-    switch (t) {
+    switch (a) {
         case "NATIONAL":
-            return n ? (r = B(n, e.carrierCode, "NATIONAL", a, d), ed(r, e.ext, a, d.formatExtension)) : "";
+            return n ? (r = B(n, e.carrierCode, "NATIONAL", t, d), ed(r, e.ext, t, d.formatExtension)) : "";
         case "INTERNATIONAL":
-            return n ? (r = B(n, null, "INTERNATIONAL", a, d), r = "+".concat(i, " ").concat(r), ed(r, e.ext, a, d.formatExtension)) : "+".concat(i);
+            return n ? (r = B(n, null, "INTERNATIONAL", t, d), r = "+".concat(i, " ").concat(r), ed(r, e.ext, t, d.formatExtension)) : "+".concat(i);
         case "E.164":
             return "+".concat(i).concat(n);
         case "RFC3966":
-            return Id({
+            return Sd({
                 number: "+".concat(i).concat(n),
                 ext: e.ext
             });
         case "IDD":
             if (!d.fromCountry) return;
-            var o = U0(n, e.carrierCode, i, d.fromCountry, a);
-            return ed(o, e.ext, a, d.formatExtension);
+            var o = U0(n, e.carrierCode, i, d.fromCountry, t);
+            return ed(o, e.ext, t, d.formatExtension);
         default:
-            throw new Error('Unknown "format" argument passed to "formatNumber()": "'.concat(t, '"'))
+            throw new Error('Unknown "format" argument passed to "formatNumber()": "'.concat(a, '"'))
     }
 }
 
-function B(e, t, d, a, i) {
-    var n = H0(a.formats(), e);
+function B(e, a, d, t, i) {
+    var n = H0(t.formats(), e);
     return n ? E(e, n, {
         useInternationalFormat: d === "INTERNATIONAL",
         withNationalPrefix: !(n.nationalPrefixIsOptionalWhenFormattingInNationalFormat() && i && i.nationalPrefix === !1),
-        carrierCode: t,
-        metadata: a
+        carrierCode: a,
+        metadata: t
     }) : e
 }
 
-function H0(e, t) {
-    for (var d = G0(e), a; !(a = d()).done;) {
-        var i = a.value;
+function H0(e, a) {
+    for (var d = G0(e), t; !(t = d()).done;) {
+        var i = t.value;
         if (i.leadingDigitsPatterns().length > 0) {
             var n = i.leadingDigitsPatterns()[i.leadingDigitsPatterns().length - 1];
-            if (t.search(n) !== 0) continue
+            if (a.search(n) !== 0) continue
         }
-        if (f(t, i.pattern())) return i
+        if (f(a, i.pattern())) return i
     }
 }
 
-function ed(e, t, d, a) {
-    return t ? a(e, t, d) : e
+function ed(e, a, d, t) {
+    return a ? t(e, a, d) : e
 }
 
-function U0(e, t, d, a, i) {
-    var n = v(a, i.metadata);
+function U0(e, a, d, t, i) {
+    var n = v(t, i.metadata);
     if (n === d) {
-        var r = B(e, t, "NATIONAL", i);
+        var r = B(e, a, "NATIONAL", i);
         return d === "1" ? d + " " + r : r
     }
-    var o = dd(a, void 0, i.metadata);
+    var o = dd(t, void 0, i.metadata);
     if (o) return "".concat(o, " ").concat(d, " ").concat(B(e, null, "INTERNATIONAL", i))
 }
 
-function wd(e, t) {
+function wd(e, a) {
     var d = Object.keys(e);
     if (Object.getOwnPropertySymbols) {
-        var a = Object.getOwnPropertySymbols(e);
-        t && (a = a.filter(function(i) {
+        var t = Object.getOwnPropertySymbols(e);
+        a && (t = t.filter(function(i) {
             return Object.getOwnPropertyDescriptor(e, i).enumerable
-        })), d.push.apply(d, a)
+        })), d.push.apply(d, t)
     }
     return d
 }
 
 function Md(e) {
-    for (var t = 1; t < arguments.length; t++) {
-        var d = arguments[t] != null ? arguments[t] : {};
-        t % 2 ? wd(Object(d), !0).forEach(function(a) {
-            V0(e, a, d[a])
-        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(d)) : wd(Object(d)).forEach(function(a) {
-            Object.defineProperty(e, a, Object.getOwnPropertyDescriptor(d, a))
+    for (var a = 1; a < arguments.length; a++) {
+        var d = arguments[a] != null ? arguments[a] : {};
+        a % 2 ? wd(Object(d), !0).forEach(function(t) {
+            V0(e, t, d[t])
+        }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(d)) : wd(Object(d)).forEach(function(t) {
+            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(d, t))
         })
     }
     return e
 }
 
-function V0(e, t, d) {
-    return t in e ? Object.defineProperty(e, t, {
+function V0(e, a, d) {
+    return a in e ? Object.defineProperty(e, a, {
         value: d,
         enumerable: !0,
         configurable: !0,
         writable: !0
-    }) : e[t] = d, e
+    }) : e[a] = d, e
 }
 
-function W0(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function W0(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function Od(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function Od(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function K0(e, t, d) {
-    return t && Od(e.prototype, t), d && Od(e, d), Object.defineProperty(e, "prototype", {
+function K0(e, a, d) {
+    return a && Od(e.prototype, a), d && Od(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var Y0 = !1,
     Ld = function() {
-        function e(t, d, a) {
-            if (W0(this, e), !t) throw new TypeError("`country` or `countryCallingCode` not passed");
+        function e(a, d, t) {
+            if (W0(this, e), !a) throw new TypeError("`country` or `countryCallingCode` not passed");
             if (!d) throw new TypeError("`nationalNumber` not passed");
-            if (!a) throw new TypeError("`metadata` not passed");
-            var i = q0(t, a),
+            if (!t) throw new TypeError("`metadata` not passed");
+            var i = q0(a, t),
                 n = i.country,
                 r = i.countryCallingCode;
             this.country = n, this.countryCallingCode = r, this.nationalNumber = d, this.number = "+" + this.countryCallingCode + this.nationalNumber, this.getMetadata = function() {
-                return a
+                return t
             }
         }
         return K0(e, [{
             key: "setExt",
             value: function(d) {
                 this.ext = d
             }
@@ -3928,16 +3928,16 @@
             value: function() {
                 return C(this, {
                     v2: !0
                 }, this.getMetadata())
             }
         }, {
             key: "format",
-            value: function(d, a) {
-                return td(this, d, a ? Md(Md({}, a), {}, {
+            value: function(d, t) {
+                return ad(this, d, t ? Md(Md({}, t), {}, {
                     v2: !0
                 }) : {
                     v2: !0
                 }, this.getMetadata())
             }
         }, {
             key: "formatNational",
@@ -3952,287 +3952,287 @@
         }, {
             key: "getURI",
             value: function(d) {
                 return this.format("RFC3966", d)
             }
         }]), e
     }();
-var z0 = function(t) {
-    return /^[A-Z]{2}$/.test(t)
+var z0 = function(a) {
+    return /^[A-Z]{2}$/.test(a)
 };
 
-function q0(e, t) {
-    var d, a, i = new u(t);
-    return z0(e) ? (d = e, i.selectNumberingPlan(d), a = i.countryCallingCode()) : (a = e, Y0 && i.isNonGeographicCallingCode(a) && (d = "001")), {
+function q0(e, a) {
+    var d, t, i = new u(a);
+    return z0(e) ? (d = e, i.selectNumberingPlan(d), t = i.countryCallingCode()) : (t = e, Y0 && i.isNonGeographicCallingCode(t) && (d = "001")), {
         country: d,
-        countryCallingCode: a
+        countryCallingCode: t
     }
 }
 var Z0 = new RegExp("([" + k + "])");
 
-function A(e, t, d, a) {
-    if (t) {
-        var i = new u(a);
-        i.selectNumberingPlan(t, d);
+function A(e, a, d, t) {
+    if (a) {
+        var i = new u(t);
+        i.selectNumberingPlan(a, d);
         var n = new RegExp(i.IDDPrefix());
         if (e.search(n) === 0) {
             e = e.slice(e.match(n)[0].length);
             var r = e.match(Z0);
             if (!(r && r[1] != null && r[1].length > 0 && r[1] === "0")) return e
         }
     }
 }
 
-function N(e, t) {
-    if (e && t.numberingPlan.nationalPrefixForParsing()) {
-        var d = new RegExp("^(?:" + t.numberingPlan.nationalPrefixForParsing() + ")"),
-            a = d.exec(e);
-        if (a) {
-            var i, n, r = a.length - 1,
-                o = r > 0 && a[r];
-            if (t.nationalPrefixTransformRule() && o) i = e.replace(d, t.nationalPrefixTransformRule()), r > 1 && (n = a[1]);
+function N(e, a) {
+    if (e && a.numberingPlan.nationalPrefixForParsing()) {
+        var d = new RegExp("^(?:" + a.numberingPlan.nationalPrefixForParsing() + ")"),
+            t = d.exec(e);
+        if (t) {
+            var i, n, r = t.length - 1,
+                o = r > 0 && t[r];
+            if (a.nationalPrefixTransformRule() && o) i = e.replace(d, a.nationalPrefixTransformRule()), r > 1 && (n = t[1]);
             else {
-                var s = a[0];
-                i = e.slice(s.length), o && (n = a[1])
+                var s = t[0];
+                i = e.slice(s.length), o && (n = t[1])
             }
             var l;
             if (o) {
-                var g = e.indexOf(a[1]),
+                var g = e.indexOf(t[1]),
                     h = e.slice(0, g);
-                h === t.numberingPlan.nationalPrefix() && (l = t.numberingPlan.nationalPrefix())
-            } else l = a[0];
+                h === a.numberingPlan.nationalPrefix() && (l = a.numberingPlan.nationalPrefix())
+            } else l = t[0];
             return {
                 nationalNumber: i,
                 nationalPrefix: l,
                 carrierCode: n
             }
         }
     }
     return {
         nationalNumber: e
     }
 }
 
-function j(e, t) {
-    var d = N(e, t),
-        a = d.carrierCode,
+function j(e, a) {
+    var d = N(e, a),
+        t = d.carrierCode,
         i = d.nationalNumber;
     if (i !== e) {
-        if (!X0(e, i, t)) return {
+        if (!X0(e, i, a)) return {
             nationalNumber: e
         };
-        if (t.possibleLengths() && !J0(i, t)) return {
+        if (a.possibleLengths() && !J0(i, a)) return {
             nationalNumber: e
         }
     }
     return {
         nationalNumber: i,
-        carrierCode: a
+        carrierCode: t
     }
 }
 
-function X0(e, t, d) {
-    return !(f(e, d.nationalNumberPattern()) && !f(t, d.nationalNumberPattern()))
+function X0(e, a, d) {
+    return !(f(e, d.nationalNumberPattern()) && !f(a, d.nationalNumberPattern()))
 }
 
-function J0(e, t) {
-    switch (b(e, t)) {
+function J0(e, a) {
+    switch (b(e, a)) {
         case "TOO_SHORT":
         case "INVALID_LENGTH":
             return !1;
         default:
             return !0
     }
 }
 
-function F(e, t, d, a) {
-    var i = t ? v(t, a) : d;
+function F(e, a, d, t) {
+    var i = a ? v(a, t) : d;
     if (e.indexOf(i) === 0) {
-        a = new u(a), a.selectNumberingPlan(t, d);
+        t = new u(t), t.selectNumberingPlan(a, d);
         var n = e.slice(i.length),
-            r = j(n, a),
+            r = j(n, t),
             o = r.nationalNumber,
-            s = j(e, a),
+            s = j(e, t),
             l = s.nationalNumber;
-        if (!f(l, a.nationalNumberPattern()) && f(o, a.nationalNumberPattern()) || b(l, a) === "TOO_LONG") return {
+        if (!f(l, t.nationalNumberPattern()) && f(o, t.nationalNumberPattern()) || b(l, t) === "TOO_LONG") return {
             countryCallingCode: i,
             number: n
         }
     }
     return {
         number: e
     }
 }
 
-function ad(e, t, d, a) {
+function td(e, a, d, t) {
     if (!e) return {};
     var i;
     if (e[0] !== "+") {
-        var n = A(e, t, d, a);
+        var n = A(e, a, d, t);
         if (n && n !== e) i = !0, e = "+" + n;
         else {
-            if (t || d) {
-                var r = F(e, t, d, a),
+            if (a || d) {
+                var r = F(e, a, d, t),
                     o = r.countryCallingCode,
                     s = r.number;
                 if (o) return {
                     countryCallingCodeSource: "FROM_NUMBER_WITHOUT_PLUS_SIGN",
                     countryCallingCode: o,
                     number: s
                 }
             }
             return {
                 number: e
             }
         }
     }
     if (e[1] === "0") return {};
-    a = new u(a);
+    t = new u(t);
     for (var l = 2; l - 1 <= bd && l <= e.length;) {
         var g = e.slice(1, l);
-        if (a.hasCallingCode(g)) return a.selectNumberingPlan(g), {
+        if (t.hasCallingCode(g)) return t.selectNumberingPlan(g), {
             countryCallingCodeSource: i ? "FROM_NUMBER_WITH_IDD" : "FROM_NUMBER_WITH_PLUS_SIGN",
             countryCallingCode: g,
             number: e.slice(l)
         };
         l++
     }
     return {}
 }
 
-function Q0(e, t) {
+function Q0(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = de(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = de(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function de(e, t) {
+function de(e, a) {
     if (e) {
-        if (typeof e == "string") return Rd(e, t);
+        if (typeof e == "string") return Rd(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Rd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Rd(e, a)
     }
 }
 
-function Rd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Rd(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function w(e, t) {
-    var d = t.countries,
-        a = t.defaultCountry,
-        i = t.metadata;
+function w(e, a) {
+    var d = a.countries,
+        t = a.defaultCountry,
+        i = a.metadata;
     i = new u(i);
     for (var n = [], r = Q0(d), o; !(o = r()).done;) {
         var s = o.value;
         if (i.country(s), i.leadingDigits()) {
             if (e && e.search(i.leadingDigits()) === 0) return s
         } else if (C({
                 phone: e,
                 country: s
             }, void 0, i.metadata))
-            if (a) {
-                if (s === a) return s;
+            if (t) {
+                if (s === t) return s;
                 n.push(s)
             } else return s
     }
     if (n.length > 0) return n[0]
 }
 var ee = !1;
 
-function id(e, t) {
-    var d = t.nationalNumber,
-        a = t.defaultCountry,
-        i = t.metadata;
+function id(e, a) {
+    var d = a.nationalNumber,
+        t = a.defaultCountry,
+        i = a.metadata;
     if (ee && i.isNonGeographicCallingCode(e)) return "001";
     var n = i.getCountryCodesForCallingCode(e);
     if (n) return n.length === 1 ? n[0] : w(d, {
         countries: n,
-        defaultCountry: a,
+        defaultCountry: t,
         metadata: i.metadata
     })
 }
 
-function te(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function ae(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function Dd(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function Dd(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function ae(e, t, d) {
-    return t && Dd(e.prototype, t), d && Dd(e, d), Object.defineProperty(e, "prototype", {
+function te(e, a, d) {
+    return a && Dd(e.prototype, a), d && Dd(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var Gd = function() {
-    function e(t) {
-        var d = t.onCountryChange,
-            a = t.onCallingCodeChange;
-        te(this, e), this.onCountryChange = d, this.onCallingCodeChange = a
+    function e(a) {
+        var d = a.onCountryChange,
+            t = a.onCallingCodeChange;
+        ae(this, e), this.onCountryChange = d, this.onCallingCodeChange = t
     }
-    return ae(e, [{
+    return te(e, [{
         key: "reset",
         value: function(d) {
-            var a = d.country,
+            var t = d.country,
                 i = d.callingCode;
-            this.international = !1, this.missingPlus = !1, this.IDDPrefix = void 0, this.callingCode = void 0, this.digits = "", this.resetNationalSignificantNumber(), this.initCountryAndCallingCode(a, i)
+            this.international = !1, this.missingPlus = !1, this.IDDPrefix = void 0, this.callingCode = void 0, this.digits = "", this.resetNationalSignificantNumber(), this.initCountryAndCallingCode(t, i)
         }
     }, {
         key: "resetNationalSignificantNumber",
         value: function() {
             this.nationalSignificantNumber = this.getNationalDigits(), this.nationalSignificantNumberMatchesInput = !0, this.nationalPrefix = void 0, this.carrierCode = void 0, this.complexPrefixBeforeNationalSignificantNumber = void 0
         }
     }, {
         key: "update",
         value: function(d) {
-            for (var a = 0, i = Object.keys(d); a < i.length; a++) {
-                var n = i[a];
+            for (var t = 0, i = Object.keys(d); t < i.length; t++) {
+                var n = i[t];
                 this[n] = d[n]
             }
         }
     }, {
         key: "initCountryAndCallingCode",
-        value: function(d, a) {
-            this.setCountry(d), this.setCallingCode(a)
+        value: function(d, t) {
+            this.setCountry(d), this.setCallingCode(t)
         }
     }, {
         key: "setCountry",
         value: function(d) {
             this.country = d, this.onCountryChange(d)
         }
     }, {
         key: "setCallingCode",
         value: function(d) {
             this.callingCode = d, this.onCallingCodeChange(d, this.country)
         }
     }, {
         key: "startInternationalNumber",
-        value: function(d, a) {
-            this.international = !0, this.initCountryAndCallingCode(d, a)
+        value: function(d, t) {
+            this.international = !0, this.initCountryAndCallingCode(d, t)
         }
     }, {
         key: "appendDigits",
         value: function(d) {
             this.digits += d
         }
     }, {
@@ -4249,167 +4249,167 @@
         key: "getDigitsWithoutInternationalPrefix",
         value: function() {
             return this.international && this.IDDPrefix ? this.digits.slice(this.IDDPrefix.length) : this.digits
         }
     }]), e
 }();
 
-function ie(e, t) {
+function ie(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = ne(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = ne(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function ne(e, t) {
+function ne(e, a) {
     if (e) {
-        if (typeof e == "string") return Bd(e, t);
+        if (typeof e == "string") return Bd(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Bd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Bd(e, a)
     }
 }
 
-function Bd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Bd(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 var c = "x",
     nd = new RegExp(c);
 
-function M(e, t) {
-    if (t < 1) return "";
-    for (var d = ""; t > 1;) t & 1 && (d += e), t >>= 1, e += e;
+function M(e, a) {
+    if (a < 1) return "";
+    for (var d = ""; a > 1;) a & 1 && (d += e), a >>= 1, e += e;
     return d + e
 }
 
-function rd(e, t) {
-    return e[t] === ")" && t++, re(e.slice(0, t))
+function rd(e, a) {
+    return e[a] === ")" && a++, re(e.slice(0, a))
 }
 
 function re(e) {
-    for (var t = [], d = 0; d < e.length;) e[d] === "(" ? t.push(d) : e[d] === ")" && t.pop(), d++;
-    var a = 0,
+    for (var a = [], d = 0; d < e.length;) e[d] === "(" ? a.push(d) : e[d] === ")" && a.pop(), d++;
+    var t = 0,
         i = "";
-    t.push(e.length);
-    for (var n = 0, r = t; n < r.length; n++) {
+    a.push(e.length);
+    for (var n = 0, r = a; n < r.length; n++) {
         var o = r[n];
-        i += e.slice(a, o), a = o + 1
+        i += e.slice(t, o), t = o + 1
     }
     return i
 }
 
-function jd(e, t, d) {
-    for (var a = ie(d.split("")), i; !(i = a()).done;) {
+function jd(e, a, d) {
+    for (var t = ie(d.split("")), i; !(i = t()).done;) {
         var n = i.value;
-        if (e.slice(t + 1).search(nd) < 0) return;
-        t = e.search(nd), e = e.replace(nd, n)
+        if (e.slice(a + 1).search(nd) < 0) return;
+        a = e.search(nd), e = e.replace(nd, n)
     }
-    return [e, t]
+    return [e, a]
 }
 
-function od(e, t, d) {
-    var a = d.metadata,
+function od(e, a, d) {
+    var t = d.metadata,
         i = d.shouldTryNationalPrefixFormattingRule,
         n = d.getSeparatorAfterNationalPrefix,
-        r = new RegExp("^(?:".concat(t.pattern(), ")$"));
-    if (r.test(e.nationalSignificantNumber)) return oe(e, t, {
-        metadata: a,
+        r = new RegExp("^(?:".concat(a.pattern(), ")$"));
+    if (r.test(e.nationalSignificantNumber)) return oe(e, a, {
+        metadata: t,
         shouldTryNationalPrefixFormattingRule: i,
         getSeparatorAfterNationalPrefix: n
     })
 }
 
-function Ud(e, t) {
-    return b(e, t) === "IS_POSSIBLE"
+function Ud(e, a) {
+    return b(e, a) === "IS_POSSIBLE"
 }
 
-function oe(e, t, d) {
-    var a = d.metadata,
+function oe(e, a, d) {
+    var t = d.metadata,
         i = d.shouldTryNationalPrefixFormattingRule,
         n = d.getSeparatorAfterNationalPrefix,
         r = e.nationalSignificantNumber,
         o = e.international,
         s = e.nationalPrefix,
         l = e.carrierCode;
-    if (i(t)) {
-        var g = Hd(e, t, {
+    if (i(a)) {
+        var g = Hd(e, a, {
             useNationalPrefixFormattingRule: !0,
             getSeparatorAfterNationalPrefix: n,
-            metadata: a
+            metadata: t
         });
         if (g) return g
     }
-    return Hd(e, t, {
+    return Hd(e, a, {
         useNationalPrefixFormattingRule: !1,
         getSeparatorAfterNationalPrefix: n,
-        metadata: a
+        metadata: t
     })
 }
 
-function Hd(e, t, d) {
-    var a = d.metadata,
+function Hd(e, a, d) {
+    var t = d.metadata,
         i = d.useNationalPrefixFormattingRule,
         n = d.getSeparatorAfterNationalPrefix,
-        r = E(e.nationalSignificantNumber, t, {
+        r = E(e.nationalSignificantNumber, a, {
             carrierCode: e.carrierCode,
             useInternationalFormat: e.international,
             withNationalPrefix: i,
-            metadata: a
+            metadata: t
         });
-    if (i || (e.nationalPrefix ? r = e.nationalPrefix + n(t) + r : e.complexPrefixBeforeNationalSignificantNumber && (r = e.complexPrefixBeforeNationalSignificantNumber + " " + r)), se(r, e)) return r
+    if (i || (e.nationalPrefix ? r = e.nationalPrefix + n(a) + r : e.complexPrefixBeforeNationalSignificantNumber && (r = e.complexPrefixBeforeNationalSignificantNumber + " " + r)), se(r, e)) return r
 }
 
-function se(e, t) {
-    return x(e) === t.getNationalDigits()
+function se(e, a) {
+    return x(e) === a.getNationalDigits()
 }
 
-function le(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function le(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function Vd(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function Vd(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function ue(e, t, d) {
-    return t && Vd(e.prototype, t), d && Vd(e, d), Object.defineProperty(e, "prototype", {
+function ue(e, a, d) {
+    return a && Vd(e.prototype, a), d && Vd(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var Wd = function() {
     function e() {
         le(this, e)
     }
     return ue(e, [{
         key: "parse",
         value: function(d) {
             if (this.context = [{
                     or: !0,
                     instructions: []
                 }], this.parsePattern(d), this.context.length !== 1) throw new Error("Non-finalized contexts left when pattern parse ended");
-            var a = this.context[0],
-                i = a.branches,
-                n = a.instructions;
+            var t = this.context[0],
+                i = t.branches,
+                n = t.instructions;
             if (i) return {
                 op: "|",
                 args: i.concat([sd(n)])
             };
             if (n.length === 0) throw new Error("Pattern is required");
             return n.length === 1 ? n[0] : n
         }
@@ -4428,23 +4428,23 @@
         value: function() {
             return this.context[this.context.length - 1]
         }
     }, {
         key: "parsePattern",
         value: function(d) {
             if (!d) throw new Error("Pattern is required");
-            var a = d.match(ce);
-            if (!a) {
+            var t = d.match(ce);
+            if (!t) {
                 if (fe.test(d)) throw new Error("Illegal characters found in a pattern: ".concat(d));
                 this.getContext().instructions = this.getContext().instructions.concat(d.split(""));
                 return
             }
-            var i = a[1],
-                n = d.slice(0, a.index),
-                r = d.slice(a.index + i.length);
+            var i = t[1],
+                n = d.slice(0, t.index),
+                r = d.slice(t.index + i.length);
             switch (i) {
                 case "(?:":
                     n && this.parsePattern(n), this.startContext({
                         or: !0,
                         instructions: [],
                         branches: []
                     });
@@ -4483,119 +4483,119 @@
             }
             r && this.parsePattern(r)
         }
     }]), e
 }();
 
 function ge(e) {
-    for (var t = [], d = 0; d < e.length;) {
+    for (var a = [], d = 0; d < e.length;) {
         if (e[d] === "-") {
             if (d === 0 || d === e.length - 1) throw new Error("Couldn't parse a one-of set pattern: ".concat(e));
-            for (var a = e[d - 1].charCodeAt(0) + 1, i = e[d + 1].charCodeAt(0) - 1, n = a; n <= i;) t.push(String.fromCharCode(n)), n++
-        } else t.push(e[d]);
+            for (var t = e[d - 1].charCodeAt(0) + 1, i = e[d + 1].charCodeAt(0) - 1, n = t; n <= i;) a.push(String.fromCharCode(n)), n++
+        } else a.push(e[d]);
         d++
     }
-    return t
+    return a
 }
 var fe = /[\(\)\[\]\?\:\|]/,
     ce = new RegExp("(\\||\\(\\?\\:|\\)|\\[|\\])");
 
 function sd(e) {
     return e.length === 1 ? e[0] : e
 }
 
-function Kd(e, t) {
+function Kd(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = $e(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = $e(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function $e(e, t) {
+function $e(e, a) {
     if (e) {
-        if (typeof e == "string") return Yd(e, t);
+        if (typeof e == "string") return Yd(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Yd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Yd(e, a)
     }
 }
 
-function Yd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Yd(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function me(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function me(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function zd(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function zd(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function he(e, t, d) {
-    return t && zd(e.prototype, t), d && zd(e, d), Object.defineProperty(e, "prototype", {
+function he(e, a, d) {
+    return a && zd(e.prototype, a), d && zd(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var qd = function() {
-    function e(t) {
-        me(this, e), this.matchTree = new Wd().parse(t)
+    function e(a) {
+        me(this, e), this.matchTree = new Wd().parse(a)
     }
     return he(e, [{
         key: "match",
         value: function(d) {
-            var a = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
-                i = a.allowOverflow;
+            var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
+                i = t.allowOverflow;
             if (!d) throw new Error("String is required");
             var n = ld(d.split(""), this.matchTree, !0);
             if (n && n.match && delete n.matchedChars, !(n && n.overflow && !i)) return n
         }
     }]), e
 }();
 
-function ld(e, t, d) {
-    if (typeof t == "string") {
-        var a = e.join("");
-        return t.indexOf(a) === 0 ? e.length === t.length ? {
+function ld(e, a, d) {
+    if (typeof a == "string") {
+        var t = e.join("");
+        return a.indexOf(t) === 0 ? e.length === a.length ? {
             match: !0,
             matchedChars: e
         } : {
             partialMatch: !0
-        } : a.indexOf(t) === 0 ? d && e.length > t.length ? {
+        } : t.indexOf(a) === 0 ? d && e.length > a.length ? {
             overflow: !0
         } : {
             match: !0,
-            matchedChars: e.slice(0, t.length)
+            matchedChars: e.slice(0, a.length)
         } : void 0
     }
-    if (Array.isArray(t)) {
-        for (var i = e.slice(), n = 0; n < t.length;) {
-            var r = t[n],
-                o = ld(i, r, d && n === t.length - 1);
+    if (Array.isArray(a)) {
+        for (var i = e.slice(), n = 0; n < a.length;) {
+            var r = a[n],
+                o = ld(i, r, d && n === a.length - 1);
             if (o) {
                 if (o.overflow) return o;
                 if (o.match) {
-                    if (i = i.slice(o.matchedChars.length), i.length === 0) return n === t.length - 1 ? {
+                    if (i = i.slice(o.matchedChars.length), i.length === 0) return n === a.length - 1 ? {
                         match: !0,
                         matchedChars: e
                     } : {
                         partialMatch: !0
                     }
                 } else {
                     if (o.partialMatch) return {
@@ -4610,17 +4610,17 @@
         return d ? {
             overflow: !0
         } : {
             match: !0,
             matchedChars: e.slice(0, e.length - i.length)
         }
     }
-    switch (t.op) {
+    switch (a.op) {
         case "|":
-            for (var s, l = Kd(t.args), g; !(g = l()).done;) {
+            for (var s, l = Kd(a.args), g; !(g = l()).done;) {
                 var h = g.value,
                     $ = ld(e, h, d);
                 if ($) {
                     if ($.overflow) return $;
                     if ($.match) return {
                         match: !0,
                         matchedChars: $.matchedChars
@@ -4630,79 +4630,79 @@
 `.concat(JSON.stringify($, null, 2)))
                 }
             }
             return s ? {
                 partialMatch: !0
             } : void 0;
         case "[]":
-            for (var O = Kd(t.args), L; !(L = O()).done;) {
-                var S = L.value;
-                if (e[0] === S) return e.length === 1 ? {
+            for (var O = Kd(a.args), L; !(L = O()).done;) {
+                var I = L.value;
+                if (e[0] === I) return e.length === 1 ? {
                     match: !0,
                     matchedChars: e
                 } : d ? {
                     overflow: !0
                 } : {
                     match: !0,
-                    matchedChars: [S]
+                    matchedChars: [I]
                 }
             }
             return;
         default:
-            throw new Error("Unsupported instruction tree: ".concat(t))
+            throw new Error("Unsupported instruction tree: ".concat(a))
     }
 }
 
-function Zd(e, t) {
+function Zd(e, a) {
     var d = typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d) return (d = d.call(e)).next.bind(d);
-    if (Array.isArray(e) || (d = be(e)) || t && e && typeof e.length == "number") {
+    if (Array.isArray(e) || (d = be(e)) || a && e && typeof e.length == "number") {
         d && (e = d);
-        var a = 0;
+        var t = 0;
         return function() {
-            return a >= e.length ? {
+            return t >= e.length ? {
                 done: !0
             } : {
                 done: !1,
-                value: e[a++]
+                value: e[t++]
             }
         }
     }
     throw new TypeError(`Invalid attempt to iterate non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function be(e, t) {
+function be(e, a) {
     if (e) {
-        if (typeof e == "string") return Xd(e, t);
+        if (typeof e == "string") return Xd(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Xd(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return Xd(e, a)
     }
 }
 
-function Xd(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function Xd(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function ve(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function ve(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function Jd(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function Jd(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function xe(e, t, d) {
-    return t && Jd(e.prototype, t), d && Jd(e, d), Object.defineProperty(e, "prototype", {
+function xe(e, a, d) {
+    return a && Jd(e.prototype, a), d && Jd(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var ud = "9",
     pe = 15,
     ye = M(ud, pe),
     ke = /[- ]/,
@@ -4712,154 +4712,154 @@
     },
     Ce = H && function() {
         return /\d(?=[^,}][^,}])/g
     },
     Ne = new RegExp("[" + m + "]*\\$1[" + m + "]*(\\$\\d[" + m + "]*)*$"),
     Qd = 3,
     d0 = function() {
-        function e(t) {
-            var d = t.state,
-                a = t.metadata;
-            ve(this, e), this.metadata = a, this.resetFormat()
+        function e(a) {
+            var d = a.state,
+                t = a.metadata;
+            ve(this, e), this.metadata = t, this.resetFormat()
         }
         return xe(e, [{
             key: "resetFormat",
             value: function() {
                 this.chosenFormat = void 0, this.template = void 0, this.nationalNumberTemplate = void 0, this.populatedNationalNumberTemplate = void 0, this.populatedNationalNumberTemplatePosition = -1
             }
         }, {
             key: "reset",
-            value: function(d, a) {
-                this.resetFormat(), d ? (this.isNANP = d.callingCode() === "1", this.matchingFormats = d.formats(), a.nationalSignificantNumber && this.narrowDownMatchingFormats(a)) : (this.isNANP = void 0, this.matchingFormats = [])
+            value: function(d, t) {
+                this.resetFormat(), d ? (this.isNANP = d.callingCode() === "1", this.matchingFormats = d.formats(), t.nationalSignificantNumber && this.narrowDownMatchingFormats(t)) : (this.isNANP = void 0, this.matchingFormats = [])
             }
         }, {
             key: "format",
-            value: function(d, a) {
+            value: function(d, t) {
                 var i = this;
-                if (Ud(a.nationalSignificantNumber, this.metadata))
+                if (Ud(t.nationalSignificantNumber, this.metadata))
                     for (var n = Zd(this.matchingFormats), r; !(r = n()).done;) {
                         var o = r.value,
-                            s = od(a, o, {
+                            s = od(t, o, {
                                 metadata: this.metadata,
                                 shouldTryNationalPrefixFormattingRule: function(g) {
                                     return i.shouldTryNationalPrefixFormattingRule(g, {
-                                        international: a.international,
-                                        nationalPrefix: a.nationalPrefix
+                                        international: t.international,
+                                        nationalPrefix: t.nationalPrefix
                                     })
                                 },
                                 getSeparatorAfterNationalPrefix: function(g) {
                                     return i.getSeparatorAfterNationalPrefix(g)
                                 }
                             });
-                        if (s) return this.resetFormat(), this.chosenFormat = o, this.setNationalNumberTemplate(s.replace(/\d/g, c), a), this.populatedNationalNumberTemplate = s, this.populatedNationalNumberTemplatePosition = this.template.lastIndexOf(c), s
+                        if (s) return this.resetFormat(), this.chosenFormat = o, this.setNationalNumberTemplate(s.replace(/\d/g, c), t), this.populatedNationalNumberTemplate = s, this.populatedNationalNumberTemplatePosition = this.template.lastIndexOf(c), s
                     }
-                return this.formatNationalNumberWithNextDigits(d, a)
+                return this.formatNationalNumberWithNextDigits(d, t)
             }
         }, {
             key: "formatNationalNumberWithNextDigits",
-            value: function(d, a) {
+            value: function(d, t) {
                 var i = this.chosenFormat,
-                    n = this.chooseFormat(a);
-                if (n) return n === i ? this.formatNextNationalNumberDigits(d) : this.formatNextNationalNumberDigits(a.getNationalDigits())
+                    n = this.chooseFormat(t);
+                if (n) return n === i ? this.formatNextNationalNumberDigits(d) : this.formatNextNationalNumberDigits(t.getNationalDigits())
             }
         }, {
             key: "narrowDownMatchingFormats",
             value: function(d) {
-                var a = this,
+                var t = this,
                     i = d.nationalSignificantNumber,
                     n = d.nationalPrefix,
                     r = d.international,
                     o = i,
                     s = o.length - Qd;
                 s < 0 && (s = 0), this.matchingFormats = this.matchingFormats.filter(function(l) {
-                    return a.formatSuits(l, r, n) && a.formatMatches(l, o, s)
+                    return t.formatSuits(l, r, n) && t.formatMatches(l, o, s)
                 }), this.chosenFormat && this.matchingFormats.indexOf(this.chosenFormat) === -1 && this.resetFormat()
             }
         }, {
             key: "formatSuits",
-            value: function(d, a, i) {
-                return !(i && !d.usesNationalPrefix() && !d.nationalPrefixIsOptionalWhenFormattingInNationalFormat() || !a && !i && d.nationalPrefixIsMandatoryWhenFormattingInNationalFormat())
+            value: function(d, t, i) {
+                return !(i && !d.usesNationalPrefix() && !d.nationalPrefixIsOptionalWhenFormattingInNationalFormat() || !t && !i && d.nationalPrefixIsMandatoryWhenFormattingInNationalFormat())
             }
         }, {
             key: "formatMatches",
-            value: function(d, a, i) {
+            value: function(d, t, i) {
                 var n = d.leadingDigitsPatterns().length;
                 if (n === 0) return !0;
                 i = Math.min(i, n - 1);
                 var r = d.leadingDigitsPatterns()[i];
-                if (a.length < Qd) try {
-                    return new qd(r).match(a, {
+                if (t.length < Qd) try {
+                    return new qd(r).match(t, {
                         allowOverflow: !0
                     }) !== void 0
                 } catch (o) {
                     return console.error(o), !0
                 }
-                return new RegExp("^(".concat(r, ")")).test(a)
+                return new RegExp("^(".concat(r, ")")).test(t)
             }
         }, {
             key: "getFormatFormat",
-            value: function(d, a) {
-                return a ? d.internationalFormat() : d.format()
+            value: function(d, t) {
+                return t ? d.internationalFormat() : d.format()
             }
         }, {
             key: "chooseFormat",
             value: function(d) {
-                for (var a = this, i = function() {
+                for (var t = this, i = function() {
                         var l = r.value;
-                        return a.chosenFormat === l ? "break" : Ne.test(a.getFormatFormat(l, d.international)) ? a.createTemplateForFormat(l, d) ? (a.chosenFormat = l, "break") : (a.matchingFormats = a.matchingFormats.filter(function(g) {
+                        return t.chosenFormat === l ? "break" : Ne.test(t.getFormatFormat(l, d.international)) ? t.createTemplateForFormat(l, d) ? (t.chosenFormat = l, "break") : (t.matchingFormats = t.matchingFormats.filter(function(g) {
                             return g !== l
                         }), "continue") : "continue"
                     }, n = Zd(this.matchingFormats.slice()), r; !(r = n()).done;) {
                     var o = i();
                     if (o === "break") break
                 }
                 return this.chosenFormat || this.resetFormat(), this.chosenFormat
             }
         }, {
             key: "createTemplateForFormat",
-            value: function(d, a) {
+            value: function(d, t) {
                 if (!(H && d.pattern().indexOf("|") >= 0)) {
-                    var i = this.getTemplateForFormat(d, a);
-                    if (i) return this.setNationalNumberTemplate(i, a), !0
+                    var i = this.getTemplateForFormat(d, t);
+                    if (i) return this.setNationalNumberTemplate(i, t), !0
                 }
             }
         }, {
             key: "getSeparatorAfterNationalPrefix",
             value: function(d) {
                 return this.isNANP || d && d.nationalPrefixFormattingRule() && ke.test(d.nationalPrefixFormattingRule()) ? " " : ""
             }
         }, {
             key: "getInternationalPrefixBeforeCountryCallingCode",
-            value: function(d, a) {
+            value: function(d, t) {
                 var i = d.IDDPrefix,
                     n = d.missingPlus;
-                return i ? a && a.spacing === !1 ? i : i + " " : n ? "" : "+"
+                return i ? t && t.spacing === !1 ? i : i + " " : n ? "" : "+"
             }
         }, {
             key: "getTemplate",
             value: function(d) {
                 if (this.template) {
-                    for (var a = -1, i = 0, n = d.international ? this.getInternationalPrefixBeforeCountryCallingCode(d, {
+                    for (var t = -1, i = 0, n = d.international ? this.getInternationalPrefixBeforeCountryCallingCode(d, {
                             spacing: !1
-                        }) : ""; i < n.length + d.getDigitsWithoutInternationalPrefix().length;) a = this.template.indexOf(c, a + 1), i++;
-                    return rd(this.template, a + 1)
+                        }) : ""; i < n.length + d.getDigitsWithoutInternationalPrefix().length;) t = this.template.indexOf(c, t + 1), i++;
+                    return rd(this.template, t + 1)
                 }
             }
         }, {
             key: "setNationalNumberTemplate",
-            value: function(d, a) {
-                this.nationalNumberTemplate = d, this.populatedNationalNumberTemplate = d, this.populatedNationalNumberTemplatePosition = -1, a.international ? this.template = this.getInternationalPrefixBeforeCountryCallingCode(a).replace(/[\d\+]/g, c) + M(c, a.callingCode.length) + " " + d : this.template = d
+            value: function(d, t) {
+                this.nationalNumberTemplate = d, this.populatedNationalNumberTemplate = d, this.populatedNationalNumberTemplatePosition = -1, t.international ? this.template = this.getInternationalPrefixBeforeCountryCallingCode(t).replace(/[\d\+]/g, c) + M(c, t.callingCode.length) + " " + d : this.template = d
             }
         }, {
             key: "getTemplateForFormat",
-            value: function(d, a) {
-                var i = a.nationalSignificantNumber,
-                    n = a.international,
-                    r = a.nationalPrefix,
-                    o = a.complexPrefixBeforeNationalSignificantNumber,
+            value: function(d, t) {
+                var i = t.nationalSignificantNumber,
+                    n = t.international,
+                    r = t.nationalPrefix,
+                    o = t.complexPrefixBeforeNationalSignificantNumber,
                     s = d.pattern();
                 H && (s = s.replace(_e(), "\\d").replace(Ce(), "\\d"));
                 var l = ye.match(s)[0];
                 if (!(i.length > l.length)) {
                     var g = new RegExp("^" + s + "$"),
                         h = i.replace(/\d/g, ud);
                     g.test(h) && (l = h);
@@ -4867,382 +4867,382 @@
                         O;
                     if (this.shouldTryNationalPrefixFormattingRule(d, {
                             international: n,
                             nationalPrefix: r
                         })) {
                         var L = $.replace(Q, d.nationalPrefixFormattingRule());
                         if (x(d.nationalPrefixFormattingRule()) === (r || "") + x("$1") && ($ = L, O = !0, r))
-                            for (var S = r.length; S > 0;) $ = $.replace(/\d/, c), S--
+                            for (var I = r.length; I > 0;) $ = $.replace(/\d/, c), I--
                     }
                     var p = l.replace(new RegExp(s), $).replace(new RegExp(ud, "g"), c);
                     return O || (o ? p = M(c, o.length) + " " + p : r && (p = M(c, r.length) + this.getSeparatorAfterNationalPrefix(d) + p)), n && (p = T(p)), p
                 }
             }
         }, {
             key: "formatNextNationalNumberDigits",
             value: function(d) {
-                var a = jd(this.populatedNationalNumberTemplate, this.populatedNationalNumberTemplatePosition, d);
-                if (!a) {
+                var t = jd(this.populatedNationalNumberTemplate, this.populatedNationalNumberTemplatePosition, d);
+                if (!t) {
                     this.resetFormat();
                     return
                 }
-                return this.populatedNationalNumberTemplate = a[0], this.populatedNationalNumberTemplatePosition = a[1], rd(this.populatedNationalNumberTemplate, this.populatedNationalNumberTemplatePosition + 1)
+                return this.populatedNationalNumberTemplate = t[0], this.populatedNationalNumberTemplatePosition = t[1], rd(this.populatedNationalNumberTemplate, this.populatedNationalNumberTemplatePosition + 1)
             }
         }, {
             key: "shouldTryNationalPrefixFormattingRule",
-            value: function(d, a) {
-                var i = a.international,
-                    n = a.nationalPrefix;
+            value: function(d, t) {
+                var i = t.international,
+                    n = t.nationalPrefix;
                 if (d.nationalPrefixFormattingRule()) {
                     var r = d.usesNationalPrefix();
                     if (r && n || !r && !i) return !0
                 }
             }
         }]), e
     }();
 
-function a0(e, t) {
-    return Te(e) || Ie(e, t) || Se(e, t) || Pe()
+function t0(e, a) {
+    return Te(e) || Se(e, a) || Ie(e, a) || Pe()
 }
 
 function Pe() {
     throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function Se(e, t) {
+function Ie(e, a) {
     if (e) {
-        if (typeof e == "string") return e0(e, t);
+        if (typeof e == "string") return e0(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return e0(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return e0(e, a)
     }
 }
 
-function e0(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function e0(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function Ie(e, t) {
+function Se(e, a) {
     var d = e == null ? null : typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d != null) {
-        var a = [],
+        var t = [],
             i = !0,
             n = !1,
             r, o;
         try {
-            for (d = d.call(e); !(i = (r = d.next()).done) && (a.push(r.value), !(t && a.length === t)); i = !0);
+            for (d = d.call(e); !(i = (r = d.next()).done) && (t.push(r.value), !(a && t.length === a)); i = !0);
         } catch (s) {
             n = !0, o = s
         } finally {
             try {
                 !i && d.return != null && d.return()
             } finally {
                 if (n) throw o
             }
         }
-        return a
+        return t
     }
 }
 
 function Te(e) {
     if (Array.isArray(e)) return e
 }
 
-function Ee(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function Ee(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function t0(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function a0(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function Ae(e, t, d) {
-    return t && t0(e.prototype, t), d && t0(e, d), Object.defineProperty(e, "prototype", {
+function Ae(e, a, d) {
+    return a && a0(e.prototype, a), d && a0(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var Fe = "[" + m + k + "]+",
     we = new RegExp("^" + Fe + "$", "i"),
     Me = "(?:[" + vd + "][" + m + k + "]*|[" + m + k + "]+)",
     Oe = new RegExp("[^" + m + k + "]+.*$"),
     Le = /[^\d\[\]]/,
     i0 = function() {
-        function e(t) {
-            var d = t.defaultCountry,
-                a = t.defaultCallingCode,
-                i = t.metadata,
-                n = t.onNationalSignificantNumberChange;
-            Ee(this, e), this.defaultCountry = d, this.defaultCallingCode = a, this.metadata = i, this.onNationalSignificantNumberChange = n
+        function e(a) {
+            var d = a.defaultCountry,
+                t = a.defaultCallingCode,
+                i = a.metadata,
+                n = a.onNationalSignificantNumberChange;
+            Ee(this, e), this.defaultCountry = d, this.defaultCallingCode = t, this.metadata = i, this.onNationalSignificantNumberChange = n
         }
         return Ae(e, [{
             key: "input",
-            value: function(d, a) {
+            value: function(d, t) {
                 var i = Ge(d),
-                    n = a0(i, 2),
+                    n = t0(i, 2),
                     r = n[0],
                     o = n[1],
                     s = x(r),
                     l;
-                return o && (a.digits || (a.startInternationalNumber(), s || (l = !0))), s && this.inputDigits(s, a), {
+                return o && (t.digits || (t.startInternationalNumber(), s || (l = !0))), s && this.inputDigits(s, t), {
                     digits: s,
                     justLeadingPlus: l
                 }
             }
         }, {
             key: "inputDigits",
-            value: function(d, a) {
-                var i = a.digits,
+            value: function(d, t) {
+                var i = t.digits,
                     n = i.length < 3 && i.length + d.length >= 3;
-                if (a.appendDigits(d), n && this.extractIddPrefix(a), this.isWaitingForCountryCallingCode(a)) {
-                    if (!this.extractCountryCallingCode(a)) return
-                } else a.appendNationalSignificantNumberDigits(d);
-                a.international || this.hasExtractedNationalSignificantNumber || this.extractNationalSignificantNumber(a.getNationalDigits(), function(r) {
-                    return a.update(r)
+                if (t.appendDigits(d), n && this.extractIddPrefix(t), this.isWaitingForCountryCallingCode(t)) {
+                    if (!this.extractCountryCallingCode(t)) return
+                } else t.appendNationalSignificantNumberDigits(d);
+                t.international || this.hasExtractedNationalSignificantNumber || this.extractNationalSignificantNumber(t.getNationalDigits(), function(r) {
+                    return t.update(r)
                 })
             }
         }, {
             key: "isWaitingForCountryCallingCode",
             value: function(d) {
-                var a = d.international,
+                var t = d.international,
                     i = d.callingCode;
-                return a && !i
+                return t && !i
             }
         }, {
             key: "extractCountryCallingCode",
             value: function(d) {
-                var a = ad("+" + d.getDigitsWithoutInternationalPrefix(), this.defaultCountry, this.defaultCallingCode, this.metadata.metadata),
-                    i = a.countryCallingCode,
-                    n = a.number;
+                var t = td("+" + d.getDigitsWithoutInternationalPrefix(), this.defaultCountry, this.defaultCallingCode, this.metadata.metadata),
+                    i = t.countryCallingCode,
+                    n = t.number;
                 if (i) return d.setCallingCode(i), d.update({
                     nationalSignificantNumber: n
                 }), !0
             }
         }, {
             key: "reset",
             value: function(d) {
                 if (d) {
                     this.hasSelectedNumberingPlan = !0;
-                    var a = d._nationalPrefixForParsing();
-                    this.couldPossiblyExtractAnotherNationalSignificantNumber = a && Le.test(a)
+                    var t = d._nationalPrefixForParsing();
+                    this.couldPossiblyExtractAnotherNationalSignificantNumber = t && Le.test(t)
                 } else this.hasSelectedNumberingPlan = void 0, this.couldPossiblyExtractAnotherNationalSignificantNumber = void 0
             }
         }, {
             key: "extractNationalSignificantNumber",
-            value: function(d, a) {
+            value: function(d, t) {
                 if (this.hasSelectedNumberingPlan) {
                     var i = N(d, this.metadata),
                         n = i.nationalPrefix,
                         r = i.nationalNumber,
                         o = i.carrierCode;
-                    if (r !== d) return this.onExtractedNationalNumber(n, o, r, d, a), !0
+                    if (r !== d) return this.onExtractedNationalNumber(n, o, r, d, t), !0
                 }
             }
         }, {
             key: "extractAnotherNationalSignificantNumber",
-            value: function(d, a, i) {
+            value: function(d, t, i) {
                 if (!this.hasExtractedNationalSignificantNumber) return this.extractNationalSignificantNumber(d, i);
                 if (this.couldPossiblyExtractAnotherNationalSignificantNumber) {
                     var n = N(d, this.metadata),
                         r = n.nationalPrefix,
                         o = n.nationalNumber,
                         s = n.carrierCode;
-                    if (o !== a) return this.onExtractedNationalNumber(r, s, o, d, i), !0
+                    if (o !== t) return this.onExtractedNationalNumber(r, s, o, d, i), !0
                 }
             }
         }, {
             key: "onExtractedNationalNumber",
-            value: function(d, a, i, n, r) {
+            value: function(d, t, i, n, r) {
                 var o, s, l = n.lastIndexOf(i);
                 if (l >= 0 && l === n.length - i.length) {
                     s = !0;
                     var g = n.slice(0, l);
                     g !== d && (o = g)
                 }
                 r({
                     nationalPrefix: d,
-                    carrierCode: a,
+                    carrierCode: t,
                     nationalSignificantNumber: i,
                     nationalSignificantNumberMatchesInput: s,
                     complexPrefixBeforeNationalSignificantNumber: o
                 }), this.hasExtractedNationalSignificantNumber = !0, this.onNationalSignificantNumberChange()
             }
         }, {
             key: "reExtractNationalSignificantNumber",
             value: function(d) {
-                if (this.extractAnotherNationalSignificantNumber(d.getNationalDigits(), d.nationalSignificantNumber, function(a) {
-                        return d.update(a)
+                if (this.extractAnotherNationalSignificantNumber(d.getNationalDigits(), d.nationalSignificantNumber, function(t) {
+                        return d.update(t)
                     })) return !0;
                 if (this.extractIddPrefix(d)) return this.extractCallingCodeAndNationalSignificantNumber(d), !0;
                 if (this.fixMissingPlus(d)) return this.extractCallingCodeAndNationalSignificantNumber(d), !0
             }
         }, {
             key: "extractIddPrefix",
             value: function(d) {
-                var a = d.international,
+                var t = d.international,
                     i = d.IDDPrefix,
                     n = d.digits,
                     r = d.nationalSignificantNumber;
-                if (!(a || i)) {
+                if (!(t || i)) {
                     var o = A(n, this.defaultCountry, this.defaultCallingCode, this.metadata.metadata);
                     if (o !== void 0 && o !== n) return d.update({
                         IDDPrefix: n.slice(0, n.length - o.length)
                     }), this.startInternationalNumber(d, {
                         country: void 0,
                         callingCode: void 0
                     }), !0
                 }
             }
         }, {
             key: "fixMissingPlus",
             value: function(d) {
                 if (!d.international) {
-                    var a = F(d.digits, this.defaultCountry, this.defaultCallingCode, this.metadata.metadata),
-                        i = a.countryCallingCode,
-                        n = a.number;
+                    var t = F(d.digits, this.defaultCountry, this.defaultCallingCode, this.metadata.metadata),
+                        i = t.countryCallingCode,
+                        n = t.number;
                     if (i) return d.update({
                         missingPlus: !0
                     }), this.startInternationalNumber(d, {
                         country: d.country,
                         callingCode: i
                     }), !0
                 }
             }
         }, {
             key: "startInternationalNumber",
-            value: function(d, a) {
-                var i = a.country,
-                    n = a.callingCode;
+            value: function(d, t) {
+                var i = t.country,
+                    n = t.callingCode;
                 d.startInternationalNumber(i, n), d.nationalSignificantNumber && (d.resetNationalSignificantNumber(), this.onNationalSignificantNumberChange(), this.hasExtractedNationalSignificantNumber = void 0)
             }
         }, {
             key: "extractCallingCodeAndNationalSignificantNumber",
             value: function(d) {
-                this.extractCountryCallingCode(d) && this.extractNationalSignificantNumber(d.getNationalDigits(), function(a) {
-                    return d.update(a)
+                this.extractCountryCallingCode(d) && this.extractNationalSignificantNumber(d.getNationalDigits(), function(t) {
+                    return d.update(t)
                 })
             }
         }]), e
     }();
 
 function Re(e) {
-    var t = e.search(Me);
-    if (!(t < 0)) {
-        e = e.slice(t);
+    var a = e.search(Me);
+    if (!(a < 0)) {
+        e = e.slice(a);
         var d;
         return e[0] === "+" && (d = !0, e = e.slice(1)), e = e.replace(Oe, ""), d && (e = "+" + e), e
     }
 }
 
 function De(e) {
-    var t = Re(e) || "";
-    return t[0] === "+" ? [t.slice(1), !0] : [t]
+    var a = Re(e) || "";
+    return a[0] === "+" ? [a.slice(1), !0] : [a]
 }
 
 function Ge(e) {
-    var t = De(e),
-        d = a0(t, 2),
-        a = d[0],
+    var a = De(e),
+        d = t0(a, 2),
+        t = d[0],
         i = d[1];
-    return we.test(a) || (a = ""), [a, i]
+    return we.test(t) || (t = ""), [t, i]
 }
 
-function Be(e, t) {
-    return Ve(e) || Ue(e, t) || He(e, t) || je()
+function Be(e, a) {
+    return Ve(e) || Ue(e, a) || He(e, a) || je()
 }
 
 function je() {
     throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
 }
 
-function He(e, t) {
+function He(e, a) {
     if (e) {
-        if (typeof e == "string") return n0(e, t);
+        if (typeof e == "string") return n0(e, a);
         var d = Object.prototype.toString.call(e).slice(8, -1);
         if (d === "Object" && e.constructor && (d = e.constructor.name), d === "Map" || d === "Set") return Array.from(e);
-        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return n0(e, t)
+        if (d === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(d)) return n0(e, a)
     }
 }
 
-function n0(e, t) {
-    (t == null || t > e.length) && (t = e.length);
-    for (var d = 0, a = new Array(t); d < t; d++) a[d] = e[d];
-    return a
+function n0(e, a) {
+    (a == null || a > e.length) && (a = e.length);
+    for (var d = 0, t = new Array(a); d < a; d++) t[d] = e[d];
+    return t
 }
 
-function Ue(e, t) {
+function Ue(e, a) {
     var d = e == null ? null : typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
     if (d != null) {
-        var a = [],
+        var t = [],
             i = !0,
             n = !1,
             r, o;
         try {
-            for (d = d.call(e); !(i = (r = d.next()).done) && (a.push(r.value), !(t && a.length === t)); i = !0);
+            for (d = d.call(e); !(i = (r = d.next()).done) && (t.push(r.value), !(a && t.length === a)); i = !0);
         } catch (s) {
             n = !0, o = s
         } finally {
             try {
                 !i && d.return != null && d.return()
             } finally {
                 if (n) throw o
             }
         }
-        return a
+        return t
     }
 }
 
 function Ve(e) {
     if (Array.isArray(e)) return e
 }
 
-function We(e, t) {
-    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+function We(e, a) {
+    if (!(e instanceof a)) throw new TypeError("Cannot call a class as a function")
 }
 
-function r0(e, t) {
-    for (var d = 0; d < t.length; d++) {
-        var a = t[d];
-        a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
+function r0(e, a) {
+    for (var d = 0; d < a.length; d++) {
+        var t = a[d];
+        t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(e, t.key, t)
     }
 }
 
-function Ke(e, t, d) {
-    return t && r0(e.prototype, t), d && r0(e, d), Object.defineProperty(e, "prototype", {
+function Ke(e, a, d) {
+    return a && r0(e.prototype, a), d && r0(e, d), Object.defineProperty(e, "prototype", {
         writable: !1
     }), e
 }
 var o0 = !1,
     U = function() {
-        function e(t, d) {
+        function e(a, d) {
             We(this, e), this.metadata = new u(d);
-            var a = this.getCountryAndCallingCode(t),
-                i = Be(a, 2),
+            var t = this.getCountryAndCallingCode(a),
+                i = Be(t, 2),
                 n = i[0],
                 r = i[1];
             this.defaultCountry = n, this.defaultCallingCode = r, this.reset()
         }
         return Ke(e, [{
             key: "getCountryAndCallingCode",
             value: function(d) {
-                var a, i;
-                return d && (_(d) ? (a = d.defaultCountry, i = d.defaultCallingCode) : a = d), a && !this.metadata.hasCountry(a) && (a = void 0), i && o0 && this.metadata.isNonGeographicCallingCode(i) && (a = "001"), [a, i]
+                var t, i;
+                return d && (_(d) ? (t = d.defaultCountry, i = d.defaultCallingCode) : t = d), t && !this.metadata.hasCountry(t) && (t = void 0), i && o0 && this.metadata.isNonGeographicCallingCode(i) && (t = "001"), [t, i]
             }
         }, {
             key: "input",
             value: function(d) {
-                var a = this.parser.input(d, this.state),
-                    i = a.digits,
-                    n = a.justLeadingPlus;
+                var t = this.parser.input(d, this.state),
+                    i = t.digits,
+                    n = t.justLeadingPlus;
                 if (n) this.formattedOutput = "+";
                 else if (i) {
                     this.determineTheCountryIfNeeded(), this.state.nationalSignificantNumber && this.formatter.narrowDownMatchingFormats(this.state);
                     var r;
                     if (this.metadata.hasSelectedNumberingPlan() && (r = this.formatter.format(i, this.state)), r === void 0 && this.parser.reExtractNationalSignificantNumber(this.state)) {
                         this.determineTheCountryIfNeeded();
                         var o = this.state.getNationalDigits();
@@ -5310,34 +5310,34 @@
             key: "determineTheCountryIfNeeded",
             value: function() {
                 (!this.state.country || this.isCountryCallingCodeAmbiguous()) && this.determineTheCountry()
             }
         }, {
             key: "getFullNumber",
             value: function(d) {
-                var a = this;
+                var t = this;
                 if (this.isInternational()) {
                     var i = function(o) {
-                            return a.formatter.getInternationalPrefixBeforeCountryCallingCode(a.state, {
+                            return t.formatter.getInternationalPrefixBeforeCountryCallingCode(t.state, {
                                 spacing: !!o
                             }) + o
                         },
                         n = this.state.callingCode;
                     return i(n ? d ? "".concat(n, " ").concat(d) : n : "".concat(this.state.getDigitsWithoutInternationalPrefix()))
                 }
                 return d
             }
         }, {
             key: "getNonFormattedNationalNumberWithPrefix",
             value: function() {
                 var d = this.state,
-                    a = d.nationalSignificantNumber,
+                    t = d.nationalSignificantNumber,
                     i = d.complexPrefixBeforeNationalSignificantNumber,
                     n = d.nationalPrefix,
-                    r = a,
+                    r = t,
                     o = i || n;
                 return o && (r = o + r), r
             }
         }, {
             key: "getNonFormattedNumber",
             value: function() {
                 var d = this.state.nationalSignificantNumberMatchesInput;
@@ -5349,66 +5349,66 @@
                 var d = this.getNonFormattedNumber();
                 if (d) return d.replace(/[\+\d]/g, c)
             }
         }, {
             key: "isCountryCallingCodeAmbiguous",
             value: function() {
                 var d = this.state.callingCode,
-                    a = this.metadata.getCountryCodesForCallingCode(d);
-                return a && a.length > 1
+                    t = this.metadata.getCountryCodesForCallingCode(d);
+                return t && t.length > 1
             }
         }, {
             key: "determineTheCountry",
             value: function() {
                 this.state.setCountry(id(this.isInternational() ? this.state.callingCode : this.defaultCallingCode, {
                     nationalNumber: this.state.nationalSignificantNumber,
                     defaultCountry: this.defaultCountry,
                     metadata: this.metadata
                 }))
             }
         }, {
             key: "getNumberValue",
             value: function() {
                 var d = this.state,
-                    a = d.digits,
+                    t = d.digits,
                     i = d.callingCode,
                     n = d.country,
                     r = d.nationalSignificantNumber;
-                if (a) {
-                    if (this.isInternational()) return i ? "+" + i + r : "+" + a;
+                if (t) {
+                    if (this.isInternational()) return i ? "+" + i + r : "+" + t;
                     if (n || i) {
                         var o = n ? this.metadata.countryCallingCode() : i;
                         return "+" + o + r
                     }
                 }
             }
         }, {
             key: "getNumber",
             value: function() {
                 var d = this.state,
-                    a = d.nationalSignificantNumber,
+                    t = d.nationalSignificantNumber,
                     i = d.carrierCode,
                     n = d.callingCode,
                     r = this._getCountry();
-                if (a && !(!r && !n)) {
+                if (t && !(!r && !n)) {
                     if (r && r === this.defaultCountry) {
                         var o = new u(this.metadata.metadata);
                         o.selectNumberingPlan(r);
                         var s = o.numberingPlan.callingCode(),
                             l = this.metadata.getCountryCodesForCallingCode(s);
                         if (l.length > 1) {
-                            var g = w(a, {
+                            var g = w(t, {
                                 countries: l,
                                 defaultCountry: this.defaultCountry,
                                 metadata: this.metadata.metadata
                             });
                             g && (r = g)
                         }
                     }
-                    var h = new Ld(r || n, a, this.metadata.metadata);
+                    var h = new Ld(r || n, t, this.metadata.metadata);
                     return i && (h.carrierCode = i), h
                 }
             }
         }, {
             key: "isPossible",
             value: function() {
                 var d = this.getNumber();
@@ -5445,19 +5445,19 @@
 function P(e) {
     return U.call(this, e, R)
 }
 P.prototype = Object.create(U.prototype, {});
 P.prototype.constructor = P;
 
 function gd() {
-    return I(V, arguments)
+    return S(V, arguments)
 }
 
 function fd() {
-    return I(v, arguments)
+    return S(v, arguments)
 }
 var s0 = new Map([
     ["AF", "Afghanistan"],
     ["AX", "\xC5land Islands"],
     ["AL", "Albania"],
     ["DZ", "Algeria"],
     ["AS", "American Samoa"],
@@ -5708,176 +5708,184 @@
     ["YE", "Yemen"],
     ["ZM", "Zambia"],
     ["ZW", "Zimbabwe"]
 ]);
 var l0 = '\uFEFF[is=django-phone-number]{--dummy-style: none}[is=django-phone-number]+[role=textbox]{display:flex;justify-content:flex-start}[is=django-phone-number]+[role=textbox].focus{--dummy-style: none}[is=django-phone-number]+[role=textbox]>.international-picker{display:flex;align-items:center;justify-content:flex-end;cursor:pointer}[is=django-phone-number]+[role=textbox]>.international-picker:empty::after{content:"";display:block;width:0;height:0;margin-right:12px;border-style:solid;border-width:5px 5px 0 5px;border-color:#000 rgba(0,0,0,0) rgba(0,0,0,0) rgba(0,0,0,0)}[is=django-phone-number]+[role=textbox]>.international-picker span{width:24px}[is=django-phone-number]+[role=textbox]>.phone-number-edit{overflow-x:hidden;margin-left:.5rem;flex-grow:1}[is=django-phone-number]+[role=textbox]>.phone-number-edit:focus-visible{outline:none}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog]{display:flex;flex-direction:column;box-shadow:#d3d3d3 0 0 1rem;position:absolute;top:0;left:0;background-color:#f8f8f8}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] input[type=search]{width:100%;margin:3px 0}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] input[type=search]:focus{--dummy-style: none}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] ul{list-style:none;padding:0;margin:0;overflow-y:scroll;max-height:450px}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] ul li{padding:.25rem;cursor:pointer}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] ul li:hover{background-color:rgba(0,0,0,.05)}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] ul li.selected{background-color:#e0ecf4;border:1px solid rgba(0,0,0,.15)}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog]+[role=dialog] ul li span{margin-right:.5rem}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog][aria-expanded=false]+[role=dialog]{display:none}[is=django-phone-number]+[role=textbox][aria-haspopup=dialog][aria-expanded=true]+[role=dialog]{display:block}.fib,.fi{background-size:contain;background-position:50%;background-repeat:no-repeat}.fi{position:relative;display:inline-block;width:1.333333em;line-height:1em}.fi:before{content:"\xA0"}.fi.fis{width:1em}.fi-xx{background-image:url(/static/node_modules/flag-icons/flags/4x3/xx.svg)}.fi-xx.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/xx.svg)}.fi-ad{background-image:url(/static/node_modules/flag-icons/flags/4x3/ad.svg)}.fi-ad.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ad.svg)}.fi-ae{background-image:url(/static/node_modules/flag-icons/flags/4x3/ae.svg)}.fi-ae.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ae.svg)}.fi-af{background-image:url(/static/node_modules/flag-icons/flags/4x3/af.svg)}.fi-af.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/af.svg)}.fi-ag{background-image:url(/static/node_modules/flag-icons/flags/4x3/ag.svg)}.fi-ag.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ag.svg)}.fi-ai{background-image:url(/static/node_modules/flag-icons/flags/4x3/ai.svg)}.fi-ai.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ai.svg)}.fi-al{background-image:url(/static/node_modules/flag-icons/flags/4x3/al.svg)}.fi-al.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/al.svg)}.fi-am{background-image:url(/static/node_modules/flag-icons/flags/4x3/am.svg)}.fi-am.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/am.svg)}.fi-ao{background-image:url(/static/node_modules/flag-icons/flags/4x3/ao.svg)}.fi-ao.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ao.svg)}.fi-aq{background-image:url(/static/node_modules/flag-icons/flags/4x3/aq.svg)}.fi-aq.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/aq.svg)}.fi-ar{background-image:url(/static/node_modules/flag-icons/flags/4x3/ar.svg)}.fi-ar.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ar.svg)}.fi-as{background-image:url(/static/node_modules/flag-icons/flags/4x3/as.svg)}.fi-as.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/as.svg)}.fi-at{background-image:url(/static/node_modules/flag-icons/flags/4x3/at.svg)}.fi-at.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/at.svg)}.fi-au{background-image:url(/static/node_modules/flag-icons/flags/4x3/au.svg)}.fi-au.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/au.svg)}.fi-aw{background-image:url(/static/node_modules/flag-icons/flags/4x3/aw.svg)}.fi-aw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/aw.svg)}.fi-ax{background-image:url(/static/node_modules/flag-icons/flags/4x3/ax.svg)}.fi-ax.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ax.svg)}.fi-az{background-image:url(/static/node_modules/flag-icons/flags/4x3/az.svg)}.fi-az.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/az.svg)}.fi-ba{background-image:url(/static/node_modules/flag-icons/flags/4x3/ba.svg)}.fi-ba.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ba.svg)}.fi-bb{background-image:url(/static/node_modules/flag-icons/flags/4x3/bb.svg)}.fi-bb.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bb.svg)}.fi-bd{background-image:url(/static/node_modules/flag-icons/flags/4x3/bd.svg)}.fi-bd.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bd.svg)}.fi-be{background-image:url(/static/node_modules/flag-icons/flags/4x3/be.svg)}.fi-be.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/be.svg)}.fi-bf{background-image:url(/static/node_modules/flag-icons/flags/4x3/bf.svg)}.fi-bf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bf.svg)}.fi-bg{background-image:url(/static/node_modules/flag-icons/flags/4x3/bg.svg)}.fi-bg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bg.svg)}.fi-bh{background-image:url(/static/node_modules/flag-icons/flags/4x3/bh.svg)}.fi-bh.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bh.svg)}.fi-bi{background-image:url(/static/node_modules/flag-icons/flags/4x3/bi.svg)}.fi-bi.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bi.svg)}.fi-bj{background-image:url(/static/node_modules/flag-icons/flags/4x3/bj.svg)}.fi-bj.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bj.svg)}.fi-bl{background-image:url(/static/node_modules/flag-icons/flags/4x3/bl.svg)}.fi-bl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bl.svg)}.fi-bm{background-image:url(/static/node_modules/flag-icons/flags/4x3/bm.svg)}.fi-bm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bm.svg)}.fi-bn{background-image:url(/static/node_modules/flag-icons/flags/4x3/bn.svg)}.fi-bn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bn.svg)}.fi-bo{background-image:url(/static/node_modules/flag-icons/flags/4x3/bo.svg)}.fi-bo.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bo.svg)}.fi-bq{background-image:url(/static/node_modules/flag-icons/flags/4x3/bq.svg)}.fi-bq.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bq.svg)}.fi-br{background-image:url(/static/node_modules/flag-icons/flags/4x3/br.svg)}.fi-br.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/br.svg)}.fi-bs{background-image:url(/static/node_modules/flag-icons/flags/4x3/bs.svg)}.fi-bs.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bs.svg)}.fi-bt{background-image:url(/static/node_modules/flag-icons/flags/4x3/bt.svg)}.fi-bt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bt.svg)}.fi-bv{background-image:url(/static/node_modules/flag-icons/flags/4x3/bv.svg)}.fi-bv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bv.svg)}.fi-bw{background-image:url(/static/node_modules/flag-icons/flags/4x3/bw.svg)}.fi-bw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bw.svg)}.fi-by{background-image:url(/static/node_modules/flag-icons/flags/4x3/by.svg)}.fi-by.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/by.svg)}.fi-bz{background-image:url(/static/node_modules/flag-icons/flags/4x3/bz.svg)}.fi-bz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/bz.svg)}.fi-ca{background-image:url(/static/node_modules/flag-icons/flags/4x3/ca.svg)}.fi-ca.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ca.svg)}.fi-cc{background-image:url(/static/node_modules/flag-icons/flags/4x3/cc.svg)}.fi-cc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cc.svg)}.fi-cd{background-image:url(/static/node_modules/flag-icons/flags/4x3/cd.svg)}.fi-cd.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cd.svg)}.fi-cf{background-image:url(/static/node_modules/flag-icons/flags/4x3/cf.svg)}.fi-cf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cf.svg)}.fi-cg{background-image:url(/static/node_modules/flag-icons/flags/4x3/cg.svg)}.fi-cg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cg.svg)}.fi-ch{background-image:url(/static/node_modules/flag-icons/flags/4x3/ch.svg)}.fi-ch.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ch.svg)}.fi-ci{background-image:url(/static/node_modules/flag-icons/flags/4x3/ci.svg)}.fi-ci.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ci.svg)}.fi-ck{background-image:url(/static/node_modules/flag-icons/flags/4x3/ck.svg)}.fi-ck.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ck.svg)}.fi-cl{background-image:url(/static/node_modules/flag-icons/flags/4x3/cl.svg)}.fi-cl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cl.svg)}.fi-cm{background-image:url(/static/node_modules/flag-icons/flags/4x3/cm.svg)}.fi-cm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cm.svg)}.fi-cn{background-image:url(/static/node_modules/flag-icons/flags/4x3/cn.svg)}.fi-cn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cn.svg)}.fi-co{background-image:url(/static/node_modules/flag-icons/flags/4x3/co.svg)}.fi-co.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/co.svg)}.fi-cr{background-image:url(/static/node_modules/flag-icons/flags/4x3/cr.svg)}.fi-cr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cr.svg)}.fi-cu{background-image:url(/static/node_modules/flag-icons/flags/4x3/cu.svg)}.fi-cu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cu.svg)}.fi-cv{background-image:url(/static/node_modules/flag-icons/flags/4x3/cv.svg)}.fi-cv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cv.svg)}.fi-cw{background-image:url(/static/node_modules/flag-icons/flags/4x3/cw.svg)}.fi-cw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cw.svg)}.fi-cx{background-image:url(/static/node_modules/flag-icons/flags/4x3/cx.svg)}.fi-cx.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cx.svg)}.fi-cy{background-image:url(/static/node_modules/flag-icons/flags/4x3/cy.svg)}.fi-cy.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cy.svg)}.fi-cz{background-image:url(/static/node_modules/flag-icons/flags/4x3/cz.svg)}.fi-cz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cz.svg)}.fi-de{background-image:url(/static/node_modules/flag-icons/flags/4x3/de.svg)}.fi-de.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/de.svg)}.fi-dj{background-image:url(/static/node_modules/flag-icons/flags/4x3/dj.svg)}.fi-dj.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/dj.svg)}.fi-dk{background-image:url(/static/node_modules/flag-icons/flags/4x3/dk.svg)}.fi-dk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/dk.svg)}.fi-dm{background-image:url(/static/node_modules/flag-icons/flags/4x3/dm.svg)}.fi-dm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/dm.svg)}.fi-do{background-image:url(/static/node_modules/flag-icons/flags/4x3/do.svg)}.fi-do.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/do.svg)}.fi-dz{background-image:url(/static/node_modules/flag-icons/flags/4x3/dz.svg)}.fi-dz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/dz.svg)}.fi-ec{background-image:url(/static/node_modules/flag-icons/flags/4x3/ec.svg)}.fi-ec.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ec.svg)}.fi-ee{background-image:url(/static/node_modules/flag-icons/flags/4x3/ee.svg)}.fi-ee.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ee.svg)}.fi-eg{background-image:url(/static/node_modules/flag-icons/flags/4x3/eg.svg)}.fi-eg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/eg.svg)}.fi-eh{background-image:url(/static/node_modules/flag-icons/flags/4x3/eh.svg)}.fi-eh.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/eh.svg)}.fi-er{background-image:url(/static/node_modules/flag-icons/flags/4x3/er.svg)}.fi-er.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/er.svg)}.fi-es{background-image:url(/static/node_modules/flag-icons/flags/4x3/es.svg)}.fi-es.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/es.svg)}.fi-et{background-image:url(/static/node_modules/flag-icons/flags/4x3/et.svg)}.fi-et.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/et.svg)}.fi-fi{background-image:url(/static/node_modules/flag-icons/flags/4x3/fi.svg)}.fi-fi.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/fi.svg)}.fi-fj{background-image:url(/static/node_modules/flag-icons/flags/4x3/fj.svg)}.fi-fj.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/fj.svg)}.fi-fk{background-image:url(/static/node_modules/flag-icons/flags/4x3/fk.svg)}.fi-fk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/fk.svg)}.fi-fm{background-image:url(/static/node_modules/flag-icons/flags/4x3/fm.svg)}.fi-fm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/fm.svg)}.fi-fo{background-image:url(/static/node_modules/flag-icons/flags/4x3/fo.svg)}.fi-fo.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/fo.svg)}.fi-fr{background-image:url(/static/node_modules/flag-icons/flags/4x3/fr.svg)}.fi-fr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/fr.svg)}.fi-ga{background-image:url(/static/node_modules/flag-icons/flags/4x3/ga.svg)}.fi-ga.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ga.svg)}.fi-gb{background-image:url(/static/node_modules/flag-icons/flags/4x3/gb.svg)}.fi-gb.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gb.svg)}.fi-gd{background-image:url(/static/node_modules/flag-icons/flags/4x3/gd.svg)}.fi-gd.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gd.svg)}.fi-ge{background-image:url(/static/node_modules/flag-icons/flags/4x3/ge.svg)}.fi-ge.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ge.svg)}.fi-gf{background-image:url(/static/node_modules/flag-icons/flags/4x3/gf.svg)}.fi-gf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gf.svg)}.fi-gg{background-image:url(/static/node_modules/flag-icons/flags/4x3/gg.svg)}.fi-gg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gg.svg)}.fi-gh{background-image:url(/static/node_modules/flag-icons/flags/4x3/gh.svg)}.fi-gh.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gh.svg)}.fi-gi{background-image:url(/static/node_modules/flag-icons/flags/4x3/gi.svg)}.fi-gi.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gi.svg)}.fi-gl{background-image:url(/static/node_modules/flag-icons/flags/4x3/gl.svg)}.fi-gl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gl.svg)}.fi-gm{background-image:url(/static/node_modules/flag-icons/flags/4x3/gm.svg)}.fi-gm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gm.svg)}.fi-gn{background-image:url(/static/node_modules/flag-icons/flags/4x3/gn.svg)}.fi-gn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gn.svg)}.fi-gp{background-image:url(/static/node_modules/flag-icons/flags/4x3/gp.svg)}.fi-gp.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gp.svg)}.fi-gq{background-image:url(/static/node_modules/flag-icons/flags/4x3/gq.svg)}.fi-gq.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gq.svg)}.fi-gr{background-image:url(/static/node_modules/flag-icons/flags/4x3/gr.svg)}.fi-gr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gr.svg)}.fi-gs{background-image:url(/static/node_modules/flag-icons/flags/4x3/gs.svg)}.fi-gs.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gs.svg)}.fi-gt{background-image:url(/static/node_modules/flag-icons/flags/4x3/gt.svg)}.fi-gt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gt.svg)}.fi-gu{background-image:url(/static/node_modules/flag-icons/flags/4x3/gu.svg)}.fi-gu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gu.svg)}.fi-gw{background-image:url(/static/node_modules/flag-icons/flags/4x3/gw.svg)}.fi-gw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gw.svg)}.fi-gy{background-image:url(/static/node_modules/flag-icons/flags/4x3/gy.svg)}.fi-gy.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gy.svg)}.fi-hk{background-image:url(/static/node_modules/flag-icons/flags/4x3/hk.svg)}.fi-hk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/hk.svg)}.fi-hm{background-image:url(/static/node_modules/flag-icons/flags/4x3/hm.svg)}.fi-hm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/hm.svg)}.fi-hn{background-image:url(/static/node_modules/flag-icons/flags/4x3/hn.svg)}.fi-hn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/hn.svg)}.fi-hr{background-image:url(/static/node_modules/flag-icons/flags/4x3/hr.svg)}.fi-hr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/hr.svg)}.fi-ht{background-image:url(/static/node_modules/flag-icons/flags/4x3/ht.svg)}.fi-ht.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ht.svg)}.fi-hu{background-image:url(/static/node_modules/flag-icons/flags/4x3/hu.svg)}.fi-hu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/hu.svg)}.fi-id{background-image:url(/static/node_modules/flag-icons/flags/4x3/id.svg)}.fi-id.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/id.svg)}.fi-ie{background-image:url(/static/node_modules/flag-icons/flags/4x3/ie.svg)}.fi-ie.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ie.svg)}.fi-il{background-image:url(/static/node_modules/flag-icons/flags/4x3/il.svg)}.fi-il.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/il.svg)}.fi-im{background-image:url(/static/node_modules/flag-icons/flags/4x3/im.svg)}.fi-im.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/im.svg)}.fi-in{background-image:url(/static/node_modules/flag-icons/flags/4x3/in.svg)}.fi-in.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/in.svg)}.fi-io{background-image:url(/static/node_modules/flag-icons/flags/4x3/io.svg)}.fi-io.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/io.svg)}.fi-iq{background-image:url(/static/node_modules/flag-icons/flags/4x3/iq.svg)}.fi-iq.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/iq.svg)}.fi-ir{background-image:url(/static/node_modules/flag-icons/flags/4x3/ir.svg)}.fi-ir.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ir.svg)}.fi-is{background-image:url(/static/node_modules/flag-icons/flags/4x3/is.svg)}.fi-is.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/is.svg)}.fi-it{background-image:url(/static/node_modules/flag-icons/flags/4x3/it.svg)}.fi-it.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/it.svg)}.fi-je{background-image:url(/static/node_modules/flag-icons/flags/4x3/je.svg)}.fi-je.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/je.svg)}.fi-jm{background-image:url(/static/node_modules/flag-icons/flags/4x3/jm.svg)}.fi-jm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/jm.svg)}.fi-jo{background-image:url(/static/node_modules/flag-icons/flags/4x3/jo.svg)}.fi-jo.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/jo.svg)}.fi-jp{background-image:url(/static/node_modules/flag-icons/flags/4x3/jp.svg)}.fi-jp.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/jp.svg)}.fi-ke{background-image:url(/static/node_modules/flag-icons/flags/4x3/ke.svg)}.fi-ke.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ke.svg)}.fi-kg{background-image:url(/static/node_modules/flag-icons/flags/4x3/kg.svg)}.fi-kg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kg.svg)}.fi-kh{background-image:url(/static/node_modules/flag-icons/flags/4x3/kh.svg)}.fi-kh.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kh.svg)}.fi-ki{background-image:url(/static/node_modules/flag-icons/flags/4x3/ki.svg)}.fi-ki.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ki.svg)}.fi-km{background-image:url(/static/node_modules/flag-icons/flags/4x3/km.svg)}.fi-km.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/km.svg)}.fi-kn{background-image:url(/static/node_modules/flag-icons/flags/4x3/kn.svg)}.fi-kn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kn.svg)}.fi-kp{background-image:url(/static/node_modules/flag-icons/flags/4x3/kp.svg)}.fi-kp.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kp.svg)}.fi-kr{background-image:url(/static/node_modules/flag-icons/flags/4x3/kr.svg)}.fi-kr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kr.svg)}.fi-kw{background-image:url(/static/node_modules/flag-icons/flags/4x3/kw.svg)}.fi-kw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kw.svg)}.fi-ky{background-image:url(/static/node_modules/flag-icons/flags/4x3/ky.svg)}.fi-ky.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ky.svg)}.fi-kz{background-image:url(/static/node_modules/flag-icons/flags/4x3/kz.svg)}.fi-kz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/kz.svg)}.fi-la{background-image:url(/static/node_modules/flag-icons/flags/4x3/la.svg)}.fi-la.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/la.svg)}.fi-lb{background-image:url(/static/node_modules/flag-icons/flags/4x3/lb.svg)}.fi-lb.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lb.svg)}.fi-lc{background-image:url(/static/node_modules/flag-icons/flags/4x3/lc.svg)}.fi-lc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lc.svg)}.fi-li{background-image:url(/static/node_modules/flag-icons/flags/4x3/li.svg)}.fi-li.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/li.svg)}.fi-lk{background-image:url(/static/node_modules/flag-icons/flags/4x3/lk.svg)}.fi-lk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lk.svg)}.fi-lr{background-image:url(/static/node_modules/flag-icons/flags/4x3/lr.svg)}.fi-lr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lr.svg)}.fi-ls{background-image:url(/static/node_modules/flag-icons/flags/4x3/ls.svg)}.fi-ls.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ls.svg)}.fi-lt{background-image:url(/static/node_modules/flag-icons/flags/4x3/lt.svg)}.fi-lt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lt.svg)}.fi-lu{background-image:url(/static/node_modules/flag-icons/flags/4x3/lu.svg)}.fi-lu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lu.svg)}.fi-lv{background-image:url(/static/node_modules/flag-icons/flags/4x3/lv.svg)}.fi-lv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/lv.svg)}.fi-ly{background-image:url(/static/node_modules/flag-icons/flags/4x3/ly.svg)}.fi-ly.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ly.svg)}.fi-ma{background-image:url(/static/node_modules/flag-icons/flags/4x3/ma.svg)}.fi-ma.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ma.svg)}.fi-mc{background-image:url(/static/node_modules/flag-icons/flags/4x3/mc.svg)}.fi-mc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mc.svg)}.fi-md{background-image:url(/static/node_modules/flag-icons/flags/4x3/md.svg)}.fi-md.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/md.svg)}.fi-me{background-image:url(/static/node_modules/flag-icons/flags/4x3/me.svg)}.fi-me.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/me.svg)}.fi-mf{background-image:url(/static/node_modules/flag-icons/flags/4x3/mf.svg)}.fi-mf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mf.svg)}.fi-mg{background-image:url(/static/node_modules/flag-icons/flags/4x3/mg.svg)}.fi-mg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mg.svg)}.fi-mh{background-image:url(/static/node_modules/flag-icons/flags/4x3/mh.svg)}.fi-mh.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mh.svg)}.fi-mk{background-image:url(/static/node_modules/flag-icons/flags/4x3/mk.svg)}.fi-mk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mk.svg)}.fi-ml{background-image:url(/static/node_modules/flag-icons/flags/4x3/ml.svg)}.fi-ml.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ml.svg)}.fi-mm{background-image:url(/static/node_modules/flag-icons/flags/4x3/mm.svg)}.fi-mm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mm.svg)}.fi-mn{background-image:url(/static/node_modules/flag-icons/flags/4x3/mn.svg)}.fi-mn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mn.svg)}.fi-mo{background-image:url(/static/node_modules/flag-icons/flags/4x3/mo.svg)}.fi-mo.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mo.svg)}.fi-mp{background-image:url(/static/node_modules/flag-icons/flags/4x3/mp.svg)}.fi-mp.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mp.svg)}.fi-mq{background-image:url(/static/node_modules/flag-icons/flags/4x3/mq.svg)}.fi-mq.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mq.svg)}.fi-mr{background-image:url(/static/node_modules/flag-icons/flags/4x3/mr.svg)}.fi-mr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mr.svg)}.fi-ms{background-image:url(/static/node_modules/flag-icons/flags/4x3/ms.svg)}.fi-ms.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ms.svg)}.fi-mt{background-image:url(/static/node_modules/flag-icons/flags/4x3/mt.svg)}.fi-mt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mt.svg)}.fi-mu{background-image:url(/static/node_modules/flag-icons/flags/4x3/mu.svg)}.fi-mu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mu.svg)}.fi-mv{background-image:url(/static/node_modules/flag-icons/flags/4x3/mv.svg)}.fi-mv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mv.svg)}.fi-mw{background-image:url(/static/node_modules/flag-icons/flags/4x3/mw.svg)}.fi-mw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mw.svg)}.fi-mx{background-image:url(/static/node_modules/flag-icons/flags/4x3/mx.svg)}.fi-mx.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mx.svg)}.fi-my{background-image:url(/static/node_modules/flag-icons/flags/4x3/my.svg)}.fi-my.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/my.svg)}.fi-mz{background-image:url(/static/node_modules/flag-icons/flags/4x3/mz.svg)}.fi-mz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/mz.svg)}.fi-na{background-image:url(/static/node_modules/flag-icons/flags/4x3/na.svg)}.fi-na.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/na.svg)}.fi-nc{background-image:url(/static/node_modules/flag-icons/flags/4x3/nc.svg)}.fi-nc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/nc.svg)}.fi-ne{background-image:url(/static/node_modules/flag-icons/flags/4x3/ne.svg)}.fi-ne.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ne.svg)}.fi-nf{background-image:url(/static/node_modules/flag-icons/flags/4x3/nf.svg)}.fi-nf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/nf.svg)}.fi-ng{background-image:url(/static/node_modules/flag-icons/flags/4x3/ng.svg)}.fi-ng.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ng.svg)}.fi-ni{background-image:url(/static/node_modules/flag-icons/flags/4x3/ni.svg)}.fi-ni.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ni.svg)}.fi-nl{background-image:url(/static/node_modules/flag-icons/flags/4x3/nl.svg)}.fi-nl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/nl.svg)}.fi-no{background-image:url(/static/node_modules/flag-icons/flags/4x3/no.svg)}.fi-no.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/no.svg)}.fi-np{background-image:url(/static/node_modules/flag-icons/flags/4x3/np.svg)}.fi-np.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/np.svg)}.fi-nr{background-image:url(/static/node_modules/flag-icons/flags/4x3/nr.svg)}.fi-nr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/nr.svg)}.fi-nu{background-image:url(/static/node_modules/flag-icons/flags/4x3/nu.svg)}.fi-nu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/nu.svg)}.fi-nz{background-image:url(/static/node_modules/flag-icons/flags/4x3/nz.svg)}.fi-nz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/nz.svg)}.fi-om{background-image:url(/static/node_modules/flag-icons/flags/4x3/om.svg)}.fi-om.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/om.svg)}.fi-pa{background-image:url(/static/node_modules/flag-icons/flags/4x3/pa.svg)}.fi-pa.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pa.svg)}.fi-pe{background-image:url(/static/node_modules/flag-icons/flags/4x3/pe.svg)}.fi-pe.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pe.svg)}.fi-pf{background-image:url(/static/node_modules/flag-icons/flags/4x3/pf.svg)}.fi-pf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pf.svg)}.fi-pg{background-image:url(/static/node_modules/flag-icons/flags/4x3/pg.svg)}.fi-pg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pg.svg)}.fi-ph{background-image:url(/static/node_modules/flag-icons/flags/4x3/ph.svg)}.fi-ph.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ph.svg)}.fi-pk{background-image:url(/static/node_modules/flag-icons/flags/4x3/pk.svg)}.fi-pk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pk.svg)}.fi-pl{background-image:url(/static/node_modules/flag-icons/flags/4x3/pl.svg)}.fi-pl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pl.svg)}.fi-pm{background-image:url(/static/node_modules/flag-icons/flags/4x3/pm.svg)}.fi-pm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pm.svg)}.fi-pn{background-image:url(/static/node_modules/flag-icons/flags/4x3/pn.svg)}.fi-pn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pn.svg)}.fi-pr{background-image:url(/static/node_modules/flag-icons/flags/4x3/pr.svg)}.fi-pr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pr.svg)}.fi-ps{background-image:url(/static/node_modules/flag-icons/flags/4x3/ps.svg)}.fi-ps.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ps.svg)}.fi-pt{background-image:url(/static/node_modules/flag-icons/flags/4x3/pt.svg)}.fi-pt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pt.svg)}.fi-pw{background-image:url(/static/node_modules/flag-icons/flags/4x3/pw.svg)}.fi-pw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pw.svg)}.fi-py{background-image:url(/static/node_modules/flag-icons/flags/4x3/py.svg)}.fi-py.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/py.svg)}.fi-qa{background-image:url(/static/node_modules/flag-icons/flags/4x3/qa.svg)}.fi-qa.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/qa.svg)}.fi-re{background-image:url(/static/node_modules/flag-icons/flags/4x3/re.svg)}.fi-re.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/re.svg)}.fi-ro{background-image:url(/static/node_modules/flag-icons/flags/4x3/ro.svg)}.fi-ro.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ro.svg)}.fi-rs{background-image:url(/static/node_modules/flag-icons/flags/4x3/rs.svg)}.fi-rs.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/rs.svg)}.fi-ru{background-image:url(/static/node_modules/flag-icons/flags/4x3/ru.svg)}.fi-ru.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ru.svg)}.fi-rw{background-image:url(/static/node_modules/flag-icons/flags/4x3/rw.svg)}.fi-rw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/rw.svg)}.fi-sa{background-image:url(/static/node_modules/flag-icons/flags/4x3/sa.svg)}.fi-sa.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sa.svg)}.fi-sb{background-image:url(/static/node_modules/flag-icons/flags/4x3/sb.svg)}.fi-sb.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sb.svg)}.fi-sc{background-image:url(/static/node_modules/flag-icons/flags/4x3/sc.svg)}.fi-sc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sc.svg)}.fi-sd{background-image:url(/static/node_modules/flag-icons/flags/4x3/sd.svg)}.fi-sd.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sd.svg)}.fi-se{background-image:url(/static/node_modules/flag-icons/flags/4x3/se.svg)}.fi-se.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/se.svg)}.fi-sg{background-image:url(/static/node_modules/flag-icons/flags/4x3/sg.svg)}.fi-sg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sg.svg)}.fi-sh{background-image:url(/static/node_modules/flag-icons/flags/4x3/sh.svg)}.fi-sh.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sh.svg)}.fi-si{background-image:url(/static/node_modules/flag-icons/flags/4x3/si.svg)}.fi-si.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/si.svg)}.fi-sj{background-image:url(/static/node_modules/flag-icons/flags/4x3/sj.svg)}.fi-sj.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sj.svg)}.fi-sk{background-image:url(/static/node_modules/flag-icons/flags/4x3/sk.svg)}.fi-sk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sk.svg)}.fi-sl{background-image:url(/static/node_modules/flag-icons/flags/4x3/sl.svg)}.fi-sl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sl.svg)}.fi-sm{background-image:url(/static/node_modules/flag-icons/flags/4x3/sm.svg)}.fi-sm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sm.svg)}.fi-sn{background-image:url(/static/node_modules/flag-icons/flags/4x3/sn.svg)}.fi-sn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sn.svg)}.fi-so{background-image:url(/static/node_modules/flag-icons/flags/4x3/so.svg)}.fi-so.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/so.svg)}.fi-sr{background-image:url(/static/node_modules/flag-icons/flags/4x3/sr.svg)}.fi-sr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sr.svg)}.fi-ss{background-image:url(/static/node_modules/flag-icons/flags/4x3/ss.svg)}.fi-ss.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ss.svg)}.fi-st{background-image:url(/static/node_modules/flag-icons/flags/4x3/st.svg)}.fi-st.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/st.svg)}.fi-sv{background-image:url(/static/node_modules/flag-icons/flags/4x3/sv.svg)}.fi-sv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sv.svg)}.fi-sx{background-image:url(/static/node_modules/flag-icons/flags/4x3/sx.svg)}.fi-sx.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sx.svg)}.fi-sy{background-image:url(/static/node_modules/flag-icons/flags/4x3/sy.svg)}.fi-sy.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sy.svg)}.fi-sz{background-image:url(/static/node_modules/flag-icons/flags/4x3/sz.svg)}.fi-sz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sz.svg)}.fi-tc{background-image:url(/static/node_modules/flag-icons/flags/4x3/tc.svg)}.fi-tc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tc.svg)}.fi-td{background-image:url(/static/node_modules/flag-icons/flags/4x3/td.svg)}.fi-td.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/td.svg)}.fi-tf{background-image:url(/static/node_modules/flag-icons/flags/4x3/tf.svg)}.fi-tf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tf.svg)}.fi-tg{background-image:url(/static/node_modules/flag-icons/flags/4x3/tg.svg)}.fi-tg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tg.svg)}.fi-th{background-image:url(/static/node_modules/flag-icons/flags/4x3/th.svg)}.fi-th.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/th.svg)}.fi-tj{background-image:url(/static/node_modules/flag-icons/flags/4x3/tj.svg)}.fi-tj.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tj.svg)}.fi-tk{background-image:url(/static/node_modules/flag-icons/flags/4x3/tk.svg)}.fi-tk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tk.svg)}.fi-tl{background-image:url(/static/node_modules/flag-icons/flags/4x3/tl.svg)}.fi-tl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tl.svg)}.fi-tm{background-image:url(/static/node_modules/flag-icons/flags/4x3/tm.svg)}.fi-tm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tm.svg)}.fi-tn{background-image:url(/static/node_modules/flag-icons/flags/4x3/tn.svg)}.fi-tn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tn.svg)}.fi-to{background-image:url(/static/node_modules/flag-icons/flags/4x3/to.svg)}.fi-to.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/to.svg)}.fi-tr{background-image:url(/static/node_modules/flag-icons/flags/4x3/tr.svg)}.fi-tr.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tr.svg)}.fi-tt{background-image:url(/static/node_modules/flag-icons/flags/4x3/tt.svg)}.fi-tt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tt.svg)}.fi-tv{background-image:url(/static/node_modules/flag-icons/flags/4x3/tv.svg)}.fi-tv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tv.svg)}.fi-tw{background-image:url(/static/node_modules/flag-icons/flags/4x3/tw.svg)}.fi-tw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tw.svg)}.fi-tz{background-image:url(/static/node_modules/flag-icons/flags/4x3/tz.svg)}.fi-tz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/tz.svg)}.fi-ua{background-image:url(/static/node_modules/flag-icons/flags/4x3/ua.svg)}.fi-ua.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ua.svg)}.fi-ug{background-image:url(/static/node_modules/flag-icons/flags/4x3/ug.svg)}.fi-ug.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ug.svg)}.fi-um{background-image:url(/static/node_modules/flag-icons/flags/4x3/um.svg)}.fi-um.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/um.svg)}.fi-us{background-image:url(/static/node_modules/flag-icons/flags/4x3/us.svg)}.fi-us.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/us.svg)}.fi-uy{background-image:url(/static/node_modules/flag-icons/flags/4x3/uy.svg)}.fi-uy.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/uy.svg)}.fi-uz{background-image:url(/static/node_modules/flag-icons/flags/4x3/uz.svg)}.fi-uz.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/uz.svg)}.fi-va{background-image:url(/static/node_modules/flag-icons/flags/4x3/va.svg)}.fi-va.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/va.svg)}.fi-vc{background-image:url(/static/node_modules/flag-icons/flags/4x3/vc.svg)}.fi-vc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/vc.svg)}.fi-ve{background-image:url(/static/node_modules/flag-icons/flags/4x3/ve.svg)}.fi-ve.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ve.svg)}.fi-vg{background-image:url(/static/node_modules/flag-icons/flags/4x3/vg.svg)}.fi-vg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/vg.svg)}.fi-vi{background-image:url(/static/node_modules/flag-icons/flags/4x3/vi.svg)}.fi-vi.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/vi.svg)}.fi-vn{background-image:url(/static/node_modules/flag-icons/flags/4x3/vn.svg)}.fi-vn.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/vn.svg)}.fi-vu{background-image:url(/static/node_modules/flag-icons/flags/4x3/vu.svg)}.fi-vu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/vu.svg)}.fi-wf{background-image:url(/static/node_modules/flag-icons/flags/4x3/wf.svg)}.fi-wf.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/wf.svg)}.fi-ws{background-image:url(/static/node_modules/flag-icons/flags/4x3/ws.svg)}.fi-ws.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ws.svg)}.fi-ye{background-image:url(/static/node_modules/flag-icons/flags/4x3/ye.svg)}.fi-ye.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ye.svg)}.fi-yt{background-image:url(/static/node_modules/flag-icons/flags/4x3/yt.svg)}.fi-yt.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/yt.svg)}.fi-za{background-image:url(/static/node_modules/flag-icons/flags/4x3/za.svg)}.fi-za.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/za.svg)}.fi-zm{background-image:url(/static/node_modules/flag-icons/flags/4x3/zm.svg)}.fi-zm.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/zm.svg)}.fi-zw{background-image:url(/static/node_modules/flag-icons/flags/4x3/zw.svg)}.fi-zw.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/zw.svg)}.fi-arab{background-image:url(/static/node_modules/flag-icons/flags/4x3/arab.svg)}.fi-arab.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/arab.svg)}.fi-cefta{background-image:url(/static/node_modules/flag-icons/flags/4x3/cefta.svg)}.fi-cefta.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cefta.svg)}.fi-cp{background-image:url(/static/node_modules/flag-icons/flags/4x3/cp.svg)}.fi-cp.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/cp.svg)}.fi-dg{background-image:url(/static/node_modules/flag-icons/flags/4x3/dg.svg)}.fi-dg.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/dg.svg)}.fi-eac{background-image:url(/static/node_modules/flag-icons/flags/4x3/eac.svg)}.fi-eac.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/eac.svg)}.fi-es-ct{background-image:url(/static/node_modules/flag-icons/flags/4x3/es-ct.svg)}.fi-es-ct.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/es-ct.svg)}.fi-es-ga{background-image:url(/static/node_modules/flag-icons/flags/4x3/es-ga.svg)}.fi-es-ga.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/es-ga.svg)}.fi-es-pv{background-image:url(/static/node_modules/flag-icons/flags/4x3/es-pv.svg)}.fi-es-pv.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/es-pv.svg)}.fi-eu{background-image:url(/static/node_modules/flag-icons/flags/4x3/eu.svg)}.fi-eu.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/eu.svg)}.fi-gb-eng{background-image:url(/static/node_modules/flag-icons/flags/4x3/gb-eng.svg)}.fi-gb-eng.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gb-eng.svg)}.fi-gb-nir{background-image:url(/static/node_modules/flag-icons/flags/4x3/gb-nir.svg)}.fi-gb-nir.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gb-nir.svg)}.fi-gb-sct{background-image:url(/static/node_modules/flag-icons/flags/4x3/gb-sct.svg)}.fi-gb-sct.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gb-sct.svg)}.fi-gb-wls{background-image:url(/static/node_modules/flag-icons/flags/4x3/gb-wls.svg)}.fi-gb-wls.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/gb-wls.svg)}.fi-ic{background-image:url(/static/node_modules/flag-icons/flags/4x3/ic.svg)}.fi-ic.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/ic.svg)}.fi-pc{background-image:url(/static/node_modules/flag-icons/flags/4x3/pc.svg)}.fi-pc.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/pc.svg)}.fi-sh-ac{background-image:url(/static/node_modules/flag-icons/flags/4x3/sh-ac.svg)}.fi-sh-ac.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sh-ac.svg)}.fi-sh-hl{background-image:url(/static/node_modules/flag-icons/flags/4x3/sh-hl.svg)}.fi-sh-hl.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sh-hl.svg)}.fi-sh-ta{background-image:url(/static/node_modules/flag-icons/flags/4x3/sh-ta.svg)}.fi-sh-ta.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/sh-ta.svg)}.fi-un{background-image:url(/static/node_modules/flag-icons/flags/4x3/un.svg)}.fi-un.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/un.svg)}.fi-xk{background-image:url(/static/node_modules/flag-icons/flags/4x3/xk.svg)}.fi-xk.fis{background-image:url(/static/node_modules/flag-icons/flags/1x1/xk.svg)}';
 var u0 = typeof window.gettext == "function" ? window.gettext : e => e,
     cd = class {
-        constructor(t) {
+        constructor(a) {
             this.baseSelector = '[is="django-phone-number"]';
             this.hasFocus = !1;
             this.isOpen = !1;
             this.isPristine = !0;
             this.possibleCallingCode = null;
-            this.formResetted = t => {
+            this.cleanup = () => {};
+            this.formResetted = a => {
                 this.asYouType.reset(), this.initializeValue(this.inputElement.defaultValue)
             };
-            this.handleFocus = t => {
-                this.editField === t.target && (this.editField.ariaBusy = "true", this.textBox.classList.add("focus"), this.inputElement.dispatchEvent(new Event("focus")), t.preventDefault(), this.hasFocus = !0)
+            this.handleFocus = a => {
+                this.editField === a.target && (this.editField.ariaBusy = "true", this.textBox.classList.add("focus"), this.inputElement.dispatchEvent(new Event("focus")), a.preventDefault(), this.hasFocus = !0)
             };
-            this.handleInput = t => {
-                t.target instanceof HTMLElement && this.editField === t.target && (this.editField.innerText.length === 0 ? this.isPristine = !0 : this.isPristine ? this.placeInputField(t.target.innerText) : this.updateInputField(t.target.innerText))
+            this.handleInput = a => {
+                a.target instanceof HTMLElement && this.editField === a.target && (this.editField.innerText.length === 0 ? this.isPristine = !0 : this.isPristine ? this.placeInputField(a.target.innerText) : this.updateInputField(a.target.innerText))
             };
             this.handleBlur = () => {
                 setTimeout(() => {
                     this.hasFocus && (this.editField.ariaBusy = "false", this.textBox.classList.remove("focus"), this.hasFocus = !1, this.inputElement.dispatchEvent(new Event("blur")))
                 }, 0)
             };
-            this.handleClick = t => {
+            this.handleClick = a => {
                 let d = null,
-                    a = null,
-                    i = t.target instanceof Element ? t.target : null;
+                    t = null,
+                    i = a.target instanceof Element ? a.target : null;
                 for (; i;) {
                     if (i === this.countryLookupField) return;
-                    if (i.hasAttribute("data-country") && (d = i.getAttribute("data-country"), a = i.getAttribute("data-calling-code")), i === this.internationalSelector && d && a) {
-                        this.setInternationalCode(d, a);
+                    if (i.hasAttribute("data-country") && (d = i.getAttribute("data-country"), t = i.getAttribute("data-calling-code")), i === this.internationalSelector && d && t) {
+                        this.setInternationalCode(d, t);
                         break
                     }
                     if (i === this.internationalOpener) {
                         this.openInternationalSelector();
                         return
                     }
                     i = i.parentElement
                 }
                 this.closeInternationalSelector()
             };
-            this.handleSearch = t => {
+            this.handleSearch = a => {
                 let d = this.countryLookupField.value.toLowerCase();
-                this.internationalSelector.querySelectorAll("li[data-country]").forEach(a => {
-                    let i = a.innerText.toLowerCase();
-                    a.hidden = !i.includes(d)
+                for (; d.startsWith("0");) d = d.slice(1);
+                this.internationalSelector.querySelectorAll("li[data-country]").forEach(t => {
+                    let i = t.innerText.toLowerCase();
+                    t.hidden = !i.includes(d)
                 })
             };
-            this.handleKeypress = t => {
-                var a, i;
+            this.handleKeypress = a => {
                 let d = n => {
                     this.deselectAll(), n.classList.add("selected"), n.scrollIntoView()
                 };
-                if (this.isOpen) switch (t.key) {
+                if (!this.isOpen) return;
+                let t = Array.from(this.internationalSelector.querySelectorAll("li[data-country]:not([hidden])")),
+                    i = t.findIndex(n => n.classList.contains("selected"));
+                switch (a.key) {
                     case "Enter":
                         let n = this.internationalSelector.querySelector("li[data-country].selected");
                         if (n instanceof HTMLLIElement) {
                             let s = n.getAttribute("data-country"),
                                 l = n.getAttribute("data-calling-code");
                             this.closeInternationalSelector(), this.setInternationalCode(s, l)
                         }
                         break;
                     case "Escape":
                         this.closeInternationalSelector();
                         break;
                     case "ArrowUp":
-                        let r = (a = this.internationalSelector.querySelector("li[data-country].selected")) == null ? void 0 : a.previousElementSibling;
-                        r || (r = this.possibleCallingCode ?? this.internationalSelector.querySelector("li[data-country]:last-child")), r instanceof HTMLLIElement && d(r), t.preventDefault();
+                        let r = t[i - 1] ?? t.slice(-1)[0];
+                        r instanceof HTMLLIElement && d(r), a.preventDefault();
                         break;
                     case "ArrowDown":
-                        let o = (i = this.internationalSelector.querySelector("li[data-country].selected")) == null ? void 0 : i.nextElementSibling;
-                        o || (o = this.possibleCallingCode ?? this.internationalSelector.querySelector("li[data-country]:first-child")), o instanceof HTMLLIElement && d(o), t.preventDefault();
+                        let o = t[i + 1] ?? t[0];
+                        o instanceof HTMLLIElement && d(o), a.preventDefault();
                         break;
                     case "+":
-                        this.closeInternationalSelector(), this.editField.focus(), this.updateInputField(t.key), t.preventDefault();
+                        this.closeInternationalSelector(), this.editField.focus(), this.updateInputField(a.key), a.preventDefault();
                         break;
                     default:
                         break
                 }
             };
             this.updatePosition = () => {
-                let t = this.textBox.style.zIndex ? parseInt(this.textBox.style.zIndex) : 0;
+                let a = this.textBox.style.zIndex ? parseInt(this.textBox.style.zIndex) : 0;
                 hd(this.textBox, this.internationalSelector, {
                     middleware: [md()]
                 }).then(() => Object.assign(this.internationalSelector.style, {
-                    zIndex: `${t+1}`
+                    zIndex: `${a+1}`
                 }))
             };
             this.deselectAll = () => {
-                this.internationalSelector.querySelectorAll("li[data-country]").forEach(t => {
-                    t.classList.remove("selected"), t.hidden = !1
+                this.internationalSelector.querySelectorAll("li[data-country]").forEach(a => {
+                    a.classList.remove("selected")
+                })
+            };
+            this.clearSearch = () => {
+                this.internationalSelector.querySelectorAll("li[data-country]").forEach(a => {
+                    a.hidden = !1
                 })
             };
-            this.inputElement = t, this.codeCountryMap = this.createCountriesMap();
+            this.inputElement = a, this.codeCountryMap = this.createCountriesMap();
             let d = new Intl.Collator(document.documentElement.lang ?? "en").compare;
             this.codeCountryMap = this.codeCountryMap.sort((i, n) => d(i[0], n[0]));
-            let a = t.getAttribute("default-country-code");
-            this.defaultCountryCode = a ? a.toUpperCase() : void 0, this.mobileOnly = t.hasAttribute("mobile-only"), this.asYouType = new P(this.defaultCountryCode), this.textBox = this.createTextBox(), this.editField = this.textBox.querySelector(".phone-number-edit"), this.internationalOpener = this.textBox.querySelector(".international-picker"), this.internationalSelector = this.textBox.nextElementSibling, this.countryLookupField = this.internationalSelector.querySelector('input[type="search"]'), y.stylesAreInstalled(this.baseSelector) || this.transferStyles(), this.transferClasses()
+            let t = a.getAttribute("default-country-code");
+            this.defaultCountryCode = t ? t.toUpperCase() : void 0, this.mobileOnly = a.hasAttribute("mobile-only"), this.asYouType = new P(this.defaultCountryCode), this.textBox = this.createTextBox(), this.editField = this.textBox.querySelector(".phone-number-edit"), this.internationalOpener = this.textBox.querySelector(".international-picker"), this.internationalSelector = this.textBox.nextElementSibling, this.countryLookupField = this.internationalSelector.querySelector('input[type="search"]'), y.stylesAreInstalled(this.baseSelector) || this.transferStyles(), this.transferClasses()
         }
-        initializeValue(t) {
-            t ? (this.editField.innerText = this.asYouType.input(t), this.inputElement.value = this.asYouType.getNumberValue() ?? t, this.decorateInputField(this.asYouType.getCountry())) : (this.editField.innerText = this.inputElement.value = "", this.decorateInputField())
+        initializeValue(a) {
+            a ? (this.editField.innerText = this.asYouType.input(a), this.inputElement.value = this.asYouType.getNumberValue() ?? a, this.decorateInputField(this.asYouType.getCountry())) : (this.editField.innerText = this.inputElement.value = "", this.decorateInputField())
         }
         createCountriesMap() {
-            return gd().map(t => [u0(s0.get(t) ?? ""), fd(t), t])
+            return gd().map(a => [u0(s0.get(a) ?? ""), fd(a), a])
         }
         createTextBox() {
-            let t = ['<div role="textbox" aria-expanded="false" aria-haspopup="dialog">', '<div class="international-picker"></div>', '<div class="phone-number-edit" contenteditable="true"></div>', "</div>", '<div role="dialog" aria-modal="true">', `<input type="search" placeholder="${u0("Search \u2026")}">`, "<ul>"];
-            for (let [d, a, i] of this.codeCountryMap) t.push(`<li data-country="${i}" data-calling-code="${a}">`), t.push(`<span class="fi fi-${i.toLowerCase()} fib"></span>${d} <strong>+${a}</strong>`), t.push("</li>");
-            return t.push("</div>"), this.inputElement.insertAdjacentHTML("afterend", t.join("")), this.inputElement.nextElementSibling
+            let a = ['<div role="textbox" aria-expanded="false" aria-haspopup="dialog">', '<div class="international-picker"></div>', '<div class="phone-number-edit" contenteditable="true"></div>', "</div>", '<div role="dialog" aria-modal="true">', `<input type="search" placeholder="${u0("Search \u2026")}">`, "<ul>"];
+            for (let [d, t, i] of this.codeCountryMap) a.push(`<li data-country="${i}" data-calling-code="${t}">`), a.push(`<span class="fi fi-${i.toLowerCase()} fib"></span>${d} <strong>+${t}</strong>`), a.push("</li>");
+            return a.push("</div>"), this.inputElement.insertAdjacentHTML("afterend", a.join("")), this.inputElement.nextElementSibling
         }
         installEventHandlers() {
             this.editField.addEventListener("focus", this.handleFocus), this.editField.addEventListener("input", this.handleInput), this.editField.addEventListener("blur", this.handleBlur), this.countryLookupField.addEventListener("input", this.handleSearch), document.addEventListener("click", this.handleClick), document.addEventListener("keydown", this.handleKeypress), this.inputElement.form && this.inputElement.form.addEventListener("reset", this.formResetted)
         }
         setCaretToEnd() {
-            let t = this.editField.childNodes[0];
-            if (!t) return;
+            let a = this.editField.childNodes[0];
+            if (!a) return;
             let d = document.createRange();
-            d.setStart(t, t.length), d.collapse(!0);
-            let a = window.getSelection();
-            a.removeAllRanges(), a.addRange(d)
+            d.setStart(a, a.length), d.collapse(!0);
+            let t = window.getSelection();
+            t.removeAllRanges(), t.addRange(d)
         }
         openInternationalSelector() {
             this.internationalSelector.parentElement.style.position = "relative", this.cleanup = $d(this.textBox, this.internationalSelector, this.updatePosition), this.textBox.setAttribute("aria-expanded", "true");
-            let t = this.internationalSelector.getBoundingClientRect();
-            this.internationalSelector.style.width = `${Math.round(t.width)}px`, this.isOpen = !0, this.isPristine = !0, this.countryLookupField.value = "", this.deselectAll();
+            let a = this.internationalSelector.getBoundingClientRect();
+            this.internationalSelector.style.width = `${Math.round(a.width)}px`, this.isOpen = !0, this.isPristine = !0, this.countryLookupField.value = "", this.deselectAll(), this.clearSearch();
             let d = this.asYouType.getCountry();
             if (d) {
-                let a = this.internationalSelector.querySelector(`[data-country="${d}"]`);
-                a instanceof HTMLLIElement && (a.classList.add("selected"), a.scrollIntoView())
+                let t = this.internationalSelector.querySelector(`[data-country="${d}"]`);
+                t instanceof HTMLLIElement && (t.classList.add("selected"), t.scrollIntoView())
             }
             this.countryLookupField.focus()
         }
         closeInternationalSelector() {
-            var t;
-            this.isOpen = !1, this.textBox.setAttribute("aria-expanded", "false"), (t = this.cleanup) == null || t.call(this)
+            this.isOpen = !1, this.textBox.setAttribute("aria-expanded", "false"), this.cleanup()
         }
-        setInternationalCode(t, d) {
+        setInternationalCode(a, d) {
             var i;
-            this.decorateInputField(t);
-            let a = ((i = this.asYouType.getNumber()) == null ? void 0 : i.nationalNumber) ?? "";
-            this.inputElement.value = this.editField.innerText = `+${d}${a}`, this.inputElement.dispatchEvent(new Event("input")), this.isPristine = !1, this.editField.focus(), window.setTimeout(() => {
+            this.decorateInputField(a);
+            let t = ((i = this.asYouType.getNumber()) == null ? void 0 : i.nationalNumber) ?? "";
+            this.inputElement.value = this.editField.innerText = `+${d}${t}`, this.inputElement.dispatchEvent(new Event("input")), this.isPristine = !1, this.editField.focus(), window.setTimeout(() => {
                 this.setCaretToEnd()
             }, 0)
         }
-        placeInputField(t) {
-            this.asYouType.reset(), t.startsWith("+") ? (this.updateInputField(t), this.setCaretToEnd()) : this.defaultCountryCode ? (this.asYouType.input(t), this.updateInputField(this.asYouType.getNumberValue()), this.setCaretToEnd()) : (this.editField.innerText = "", this.openInternationalSelector())
+        placeInputField(a) {
+            this.asYouType.reset(), a.startsWith("+") ? (this.updateInputField(a), this.setCaretToEnd()) : this.defaultCountryCode ? (this.asYouType.input(a), this.updateInputField(this.asYouType.getNumberValue()), this.setCaretToEnd()) : (this.editField.innerText = "", this.openInternationalSelector())
         }
-        updateInputField(t) {
+        updateInputField(a) {
             this.asYouType.reset();
             let d = window.getSelection(),
-                a = d.rangeCount ? d.getRangeAt(0).startOffset : 0;
-            this.editField.innerText.length === a && ++a, this.editField.innerText = this.asYouType.input(t);
+                t = d.rangeCount ? d.getRangeAt(0).startOffset : 0;
+            this.editField.innerText.length === t && ++t, this.editField.innerText = this.asYouType.input(a);
             let i = this.editField.childNodes[0],
                 n = document.createRange();
-            n.setStart(i, Math.min(a, i.length)), n.collapse(!0), d.removeAllRanges(), d.addRange(n), this.inputElement.value = this.asYouType.getNumberValue() ?? "", this.decorateInputField(this.asYouType.getCountry()), this.inputElement.dispatchEvent(new Event("input")), this.isPristine = !1
+            n.setStart(i, Math.min(t, i.length)), n.collapse(!0), d.removeAllRanges(), d.addRange(n), this.inputElement.value = this.asYouType.getNumberValue() ?? "", this.decorateInputField(this.asYouType.getCountry()), this.inputElement.dispatchEvent(new Event("input")), this.isPristine = !1
         }
-        decorateInputField(t) {
-            t ? this.internationalOpener.innerHTML = `<span class="fi fi-${t.toLowerCase()} fib"></span>` : this.internationalOpener.innerHTML = ""
+        decorateInputField(a) {
+            a ? this.internationalOpener.innerHTML = `<span class="fi fi-${a.toLowerCase()} fib"></span>` : this.internationalOpener.innerHTML = ""
         }
         transferStyles() {
-            let t = document.createElement("style"),
+            let a = document.createElement("style"),
                 d = !1;
-            t.innerText = l0, document.head.appendChild(t), this.inputElement.style.transition = "none";
-            for (let a = 0; t.sheet && a < t.sheet.cssRules.length; a++) {
-                let i = t.sheet.cssRules.item(a),
+            a.innerText = l0, document.head.appendChild(a), this.inputElement.style.transition = "none";
+            for (let t = 0; a.sheet && t < a.sheet.cssRules.length; t++) {
+                let i = a.sheet.cssRules.item(t),
                     n = "";
                 switch (i.selectorText.trim()) {
                     case this.baseSelector:
                         d = !0;
                         break;
                     case `${this.baseSelector} + [role="textbox"]`:
                         n = y.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "color", "outline", "height", "line-height", "padding"]);
@@ -5896,28 +5904,28 @@
                         break;
                     case `${this.baseSelector} + [role="textbox"][aria-haspopup="dialog"] + [role="dialog"] ul`:
                         n = `${i.selectorText}{height:${Math.floor(window.innerHeight/3)}px;}`;
                         break;
                     default:
                         break
                 }
-                n && t.sheet.insertRule(`${i.selectorText}{${n}}`, ++a)
+                n && a.sheet.insertRule(`${i.selectorText}{${n}}`, ++t)
             }
             if (this.inputElement.style.transition = "", !d) throw new Error(`Could not load styles for ${this.baseSelector}`)
         }
         transferClasses() {
             this.inputElement.classList.remove(...this.inputElement.classList), this.inputElement.style.transition = "", this.inputElement.hidden = !0
         }
         initialize() {
             this.installEventHandlers(), this.initializeValue(this.inputElement.defaultValue)
         }
         checkValidity() {
-            var t;
+            var a;
             if (this.asYouType.isValid()) {
-                if (this.mobileOnly && ((t = this.asYouType.getNumber()) == null ? void 0 : t.getType()) !== "MOBILE") return this.inputElement.setCustomValidity("Invalid mobile number"), !1
+                if (this.mobileOnly && ((a = this.asYouType.getNumber()) == null ? void 0 : a.getType()) !== "MOBILE") return this.inputElement.setCustomValidity("Invalid mobile number"), !1
             } else return this.inputElement.setCustomValidity("Invalid phone number"), !1;
             return !0
         }
     },
     W = Symbol("DjangoPhoneNumberElement"),
     g0 = class extends HTMLInputElement {
         constructor() {
```

### Comparing `django_formset-1.4.3/formset/static/formset/js/RichtextArea-PVV6GJIQ.js` & `django_formset-1.4.4/formset/static/formset/js/RichtextArea-LQJSGPD7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     a as fa,
     b as ha,
     c as pa,
     f as Vi
-} from "./chunk-YMY5H5XX.js";
+} from "./chunk-54ILQ33N.js";
 import {
     a as ma
 } from "./chunk-FDUUONAQ.js";
 import {
     e as ji
 } from "./chunk-RLE6ONWJ.js";
 import {
```

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-65OJRBX6.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-65OJRBX6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-FDUUONAQ.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-FDUUONAQ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-IH7AT57W.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-3FM5H3DO.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-NOGHTXP6.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-NOGHTXP6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-P2VM2T3G.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-P2VM2T3G.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-R3EYKSPB.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-IUS6Z5AU.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-RLE6ONWJ.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-RLE6ONWJ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-SERXULES.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-SERXULES.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-TRJBB73N.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-MC5NQ26F.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-W5RPWA2M.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-W5RPWA2M.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/chunk-YMY5H5XX.js` & `django_formset-1.4.4/formset/static/formset/js/chunk-54ILQ33N.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/static/formset/js/django-formset.js` & `django_formset-1.4.4/formset/static/formset/js/django-formset.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 import {
     a as er,
     b as tr,
     c as rr,
     d as M,
     e as ot,
     f as lt
-} from "./chunk-YMY5H5XX.js";
+} from "./chunk-54ILQ33N.js";
 import {
     a as it
 } from "./chunk-FDUUONAQ.js";
 import {
     a as st
 } from "./chunk-65OJRBX6.js";
 import {
@@ -2038,65 +2038,65 @@
 
     function r(o, u, d, c = void 0) {
         customElements.get(u) instanceof Function ? o() : (window.customElements.define(u, d, c), window.customElements.whenDefined(u).then(() => o()))
     }
 
     function i(o) {
         o.querySelector('select[is="django-selectize"]') && t.push(new Promise((d, c) => {
-            import("./DjangoSelectize-FCAZIQIK.js").then(({
+            import("./DjangoSelectize-7RDFNLMN.js").then(({
                 DjangoSelectizeElement: l
             }) => {
                 r(d, "django-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('select[is="django-country-selectize"]') && t.push(new Promise((d, c) => {
-            import("./CountrySelectize-SV3ETVIG.js").then(({
+            import("./CountrySelectize-JKM7Q3A2.js").then(({
                 CountrySelectizeElement: l
             }) => {
                 r(d, "django-country-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector("django-sortable-select") ? t.push(new Promise((d, c) => {
-            import("./SortableSelect-3ABJOEP2.js").then(({
+            import("./SortableSelect-UDJCCTN4.js").then(({
                 SortableSelectElement: l
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-TFBRBEV6.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-XUGCVBT5.js").then(({
                     DualSelectorElement: k
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? d() : (window.customElements.define("django-dual-selector", k, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => d()))
                 }).catch(k => c(k))
             }).catch(l => c(l))
         })) : o.querySelector('select[is="django-dual-selector"]') && t.push(new Promise((d, c) => {
-            import("./DualSelector-TFBRBEV6.js").then(({
+            import("./DualSelector-XUGCVBT5.js").then(({
                 DualSelectorElement: l
             }) => {
                 r(d, "django-dual-selector", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-phone-number"]') && t.push(new Promise((d, c) => {
-            import("./PhoneNumber-XY2VHR24.js").then(({
+            import("./PhoneNumber-FXLXZ74J.js").then(({
                 PhoneNumberElement: l
             }) => {
                 r(d, "django-phone-number", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelectorAll('textarea[is="django-richtext"]').forEach(d => {
             t.push(new Promise((c, l) => {
                 let k = () => {
                     d.isInitialized ? c() : d.addEventListener("connected", () => c(), {
                         once: !0
                     })
                 };
-                import("./RichtextArea-PVV6GJIQ.js").then(({
+                import("./RichtextArea-LQJSGPD7.js").then(({
                     RichTextAreaElement: G
                 }) => {
                     customElements.get("django-richtext") instanceof Function ? k() : (window.customElements.define("django-richtext", G, {
                         extends: "textarea"
                     }), window.customElements.whenDefined("django-richtext").then(k))
                 }).catch(G => l(G))
             }))
@@ -2105,103 +2105,103 @@
                 DjangoSlugElement: l
             }) => {
                 r(d, "django-slug", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateFieldElement: l
             }) => {
                 r(d, "django-datefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-6GWQDXEH.js").then(({
+            import("./Calendar-TWTCQYBD.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DatePickerElement: l
             }) => {
                 r(d, "django-datepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateTimeFieldElement: l
             }) => {
                 r(d, "django-datetimefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-6GWQDXEH.js").then(({
+            import("./Calendar-TWTCQYBD.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateTimePickerElement: l
             }) => {
                 r(d, "django-datetimepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateRangeFieldElement: l
             }) => {
                 r(d, "django-daterangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-6GWQDXEH.js").then(({
+            import("./Calendar-TWTCQYBD.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-daterangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateRangePickerElement: l
             }) => {
                 r(d, "django-daterangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateTimeRangeFieldElement: l
             }) => {
                 r(d, "django-datetimerangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-6GWQDXEH.js").then(({
+            import("./Calendar-TWTCQYBD.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimerangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-7RV5MOXB.js").then(({
+            import("./DateTime-WWADX7D6.js").then(({
                 DateTimeRangePickerElement: l
             }) => {
                 r(d, "django-datetimerangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         }))
```

### Comparing `django_formset-1.4.3/formset/static/formset/tiptap-extensions/footnote.js` & `django_formset-1.4.4/formset/static/formset/tiptap-extensions/footnote.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/calendar/hours.html` & `django_formset-1.4.4/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/calendar/months.html` & `django_formset-1.4.4/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/calendar/weeks.html` & `django_formset-1.4.4/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/calendar/years.html` & `django_formset-1.4.4/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/bootstrap/widgets/file.html` & `django_formset-1.4.4/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/bulma/widgets/dual_selector.html` & `django_formset-1.4.4/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/bulma/widgets/file.html` & `django_formset-1.4.4/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/default/collection.html` & `django_formset-1.4.4/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/default/fieldset.html` & `django_formset-1.4.4/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/default/form_dialog.html` & `django_formset-1.4.4/formset/templates/formset/default/form_dialog.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/default/widgets/dual_selector.html` & `django_formset-1.4.4/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/default/widgets/file.html` & `django_formset-1.4.4/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/default/widgets/selectize.html` & `django_formset-1.4.4/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/foundation/widgets/dual_selector.html` & `django_formset-1.4.4/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/foundation/widgets/file.html` & `django_formset-1.4.4/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/blockquote.svg` & `django_formset-1.4.4/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/calendar-today.svg` & `django_formset-1.4.4/formset/templates/formset/icons/calendar-today.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/footnote.svg` & `django_formset-1.4.4/formset/templates/formset/icons/footnote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/letters.svg` & `django_formset-1.4.4/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/placeholder.svg` & `django_formset-1.4.4/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/questionmark.svg` & `django_formset-1.4.4/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/strike.svg` & `django_formset-1.4.4/formset/templates/formset/icons/strike.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/subscript.svg` & `django_formset-1.4.4/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/icons/unlink.svg` & `django_formset-1.4.4/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/richtext/align.html` & `django_formset-1.4.4/formset/templates/formset/richtext/align.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/richtext/color.html` & `django_formset-1.4.4/formset/templates/formset/richtext/color.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/richtext/heading.html` & `django_formset-1.4.4/formset/templates/formset/richtext/heading.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django_formset-1.4.4/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/tailwind/widgets/file.html` & `django_formset-1.4.4/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templates/formset/uikit/widgets/file.html` & `django_formset-1.4.4/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templatetags/formsetify.py` & `django_formset-1.4.4/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templatetags/phonenumber.py` & `django_formset-1.4.4/formset/templatetags/phonenumber.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/templatetags/richtext.py` & `django_formset-1.4.4/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/upload.py` & `django_formset-1.4.4/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/utils.py` & `django_formset-1.4.4/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/views.py` & `django_formset-1.4.4/formset/views.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/formset/widgets.py` & `django_formset-1.4.4/formset/widgets.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4.3/setup.py` & `django_formset-1.4.4/setup.py`

 * *Files identical despite different names*

