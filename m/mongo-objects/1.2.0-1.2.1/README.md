# Comparing `tmp/mongo_objects-1.2.0.tar.gz` & `tmp/mongo_objects-1.2.1.tar.gz`

## Comparing `mongo_objects-1.2.0.tar` & `mongo_objects-1.2.1.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/.buildinfo
--rw-r--r--   0        0        0    32726 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoDictProxy.html
--rw-r--r--   0        0        0    37165 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoListProxy.html
--rw-r--r--   0        0        0    34866 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoSingleProxy.html
--rw-r--r--   0        0        0    86142 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoUserDict.html
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/customization.html
--rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/genindex.html
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/index.html
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/objects.inv
--rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/proxy_overview.html
--rw-r--r--   0        0        0    15225 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/quickstart.html
--rw-r--r--   0        0        0    49234 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/sample.html
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/search.html
--rw-r--r--   0        0        0    30606 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/searchindex.js
--rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-feature.png
--rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-gift.png
--rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-ticket-type-1.png
--rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-ticket-type-2.png
--rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-ticket-type-3.png
--rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-venue.png
--rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/create-event.png
--rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/purchase-ticket.png
--rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/vip-ticket-detail-1.png
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoDictProxy.rst.txt
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoListProxy.rst.txt
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoSingleProxy.rst.txt
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoUserDict.rst.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/customization.rst.txt
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/index.rst.txt
--rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/proxy_overview.rst.txt
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/quickstart.rst.txt
--rw-r--r--   0        0        0    19506 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/sample.rst.txt
--rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-feature.png
--rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-gift.png
--rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-ticket-type-1.png
--rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-ticket-type-2.png
--rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-ticket-type-3.png
--rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-venue.png
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/alabaster.css
--rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/basic.css
--rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/create-event.png
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/doctools.js
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/plus.png
--rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/purchase-ticket.png
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/pygments.css
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/searchtools.js
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/vip-ticket-detail-1.png
--rw-r--r--   0        0        0    29582 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/mongo_objects_sample.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/requirements.txt
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/run-sample-app
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/static/base.css
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/admin-event-detail.jinja
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/admin-event-list.jinja
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/admin-ticket-detail.jinja
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/base.jinja
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-event.jinja
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-feature.jinja
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-gift.jinja
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-ticket-type.jinja
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-venue.jinja
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/customer-event-detail.jinja
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/customer-event-list.jinja
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/customer-purchase-ticket.jinja
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/form-tools.jinja
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/index.jinja
--rw-r--r--   0        0        0    62761 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/src/mongo_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0    34946 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    38456 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    34289 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    40908 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    22162 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    20130 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_proxy_combo.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/README.rst
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/.buildinfo
+-rw-r--r--   0        0        0    32726 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/MongoDictProxy.html
+-rw-r--r--   0        0        0    37165 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/MongoListProxy.html
+-rw-r--r--   0        0        0    34866 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/MongoSingleProxy.html
+-rw-r--r--   0        0        0    86142 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/MongoUserDict.html
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/customization.html
+-rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/genindex.html
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/index.html
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/objects.inv
+-rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/proxy_overview.html
+-rw-r--r--   0        0        0    15225 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/quickstart.html
+-rw-r--r--   0        0        0    49234 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/sample.html
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/search.html
+-rw-r--r--   0        0        0    37058 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/searchindex.js
+-rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/add-feature.png
+-rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/add-gift.png
+-rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/add-ticket-type-1.png
+-rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/add-ticket-type-2.png
+-rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/add-ticket-type-3.png
+-rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/add-venue.png
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/create-event.png
+-rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/purchase-ticket.png
+-rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_images/vip-ticket-detail-1.png
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/MongoDictProxy.rst.txt
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/MongoListProxy.rst.txt
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/MongoSingleProxy.rst.txt
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/MongoUserDict.rst.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/customization.rst.txt
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/proxy_overview.rst.txt
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/quickstart.rst.txt
+-rw-r--r--   0        0        0    19506 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_sources/sample.rst.txt
+-rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/add-feature.png
+-rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/add-gift.png
+-rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/add-ticket-type-1.png
+-rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/add-ticket-type-2.png
+-rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/add-ticket-type-3.png
+-rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/add-venue.png
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/alabaster.css
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/basic.css
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/create-event.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/doctools.js
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/plus.png
+-rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/purchase-ticket.png
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/docs/_static/vip-ticket-detail-1.png
+-rw-r--r--   0        0        0    29582 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/mongo_objects_sample.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/requirements.txt
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/run-sample-app
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/static/base.css
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/admin-event-detail.jinja
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/admin-event-list.jinja
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/admin-ticket-detail.jinja
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/base.jinja
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/create-update-event.jinja
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/create-update-feature.jinja
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/create-update-gift.jinja
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/create-update-ticket-type.jinja
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/create-update-venue.jinja
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/customer-event-detail.jinja
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/customer-event-list.jinja
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/customer-purchase-ticket.jinja
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/form-tools.jinja
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/sample/templates/index.jinja
+-rw-r--r--   0        0        0    63120 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/src/mongo_objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/requirements.txt
+-rw-r--r--   0        0        0    36499 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    40045 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    40926 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    22162 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    20130 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/tests/test_proxy_combo.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/README.rst
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 mongo_objects-1.2.1/PKG-INFO
```

### Comparing `mongo_objects-1.2.0/docs/MongoDictProxy.html` & `mongo_objects-1.2.1/docs/MongoDictProxy.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoDictProxy &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>MongoDictProxy &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoListProxy" href="MongoListProxy.html" />
     <link rel="prev" title="Proxy Overview" href="proxy_overview.html" />
