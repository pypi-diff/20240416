# Comparing `tmp/stav-0.2.dev1.tar.gz` & `tmp/stav-0.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stav-0.2.dev1.tar", last modified: Tue Nov 14 07:38:27 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `stav-0.2.dev1.tar` & `stav-0.2.dev4.tar`

### file list

```diff
@@ -1,17 +1,50 @@
-drwxr-xr-x   0 arthit     (501) staff       (20)        0 2023-11-14 07:38:27.742010 stav-0.2.dev1/
--rw-r--r--   0 arthit     (501) staff       (20)     1077 2023-09-25 13:43:17.000000 stav-0.2.dev1/LICENSE.txt
--rw-r--r--   0 arthit     (501) staff       (20)     1071 2023-11-14 07:38:27.741555 stav-0.2.dev1/PKG-INFO
--rw-r--r--   0 arthit     (501) staff       (20)      265 2023-11-14 05:49:19.000000 stav-0.2.dev1/README.md
--rw-r--r--   0 arthit     (501) staff       (20)       38 2023-11-14 07:38:27.742152 stav-0.2.dev1/setup.cfg
--rw-r--r--   0 arthit     (501) staff       (20)     1443 2023-11-14 07:38:03.000000 stav-0.2.dev1/setup.py
-drwxr-xr-x   0 arthit     (501) staff       (20)        0 2023-11-14 07:38:27.738100 stav-0.2.dev1/stav/
--rw-r--r--   0 arthit     (501) staff       (20)     3563 2023-11-14 07:37:53.000000 stav-0.2.dev1/stav/__init__.py
-drwxr-xr-x   0 arthit     (501) staff       (20)        0 2023-11-14 07:38:27.740023 stav-0.2.dev1/stav/eu/
--rw-r--r--   0 arthit     (501) staff       (20)       50 2023-09-22 14:00:58.000000 stav-0.2.dev1/stav/eu/__init__.py
-drwxr-xr-x   0 arthit     (501) staff       (20)        0 2023-11-14 07:38:27.740721 stav-0.2.dev1/stav/eu/aia/
--rw-r--r--   0 arthit     (501) staff       (20)     1223 2023-11-14 05:47:32.000000 stav-0.2.dev1/stav/eu/aia/__init__.py
-drwxr-xr-x   0 arthit     (501) staff       (20)        0 2023-11-14 07:38:27.739679 stav-0.2.dev1/stav.egg-info/
--rw-r--r--   0 arthit     (501) staff       (20)     1071 2023-11-14 07:38:27.000000 stav-0.2.dev1/stav.egg-info/PKG-INFO
--rw-r--r--   0 arthit     (501) staff       (20)      203 2023-11-14 07:38:27.000000 stav-0.2.dev1/stav.egg-info/SOURCES.txt
--rw-r--r--   0 arthit     (501) staff       (20)        1 2023-11-14 07:38:27.000000 stav-0.2.dev1/stav.egg-info/dependency_links.txt
--rw-r--r--   0 arthit     (501) staff       (20)        5 2023-11-14 07:38:27.000000 stav-0.2.dev1/stav.egg-info/top_level.txt
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 stav-0.2.dev4/ai-stakeholders.drawio
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 stav-0.2.dev4/catalog-v001.xml
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav-eu-aia.ttl
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav-th-aisbd.ttl
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav-us-aaa.ttl
+-rw-r--r--   0        0        0    23653 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav.ttl
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/.htaccess
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/406.html
+-rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/index.html
+-rw-r--r--   0        0        0    31071 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.jsonld
+-rw-r--r--   0        0        0    37077 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.nt
+-rw-r--r--   0        0        0    28158 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.owl
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.ttl
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/readme.md
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/extra.css
+-rw-r--r--   0        0        0    91556 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/jquery.js
+-rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/marked.min.js
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/owl.css
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/primer.css
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/rdf.icon
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/rec.css
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/favicon.ico
+-rw-r--r--   0        0        0    35533 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/index.html
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/license.txt
+-rw-r--r--   0        0        0    42681 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/css/webvowl.app.css
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/css/webvowl.css
+-rw-r--r--   0        0        0    74704 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/data/foaf.json
+-rw-r--r--   0        0        0    39197 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/data/ontology.json
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/data/template.json
+-rw-r--r--   0        0        0   151725 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/js/d3.min.js
+-rw-r--r--   0        0        0   350028 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/js/webvowl.app.js
+-rw-r--r--   0        0        0   751167 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/js/webvowl.js
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 stav-0.2.dev4/notebooks/mlflowstav.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 stav-0.2.dev4/notebooks/use_instruction.txt
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stav-0.2.dev4/notebooks/mlruns/0/meta.yaml
+-rw-r--r--   0        0        0  2246897 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf
+-rw-r--r--   0        0        0  3015403 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
+-rw-r--r--   0        0        0   828085 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/oss_na24_template.pptx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/~$ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/__about__.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/eu/__init__.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/eu/aia/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 stav-0.2.dev4/tests/__init__.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 stav-0.2.dev4/tools/ttltopy.ipynb
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 stav-0.2.dev4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stav-0.2.dev4/LICENSE.txt
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 stav-0.2.dev4/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 stav-0.2.dev4/pyproject.toml
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 stav-0.2.dev4/PKG-INFO
```

