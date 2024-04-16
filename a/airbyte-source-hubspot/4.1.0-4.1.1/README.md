# Comparing `tmp/airbyte_source_hubspot-4.1.0.tar.gz` & `tmp/airbyte_source_hubspot-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_hubspot-4.1.0.tar", max compression
+gzip compressed data, was "airbyte_source_hubspot-4.1.1.tar", max compression
```

## Comparing `airbyte_source_hubspot-4.1.0.tar` & `airbyte_source_hubspot-4.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     4514 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/README.md
--rw-r--r--   0        0        0      760 2024-04-08 14:43:31.106148 airbyte_source_hubspot-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      124 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/__init__.py
--rw-r--r--   0        0        0      154 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/constants.py
--rw-r--r--   0        0        0     1885 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/errors.py
--rw-r--r--   0        0        0     3809 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/helpers.py
--rw-r--r--   0        0        0      233 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/run.py
--rw-r--r--   0        0        0     3343 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/campaigns.json
--rw-r--r--   0        0        0      506 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/companies.json
--rw-r--r--   0        0        0      693 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/companies_property_history.json
--rw-r--r--   0        0        0     3054 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contact_lists.json
--rw-r--r--   0        0        0      517 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts.json
--rw-r--r--   0        0        0      908 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_form_submissions.json
--rw-r--r--   0        0        0      471 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_list_memberships.json
--rw-r--r--   0        0        0     3293 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_merged_audit.json
--rw-r--r--   0        0        0      986 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_property_history.json
--rw-r--r--   0        0        0     1553 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deal_pipelines.json
--rw-r--r--   0        0        0    18485 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deals.json
--rw-r--r--   0        0        0    18562 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deals_archived.json
--rw-r--r--   0        0        0      690 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deals_property_history.json
--rw-r--r--   0        0        0     4792 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/email_events.json
--rw-r--r--   0        0        0      784 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/email_subscriptions.json
--rw-r--r--   0        0        0    18307 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements.json
--rw-r--r--   0        0        0    10057 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_calls.json
--rw-r--r--   0        0        0    14599 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_emails.json
--rw-r--r--   0        0        0     9913 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_meetings.json
--rw-r--r--   0        0        0     6592 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_notes.json
--rw-r--r--   0        0        0    11391 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_tasks.json
--rw-r--r--   0        0        0     3087 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/feedback_submissions.json
--rw-r--r--   0        0        0      710 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/form_submissions.json
--rw-r--r--   0        0        0     5053 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/forms.json
--rw-r--r--   0        0        0     2217 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/goals.json
--rw-r--r--   0        0        0      398 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/line_items.json
--rw-r--r--   0        0        0    18730 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/marketing_emails.json
--rw-r--r--   0        0        0      986 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/owners.json
--rw-r--r--   0        0        0      986 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/owners_archived.json
--rw-r--r--   0        0        0      398 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/products.json
--rw-r--r--   0        0        0     3742 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/shared/default_event_properties.json
--rw-r--r--   0        0        0     1264 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/subscription_changes.json
--rw-r--r--   0        0        0     1647 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/ticket_pipelines.json
--rw-r--r--   0        0        0      751 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/tickets.json
--rw-r--r--   0        0        0     3905 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/schemas/workflows.json
--rw-r--r--   0        0        0     9768 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/source.py
--rw-r--r--   0        0        0     4559 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/spec.yaml
--rw-r--r--   0        0        0    96413 2024-04-08 10:52:10.000000 airbyte_source_hubspot-4.1.0/source_hubspot/streams.py
--rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4514 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/README.md
+-rw-r--r--   0        0        0      796 2024-04-16 18:10:05.724397 airbyte_source_hubspot-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/constants.py
+-rw-r--r--   0        0        0     1885 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/errors.py
+-rw-r--r--   0        0        0     3809 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/helpers.py
+-rw-r--r--   0        0        0      233 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/run.py
+-rw-r--r--   0        0        0     3343 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/campaigns.json
+-rw-r--r--   0        0        0      506 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/companies.json
+-rw-r--r--   0        0        0      693 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/companies_property_history.json
+-rw-r--r--   0        0        0     3054 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contact_lists.json
+-rw-r--r--   0        0        0      517 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts.json
+-rw-r--r--   0        0        0      908 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_form_submissions.json
+-rw-r--r--   0        0        0      471 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_list_memberships.json
+-rw-r--r--   0        0        0     3293 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_merged_audit.json
+-rw-r--r--   0        0        0      986 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_property_history.json
+-rw-r--r--   0        0        0     1553 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deal_pipelines.json
+-rw-r--r--   0        0        0    18485 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deals.json
+-rw-r--r--   0        0        0    18562 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deals_archived.json
+-rw-r--r--   0        0        0      690 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deals_property_history.json
+-rw-r--r--   0        0        0     4792 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/email_events.json
+-rw-r--r--   0        0        0      784 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/email_subscriptions.json
+-rw-r--r--   0        0        0    18307 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements.json
+-rw-r--r--   0        0        0    10057 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_calls.json
+-rw-r--r--   0        0        0    14599 2024-04-16 18:06:19.356625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_emails.json
+-rw-r--r--   0        0        0     9913 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_meetings.json
+-rw-r--r--   0        0        0     6592 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_notes.json
+-rw-r--r--   0        0        0    11391 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_tasks.json
+-rw-r--r--   0        0        0     3087 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/feedback_submissions.json
+-rw-r--r--   0        0        0      710 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/form_submissions.json
+-rw-r--r--   0        0        0     5053 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/forms.json
+-rw-r--r--   0        0        0     2217 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/goals.json
+-rw-r--r--   0        0        0      398 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/line_items.json
+-rw-r--r--   0        0        0    18730 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/marketing_emails.json
+-rw-r--r--   0        0        0      986 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/owners.json
+-rw-r--r--   0        0        0      986 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/owners_archived.json
+-rw-r--r--   0        0        0      398 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/products.json
+-rw-r--r--   0        0        0     3742 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/shared/default_event_properties.json
+-rw-r--r--   0        0        0     1264 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/subscription_changes.json
+-rw-r--r--   0        0        0     1647 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/ticket_pipelines.json
+-rw-r--r--   0        0        0      751 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/tickets.json
+-rw-r--r--   0        0        0     3905 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/schemas/workflows.json
+-rw-r--r--   0        0        0     9781 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/source.py
+-rw-r--r--   0        0        0     4559 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/spec.yaml
+-rw-r--r--   0        0        0    96417 2024-04-16 18:06:19.360625 airbyte_source_hubspot-4.1.1/source_hubspot/streams.py
+-rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 airbyte_source_hubspot-4.1.1/PKG-INFO
```

### Comparing `airbyte_source_hubspot-4.1.0/README.md` & `airbyte_source_hubspot-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/pyproject.toml` & `airbyte_source_hubspot-4.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.1.0"
+version = "4.1.1"
 name = "airbyte-source-hubspot"
 description = "Source implementation for HubSpot."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -28,7 +28,9 @@
 source-hubspot = "source_hubspot.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 mock = "^5.1.0"
 pytest-mock = "^3.6"
 pytest = "^6.2"