```

### Comparing `mongo_objects-1.2.0/docs/MongoListProxy.html` & `mongo_objects-1.2.1/docs/MongoListProxy.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoListProxy &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>MongoListProxy &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoSingleProxy" href="MongoSingleProxy.html" />
     <link rel="prev" title="MongoDictProxy" href="MongoDictProxy.html" />
```

### Comparing `mongo_objects-1.2.0/docs/MongoSingleProxy.html` & `mongo_objects-1.2.1/docs/MongoSingleProxy.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoSingleProxy &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>MongoSingleProxy &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="MongoListProxy" href="MongoListProxy.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `mongo_objects-1.2.0/docs/MongoUserDict.html` & `mongo_objects-1.2.1/docs/MongoUserDict.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>MongoUserDict &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>MongoUserDict &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Proxy Overview" href="proxy_overview.html" />
     <link rel="prev" title="Sample Application" href="sample.html" />
```

### Comparing `mongo_objects-1.2.0/docs/customization.html` & `mongo_objects-1.2.1/docs/customization.html`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/genindex.html` & `mongo_objects-1.2.1/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>Index &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `mongo_objects-1.2.0/docs/index.html` & `mongo_objects-1.2.1/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Introduction To mongo_objects &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>Introduction To mongo_objects &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Quickstart" href="quickstart.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
@@ -40,19 +40,20 @@
 <p>Documents are returned as user-defined UserDict subclasses, seamlessly linking user code
 with MongoDB data.</p>
 <p>Subdocuments are accessed through user-defined, dictionary-like subclasses that proxy
 data from the original parent document.</p>
 </section>
 <section id="installation">
 <h2>Installation<a class="headerlink" href="#installation" title="Link to this heading">¶</a></h2>
-<p>Install from PyPI. We recommend installing into the virtual environment
+<p>Install from <a class="reference external" href="https://pypi.org/project/mongo-objects">PyPI</a>. We recommend installing into the virtual environment
 for your Python project.:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">mongo_objects</span>
 </pre></div>
 </div>
+<p>The source code is also available <a class="reference external" href="https://github.com/lindstrom-j/mongo_objects">GitHub</a>.</p>
 </section>
 <section id="getting-started">
 <h2>Getting Started<a class="headerlink" href="#getting-started" title="Link to this heading">¶</a></h2>
 <p>Check out the <a class="reference internal" href="quickstart.html"><span class="doc">Quickstart</span></a> documentation for a brief overview of document
 and subdocument features.</p>
 <p>See the <a class="reference internal" href="sample.html"><span class="doc">Sample Application</span></a> code for a working demonstration.</p>
 <div class="toctree-wrapper compound">
```

#### html2text {}

```diff
@@ -3,17 +3,18 @@
 mongo_objects wraps pymongo with new classes to simplify access to MongoDB
 documents and subdocuments.
 Documents are returned as user-defined UserDict subclasses, seamlessly linking
 user code with MongoDB data.
 Subdocuments are accessed through user-defined, dictionary-like subclasses that
 proxy data from the original parent document.
 ********** IInnssttaallllaattiioonn_?¶ **********
-Install from PyPI. We recommend installing into the virtual environment for
+Install from _P_y_P_I. We recommend installing into the virtual environment for
 your Python project.:
 pip install mongo_objects
+The source code is also available _G_i_t_H_u_b.
 ********** GGeettttiinngg SSttaarrtteedd_?¶ **********
 Check out the _Q_u_i_c_k_s_t_a_r_t documentation for a brief overview of document and
 subdocument features.
 See the _S_a_m_p_l_e_ _A_p_p_l_i_c_a_t_i_o_n code for a working demonstration.
     * _Q_u_i_c_k_s_t_a_r_t
           o _M_o_n_g_o_D_B_ _D_o_c_u_m_e_n_t_s
           o _S_u_b_-_D_o_c_u_m_e_n_t_ _P_r_o_x_i_e_s
```

### Comparing `mongo_objects-1.2.0/docs/objects.inv` & `mongo_objects-1.2.1/docs/objects.inv`

 * *Files 15% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: mongo_objects
-# Version: 1.1.2
+# Version: 1.2.0
 # The remainder of this file is compressed using zlib.
 
 mongo_objects.MongoDictProxy py:class 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.__init__ py:method 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.container_name py:attribute 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.create py:method 1 MongoDictProxy.html#$ -
 mongo_objects.MongoDictProxy.create_key py:method 1 MongoDictProxy.html#$ -
```

### Comparing `mongo_objects-1.2.0/docs/proxy_overview.html` & `mongo_objects-1.2.1/docs/proxy_overview.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Proxy Overview &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>Proxy Overview &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoDictProxy" href="MongoDictProxy.html" />
     <link rel="prev" title="MongoUserDict" href="MongoUserDict.html" />
