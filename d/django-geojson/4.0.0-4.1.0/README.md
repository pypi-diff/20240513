# Comparing `tmp/django-geojson-4.0.0.tar.gz` & `tmp/django_geojson-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-geojson-4.0.0.tar", last modified: Mon Oct 17 09:09:24 2022, max compression
+gzip compressed data, was "django_geojson-4.1.0.tar", last modified: Mon May 13 12:08:10 2024, max compression
```

## Comparing `django-geojson-4.0.0.tar` & `django_geojson-4.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 09:09:24.070377 django-geojson-4.0.0/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     4751 2022-10-17 09:05:53.000000 django-geojson-4.0.0/CHANGES
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7651 2022-10-17 07:17:01.000000 django-geojson-4.0.0/LICENSE
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       35 2022-10-17 07:17:01.000000 django-geojson-4.0.0/MANIFEST.in
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7734 2022-10-17 09:09:24.070377 django-geojson-4.0.0/PKG-INFO
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2070 2022-10-17 08:53:09.000000 django-geojson-4.0.0/README.rst
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 09:09:24.066377 django-geojson-4.0.0/django_geojson.egg-info/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7734 2022-10-17 09:09:24.000000 django-geojson-4.0.0/django_geojson.egg-info/PKG-INFO
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      510 2022-10-17 09:09:24.000000 django-geojson-4.0.0/django_geojson.egg-info/SOURCES.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2022-10-17 09:09:24.000000 django-geojson-4.0.0/django_geojson.egg-info/dependency_links.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2022-10-17 07:17:36.000000 django-geojson-4.0.0/django_geojson.egg-info/not-zip-safe
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       74 2022-10-17 09:09:24.000000 django-geojson-4.0.0/django_geojson.egg-info/requires.txt
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       10 2022-10-17 09:09:24.000000 django-geojson-4.0.0/django_geojson.egg-info/top_level.txt
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 09:09:24.066377 django-geojson-4.0.0/djgeojson/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      415 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/__init__.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2590 2022-10-17 08:56:11.000000 django-geojson-4.0.0/djgeojson/fields.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      517 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/http.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/models.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      371 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/nogeos.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    21778 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/serializers.py
-drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 09:09:24.066377 django-geojson-4.0.0/djgeojson/templatetags/
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/templatetags/__init__.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1615 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/templatetags/geojson_tags.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    34997 2022-10-17 09:03:12.000000 django-geojson-4.0.0/djgeojson/tests.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5911 2022-10-17 07:17:01.000000 django-geojson-4.0.0/djgeojson/views.py
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       38 2022-10-17 09:09:24.070377 django-geojson-4.0.0/setup.cfg
--rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1519 2022-10-17 09:05:53.000000 django-geojson-4.0.0/setup.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 12:08:10.610978 django_geojson-4.1.0/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5216 2024-05-13 12:07:08.000000 django_geojson-4.1.0/CHANGES
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     7651 2022-10-17 07:17:01.000000 django_geojson-4.1.0/LICENSE
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       35 2022-10-17 07:17:01.000000 django_geojson-4.1.0/MANIFEST.in
+-rw-r--r--   0 gagaro    (1000) gagaro    (1000)     8421 2024-05-13 12:08:10.610978 django_geojson-4.1.0/PKG-INFO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2070 2022-10-17 08:53:09.000000 django_geojson-4.1.0/README.rst
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 12:08:10.606979 django_geojson-4.1.0/django_geojson.egg-info/
+-rw-r--r--   0 gagaro    (1000) gagaro    (1000)     8421 2024-05-13 12:08:10.000000 django_geojson-4.1.0/django_geojson.egg-info/PKG-INFO
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      510 2024-05-13 12:08:10.000000 django_geojson-4.1.0/django_geojson.egg-info/SOURCES.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2024-05-13 12:08:10.000000 django_geojson-4.1.0/django_geojson.egg-info/dependency_links.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        1 2022-10-17 07:17:36.000000 django_geojson-4.1.0/django_geojson.egg-info/not-zip-safe
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       74 2024-05-13 12:08:10.000000 django_geojson-4.1.0/django_geojson.egg-info/requires.txt
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       10 2024-05-13 12:08:10.000000 django_geojson-4.1.0/django_geojson.egg-info/top_level.txt
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 12:08:10.606979 django_geojson-4.1.0/djgeojson/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       28 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     2580 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/fields.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      518 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/http.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 07:17:01.000000 django_geojson-4.1.0/djgeojson/models.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)      345 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/nogeos.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    21744 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/serializers.py
+drwxrwxr-x   0 gagaro    (1000) gagaro    (1000)        0 2024-05-13 12:08:10.606979 django_geojson-4.1.0/djgeojson/templatetags/
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)        0 2022-10-17 07:17:01.000000 django_geojson-4.1.0/djgeojson/templatetags/__init__.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1614 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/templatetags/geojson_tags.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)    34955 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/tests.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     5877 2024-05-13 12:05:32.000000 django_geojson-4.1.0/djgeojson/views.py
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)       38 2024-05-13 12:08:10.610978 django_geojson-4.1.0/setup.cfg
+-rw-rw-r--   0 gagaro    (1000) gagaro    (1000)     1581 2024-05-13 12:06:58.000000 django_geojson-4.1.0/setup.py
```

### Comparing `django-geojson-4.0.0/CHANGES` & `django_geojson-4.1.0/CHANGES`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 =========
 CHANGELOG
 =========
 
+4.1.0 (2024-05-13)
+==================
+
+- Drop Python 3.7, Django 3.2. Support Python 3.11 and 3.12, Django 4.2 and 5.0. #123 
+
 4.0.0 (2022-10-17)
 ==================
 
 - Drop support for Python < 3.7 / Django < 3.2
 - Remove jsonfield dependency in favor of django.db.models.JSONField
+	WARNING : This can break your migration. jsonfield used to create a text column for your json data when running 'makemigrations'. However, django.db.models.JSONField creates a json column using database-backend specific column types (ie jsonb on postgresql). As such your model field that used to be a text column is now a jsonb column.
 
 3.2.1 (2022-02-21)
 ==================
 
 - Set default initial value to form field #116 
 
 3.2.0 (2021-04-15)
```

