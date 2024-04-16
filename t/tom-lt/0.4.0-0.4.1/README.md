# Comparing `tmp/tom-lt-0.4.0.tar.gz` & `tmp/tom_lt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tom-lt-0.4.0.tar", last modified: Thu May 28 15:29:04 2020, max compression
+gzip compressed data, was "tom_lt-0.4.1.tar", max compression
```

## Comparing `tom-lt-0.4.0.tar` & `tom_lt-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2020-05-28 15:29:04.066612 tom-lt-0.4.0/
--rw-rw-r--   0 david     (1000) david     (1000)     4546 2020-05-28 15:29:04.066612 tom-lt-0.4.0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     3030 2020-05-28 15:27:24.000000 tom-lt-0.4.0/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       38 2020-05-28 15:29:04.066612 tom-lt-0.4.0/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1255 2020-05-28 15:27:24.000000 tom-lt-0.4.0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2020-05-28 15:29:04.066612 tom-lt-0.4.0/tom_lt/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2020-05-27 15:36:46.000000 tom-lt-0.4.0/tom_lt/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    23978 2020-05-28 15:27:24.000000 tom-lt-0.4.0/tom_lt/lt.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2020-05-28 15:29:04.066612 tom-lt-0.4.0/tom_lt.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     4546 2020-05-28 15:29:03.000000 tom-lt-0.4.0/tom_lt.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      199 2020-05-28 15:29:04.000000 tom-lt-0.4.0/tom_lt.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2020-05-28 15:29:03.000000 tom-lt-0.4.0/tom_lt.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       32 2020-05-28 15:29:03.000000 tom-lt-0.4.0/tom_lt.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        7 2020-05-28 15:29:03.000000 tom-lt-0.4.0/tom_lt.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2024-04-16 18:49:59.313038 tom_lt-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3023 2024-04-16 18:49:59.313038 tom_lt-0.4.1/README.md
+-rw-r--r--   0        0        0     1428 2024-04-16 18:50:12.437234 tom_lt-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-04-16 18:50:12.441234 tom_lt-0.4.1/tom_lt/__init__.py
+-rw-r--r--   0        0        0    25860 2024-04-16 18:49:59.317038 tom_lt-0.4.1/tom_lt/lt.py
+-rw-r--r--   0        0        0     3685 1970-01-01 00:00:00.000000 tom_lt-0.4.1/PKG-INFO
```

### Comparing `tom-lt-0.4.0/README.md` & `tom_lt-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Liverpool Telescope facility module for the TOM Toolkit v0.4.0
+# Liverpool Telescope facility module for the TOM Toolkit
 
 
 ## Features
 This module adds [Liverpool Telescope](http://telescope.livjm.ac.uk/) support
 to the TOM Toolkit.
 
 The module implements an RTML (Remote Telescope Markup Language) payload which
```

### Comparing `tom-lt-0.4.0/tom_lt/lt.py` & `tom_lt-0.4.1/tom_lt/lt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+import logging
 import time
 
 from lxml import etree
 from suds import Client
-from dateutil.parser import parse
-from datetime import datetime
 
 from django import forms
 from django.conf import settings
 
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 
 from crispy_forms.layout import Layout, Div, HTML
 from crispy_forms.bootstrap import PrependedAppendedText, PrependedText, InlineRadios
 
 from tom_observations.facility import BaseRoboticObservationForm, BaseRoboticObservationFacility
 from tom_targets.models import Target
 
+from tom_lt import __version__
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
 
 try:
     LT_SETTINGS = settings.FACILITIES['LT']
 except (AttributeError, KeyError):
     LT_SETTINGS = {
         'proposalIDs': (('proposal ID1', ''), ('proposal ID2', '')),
         'username': '',
@@ -63,15 +66,16 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.helper.layout = Layout(
             self.common_layout,
             self.layout(),
             self.extra_layout(),
-            self.button_layout()
+            self.button_layout(),
+            self.version_layout(),
         )
 
     def is_valid(self):
         super().is_valid()
         errors = LTFacility.validate_observation(self, self.observation_payload())
         if errors:
             self.add_error(None, errors)
@@ -105,14 +109,20 @@
                 ),
                 css_class='form-row'
             ),
             HTML('<hr width="85%"><h4>Instrument Config</h4>'),
             css_class='form-row'
         )
 
+    def version_layout(self):
+        return Div(HTML('<hr>'
+                        '<em><a href="http://telescope.livjm.ac.uk" target="_blank">Liverpool Telescope</a>'
+                        ' Facility module v{{version}}</em>'
+                        ))
+
     def extra_layout(self):
         return Div()
 
     def _build_prolog(self):
         namespaces = {
             'xsi': LT_XSI_NS,
         }
@@ -173,18 +183,20 @@
         payload = self._build_prolog()
         self._build_project(payload)
         self._build_inst_schedule(payload)
         return etree.tostring(payload, encoding="unicode")
 
 
 class LT_IOO_ObservationForm(LTObservationForm):