```

### Comparing `mongo_objects-1.2.0/docs/quickstart.html` & `mongo_objects-1.2.1/docs/quickstart.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Quickstart &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>Quickstart &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Sample Application" href="sample.html" />
     <link rel="prev" title="Introduction To mongo_objects" href="index.html" />
```

### Comparing `mongo_objects-1.2.0/docs/sample.html` & `mongo_objects-1.2.1/docs/sample.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Sample Application &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>Sample Application &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="MongoUserDict" href="MongoUserDict.html" />
     <link rel="prev" title="Quickstart" href="quickstart.html" />
```

### Comparing `mongo_objects-1.2.0/docs/search.html` & `mongo_objects-1.2.1/docs/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; mongo_objects 1.1.2 documentation</title>
+    <title>Search &#8212; mongo_objects 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     
-    <script src="_static/documentation_options.js?v=6f037312"></script>
+    <script src="_static/documentation_options.js?v=6efca38a"></script>
     <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
     <script src="searchindex.js" defer="defer"></script>
```

### Comparing `mongo_objects-1.2.0/docs/searchindex.js` & `mongo_objects-1.2.1/docs/searchindex.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -198,146 +198,314 @@
         "sphinx.domains.std": 2
     },
     "filenames": ["MongoDictProxy.rst", "MongoListProxy.rst", "MongoSingleProxy.rst", "MongoUserDict.rst", "index.rst", "proxy_overview.rst", "quickstart.rst", "sample.rst"],
     "indexentries": {
         "__init__() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.__init__", false]
         ],
+        "__init__() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.__init__", false]
+        ],
         "__init__() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.__init__", false]
         ],
+        "__init__() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.__init__", false]
+        ],
+        "authorize_delete() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.authorize_delete", false]
+        ],
+        "authorize_init() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.authorize_init", false]
+        ],
+        "authorize_pre_read() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.authorize_pre_read", false]
+        ],
+        "authorize_read() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.authorize_read", false]
+        ],
+        "authorize_save() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.authorize_save", false]
+        ],
+        "collection() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.collection", false]
+        ],
+        "collection_name (mongo_objects.mongouserdict attribute)": [
+            [3, "mongo_objects.MongoUserDict.collection_name", false]
+        ],
         "container_name (mongo_objects.mongodictproxy attribute)": [
             [0, "mongo_objects.MongoDictProxy.container_name", false]
         ],
+        "container_name (mongo_objects.mongolistproxy attribute)": [
+            [1, "mongo_objects.MongoListProxy.container_name", false]
+        ],
         "container_name (mongo_objects.mongosingleproxy attribute)": [
             [2, "mongo_objects.MongoSingleProxy.container_name", false]
         ],
         "create() (mongo_objects.mongodictproxy class method)": [
             [0, "mongo_objects.MongoDictProxy.create", false]
         ],
+        "create() (mongo_objects.mongolistproxy class method)": [
+            [1, "mongo_objects.MongoListProxy.create", false]
+        ],
         "create() (mongo_objects.mongosingleproxy class method)": [
             [2, "mongo_objects.MongoSingleProxy.create", false]
         ],
         "create() (mongo_objects.polymorphicmongosingleproxy class method)": [
             [2, "mongo_objects.PolymorphicMongoSingleProxy.create", false]
         ],
         "create_key() (mongo_objects.mongodictproxy class method)": [
             [0, "mongo_objects.MongoDictProxy.create_key", false]
         ],
+        "create_key() (mongo_objects.mongolistproxy class method)": [
+            [1, "mongo_objects.MongoListProxy.create_key", false]
+        ],
         "create_key() (mongo_objects.mongosingleproxy class method)": [
             [2, "mongo_objects.MongoSingleProxy.create_key", false]
         ],
         "data() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.data", false]
         ],
+        "data() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.data", false]
+        ],
         "data() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.data", false]
         ],
+        "database (mongo_objects.mongouserdict attribute)": [
+            [3, "mongo_objects.MongoUserDict.database", false]
+        ],
         "delete() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.delete", false]
         ],
+        "delete() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.delete", false]
+        ],
         "delete() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.delete", false]
         ],
+        "delete() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.delete", false]
+        ],
         "environment variable": [
             [7, "index-0", false]
         ],
         "exists() (mongo_objects.mongodictproxy class method)": [
             [0, "mongo_objects.MongoDictProxy.exists", false]
         ],
+        "exists() (mongo_objects.mongolistproxy class method)": [
+            [1, "mongo_objects.MongoListProxy.exists", false]
+        ],
         "exists() (mongo_objects.mongosingleproxy class method)": [
             [2, "mongo_objects.MongoSingleProxy.exists", false]
         ],
+        "find() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.find", false]
+        ],
+        "find() (mongo_objects.polymorphicmongouserdict class method)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.find", false]
+        ],
+        "find_one() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.find_one", false]
+        ],
+        "find_one() (mongo_objects.polymorphicmongouserdict class method)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.find_one", false]
+        ],
         "get() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.get", false]
         ],
+        "get() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.get", false]
+        ],
         "get() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.get", false]
         ],
         "get_proxies() (mongo_objects.mongodictproxy class method)": [
             [0, "mongo_objects.MongoDictProxy.get_proxies", false]
         ],