### Comparing `django-geojson-4.0.0/LICENSE` & `django_geojson-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-geojson-4.0.0/PKG-INFO` & `django_geojson-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: django-geojson
-Version: 4.0.0
+Version: 4.1.0
 Summary: Serve vectorial map layers with Django
 Home-page: https://github.com/makinacorpus/django-geojson
 Download-URL: http://pypi.python.org/pypi/django-geojson/
 Author: Mathieu Leplatre
 Author-email: mathieu.leplatre@makina-corpus.com
 License: LPGL, see LICENSE file.
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: Django>=4.0
 Provides-Extra: field
+Requires-Dist: django-leaflet>=0.12; extra == "field"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
 
 ==============
 django-geojson
 ==============
 
 See the `documentation <https://django-geojson.readthedocs.io/en/latest/>`_ for more information.
 
@@ -85,19 +90,25 @@
 Lesser GNU Public License
 
 
 =========
 CHANGELOG
 =========
 
+4.1.0 (2024-05-13)
+==================
+
+- Drop Python 3.7, Django 3.2. Support Python 3.11 and 3.12, Django 4.2 and 5.0. #123 
+
 4.0.0 (2022-10-17)
 ==================
 
 - Drop support for Python < 3.7 / Django < 3.2
 - Remove jsonfield dependency in favor of django.db.models.JSONField