### Comparing `stav-0.2.dev1/LICENSE.txt` & `stav-0.2.dev4/docs/webvowl/license.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
+The MIT License (MIT)
 
-Copyright (c) 2023 Arthit Suriyawongkul
+Copyright (c) 2014-2019 Vincent Link, Steffen Lohmann, Eduard Marbach, Stefan Negru, Vitalis Wiens
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `stav-0.2.dev1/stav/__init__.py` & `stav-0.2.dev4/src/stav/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-__version__ = "0.2.dev1"
+# SPDX-FileCopyrightText: 2023 Arthit Suriyawongkul <suriyawa@tcd.ie>
+# SPDX-License-Identifier: Apache-2.0
 
-import stav.eu.aia
+__stav_namespace__ = ""
+
+from stav.eu.aia import LogRecord, TechnicalDocumentation
 
 AI_PROVIDER = "AIProvider"
-PREVIOUSLY_EXISTING_PROCESS_EVALUATION_DOCUMENTATION = (
-    "PreviouslyExistingProcessEvaluationDocumentation"
-)
+AI_DEPLOYER = "AIDeployer"
+
+PREVIOUSLY_EXISTING_PROCESS_EVALUATION_DOCUMENTATION = "PreviouslyExistingProcessEvaluationDocumentation"
 TECHNICAL_DOCUMENTATION_OBLIGATION = "TechnicalDocumentationObligation"
 BASELINE_PROCESS_DESCRIPTION = "BaselineProcessDescription"
 INSTRUCTIONS_OF_USE = "InstructionsOfUse"
 MAKING_AVAILABLE_ON_THE_MARKET = "MakingAvailableOnTheMarket"
 MARKET_SURVEILLENCE_AUTHORITY = "MarketSurveillenceAuthority"
 SYSTEM_GENERAL_DESCRIPTION = "SystemGeneralDescription"
 CURRENT_AND_POTENTIAL_FUTURE_IMPACTS = "CurrentAndPotentialFutureImpacts"
 TECHNICAL_DOCUMENTATION = "TechnicalDocumentation"
-QUALITY_MANAGEMENT_SYSTEM_DOCUMENTATION_OBLIGATION = (
-    "QualityManagementSystemDocumentationObligation"
-)
+QUALITY_MANAGEMENT_SYSTEM_DOCUMENTATION_OBLIGATION = "QualityManagementSystemDocumentationObligation"
 PUTTING_INTO_SERVICE = "PuttingIntoService"
 INTENDED_PURPOSES = "IntendedPurposes"
 DATA_MINIMIZATION_PRACTICES = "DataMinimizationPractices"
-PRIVACY_RISKS_AND_PRIVACY_MEASURES_EVALUATION_DOCUMENTATION = (
-    "PrivacyRisksAndPrivacyMeasuresEvaluationDocumentation"
-)
+PRIVACY_RISKS_AND_PRIVACY_MEASURES_EVALUATION_DOCUMENTATION = "PrivacyRisksAndPrivacyMeasuresEvaluationDocumentation"
 PLACING_ON_THE_MARKET = "PlacingOnTheMarket"
 INSTALLATION_INSTRUCTIONS = "InstallationInstructions"
 SYSTEM_EVALUATION_DOCUMENTATION = "SystemEvaluationDocumentation"
 PREVIOUSLY_EXISTING_PROCESS_KNOWN_NEGATIVE_IMPACT_INFORMATION = (
     "PreviouslyExistingProcessKnownNegativeImpactInformation"
 )
 PREVIOUSLY_EXISTING_PROCESS_DOCUMENTATION = "PreviouslyExistingProcessDocumentation"
 CONSUMER_RIGHTS_EVALUATION_INFORMATION = "ConsumerRightsEvaluationInformation"
 INFORMATION_CREATION_OBLIGATION = "InformationCreationObligation"
-AI_DEPLOYER = "AIDeployer"
 IMPACT_ASSESSMENT_DOCUMENTATION = "ImpactAssessmentDocumentation"
-INTENDED_BENEFITS_OVER_PREVIOUSLY_EXISTING_PROCESS = (
-    "IntendedBenefitsOverPreviouslyExistingProcess"
-)
+INTENDED_BENEFITS_OVER_PREVIOUSLY_EXISTING_PROCESS = "IntendedBenefitsOverPreviouslyExistingProcess"
 INFORMATION_SUBMISSION_OBLIGATION = "InformationSubmissionObligation"
 LOG = "Log"
 INFORMATION_SECURITY_MEASURES = "InformationSecurityMeasures"
 REGISTERATION_OBLIGATION = "RegisterationObligation"
 
 METRICS_RECALL = "MetricsRecall"
 METRICS_PRECISION = "MetricsPrecision"
 METRICS_F1 = "MetricsF1"
 METRICS_R2 = "MetricsR2"
 METRICS_RMSE = "MetricsRMSE"
 METRICS_MAE = "MetricsMAE"
 
 METRICS_ENERGY = "MetricsEnergy"
 
-DATASET_SIZE = "DataSetSize"
+DATASET_SIZE = "DatasetSize"
+
+ENERGY_CONSUMPTION = "EnergyConsumption"  # SPDX AI Profile
+AUTONOMY_TYPE = "AutonomyType"  # SPDX AI Profile
 
 __all__ = [
+    "LogRecord",
+    "TechnicalDocumentation",
     "AI_PROVIDER",
+    "AI_DEPLOYER",
     "PREVIOUSLY_EXISTING_PROCESS_EVALUATION_DOCUMENTATION",
     "TECHNICAL_DOCUMENTATION_OBLIGATION",
     "BASELINE_PROCESS_DESCRIPTION",
     "INSTRUCTIONS_OF_USE",
     "MAKING_AVAILABLE_ON_THE_MARKET",
     "MARKET_SURVEILLENCE_AUTHORITY",
     "SYSTEM_GENERAL_DESCRIPTION",
@@ -72,15 +74,14 @@
     "PLACING_ON_THE_MARKET",
     "INSTALLATION_INSTRUCTIONS",
     "SYSTEM_EVALUATION_DOCUMENTATION",
     "PREVIOUSLY_EXISTING_PROCESS_KNOWN_NEGATIVE_IMPACT_INFORMATION",
     "PREVIOUSLY_EXISTING_PROCESS_DOCUMENTATION",
     "CONSUMER_RIGHTS_EVALUATION_INFORMATION",
     "INFORMATION_CREATION_OBLIGATION",
-    "AI_DEPLOYER",
     "IMPACT_ASSESSMENT_DOCUMENTATION",
     "INTENDED_BENEFITS_OVER_PREVIOUSLY_EXISTING_PROCESS",
     "INFORMATION_SUBMISSION_OBLIGATION",
     "LOG",
     "INFORMATION_SECURITY_MEASURES",
     "REGISTERATION_OBLIGATION",
     "stav.eu.aia.TechnicalDocumentation",
@@ -88,8 +89,11 @@
     "METRICS_RECALL",
     "METRICS_PRECISION",
     "METRICS_F1",
     "METRICS_R2",
     "METRICS_RMSE",
     "METRICS_MAE",
     "METRICS_ENERGY",
+    "DATASET_SIZE",
+    "ENERGY_CONSUMPTION",
+    "AUTONOMY_TYPE",
 ]
```

### Comparing `stav-0.2.dev1/stav/eu/aia/__init__.py` & `stav-0.2.dev4/src/stav/eu/aia/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+# SPDX-FileCopyrightText: 2023 Arthit Suriyawongkul <suriyawa@tcd.ie>
+# SPDX-License-Identifier: Apache-2.0
 """
 Vocabulary for accountability artifacts from EU AI Act (draft)
 """
 
 __stav_namespace__ = "eu.aia"
 
 
-class TechnicalDocumentation(object):
+class TechnicalDocumentation:
     NAME = "technical_documentation"
 
-    class Description(object):
+    class Description:
         NAME = "description"
         INTENDED_PURPOSE = "intended_purpose"
         DEVELOPER = "developer"
         SYS_DATE = "sys_date"
         SYS_VERSION = "sys_version"
         REQ_SOFTWARE = "req_software"
         REQ_HARDWARD = "req_software"
         INSTRUCTIONS_USAGE = "instructions_usage"
         INSTRUCTIONS_INSTALLATION = "instructions_installation"
 
 
-class LogRecord(object):
+class LogRecord:
     NAME = "log_record"
 
 
 __all__ = [
     "TechnicalDocumentation",
     "LogRecord",
 ]
```