+        "get_proxies() (mongo_objects.mongolistproxy class method)": [
+            [1, "mongo_objects.MongoListProxy.get_proxies", false]
+        ],
         "get_proxies() (mongo_objects.mongosingleproxy class method)": [
             [2, "mongo_objects.MongoSingleProxy.get_proxies", false]
         ],
         "get_proxies() (mongo_objects.polymorphicmongodictproxy class method)": [
             [0, "mongo_objects.PolymorphicMongoDictProxy.get_proxies", false]
         ],
+        "get_proxies() (mongo_objects.polymorphicmongolistproxy class method)": [
+            [1, "mongo_objects.PolymorphicMongoListProxy.get_proxies", false]
+        ],
         "get_proxy() (mongo_objects.mongodictproxy class method)": [
             [0, "mongo_objects.MongoDictProxy.get_proxy", false]
         ],
+        "get_proxy() (mongo_objects.mongolistproxy class method)": [
+            [1, "mongo_objects.MongoListProxy.get_proxy", false]
+        ],
         "get_proxy() (mongo_objects.mongosingleproxy class method)": [
             [2, "mongo_objects.MongoSingleProxy.get_proxy", false]
         ],
         "get_proxy() (mongo_objects.polymorphicmongodictproxy class method)": [
             [0, "mongo_objects.PolymorphicMongoDictProxy.get_proxy", false]
         ],
+        "get_proxy() (mongo_objects.polymorphicmongolistproxy class method)": [
+            [1, "mongo_objects.PolymorphicMongoListProxy.get_proxy", false]
+        ],
         "get_proxy() (mongo_objects.polymorphicmongosingleproxy class method)": [
             [2, "mongo_objects.PolymorphicMongoSingleProxy.get_proxy", false]
         ],
+        "get_subclass_by_key() (mongo_objects.polymorphicmongouserdict class method)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.get_subclass_by_key", false]
+        ],
+        "get_subclass_from_doc() (mongo_objects.polymorphicmongouserdict class method)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.get_subclass_from_doc", false]
+        ],
+        "get_unique_integer() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.get_unique_integer", false]
+        ],
+        "get_unique_key() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.get_unique_key", false]
+        ],
         "id() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.id", false]
         ],
+        "id() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.id", false]
+        ],
         "id() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.id", false]
         ],
+        "id() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.id", false]
+        ],
         "items() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.items", false]
         ],
+        "items() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.items", false]
+        ],
         "items() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.items", false]
         ],
         "keys() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.keys", false]
         ],
+        "keys() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.keys", false]
+        ],
         "keys() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.keys", false]
         ],
+        "load_by_id() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.load_by_id", false]
+        ],
+        "load_proxy_by_id() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.load_proxy_by_id", false]
+        ],
+        "load_proxy_by_local_id() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.load_proxy_by_local_id", false]
+        ],
         "mongo_connect_uri": [
             [7, "index-0", false]
         ],
         "mongodictproxy (class in mongo_objects)": [
             [0, "mongo_objects.MongoDictProxy", false]
         ],
+        "mongolistproxy (class in mongo_objects)": [
+            [1, "mongo_objects.MongoListProxy", false]
+        ],
         "mongosingleproxy (class in mongo_objects)": [
             [2, "mongo_objects.MongoSingleProxy", false]
         ],
+        "mongouserdict (class in mongo_objects)": [
+            [3, "mongo_objects.MongoUserDict", false]
+        ],
+        "object_version (mongo_objects.mongouserdict attribute)": [
+            [3, "mongo_objects.MongoUserDict.object_version", false]
+        ],
         "polymorphicmongodictproxy (class in mongo_objects)": [
             [0, "mongo_objects.PolymorphicMongoDictProxy", false]
         ],
+        "polymorphicmongolistproxy (class in mongo_objects)": [
+            [1, "mongo_objects.PolymorphicMongoListProxy", false]
+        ],
         "polymorphicmongosingleproxy (class in mongo_objects)": [
             [2, "mongo_objects.PolymorphicMongoSingleProxy", false]
         ],
+        "polymorphicmongouserdict (class in mongo_objects)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict", false]
+        ],
         "proxy_id() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.proxy_id", false]
         ],
+        "proxy_id() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.proxy_id", false]
+        ],
         "proxy_id() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.proxy_id", false]
         ],
+        "proxy_id() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.proxy_id", false]
+        ],
         "save() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.save", false]
         ],
+        "save() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.save", false]
+        ],
         "save() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.save", false]
         ],
+        "save() (mongo_objects.mongouserdict method)": [
+            [3, "mongo_objects.MongoUserDict.save", false]
+        ],
+        "save() (mongo_objects.polymorphicmongouserdict method)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.save", false]
+        ],
         "setdefault() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.setdefault", false]
         ],
+        "setdefault() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.setdefault", false]
+        ],
         "setdefault() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.setdefault", false]
         ],