+	WARNING : This can break your migration. jsonfield used to create a text column for your json data when running 'makemigrations'. However, django.db.models.JSONField creates a json column using database-backend specific column types (ie jsonb on postgresql). As such your model field that used to be a text column is now a jsonb column.
 
 3.2.1 (2022-02-21)
 ==================
 
 - Set default initial value to form field #116 
 
 3.2.0 (2021-04-15)
```

### Comparing `django-geojson-4.0.0/README.rst` & `django_geojson-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-geojson-4.0.0/django_geojson.egg-info/PKG-INFO` & `django_geojson-4.1.0/django_geojson.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: django-geojson
-Version: 4.0.0
+Version: 4.1.0
 Summary: Serve vectorial map layers with Django
 Home-page: https://github.com/makinacorpus/django-geojson
 Download-URL: http://pypi.python.org/pypi/django-geojson/
 Author: Mathieu Leplatre
 Author-email: mathieu.leplatre@makina-corpus.com
 License: LPGL, see LICENSE file.
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+License-File: LICENSE
+Requires-Dist: Django>=4.0
 Provides-Extra: field
+Requires-Dist: django-leaflet>=0.12; extra == "field"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autobuild; extra == "docs"
 
 ==============
 django-geojson
 ==============
 
 See the `documentation <https://django-geojson.readthedocs.io/en/latest/>`_ for more information.
 
@@ -85,19 +90,25 @@
 Lesser GNU Public License
 
 
 =========
 CHANGELOG
 =========
 
+4.1.0 (2024-05-13)
+==================
+
+- Drop Python 3.7, Django 3.2. Support Python 3.11 and 3.12, Django 4.2 and 5.0. #123 
+
 4.0.0 (2022-10-17)
 ==================
 
 - Drop support for Python < 3.7 / Django < 3.2
 - Remove jsonfield dependency in favor of django.db.models.JSONField
+	WARNING : This can break your migration. jsonfield used to create a text column for your json data when running 'makemigrations'. However, django.db.models.JSONField creates a json column using database-backend specific column types (ie jsonb on postgresql). As such your model field that used to be a text column is now a jsonb column.
 
 3.2.1 (2022-02-21)
 ==================
 
 - Set default initial value to form field #116 
 
 3.2.0 (2021-04-15)
```

### Comparing `django-geojson-4.0.0/djgeojson/fields.py` & `django_geojson-4.1.0/djgeojson/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from __future__ import unicode_literals
-
+from django.core.exceptions import ValidationError
 from django.db.models import JSONField
-from django.forms.fields import JSONField as JSONFormField, InvalidJSONInput
+from django.forms.fields import InvalidJSONInput
+from django.forms.fields import JSONField as JSONFormField
 from django.forms.widgets import HiddenInput
-from django.core.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _
 
 try:
     from leaflet.forms.widgets import LeafletWidget
     HAS_LEAFLET = True
 except ImportError:
     HAS_LEAFLET = False
```

### Comparing `django-geojson-4.0.0/djgeojson/http.py` & `django_geojson-4.1.0/djgeojson/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+
 from django.http import HttpResponse
 
 
 class HttpGeoJSONResponse(HttpResponse):
     def __init__(self, **kwargs):
         kwargs['content_type'] = 'application/geo+json'
         super(HttpGeoJSONResponse, self).__init__(**kwargs)