-    binning = forms.ChoiceField(choices=[('1x1', '1x1'), ('2x2', '2x2')], initial=('2x2', '2x2'),
-                                help_text='2x2 binning is usual, giving 0.3 arcsec/pixel, \
-                                faster readout and lower readout noise. 1x1 binning should \
-                                only be selected if specifically required.')
+    binning = forms.ChoiceField(
+        choices=[('1x1', '1x1'), ('2x2', '2x2')],
+        initial=('2x2', '2x2'),
+        help_text='2x2 binning is usual, giving 0.3 arcsec/pixel, \
+                   faster readout and lower readout noise. 1x1 binning should \
+                   only be selected if specifically required.')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.filters = ('U',
                         'R',
                         'G',
                         'I',
@@ -424,36 +436,72 @@
         return schedule
 
 
 class LTFacility(BaseRoboticObservationFacility):
     name = 'LT'
     observation_types = [('IOO', 'IO:O'), ('IOI', 'IO:I'), ('SPRAT', 'SPRAT'), ('FRODO', 'FRODOSpec')]
 
+    # observation_forms should be a dictionary
+    #  * it's .items() method is called in views.py::ObservationCreateView.get_context_data()
+    #  * the keys are the observation_types; values are the ObservationForm classes
+
+    # TODO: this (required) addition seems redudant to the get_form() method below.
+    # TODO: see how get_form() is used and if it's still required
+    observation_forms = {
+        'IOO': LT_IOO_ObservationForm,
+        'IOI': LT_IOI_ObservationForm,
+        'SPRAT': LT_SPRAT_ObservationForm,
+        'FRODO': LT_FRODO_ObservationForm
+    }
+
     SITES = {
             'La Palma': {
-                'sitecode': 'orm',
+                'sitecode': 'orm',  # TODO: what does this mean? and document it.
                 'latitude': 28.762,
                 'longitude': -17.872,
                 'elevation': 2363}
             }
 
     def get_form(self, observation_type):
-        if observation_type == 'IOO':
-            return LT_IOO_ObservationForm
-        elif observation_type == 'IOI':
-            return LT_IOI_ObservationForm
-        elif observation_type == 'SPRAT':
-            return LT_SPRAT_ObservationForm
-        elif observation_type == 'FRODO':
-            return LT_FRODO_ObservationForm
-        else:
-            return LT_IOO_ObservationForm
+        """
+        """
+        try:
+            return self.observation_forms[observation_type]
+        except KeyError:
+            return self.observation_forms['IOO']
+        # This is the original implementation of this method below.
+        # I've rewritten it to use the observation_forms dictionary above.
+        #
+        # if observation_type == 'IOO':
+        #     return LT_IOO_ObservationForm
+        # elif observation_type == 'IOI':
+        #     return LT_IOI_ObservationForm
+        # elif observation_type == 'SPRAT':
+        #     return LT_SPRAT_ObservationForm
+        # elif observation_type == 'FRODO':
+        #     return LT_FRODO_ObservationForm
+        # else:
+        #     return LT_IOO_ObservationForm
+
+    def get_facility_context_data(self, **kwargs):
+        """Provide Facility-specific data to context for ObservationCreateView's template
+
+        This method is called by ObservationCreateView.get_context_data() and returns a
+        dictionary of context data to be added to the View's context
+        """
+        facility_context_data = super().get_facility_context_data(**kwargs)
+        new_context_data = {
+            'version': __version__,  # from tom_tl/__init__.py
+        }
+
+        facility_context_data.update(new_context_data)
+        return facility_context_data
 
     def submit_observation(self, observation_payload):
-        if(LT_SETTINGS['DEBUG']):
+        if (LT_SETTINGS['DEBUG']):
             payload = etree.fromstring(observation_payload)
             f = open("created.rtml", "w")
             f.write(etree.tostring(payload, encoding="unicode", pretty_print=True))
             f.close()
             return [0]
         else:
             headers = {
@@ -474,15 +522,15 @@
 
     def cancel_observation(self, observation_id):
         form = self.get_form()()
         payload = form._build_prolog()
         payload.append(form._build_project())
 
     def validate_observation(self, observation_payload):
-        if(LT_SETTINGS['DEBUG']):
+        if (LT_SETTINGS['DEBUG']):
             return []
         else:
             headers = {
                 'Username': LT_SETTINGS['username'],
                 'Password': LT_SETTINGS['password']
             }
             url = '{0}://{1}:{2}/node_agent2/node_agent?wsdl'.format('http',
@@ -491,16 +539,16 @@
             client = Client(url=url, headers=headers)
             validate_payload = etree.fromstring(observation_payload)
             # Change the payload to an inquiry mode document to test connectivity.
             validate_payload.set('mode', 'inquiry')
             # Send payload, and receive response string, removing the encoding tag which causes issue with lxml parsing
             try:
                 response = client.service.handle_rtml(validate_payload).replace('encoding="ISO-8859-1"', '')
-            except:
-                return ['Error with connection to Liverpool Telescope',
+            except Exception as e:
+                return [f'Error with connection to Liverpool Telescope: {e}',
                         'This could be due to incorrect credentials, or IP / Port settings',
                         'Occassionally, this could be due to the rebooting of systems at the Telescope Site',
                         'Please retry at another time.',
                         'If the problem persists please contact ltsupport_astronomer@ljmu.ac.uk']
 
             response_rtml = etree.fromstring(response)
             if response_rtml.get('mode') == 'offer':
```