+        "split_id() (mongo_objects.mongouserdict class method)": [
+            [3, "mongo_objects.MongoUserDict.split_id", false]
+        ],
+        "subclass_key (mongo_objects.polymorphicmongouserdict attribute)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.subclass_key", false]
+        ],
+        "subclass_key_name (mongo_objects.polymorphicmongouserdict attribute)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.subclass_key_name", false]
+        ],
+        "subclass_map (mongo_objects.polymorphicmongouserdict attribute)": [
+            [3, "mongo_objects.PolymorphicMongoUserDict.subclass_map", false]
+        ],
+        "subdoc_key_sep (mongo_objects.mongouserdict attribute)": [
+            [3, "mongo_objects.MongoUserDict.subdoc_key_sep", false]
+        ],
         "update() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.update", false]
         ],
+        "update() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.update", false]
+        ],
         "update() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.update", false]
         ],
+        "utcnow() (mongo_objects.mongouserdict static method)": [
+            [3, "mongo_objects.MongoUserDict.utcnow", false]
+        ],
         "values() (mongo_objects.mongodictproxy method)": [
             [0, "mongo_objects.MongoDictProxy.values", false]
         ],
+        "values() (mongo_objects.mongolistproxy method)": [
+            [1, "mongo_objects.MongoListProxy.values", false]
+        ],
         "values() (mongo_objects.mongosingleproxy method)": [
             [2, "mongo_objects.MongoSingleProxy.values", false]
         ]
     },
     "objects": {
         "mongo_objects": [
             [0, 0, 1, "", "MongoDictProxy"],
@@ -582,15 +750,15 @@
         "again": [0, 1, 2, 3],
         "against": [2, 3, 7],
         "align": [],
         "all": [0, 1, 2, 3, 5, 6, 7],
         "allow": [3, 5],
         "along": [0, 1, 2],
         "alreadi": [0, 1, 2, 3, 7],
-        "also": [1, 3, 5, 6, 7],
+        "also": [1, 3, 4, 5, 6, 7],
         "altern": [],
         "alternate_venu": [],
         "although": 7,
         "alwai": 2,
         "amount": [],
         "an": [0, 1, 2, 3, 4, 5, 6],
         "an_ev": 6,
@@ -621,15 +789,15 @@
         "authorize_init": 3,
         "authorize_pre_read": 3,
         "authorize_read": 3,
         "authorize_sav": 3,
         "auto": [0, 1, 2, 5, 7],
         "automat": [3, 6, 7],
         "autosav": [0, 1, 2, 3],
-        "avail": [3, 5, 7],
+        "avail": [3, 4, 5, 7],
         "avenu": 7,
         "avoid": [1, 2],
         "b": [],
         "back": [3, 4, 6, 7],
         "bag": 7,
         "bar": 7,
         "base": [2, 3, 5, 7],
@@ -851,14 +1019,15 @@
         "get_unique_integ": 3,
         "get_unique_kei": 3,
         "getticket": 7,
         "getticketsbytyp": 7,
         "gettickettyp": 7,
         "getvenu": 7,
         "gift": 7,
+        "github": 4,
         "given": 3,
         "grand": [5, 7],
         "great": 3,
         "group": 5,
         "gt": 7,
         "guarante": [3, 7],
         "guess": 6,
@@ -882,15 +1051,15 @@
         "hous": 7,
         "how": 1,
         "howev": [],
         "http": 7,
         "hybrid": 3,
         "hybridev": 3,
         "hybridid": 3,
-        "i": [0, 1, 2, 3, 5, 6, 7],
+        "i": [0, 1, 2, 3, 4, 5, 6, 7],
         "id": [0, 1, 4, 6, 7],
         "ident": [5, 7],
         "identifi": [0, 1, 2, 5, 7],
         "ignor": [0, 1, 2],
         "illustr": [6, 7],
         "imag": [],
         "imaginari": 7,
@@ -1262,15 +1431,15 @@
         "slow": 1,
         "snippet": 6,
         "so": [0, 1, 2, 3, 5],
         "sold": 7,
         "some": [3, 7],
         "someth": 0,
         "sometim": 7,
-        "sourc": [5, 7],
+        "sourc": [4, 5, 7],
         "special": 5,
         "specif": [3, 5, 7],
         "split": 3,
         "split_id": 3,
         "sponsor": 4,
         "sql": 7,
         "standard": [3, 5],
```

### Comparing `mongo_objects-1.2.0/docs/_images/add-feature.png` & `mongo_objects-1.2.1/docs/_images/add-feature.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/add-gift.png` & `mongo_objects-1.2.1/docs/_images/add-gift.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/add-ticket-type-1.png` & `mongo_objects-1.2.1/docs/_images/add-ticket-type-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/add-ticket-type-2.png` & `mongo_objects-1.2.1/docs/_images/add-ticket-type-2.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/add-ticket-type-3.png` & `mongo_objects-1.2.1/docs/_images/add-ticket-type-3.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/add-venue.png` & `mongo_objects-1.2.1/docs/_images/add-venue.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/create-event.png` & `mongo_objects-1.2.1/docs/_images/create-event.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/purchase-ticket.png` & `mongo_objects-1.2.1/docs/_images/purchase-ticket.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_images/vip-ticket-detail-1.png` & `mongo_objects-1.2.1/docs/_images/vip-ticket-detail-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/MongoDictProxy.rst.txt` & `mongo_objects-1.2.1/docs/_sources/MongoDictProxy.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/MongoListProxy.rst.txt` & `mongo_objects-1.2.1/docs/_sources/MongoListProxy.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/MongoSingleProxy.rst.txt` & `mongo_objects-1.2.1/docs/_sources/MongoSingleProxy.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/MongoUserDict.rst.txt` & `mongo_objects-1.2.1/docs/_sources/MongoUserDict.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/index.rst.txt` & `mongo_objects-1.2.1/docs/_sources/index.rst.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 Subdocuments are accessed through user-defined, dictionary-like subclasses that proxy
 data from the original parent document.
 
 
 Installation
 ------------
 
-Install from PyPI. We recommend installing into the virtual environment
+Install from `PyPI <https://pypi.org/project/mongo-objects>`_. We recommend installing into the virtual environment
 for your Python project.::
 
     pip install mongo_objects
 
+The source code is also available `GitHub <https://github.com/lindstrom-j/mongo_objects>`_.
 
 Getting Started
 ---------------
 
 Check out the :doc:`quickstart` documentation for a brief overview of document
 and subdocument features.
```

### Comparing `mongo_objects-1.2.0/docs/_sources/proxy_overview.rst.txt` & `mongo_objects-1.2.1/docs/_sources/proxy_overview.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/quickstart.rst.txt` & `mongo_objects-1.2.1/docs/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_sources/sample.rst.txt` & `mongo_objects-1.2.1/docs/_sources/sample.rst.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/add-feature.png` & `mongo_objects-1.2.1/docs/_static/add-feature.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/add-gift.png` & `mongo_objects-1.2.1/docs/_static/add-gift.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/add-ticket-type-1.png` & `mongo_objects-1.2.1/docs/_static/add-ticket-type-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/add-ticket-type-2.png` & `mongo_objects-1.2.1/docs/_static/add-ticket-type-2.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/add-ticket-type-3.png` & `mongo_objects-1.2.1/docs/_static/add-ticket-type-3.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/add-venue.png` & `mongo_objects-1.2.1/docs/_static/add-venue.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/alabaster.css` & `mongo_objects-1.2.1/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/basic.css` & `mongo_objects-1.2.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/create-event.png` & `mongo_objects-1.2.1/docs/_static/create-event.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/doctools.js` & `mongo_objects-1.2.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/language_data.js` & `mongo_objects-1.2.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/purchase-ticket.png` & `mongo_objects-1.2.1/docs/_static/purchase-ticket.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/pygments.css` & `mongo_objects-1.2.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/searchtools.js` & `mongo_objects-1.2.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/sphinx_highlight.js` & `mongo_objects-1.2.1/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/docs/_static/vip-ticket-detail-1.png` & `mongo_objects-1.2.1/docs/_static/vip-ticket-detail-1.png`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/mongo_objects_sample.py` & `mongo_objects-1.2.1/sample/mongo_objects_sample.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/run-sample-app` & `mongo_objects-1.2.1/sample/run-sample-app`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/admin-event-detail.jinja` & `mongo_objects-1.2.1/sample/templates/admin-event-detail.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/admin-event-list.jinja` & `mongo_objects-1.2.1/sample/templates/admin-event-list.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/admin-ticket-detail.jinja` & `mongo_objects-1.2.1/sample/templates/admin-ticket-detail.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/base.jinja` & `mongo_objects-1.2.1/sample/templates/base.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/create-update-event.jinja` & `mongo_objects-1.2.1/sample/templates/create-update-event.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/create-update-feature.jinja` & `mongo_objects-1.2.1/sample/templates/create-update-feature.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/create-update-gift.jinja` & `mongo_objects-1.2.1/sample/templates/create-update-gift.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/create-update-ticket-type.jinja` & `mongo_objects-1.2.1/sample/templates/create-update-ticket-type.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/create-update-venue.jinja` & `mongo_objects-1.2.1/sample/templates/create-update-venue.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/customer-event-detail.jinja` & `mongo_objects-1.2.1/sample/templates/customer-event-detail.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/customer-event-list.jinja` & `mongo_objects-1.2.1/sample/templates/customer-event-list.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/customer-purchase-ticket.jinja` & `mongo_objects-1.2.1/sample/templates/customer-purchase-ticket.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/form-tools.jinja` & `mongo_objects-1.2.1/sample/templates/form-tools.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/sample/templates/index.jinja` & `mongo_objects-1.2.1/sample/templates/index.jinja`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/src/mongo_objects.py` & `mongo_objects-1.2.1/src/mongo_objects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,18 @@
 
         # load the MongoDB document and remove the ID from the list of ids
         obj = cls.load_by_id( ids.pop(0), readonly=readonly )
 
         # assuming a parent object was loaded, loop through
         # each level of proxy using the previous object as the parent
         if obj is not None:
-            for (proxy_subclass, id) in zip( args, ids, strict=True ):
+            # COMPATABILITY: 3.10+ use zip( args, ids, strict=True )
+            if len( args ) != len( ids ):
+                raise ValueError
+            for (proxy_subclass, id) in zip( args, ids ):
                 try:
                     obj = proxy_subclass.get_proxy( obj, id )
                 except Exception as e:
                     raise
 
         # return the lowest-level object
         return obj
@@ -431,18 +434,24 @@
         :returns: an instance of the final, rightmost proxy subdocument class
           from *args*
         """
 
         # split the subdocument_id into its components
         ids = self.split_id( id )
 
+        # COMPATABILITY: 3.10+ use zip( args, ids, strict=True )
+        print( f"len ids{len(ids)}: {ids!r}" )
+        print( f"len args {len(args)} : {args!r}" )
+        if len( args ) != len( ids ):
+            raise ValueError
+
         # loop through each level of proxy using the previous object
         # as the parent
         obj = self
-        for (proxy_subclass, id) in zip( args, ids, strict=True ):
+        for (proxy_subclass, id) in zip( args, ids ):
             try:
                 obj = proxy_subclass.get_proxy( obj, id )
             except Exception as e:
                 raise
 
         # return the lowest-level object
         return obj
@@ -559,15 +568,15 @@
     def utcnow():
         """MongoDB stores milliseconds, not microseconds.
         Drop microseconds from the standard utcnow() so comparisons can be made with database times.
 
         :returns: The current time with microseconds set to 0.
         :rtype: naive :class:`datetime.datetime`
         """
-        now = datetime.datetime.now( datetime.UTC )
+        now = datetime.datetime.now( datetime.timezone.utc )
         return now.replace( microsecond=(now.microsecond // 1000) * 1000, tzinfo=None )
 
 
 
 class PolymorphicMongoUserDict( MongoUserDict ):
     """Like MongoUserDict but supports polymorphic document objects within the same collection.
```

### Comparing `mongo_objects-1.2.0/tests/test_MongoDictProxy.py` & `mongo_objects-1.2.1/tests/test_MongoDictProxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -838,15 +838,14 @@
         # verify the objects are the same
         assert result.data() == proxyA.data()
 
         # verify the parent is not readonly
         assert result.ultimate_parent.readonly is False
 
 
-
     def test_load_proxy_by_id_readonly( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], readonly=True )
 
@@ -889,64 +888,101 @@
         proxyA = getSampleProxyA
 
         # Can't load proxyB with proxyA's ID
         with pytest.raises( mongo_objects.MongoObjectsNonexistentKey ):
             result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['B'] )
 
 