```

### Comparing `django-geojson-4.0.0/djgeojson/serializers.py` & `django_geojson-4.1.0/djgeojson/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,49 +3,49 @@
     This code mainly comes from @glenrobertson's django-geoson-tiles at:
     https://github.com/glenrobertson/django-geojson-tiles/
 
     Itself, adapted from @jeffkistler's geojson serializer at: https://gist.github.com/967274
 """
 import json
 import logging
-from io import StringIO  # NOQA
-
 from contextlib import contextmanager
+from io import StringIO  # NOQA
 
 import django
 from django.db.models.base import Model
 
 try:
     from django.db.models.query import QuerySet, ValuesQuerySet
 except ImportError:
     from django.db.models.query import QuerySet
     ValuesQuerySet = None
 
-from django.forms.models import model_to_dict
-from django.core.serializers.python import (_get_model,
-                                            Serializer as PythonSerializer,
-                                            Deserializer as PythonDeserializer)
+from django.core.exceptions import ImproperlyConfigured
+from django.core.serializers.base import (
+    DeserializationError,
+    SerializationError,
+)
 from django.core.serializers.json import DjangoJSONEncoder
-from django.core.serializers.base import SerializationError, DeserializationError
+from django.core.serializers.python import Deserializer as PythonDeserializer
+from django.core.serializers.python import Serializer as PythonSerializer
+from django.core.serializers.python import _get_model
+from django.forms.models import model_to_dict
 from django.utils.encoding import smart_str
-from django.core.exceptions import ImproperlyConfigured
 
 try:
-    from django.contrib.gis.geos import WKBWriter
-    from django.contrib.gis.geos import GEOSGeometry
     from django.contrib.gis.db.models.fields import GeometryField
+    from django.contrib.gis.geos import GEOSGeometry, WKBWriter
 except (ImportError, ImproperlyConfigured):
     from .nogeos import WKBWriter
     from .nogeos import GEOSGeometry
     from .fields import GeometryField
 
 from . import GEOJSON_DEFAULT_SRID
 from .fields import GeoJSONField
 
-
 logger = logging.getLogger(__name__)
 
 
 def hasattr_lazy(obj, name):
     if isinstance(obj, dict):
         return name in obj
     return name in dir(obj)
```

### Comparing `django-geojson-4.0.0/djgeojson/templatetags/geojson_tags.py` & `django_geojson-4.1.0/djgeojson/templatetags/geojson_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import json
 import re
 
 from django import template
 from django.core.exceptions import ImproperlyConfigured
 
 try:
-    from django.contrib.gis.geos import GEOSGeometry
     from django.contrib.gis.db.models.fields import GeometryField
+    from django.contrib.gis.geos import GEOSGeometry
 except (ImportError, ImproperlyConfigured):
     from ..nogeos import GEOSGeometry
     from ..fields import GeometryField
 
 from .. import GEOJSON_DEFAULT_SRID
-from ..serializers import Serializer, DjangoGeoJSONEncoder
-
+from ..serializers import DjangoGeoJSONEncoder, Serializer
 
 register = template.Library()
 
 
 @register.filter
 def geojsonfeature(source, params=''):
     """
```

### Comparing `django-geojson-4.0.0/djgeojson/tests.py` & `django_geojson-4.1.0/djgeojson/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from __future__ import unicode_literals
-
 import json
 
 import django
-from django.forms import HiddenInput
-from django.test import TestCase
 from django.conf import settings
-from django.core import serializers
-from django.core.exceptions import ValidationError, SuspiciousOperation
 from django.contrib.gis.db import models
-from django.contrib.gis.geos import LineString, Point, GeometryCollection
+from django.contrib.gis.geos import GeometryCollection, LineString, Point
+from django.core import serializers
+from django.core.exceptions import SuspiciousOperation, ValidationError
+from django.forms import HiddenInput
+from django.test import TestCase
 from django.utils.encoding import smart_str
 
-from .templatetags.geojson_tags import geojsonfeature
+from .fields import GeoJSONField, GeoJSONFormField, GeoJSONValidator
 from .serializers import Serializer
+from .templatetags.geojson_tags import geojsonfeature
 from .views import GeoJSONLayerView, TiledGeoJSONLayerView
-from .fields import GeoJSONField, GeoJSONFormField, GeoJSONValidator
-
 
 settings.SERIALIZATION_MODULES = {'geojson': 'djgeojson.serializers'}
 
 
 class PictureMixin(object):
 
     @property
