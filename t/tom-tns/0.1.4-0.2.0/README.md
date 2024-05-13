# Comparing `tmp/tom_tns-0.1.4.tar.gz` & `tmp/tom_tns-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_tns-0.1.4.tar", max compression
+gzip compressed data, was "tom_tns-0.2.0.tar", max compression
```

## Comparing `tom_tns-0.1.4.tar` & `tom_tns-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    35149 2024-03-19 23:51:57.094857 tom_tns-0.1.4/LICENSE
--rw-r--r--   0        0        0     1845 2024-03-19 23:51:57.098857 tom_tns-0.1.4/README.md
--rw-r--r--   0        0        0     1234 2024-03-19 23:52:15.690953 tom_tns-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       99 2024-03-19 23:52:15.690953 tom_tns-0.1.4/tom_tns/__init__.py
--rw-r--r--   0        0        0       65 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/admin.py
--rw-r--r--   0        0        0      518 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/apps.py
--rw-r--r--   0        0        0    12528 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/forms.py
--rw-r--r--   0        0        0        0 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/migrations/__init__.py
--rw-r--r--   0        0        0       59 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/models.py
--rw-r--r--   0        0        0       89 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/templates/tom_tns/partials/tns_button.html
--rw-r--r--   0        0        0      190 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/templates/tom_tns/partials/tns_classify_form.html
--rw-r--r--   0        0        0      158 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/templates/tom_tns/partials/tns_report_form.html
--rw-r--r--   0        0        0     3067 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/templates/tom_tns/tns_report.html
--rw-r--r--   0        0        0        0 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/templatetags/__init__.py
--rw-r--r--   0        0        0     2978 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/templatetags/tns_extras.py
--rw-r--r--   0        0        0       62 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/tests.py
--rw-r--r--   0        0        0    10203 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/tns_api.py
--rw-r--r--   0        0        0      452 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/urls.py
--rw-r--r--   0        0        0     3225 2024-03-19 23:51:57.098857 tom_tns-0.1.4/tom_tns/views.py
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 tom_tns-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-13 21:58:48.174178 tom_tns-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5256 2024-05-13 21:58:48.178178 tom_tns-0.2.0/README.md
+-rw-r--r--   0        0        0     1234 2024-05-13 21:59:01.606088 tom_tns-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       99 2024-05-13 21:59:01.610088 tom_tns-0.2.0/tom_tns/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/admin.py
+-rw-r--r--   0        0        0      518 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/apps.py
+-rw-r--r--   0        0        0    25952 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/forms.py
+-rw-r--r--   0        0        0     2517 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/hermes_api.py
+-rw-r--r--   0        0        0        0 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/migrations/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/models.py
+-rw-r--r--   0        0        0       89 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/templates/tom_tns/partials/tns_button.html
+-rw-r--r--   0        0        0      190 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/templates/tom_tns/partials/tns_classify_form.html
+-rw-r--r--   0        0        0      158 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/templates/tom_tns/partials/tns_report_form.html
+-rw-r--r--   0        0        0     3067 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/templates/tom_tns/tns_report.html
+-rw-r--r--   0        0        0        0 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/templatetags/__init__.py
+-rw-r--r--   0        0        0     4511 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/templatetags/tns_extras.py
+-rw-r--r--   0        0        0       62 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/tests.py
+-rw-r--r--   0        0        0    11275 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/tns_api.py
+-rw-r--r--   0        0        0      531 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/urls.py
+-rw-r--r--   0        0        0     4821 2024-05-13 21:58:48.178178 tom_tns-0.2.0/tom_tns/views.py
+-rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 tom_tns-0.2.0/PKG-INFO
```

### Comparing `tom_tns-0.1.4/LICENSE` & `tom_tns-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_tns-0.1.4/pyproject.toml` & `tom_tns-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tom-tns"
-version = "0.1.4"
+version = "0.2.0"
 description = "TOMtoolkit module for reporting transients to the TNS"
 authors = ["Joseph Chatelain <jchatelain@lco.global>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "tom_tns"}]
 
 [tool.poetry.dependencies]
```

### Comparing `tom_tns-0.1.4/tom_tns/apps.py` & `tom_tns-0.2.0/tom_tns/apps.py`

 * *Files identical despite different names*

### Comparing `tom_tns-0.1.4/tom_tns/templates/tom_tns/tns_report.html` & `tom_tns-0.2.0/tom_tns/templates/tom_tns/tns_report.html`

 * *Files identical despite different names*

### Comparing `tom_tns-0.1.4/tom_tns/templatetags/tns_extras.py` & `tom_tns-0.2.0/tom_tns/templatetags/tns_extras.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django import template
 from django.conf import settings
 
-from tom_tns.tns_api import get_tns_values
+from tom_tns.tns_api import get_tns_values, map_filter_to_tns, default_authors
 from tom_tns.forms import TNSReportForm, TNSClassifyForm
 
 register = template.Library()
 
 
 # Define form Choices from Cached TNS Values
 TNS_FILTER_IDS = {name: fid for fid, name in get_tns_values('filters')}
@@ -17,29 +17,42 @@
 def report_to_tns(context):
     """
     Build context data for TNS AT Report Form.
     Includes the latest Photometry data if available.
     """
     target = context['target']
     initial = {
+        'object_name': target.name,
         'ra': target.ra,
         'dec': target.dec,
+        'submitter': context['request'].user.email,
         'reporter': f"{getattr(context['request'].user, 'get_full_name()', 'Anonymous User')},"
                     f" using {settings.TOM_NAME}",
     }
-    # Get photometry if available
-    photometry = target.reduceddatum_set.filter(data_type='photometry')
-    if photometry.exists():
-        reduced_datum = photometry.latest()
+
+    reporter = default_authors()
+    if reporter:
+        initial['reporter'] = reporter
+
+    reduced_datum = None
+    if 'datum' in context:
+        reduced_datum = context['datum']
+    else:
+        # Get photometry if available
+        photometry = target.reduceddatum_set.filter(data_type='photometry')
+        if photometry.exists():
+            reduced_datum = photometry.latest()
+    if reduced_datum:
         initial['observation_date'] = reduced_datum.timestamp
         initial['flux'] = reduced_datum.value.get('magnitude')
         initial['flux_error'] = reduced_datum.value.get('error')
         filter_name = reduced_datum.value.get('filter')
-        if filter_name in TNS_FILTER_IDS:
-            initial['filter'] = (TNS_FILTER_IDS[filter_name], filter_name)
+        mapped_filter = map_filter_to_tns(filter_name)
+        if mapped_filter in TNS_FILTER_IDS:
+            initial['filter'] = (TNS_FILTER_IDS[mapped_filter], mapped_filter)
         instrument_name = reduced_datum.value.get('instrument')
         if instrument_name in TNS_INSTRUMENT_IDS:
             initial['instrument'] = (TNS_INSTRUMENT_IDS[instrument_name], instrument_name)
     tns_report_form = TNSReportForm(initial=initial)
     return {'target': target,
             'form': tns_report_form}
 
@@ -49,22 +62,48 @@
     """
     Build context data for TNS Classification Form.
     Includes the latest Spectroscopy data if available.
     """
     target = context['target']
     initial = {
         'object_name': target.name.replace('AT', '').replace('SN', ''),
+        'ra': target.ra,
+        'dec': target.dec,
+        'submitter': context['request'].user.email,
         'classifier': f"{getattr(context['request'].user, 'get_full_name()', 'Anonymous User')},"
                       f" using {settings.TOM_NAME}",
     }
-    # Get spectroscopy if available
-    spectra = target.reduceddatum_set.filter(data_type='spectroscopy')
-    if spectra.exists():
-        reduced_datum = spectra.latest()
+
+    classifier = default_authors()
+    if classifier:
+        initial['classifier'] = classifier
+
+    # Get the list of chocies for ascii and fits files for those fields
+    ascii_files = []
+    fits_files = [(None, '')]
+    for data_product in target.dataproduct_set.all():
+        if data_product.get_file_extension().lower() in ['.ascii', '.txt']:
+            ascii_files.append((data_product.pk, data_product.get_file_name()))
+        elif data_product.get_file_extension().lower() in ['.fits', '.fits.fz']:
+            fits_files.append((data_product.pk, data_product.get_file_name()))
+    initial['ascii_file_choices'] = ascii_files
+    initial['fits_file_choices'] = fits_files
+
+    # Get the spectra details from the latest spectra reduced datum or one passed in
+    reduced_datum = None
+    if 'datum' in context:
+        reduced_datum = context['datum']
+    else:
+        spectra = target.reduceddatum_set.filter(data_type='spectroscopy')
+        if spectra.exists():
+            reduced_datum = spectra.latest()
+    if reduced_datum:
         initial['observation_date'] = reduced_datum.timestamp
-        initial['ascii_file'] = reduced_datum.data_product.data
+        if reduced_datum.data_product.get_file_extension().lower() in ['.ascii', '.txt']:
+            initial['ascii_file'] = (reduced_datum.data_product.pk, reduced_datum.data_product.get_file_name())
         instrument_name = reduced_datum.value.get('instrument')
         if instrument_name in TNS_INSTRUMENT_IDS:
             initial['instrument'] = (TNS_INSTRUMENT_IDS[instrument_name], instrument_name)
+
     tns_classify_form = TNSClassifyForm(initial=initial)
     return {'target': target,
             'form': tns_classify_form}
```

### Comparing `tom_tns-0.1.4/tom_tns/tns_api.py` & `tom_tns-0.2.0/tom_tns/tns_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,41 @@
 
 
 class BadTnsRequest(Exception):
     """ This Exception will be raised by errors during the TNS submission process """
     pass
 
 
+def submit_through_hermes():
+    """ Check if hermes credentials exist and are setup so TNS messages should be sent through hermes
+        Returns True if it should go through hermes, False if it should go directly to TNS
+    """
+    if hasattr(settings, 'DATA_SHARING') and settings.DATA_SHARING.get('hermes', {}).get('ENABLE_TNS', False):
+        return True
+    return False
+
+
+def map_filter_to_tns(filter):
+    """ Checks if a filter mapping was set in the settings, and if so returns the mapped value for the filter passed in
+    """
+    if submit_through_hermes():
+        return settings.DATA_SHARING.get('hermes', {}).get('FILTER_MAPPING', {}).get(filter)
+    else:
+        return settings.BROKERS.get('TNS', {}).get('filter_mapping', {}).get(filter)
+
+
+def default_authors():
+    """ Returns default authors if set in the settings, otherwise empty string.
+    """
+    if submit_through_hermes():
+        return settings.DATA_SHARING.get('hermes', {}).get('DEFAULT_AUTHORS', '')
+    else:
+        return settings.BROKERS.get('TNS', {}).get('default_authors', '')
+
+
 def get_tns_credentials():
     """
     Get the TNS credentials from settings.py.
     This should include the bot_id, bot_name, api_key, tns_base_url, and possibly group_name.
     """
     try:
         tns_info = settings.BROKERS['TNS']
```

### Comparing `tom_tns-0.1.4/tom_tns/views.py` & `tom_tns-0.2.0/tom_tns/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,75 +4,106 @@
 from django.views.generic.edit import FormView
 from django.views.generic.base import TemplateView
 from django.http import HttpResponseRedirect
 from django.contrib import messages
 from guardian.mixins import PermissionListMixin
 
 from tom_tns import __version__
-from tom_tns.tns_api import send_tns_report, get_tns_report_reply, get_tns_credentials, BadTnsRequest
+from tom_tns.tns_api import (send_tns_report, get_tns_report_reply, get_tns_credentials,
+                             submit_through_hermes, BadTnsRequest)
+from tom_tns.hermes_api import submit_to_hermes
 from tom_targets.models import Target, TargetName
+from tom_dataproducts.models import ReducedDatum
 
 import json
 
 
 class TNSFormView(PermissionListMixin, TemplateView):
     """
     This view is used to display the TNS report forms.
     The default form is the report form, but if the target name starts with AT, we switch to the classification form.
     """
     template_name = 'tom_tns/tns_report.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
+        context['default_form'] = 'report'
         target = Target.objects.get(pk=self.kwargs['pk'])
+        if 'datum_pk' in self.kwargs:
+            try:
+                context['datum'] = ReducedDatum.objects.get(pk=self.kwargs['datum_pk'])
+                if context['datum'].data_type == 'spectroscopy':
+                    context['default_form'] = 'classify'
+            except ReducedDatum.DoesNotExist:
+                pass
         context['tns_configured'] = bool(get_tns_credentials())
         context['target'] = target
         context['version'] = __version__  # from tom_tns.__init__.py
         # We want to establish a default tab to display.
         # by default, we start on report, but change to classify if the target name starts with AT.
         # If the target has an SN name, we warn the user that the target has likely been classified already.
-        context['default_form'] = 'report'
         for name in target.names:
             if name.upper().startswith('AT'):
                 context['default_form'] = 'classify'
             if name.upper().startswith('SN'):
                 context['default_form'] = 'supernova'
                 break
         return context
 
 
 class TNSSubmitView(FormView):
     """
     This View is used to submit the TNS report forms.
     """
+    def get_initial(self):
+        # Must override get_initial to pass in the file choice options or it will fail validation
+        initial = super().get_initial()
+        target = Target.objects.get(pk=self.kwargs['pk'])
+        ascii_files = []
+        fits_files = [(None, '')]
+        for data_product in target.dataproduct_set.all():
+            if data_product.get_file_extension().lower() in ['.ascii', '.txt']:
+                ascii_files.append((data_product.pk, data_product.get_file_name()))
+            elif data_product.get_file_extension().lower() in ['.fits', '.fits.fz']:
+                fits_files.append((data_product.pk, data_product.get_file_name()))
+        initial['ascii_file_choices'] = ascii_files
+        initial['fits_file_choices'] = fits_files
+        return initial
 
     def get_success_url(self):
         return reverse_lazy('targets:detail', kwargs=self.kwargs)
 
     def form_invalid(self, form):
         messages.error(self.request, 'The following error was encountered when submitting to the TNS: '
                                      f'{form.errors.as_json()}')
         return HttpResponseRedirect(self.get_success_url())
 
     def form_valid(self, form):
         """
         If the Form is successfully constructed, we generate the TNS report and submit it to the TNS.
         """
         try:
-            # Build TNS Report
-            tns_report = form.generate_tns_report()
-            # Submit TNS Report
-            report_id = send_tns_report(json.dumps(tns_report))
-            # Get IAU name from Report Reply
-            iau_name = get_tns_report_reply(report_id, self.request)
-            if iau_name is not None:
+            iau_name = None
+            if submit_through_hermes():
+                hermes_report, files = form.generate_hermes_report()
+                iau_name = submit_to_hermes(hermes_report, files, self.request)
+            else:
+                # Build TNS Report
+                tns_report = form.generate_tns_report()
+                # Submit TNS Report
+                report_id = send_tns_report(json.dumps(tns_report))
+                # Get IAU name from Report Reply
+                iau_name = get_tns_report_reply(report_id, self.request)
+
+            if iau_name:
                 # update the target name in Tom DB
                 target = Target.objects.get(pk=self.kwargs['pk'])
-                old_name = target.name
-                target.name = iau_name
-                target.save()
-                # Save old name as alias
-                new_alias = TargetName(name=old_name, target=target)
-                new_alias.save()
+                if target.name != iau_name:
+                    old_name = target.name
+                    target.name = iau_name
+                    target.save()
+                    # Save old name as alias
+                    new_alias = TargetName(name=old_name, target=target)
+                    new_alias.save()
         except (requests.exceptions.HTTPError, BadTnsRequest) as e:
             messages.error(self.request, f'TNS returned an error: {e}')
         return HttpResponseRedirect(self.get_success_url())
```