+    def test_load_proxy_by_id_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # loading a proxy with more classes than IDs raises a ValueError
+        with pytest.raises( ValueError ):
+            classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], classes['B'] )
+
+
     def test_load_proxy_by_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'] )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
         # verify the parent is not readonly
         assert result.ultimate_parent.readonly is False
 
 
-    def test_load_proxy_by_id_readonly_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_load_proxy_by_id_A1_readonly( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'], readonly=True )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
         # verify the parent is readonly
         assert result.ultimate_parent.readonly is True
 
 
+    def test_load_proxy_by_id_A1_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # loading a proxy with more IDs than classes raises a ValueError
+        with pytest.raises( ValueError ):
+            classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'] )
+
+
     def test_load_proxy_by_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # reload the proxy by its local ID
         result = proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'] )
 
         # verify the objects are the same
         assert result.data() == proxyA.data()
 
 
+    def test_load_proxy_by_local_id_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # loading a proxy with more classes than IDs raises a ValueError
+        with pytest.raises( ValueError ):
+            proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'], classes['B'] )
+
+
     def test_load_proxy_by_local_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'], classes['A1'] )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
 
+
+    def test_load_proxy_by_local_id_A1_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # loading a proxy with more IDs than classes raises a ValueError
+        with pytest.raises( ValueError ):
+            proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'] )
+
+
     def test_proxy_id( self, getSampleProxyA ):
         """Test single level proxy ID"""
         proxy = getSampleProxyA
         assert proxy.proxy_id() == f"{proxy.key}"
 
 
     def test_proxy_id_with_parent_id( self, getSampleProxyA ):
```

### Comparing `mongo_objects-1.2.0/tests/test_MongoListProxy.py` & `mongo_objects-1.2.1/tests/test_MongoListProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -972,64 +972,102 @@
         # Can't load proxyB with proxyA's ID
         with pytest.raises( mongo_objects.MongoObjectsNonexistentKey ):
             result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['B'] )
             # list proxies are lazy lookups and must be used to be resolved
             result.keys()
 
 