+pytz = "2024.1"
+freezegun = "0.3.4"
```

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/errors.py` & `airbyte_source_hubspot-4.1.1/source_hubspot/errors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/helpers.py` & `airbyte_source_hubspot-4.1.1/source_hubspot/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/campaigns.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/companies_property_history.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/companies_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contact_lists.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contact_lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_form_submissions.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_form_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_merged_audit.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_merged_audit.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/contacts_property_history.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/contacts_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deal_pipelines.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deal_pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deals.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deals_archived.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deals_archived.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/deals_property_history.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/deals_property_history.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/email_events.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/email_events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/email_subscriptions.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/email_subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_calls.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_calls.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_emails.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_emails.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_meetings.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_meetings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_notes.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/engagements_tasks.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/engagements_tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/feedback_submissions.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/feedback_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/form_submissions.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/form_submissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/forms.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/forms.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/goals.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/goals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/marketing_emails.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/marketing_emails.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/owners.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/owners.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/owners_archived.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/owners_archived.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/shared/default_event_properties.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/shared/default_event_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/subscription_changes.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/subscription_changes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/ticket_pipelines.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/ticket_pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/tickets.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/schemas/workflows.json` & `airbyte_source_hubspot-4.1.1/source_hubspot/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/source.py` & `airbyte_source_hubspot-4.1.1/source_hubspot/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,19 +193,20 @@
                 f"The following streams are partially available: {[s.name for s in partially_available_streams]}, "
                 f"add the following scopes to download all available data: {required_scoped}"
             )
         else:
             self.logger.info("No scopes to grant when authenticating with API key.")
             available_streams = streams
 
-        available_streams.extend(self.get_custom_object_streams(api=api, common_params=common_params))
+        custom_object_streams = list(self.get_custom_object_streams(api=api, common_params=common_params))
+        available_streams.extend(custom_object_streams)
 
         if enable_experimental_streams:
             custom_objects_web_analytics_streams = self.get_web_analytics_custom_objects_stream(
-                custom_object_stream_instances=self.get_custom_object_streams(api=api, common_params=common_params),
+                custom_object_stream_instances=custom_object_streams,
                 common_params=common_params,
             )
             available_streams.extend(custom_objects_web_analytics_streams)
 
         return available_streams
 
     def get_custom_object_streams(self, api: API, common_params: Mapping[str, Any]):
```

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/spec.yaml` & `airbyte_source_hubspot-4.1.1/source_hubspot/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_hubspot-4.1.0/source_hubspot/streams.py` & `airbyte_source_hubspot-4.1.1/source_hubspot/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
             field_props["format"] = field_format
 
         return field_props
 
     @property
     @lru_cache()
     def properties(self) -> Mapping[str, Any]:
-        """Some entities has dynamic set of properties, so we trying to resolve those at runtime"""
+        """Some entities have dynamic set of properties, so we're trying to resolve those at runtime"""
         props = {}
         if not self.entity:
             return props
         if not self.properties_scope_is_granted():
             logger.warning(
                 f"Check your API key has the following permissions granted: {self.properties_scopes}, "
                 f"to be able to fetch all properties available."
```

### Comparing `airbyte_source_hubspot-4.1.0/PKG-INFO` & `airbyte_source_hubspot-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-hubspot
-Version: 4.1.0
+Version: 4.1.1
 Summary: Source implementation for HubSpot.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