@@ -676,17 +673,17 @@
         self.p2 = FixedSridPoint.objects.create(geom=Point(253442, 532897))
 
     def test_within_viewport(self):
         self.view.args = [12, 2125, 1338]
         response = self.view.render_to_response(context={})
         geojson = json.loads(smart_str(response.content))
         self.assertEqual(len(geojson['features']), 2)
-        self.assertAlmostEqual(geojson['features'][0]['geometry']['coordinates'][0], 6.843322039261242)
+        self.assertAlmostEqual(geojson['features'][0]['geometry']['coordinates'][0], 6.843321961076886)
         self.assertAlmostEqual(geojson['features'][0]['geometry']['coordinates'][1], 52.76181518632031)
-        self.assertAlmostEqual(geojson['features'][1]['geometry']['coordinates'][0], 6.846053318324978)
+        self.assertAlmostEqual(geojson['features'][1]['geometry']['coordinates'][0], 6.846053240233331)
         self.assertAlmostEqual(geojson['features'][1]['geometry']['coordinates'][1], 52.77442791046052)
 
 
 class Address(models.Model):
     geom = GeoJSONField()
```

### Comparing `django-geojson-4.0.0/djgeojson/views.py` & `django_geojson-4.1.0/djgeojson/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 import django
 from django.core.exceptions import ImproperlyConfigured
 
 try:
     from django.contrib.gis.db.models.functions import Intersection
 except (ImportError, ImproperlyConfigured):
     Intersection = None
-from django.views.generic import ListView
+from django.core.exceptions import ImproperlyConfigured, SuspiciousOperation
 from django.utils.decorators import method_decorator
 from django.views.decorators.gzip import gzip_page
-from django.core.exceptions import SuspiciousOperation
-from django.core.exceptions import ImproperlyConfigured
+from django.views.generic import ListView
 
 try:
     from django.contrib.gis.geos import Polygon
 except (ImportError, ImproperlyConfigured):
     try:
         from django.contrib.gis.geos.geometry import Polygon
     except (ImportError, ImproperlyConfigured):
         from .nogeos import Polygon
 
 try:
     from django.contrib.gis.db.models import PointField
 except (ImportError, ImproperlyConfigured):
     from .fields import PointField
 
+from . import GEOJSON_DEFAULT_SRID
 from .http import HttpGeoJSONResponse
 from .serializers import Serializer as GeoJSONSerializer
-from . import GEOJSON_DEFAULT_SRID
 
 
 class GeoJSONResponseMixin(object):
     """
     A mixin that can be used to render a GeoJSON response.
     """
     response_class = HttpGeoJSONResponse
```

### Comparing `django-geojson-4.0.0/setup.py` & `django_geojson-4.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import os
 from io import open
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name='django-geojson',
-    version='4.0.0',
+    version='4.1.0',
     author='Mathieu Leplatre',
     author_email='mathieu.leplatre@makina-corpus.com',
     url='https://github.com/makinacorpus/django-geojson',
     download_url="http://pypi.python.org/pypi/django-geojson/",
     description="Serve vectorial map layers with Django",
     long_description=open(os.path.join(here, 'README.rst')).read() + '\n\n' +
                      open(os.path.join(here, 'CHANGES'), encoding='utf-8').read(),
     license='LPGL, see LICENSE file.',
     install_requires=[
-        'Django>=3.2',
+        'Django>=4.0',
     ],
     extras_require={
         'field': ['django-leaflet>=0.12'],
         'docs': ['sphinx', 'sphinx-autobuild'],
     },
     packages=find_packages(),
-    python_requires=">=3.5",
+    python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
     classifiers=['Topic :: Utilities',
                  'Natural Language :: English',
                  'Operating System :: OS Independent',
                  'Intended Audience :: Developers',
                  'Environment :: Web Environment',
                  'Framework :: Django',
                  'Development Status :: 5 - Production/Stable',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7',
                  'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11',
+                 'Programming Language :: Python :: 3.12',
     ],
 )
```