+    def test_load_proxy_by_id_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # loading a proxy with more classes than IDs raises a ValueError
+        with pytest.raises( ValueError ):
+            classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], classes['B'] )
+
+
     def test_load_proxy_by_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'] )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
         # verify the parent is not readonly
         assert result.ultimate_parent.readonly is False
 
 
-    def test_load_proxy_by_id_readonly_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_load_proxy_by_id_A1_readonly( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'], readonly=True )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
         # verify the parent is readonly
         assert result.ultimate_parent.readonly is True
 
 
+    def test_load_proxy_by_id_A1_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # loading a proxy with more IDs than classes raises a ValueError
+        with pytest.raises( ValueError ):
+            classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'] )
+
+
     def test_load_proxy_by_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # reload the proxy by its local ID
         result = proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'] )
 
         # verify the objects are the same
         assert result.data() == proxyA.data()
 
 
+    def test_load_proxy_by_local_id_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # loading a proxy with more classes than IDs raises a ValueError
+        with pytest.raises( ValueError ):
+            proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'], classes['B'] )
+
+
     def test_load_proxy_by_local_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'], classes['A1'] )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
 
+
+    def test_load_proxy_by_local_id_A1_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # loading a proxy with more IDs than classes raises a ValueError
+        with pytest.raises( ValueError ):
+            result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'] )
+            result.keys()
+
+
     def test_id_A1( self, getSampleProxyA1 ):
         """Test second level proxy ID"""
         proxy = getSampleProxyA1
         assert proxy.proxy_id() == f"{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_id_A1_id_with_parent_id( self, getSampleProxyA1 ):
```

### Comparing `mongo_objects-1.2.0/tests/test_MongoSingleProxy.py` & `mongo_objects-1.2.1/tests/test_MongoSingleProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -919,64 +919,100 @@
         proxyA = getSampleProxyA
 
         # Loading class B with class A's ID will work and give us class B
         result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['B'] )
         assert isinstance( result, classes['B'] )
 
 
