# Comparing `tmp/airbyte_source_hubspot-4.1.2.dev202405072234.tar.gz` & `tmp/airbyte_source_hubspot-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_hubspot-4.1.2.dev202405072234.tar", max compression
+gzip compressed data, was "airbyte_source_hubspot-4.1.3.tar", max compression
```

## Comparing `airbyte_source_hubspot-4.1.2.dev202405072234.tar` & `airbyte_source_hubspot-4.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     4524 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/README.md
--rw-r--r--   0        0        0      812 2024-05-07 22:34:48.034933 airbyte_source_hubspot-4.1.2.dev202405072234/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/__init__.py
--rw-r--r--   0        0        0      154 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/constants.py
--rw-r--r--   0        0        0     1885 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/errors.py
--rw-r--r--   0        0        0     3809 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/helpers.py
--rw-r--r--   0        0        0      233 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/run.py
--rw-r--r--   0        0        0     6624 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/campaigns.json
--rw-r--r--   0        0        0      905 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/companies.json
--rw-r--r--   0        0        0     1415 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/companies_property_history.json
--rw-r--r--   0        0        0     6086 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contact_lists.json
--rw-r--r--   0        0        0      933 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts.json
--rw-r--r--   0        0        0     1866 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_form_submissions.json
--rw-r--r--   0        0        0     1008 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_list_memberships.json
--rw-r--r--   0        0        0     6620 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_merged_audit.json
--rw-r--r--   0        0        0     2093 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_property_history.json
--rw-r--r--   0        0        0     3046 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deal_pipelines.json
--rw-r--r--   0        0        0    30732 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deals.json
--rw-r--r--   0        0        0    18631 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deals_archived.json
--rw-r--r--   0        0        0     1276 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deals_property_history.json
--rw-r--r--   0        0        0     9554 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/email_events.json
--rw-r--r--   0        0        0     1670 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/email_subscriptions.json
--rw-r--r--   0        0        0    26695 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements.json
--rw-r--r--   0        0        0    18505 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_calls.json
--rw-r--r--   0        0        0    25799 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_emails.json
--rw-r--r--   0        0        0    17798 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_meetings.json
--rw-r--r--   0        0        0    11074 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_notes.json
--rw-r--r--   0        0        0    20314 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_tasks.json
--rw-r--r--   0        0        0     5736 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/feedback_submissions.json
--rw-r--r--   0        0        0     1332 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/form_submissions.json
--rw-r--r--   0        0        0     8454 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/forms.json
--rw-r--r--   0        0        0     3717 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/goals.json
--rw-r--r--   0        0        0      692 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/line_items.json
--rw-r--r--   0        0        0    24533 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/marketing_emails.json
--rw-r--r--   0        0        0     1763 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/owners.json
--rw-r--r--   0        0        0     1733 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/owners_archived.json
--rw-r--r--   0        0        0      676 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/products.json
--rw-r--r--   0        0        0     3742 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/shared/default_event_properties.json
--rw-r--r--   0        0        0     2414 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/subscription_changes.json
--rw-r--r--   0        0        0     2976 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/ticket_pipelines.json
--rw-r--r--   0        0        0     1304 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/tickets.json
--rw-r--r--   0        0        0     7534 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/workflows.json
--rw-r--r--   0        0        0     9781 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/source.py
--rw-r--r--   0        0        0     4559 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/spec.yaml
--rw-r--r--   0        0        0    96932 2024-05-07 21:54:43.000000 airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/streams.py
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.1.2.dev202405072234/PKG-INFO
+-rw-r--r--   0        0        0     4524 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/README.md
+-rw-r--r--   0        0        0      796 2024-05-13 12:51:35.950412 airbyte_source_hubspot-4.1.3/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/__init__.py
+-rw-r--r--   0        0        0      154 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/constants.py
+-rw-r--r--   0        0        0     1885 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/errors.py
+-rw-r--r--   0        0        0     3809 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/helpers.py
+-rw-r--r--   0        0        0      233 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/run.py
+-rw-r--r--   0        0        0     6624 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/campaigns.json
+-rw-r--r--   0        0        0      905 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/companies.json
+-rw-r--r--   0        0        0     1415 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/companies_property_history.json
+-rw-r--r--   0        0        0     6086 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contact_lists.json
+-rw-r--r--   0        0        0      933 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts.json
+-rw-r--r--   0        0        0     1866 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_form_submissions.json
+-rw-r--r--   0        0        0     1008 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_list_memberships.json
+-rw-r--r--   0        0        0     6620 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_merged_audit.json
+-rw-r--r--   0        0        0     2093 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_property_history.json
+-rw-r--r--   0        0        0     3046 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deal_pipelines.json
+-rw-r--r--   0        0        0    30732 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deals.json
+-rw-r--r--   0        0        0    18631 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deals_archived.json
+-rw-r--r--   0        0        0     1276 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deals_property_history.json
+-rw-r--r--   0        0        0     9554 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/email_events.json
+-rw-r--r--   0        0        0     1670 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/email_subscriptions.json
+-rw-r--r--   0        0        0    26695 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements.json
+-rw-r--r--   0        0        0    18505 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_calls.json
+-rw-r--r--   0        0        0    25799 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_emails.json
+-rw-r--r--   0        0        0    17798 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_meetings.json
+-rw-r--r--   0        0        0    11074 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_notes.json
+-rw-r--r--   0        0        0    20314 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_tasks.json
+-rw-r--r--   0        0        0     5736 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/feedback_submissions.json
+-rw-r--r--   0        0        0     1332 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/form_submissions.json
+-rw-r--r--   0        0        0     8454 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/forms.json
+-rw-r--r--   0        0        0     3717 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/goals.json
+-rw-r--r--   0        0        0      692 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/line_items.json
+-rw-r--r--   0        0        0    24533 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/marketing_emails.json
+-rw-r--r--   0        0        0     1763 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/owners.json
+-rw-r--r--   0        0        0     1733 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/owners_archived.json
+-rw-r--r--   0        0        0      676 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/products.json
+-rw-r--r--   0        0        0     3742 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/shared/default_event_properties.json
+-rw-r--r--   0        0        0     2414 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/subscription_changes.json
+-rw-r--r--   0        0        0     2976 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/ticket_pipelines.json
+-rw-r--r--   0        0        0     1304 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/tickets.json
+-rw-r--r--   0        0        0     7534 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/schemas/workflows.json
+-rw-r--r--   0        0        0     9781 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/source.py
+-rw-r--r--   0        0        0     4559 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/spec.yaml
+-rw-r--r--   0        0        0    96762 2024-05-13 12:22:26.000000 airbyte_source_hubspot-4.1.3/source_hubspot/streams.py
+-rw-r--r--   0        0        0     5228 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.1.3/PKG-INFO
```

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/README.md` & `airbyte_source_hubspot-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/pyproject.toml` & `airbyte_source_hubspot-4.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.1.2.dev202405072234"
+version = "4.1.3"
 name = "airbyte-source-hubspot"
 description = "Source implementation for HubSpot."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/errors.py` & `airbyte_source_hubspot-4.1.3/source_hubspot/errors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/helpers.py` & `airbyte_source_hubspot-4.1.3/source_hubspot/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/campaigns.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/companies.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/companies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/companies_property_history.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/companies_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contact_lists.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contact_lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_form_submissions.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_form_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_list_memberships.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_list_memberships.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_merged_audit.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_merged_audit.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/contacts_property_history.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/contacts_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deal_pipelines.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deal_pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deals.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deals_archived.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deals_archived.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/deals_property_history.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/deals_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/email_events.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/email_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/email_subscriptions.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/email_subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_calls.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_calls.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_emails.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_emails.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_meetings.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_meetings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_notes.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/engagements_tasks.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/engagements_tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/feedback_submissions.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/feedback_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/form_submissions.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/form_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/forms.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/goals.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/goals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/line_items.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/marketing_emails.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/marketing_emails.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/owners.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/owners.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/owners_archived.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/owners_archived.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/products.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/shared/default_event_properties.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/shared/default_event_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/subscription_changes.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/subscription_changes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/ticket_pipelines.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/ticket_pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/tickets.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/schemas/workflows.json` & `airbyte_source_hubspot-4.1.3/source_hubspot/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/source.py` & `airbyte_source_hubspot-4.1.3/source_hubspot/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/spec.yaml` & `airbyte_source_hubspot-4.1.3/source_hubspot/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/source_hubspot/streams.py` & `airbyte_source_hubspot-4.1.3/source_hubspot/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import backoff
 import pendulum as pendulum
 import requests
 from airbyte_cdk.entrypoint import logger
 from airbyte_cdk.models import FailureType, SyncMode
 from airbyte_cdk.sources import Source
-from airbyte_cdk.sources.streams import CheckpointMixin, Stream
+from airbyte_cdk.sources.streams import IncrementalMixin, Stream
 from airbyte_cdk.sources.streams.availability_strategy import AvailabilityStrategy
 from airbyte_cdk.sources.streams.core import StreamData
 from airbyte_cdk.sources.streams.http import HttpStream, HttpSubStream
 from airbyte_cdk.sources.streams.http.availability_strategy import HttpAvailabilityStrategy
 from airbyte_cdk.sources.streams.http.requests_native_auth import Oauth2Authenticator, TokenAuthenticator
 from airbyte_cdk.sources.utils import casing
 from airbyte_cdk.sources.utils.schema_helpers import ResourceSchemaLoader
@@ -834,15 +834,15 @@
             yield record
 
     @property
     def availability_strategy(self) -> Optional[AvailabilityStrategy]:
         return HubspotAvailabilityStrategy()
 
 
-class ClientSideIncrementalStream(Stream, CheckpointMixin):
+class ClientSideIncrementalStream(Stream, IncrementalMixin):
     _cursor_value = ""
 
     @property
     def cursor_field(self) -> Union[str, List[str]]:
         return self.updated_at_field
 
     @property
@@ -857,18 +857,15 @@
 
     @property
     def state(self) -> Mapping[str, Any]:
         return {self.cursor_field: self._cursor_value}
 
     @state.setter
     def state(self, value: Mapping[str, Any]):
-        if value:
-            self._cursor_value = value[self.cursor_field]
-        else:
-            self._cursor_value = ""
+        self._cursor_value = value[self.cursor_field]
 
     def filter_by_state(self, stream_state: Mapping[str, Any] = None, record: Mapping[str, Any] = None) -> bool:
         """
         Filter out old records that come from source in unsorted order.
         Hubspot API uses 2 date-time formats for different endpoints:
         1. "YYYY-MM-DDTHH:mm:ss.SSSSSSZ" - date-time in ISO format
         2. "x" - date-time in timestamp in milliseconds
@@ -890,15 +887,15 @@
             )
         # compare the state with record values and get the max value between of two
         cursor_value = max(state_value, record_value)
         max_state = max(str(self.state.get(self.cursor_field)), cursor_value.format(self.cursor_field_datetime_format))
         # save the state
         self.state = {self.cursor_field: int(max_state) if int_field_type else max_state}
         # emmit record if it has bigger cursor value compare to the state (`True` only)
-        return record_value > state_value
+        return record_value >= state_value
 
     def read_records(
         self,
         sync_mode: SyncMode,
         cursor_field: List[str] = None,
         stream_slice: Mapping[str, Any] = None,
         stream_state: Mapping[str, Any] = None,
@@ -1231,15 +1228,15 @@
 
             return {"params": params, "payload": payload}
 
     def stream_slices(
         self, *, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Mapping[str, Any] = None
     ) -> Iterable[Optional[Mapping[str, Any]]]:
         self.set_sync(sync_mode, stream_state)
-        return [{}]  # I changed this from [None] since this is a more accurate depiction of what is actually being done. Sync one slice
+        return [None]
 
     def set_sync(self, sync_mode: SyncMode, stream_state):
         self._sync_mode = sync_mode
         if self._sync_mode == SyncMode.incremental:
             if stream_state:
                 if not self._state:
                     self._state = self._start_date
@@ -1360,83 +1357,28 @@
     limit_field = "count"
     primary_key = "listId"
     need_chunk = False
     scopes = {"crm.lists.read"}
     unnest_fields = ["metaData"]
 
 
-class ContactsAllBase(Stream, CheckpointMixin):
+class ContactsAllBase(Stream):
     url = "/contacts/v1/lists/all/contacts/all"
     updated_at_field = "timestamp"
     more_key = "has-more"
     data_field = "contacts"
     page_filter = "vidOffset"
     page_field = "vid-offset"
     primary_key = "canonical-vid"
+    limit_field = "count"
     scopes = {"crm.objects.contacts.read"}
     properties_scopes = {"crm.schemas.contacts.read"}
     records_field = None
     filter_field = None
     filter_value = None
-    _state = {}
-    limit_field = "count"
-    limit = 100
-
-    @property
-    def state(self) -> MutableMapping[str, Any]:
-        return self._state
-
-    @state.setter
-    def state(self, value: MutableMapping[str, Any]) -> None:
-        self._state = value
-
-    def read_records(
-        self,
-        sync_mode: SyncMode,
-        cursor_field: List[str] = None,
-        stream_slice: Mapping[str, Any] = None,
-        stream_state: Mapping[str, Any] = None,
-    ) -> Iterable[Mapping[str, Any]]:
-        """
-        This is a specialized read_records for resumable full refresh that only attempts to read a single page of records
-        at a time and updates the state w/ a synthetic cursor based on the Hubspot cursor pagination value `vidOffset`
-        """
-
-        next_page_token = stream_slice
-        try:
-            properties = self._property_wrapper
-            if properties and properties.too_many_properties:
-                records, response = self._read_stream_records(
-                    stream_slice=stream_slice,
-                    stream_state=stream_state,
-                    next_page_token=next_page_token,
-                )
-            else:
-                response = self.handle_request(
-                    stream_slice=stream_slice,
-                    stream_state=stream_state,
-                    next_page_token=next_page_token,
-                    properties=properties,
-                )
-                records = self._transform(self.parse_response(response, stream_state=stream_state, stream_slice=stream_slice))
-
-            if self.filter_old_records:
-                records = self._filter_old_records(records)
-            yield from self.record_unnester.unnest(records)
-
-            self.state = self.next_page_token(response) or {}
-
-            # Always return an empty generator just in case no records were ever yielded
-            yield from []
-        except requests.exceptions.HTTPError as e:
-            response = e.response
-            if response.status_code == HTTPStatus.UNAUTHORIZED:
-                raise AirbyteTracedException("The authentication to HubSpot has expired. Re-authenticate to restore access to HubSpot.")
-            else:
-                raise e
 
     def _transform(self, records: Iterable) -> Iterable:
         for record in super()._transform(records):
             canonical_vid = record.get("canonical-vid")
             for item in record.get(self.records_field, []):
                 yield {"canonical-vid": canonical_vid, **item}
 
@@ -1448,42 +1390,46 @@
     ) -> MutableMapping[str, Any]:
         params = super().request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
         if self.filter_field and self.filter_value:
             params.update({self.filter_field: self.filter_value})
         return params
 
 
-class ContactsListMemberships(ContactsAllBase, ABC):
+class ContactsListMemberships(ContactsAllBase, ClientSideIncrementalStream):
     """Contacts list Memberships, API v1
     The Stream was created due to issue #8477, where supporting List Memberships in Contacts stream was requested.
     According to the issue this feature is supported in API v1 by setting parameter showListMemberships=true
     in get all contacts endpoint. API will return list memberships for each contact record.
     But for syncing Contacts API v3 is used, where list memberships for contacts isn't supported.
     Therefore, new stream was created based on get all contacts endpoint of API V1.
     Docs: https://legacydocs.hubspot.com/docs/methods/contacts/get_contacts
     """
 
     records_field = "list-memberships"
     filter_field = "showListMemberships"
     filter_value = True
 
+    @property
+    def updated_at_field(self) -> str:
+        """Name of the field associated with the state"""
+        return "timestamp"
+
+    @property
+    def cursor_field_datetime_format(self) -> str:
+        """Cursor value expected to be a timestamp in milliseconds"""
+        return "x"
+
 
 class ContactsFormSubmissions(ContactsAllBase, ABC):
 
     records_field = "form-submissions"
     filter_field = "formSubmissionMode"
     filter_value = "all"
 
 
-class ContactsMergedAudit(ContactsAllBase, ABC):
-
-    records_field = "merge-audits"
-    unnest_fields = ["merged_from_email", "merged_to_email"]
-
-
 class Deals(CRMSearchStream):
     """Deals, API v3"""
 
     entity = "deal"
     last_modified_field = "hs_lastmodifieddate"
     associations = ["contacts", "companies", "line_items"]
     primary_key = "id"
@@ -2162,14 +2108,73 @@
     entity = "contact"
     last_modified_field = "lastmodifieddate"
     associations = ["contacts", "companies"]
     primary_key = "id"
     scopes = {"crm.objects.contacts.read"}
 
 
+class ContactsMergedAudit(Stream):
+    url = "/contacts/v1/contact/vids/batch/"
+    updated_at_field = "timestamp"
+    scopes = {"crm.objects.contacts.read"}
+    unnest_fields = ["merged_from_email", "merged_to_email"]
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.config = kwargs
+
+    def stream_slices(
+        self, sync_mode: SyncMode, cursor_field: List[str] = None, stream_state: Mapping[str, Any] = None, **kwargs
+    ) -> Iterable[Mapping[str, Any]]:
+        slices = []
+
+        # we can query a max of 100 contacts at a time
+        max_contacts = 100
+        slices = []
+        contact_batch = []
+
+        contacts = Contacts(**self.config)
+        contacts._sync_mode = SyncMode.full_refresh
+        contacts.filter_old_records = False
+
+        for contact in contacts.read_records(sync_mode=SyncMode.full_refresh):
+            if contact.get("properties_hs_merged_object_ids"):
+                contact_batch.append(contact["id"])
+
+                if len(contact_batch) == max_contacts:
+                    slices.append({"vid": contact_batch})
+                    contact_batch = []
+
+        if contact_batch:
+            slices.append({"vid": contact_batch})
+
+        return slices
+
+    def request_params(
+        self, stream_state: Mapping[str, Any], stream_slice: Mapping[str, Any] = None, next_page_token: Mapping[str, Any] = None
+    ) -> MutableMapping[str, Any]:
+        return {"vid": stream_slice["vid"]}
+
+    def parse_response(
+        self,
+        response: requests.Response,
+        *,
+        stream_state: Mapping[str, Any],
+        stream_slice: Mapping[str, Any] = None,
+        next_page_token: Mapping[str, Any] = None,
+    ) -> Iterable[Mapping]:
+        response = self._parse_response(response)
+        if response.get("status", None) == "error":
+            self.logger.warning(f"Stream `{self.name}` cannot be procced. {response.get('message')}")
+            return
+
+        for contact_id in list(response.keys()):
+            yield from response[contact_id]["merge-audits"]
+
+
 class EngagementsCalls(CRMSearchStream):
     entity = "calls"
     last_modified_field = "hs_lastmodifieddate"
     associations = ["contacts", "deal", "company", "tickets"]
     primary_key = "id"
     scopes = {"crm.objects.contacts.read"}
 
@@ -2275,15 +2280,15 @@
     url = "/email/public/v1/subscriptions"
     data_field = "subscriptionDefinitions"
     primary_key = "id"
     scopes = {"content"}
     filter_old_records = False
 
 
-class WebAnalyticsStream(CheckpointMixin, HttpSubStream, Stream):
+class WebAnalyticsStream(IncrementalMixin, HttpSubStream, Stream):
     """
     A base class for Web Analytics API
     Docs: https://developers.hubspot.com/docs/api/events/web-analytics
     """
 
     transformer: TypeTransformer = TypeTransformer(TransformConfig.DefaultSchemaNormalization)
```

### Comparing `airbyte_source_hubspot-4.1.2.dev202405072234/PKG-INFO` & `airbyte_source_hubspot-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-hubspot
-Version: 4.1.2.dev202405072234
+Version: 4.1.3
 Summary: Source implementation for HubSpot.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