+    def test_load_proxy_by_id_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # loading a proxy with more classes than IDs raises a ValueError
+        with pytest.raises( ValueError ):
+            classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], classes['B'] )
+
+
     def test_load_proxy_by_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'] )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
         # verify the parent is not readonly
         assert result.ultimate_parent.readonly is False
 
 
-    def test_load_proxy_by_id_readonly_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_load_proxy_by_id_A1_readonly( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'], readonly=True )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
         # verify the parent is readonly
         assert result.ultimate_parent.readonly is True
 
 
+    def test_load_proxy_by_id_A1_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # loading a proxy with more IDs than classes raises a ValueError
+        with pytest.raises( ValueError ):
+            classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'] )
+
+
     def test_load_proxy_by_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # reload the proxy by its local ID
         result = proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'] )
 
         # verify the objects are the same
         assert result.data() == proxyA.data()
 
 
+    def test_load_proxy_by_local_id_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # loading a proxy with more classes than IDs raises a ValueError
+        with pytest.raises( ValueError ):
+            proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'], classes['B'] )
+
+
     def test_load_proxy_by_local_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # reload the proxy by its ID
         result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'], classes['A1'] )
 
         # verify the objects are the same
         assert result.data() == proxyA1.data()
 
 
+    def test_load_proxy_by_local_id_A1_list_mismatch( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # loading a proxy with more IDs than classes raises a ValueError
+        with pytest.raises( ValueError ):
+            proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'] )
+
+
     def test_proxy_id( self, getSampleProxyA ):
         """Test single level proxy ID"""
         proxy = getSampleProxyA
         assert proxy.proxy_id() == f"0"
 
 
     def test_proxy_id_with_parent_id( self, getSampleProxyA ):
```

### Comparing `mongo_objects-1.2.0/tests/test_MongoUserDict.py` & `mongo_objects-1.2.1/tests/test_MongoUserDict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1222,17 +1222,17 @@
 
         # split the ID back into components
         assert MMUD.split_id( id ) == a
 
 
     def test_utcnow( self, getMMUDClass ):
         MMUD = getMMUDClass
-        startTime = datetime.datetime.now( datetime.UTC ).replace( tzinfo=None )
+        startTime = datetime.datetime.now( datetime.timezone.utc ).replace( tzinfo=None )
         mongoNow = MMUD.utcnow()
-        endTime = datetime.datetime.now( datetime.UTC ).replace( tzinfo=None )
+        endTime = datetime.datetime.now( datetime.timezone.utc ).replace( tzinfo=None )
 
         # verify that mongoNow has no microseconds
         assert mongoNow.microsecond % 1000 == 0
 
         # disregarding microseconds, verify mongoNow >= startTime
         assert mongoNow.replace(microsecond=0) >= startTime.replace(microsecond=0)
```

### Comparing `mongo_objects-1.2.0/tests/test_PolymorphicMongoDictProxy.py` & `mongo_objects-1.2.1/tests/test_PolymorphicMongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.2.1/tests/test_PolymorphicMongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/tests/test_PolymorphicMongoSingleProxy.py` & `mongo_objects-1.2.1/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/tests/test_PolymorphicMongoUserDict.py` & `mongo_objects-1.2.1/tests/test_PolymorphicMongoUserDict.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/tests/test_proxy_combo.py` & `mongo_objects-1.2.1/tests/test_proxy_combo.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/LICENSE.txt` & `mongo_objects-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/README.rst` & `mongo_objects-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/pyproject.toml` & `mongo_objects-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.2.0/PKG-INFO` & `mongo_objects-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mongo_objects
-Version: 1.2.0
+Version: 1.2.1
 Summary: Access MongoDB documents and subdocuments through user-defined UserDict and proxy objects.
 Project-URL: Homepage, https://github.com/lindstrom-j/mongo_objects
 Project-URL: Documentation, https://mongo-objects.headwaters.com.sg/en/latest/
 Project-URL: Issues, https://github.com/lindstrom-j/mongo_objects/issues
 Author-email: Jonathan Lindstrom <lindstrom.j@headwaters.com.sg>
 License: MIT License
 License-File: LICENSE.txt
```

