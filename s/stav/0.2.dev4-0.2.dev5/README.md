# Comparing `tmp/stav-0.2.dev4.tar.gz` & `tmp/stav-0.2.dev5.tar.gz`

## Comparing `stav-0.2.dev4.tar` & `stav-0.2.dev5.tar`

### file list

```diff
@@ -1,50 +1,58 @@
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 stav-0.2.dev4/ai-stakeholders.drawio
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 stav-0.2.dev4/catalog-v001.xml
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav-eu-aia.ttl
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav-th-aisbd.ttl
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav-us-aaa.ttl
--rw-r--r--   0        0        0    23653 2020-02-02 00:00:00.000000 stav-0.2.dev4/stav.ttl
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/.htaccess
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/406.html
--rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/index.html
--rw-r--r--   0        0        0    31071 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.jsonld
--rw-r--r--   0        0        0    37077 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.nt
--rw-r--r--   0        0        0    28158 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.owl
--rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/ontology.ttl
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/readme.md
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/extra.css
--rw-r--r--   0        0        0    91556 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/jquery.js
--rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/marked.min.js
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/owl.css
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/primer.css
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/rdf.icon
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/resources/rec.css
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/favicon.ico
--rw-r--r--   0        0        0    35533 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/index.html
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/license.txt
--rw-r--r--   0        0        0    42681 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/css/webvowl.app.css
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/css/webvowl.css
--rw-r--r--   0        0        0    74704 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/data/foaf.json
--rw-r--r--   0        0        0    39197 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/data/ontology.json
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/data/template.json
--rw-r--r--   0        0        0   151725 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/js/d3.min.js
--rw-r--r--   0        0        0   350028 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/js/webvowl.app.js
--rw-r--r--   0        0        0   751167 2020-02-02 00:00:00.000000 stav-0.2.dev4/docs/webvowl/js/webvowl.js
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 stav-0.2.dev4/notebooks/mlflowstav.ipynb
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 stav-0.2.dev4/notebooks/use_instruction.txt
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stav-0.2.dev4/notebooks/mlruns/0/meta.yaml
--rw-r--r--   0        0        0  2246897 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf
--rw-r--r--   0        0        0  3015403 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
--rw-r--r--   0        0        0   828085 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/oss_na24_template.pptx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 stav-0.2.dev4/presentations/~$ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/__about__.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/eu/__init__.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 stav-0.2.dev4/src/stav/eu/aia/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 stav-0.2.dev4/tests/__init__.py
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 stav-0.2.dev4/tools/ttltopy.ipynb
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 stav-0.2.dev4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stav-0.2.dev4/LICENSE.txt
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 stav-0.2.dev4/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 stav-0.2.dev4/pyproject.toml
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 stav-0.2.dev4/PKG-INFO
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 stav-0.2.dev5/ai-stakeholders.drawio
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 stav-0.2.dev5/catalog-v001.xml
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav-eu-aia.ttl
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav-th-aisbd.ttl
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav-us-aaa.ttl
+-rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav.ttl
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/.htaccess
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/406.html
+-rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/index.html
+-rw-r--r--   0        0        0    31071 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.jsonld
+-rw-r--r--   0        0        0    37077 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.nt
+-rw-r--r--   0        0        0    28158 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.owl
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.ttl
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/readme.md
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/extra.css
+-rw-r--r--   0        0        0    91556 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/jquery.js
+-rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/marked.min.js
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/owl.css
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/primer.css
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/rdf.icon
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/rec.css
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/favicon.ico
+-rw-r--r--   0        0        0    35533 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/index.html
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/license.txt
+-rw-r--r--   0        0        0    42681 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/css/webvowl.app.css
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/css/webvowl.css
+-rw-r--r--   0        0        0    74704 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/data/foaf.json
+-rw-r--r--   0        0        0    39197 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/data/ontology.json
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/data/template.json
+-rw-r--r--   0        0        0   151725 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/js/d3.min.js
+-rw-r--r--   0        0        0   350028 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/js/webvowl.app.js
+-rw-r--r--   0        0        0   751167 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/js/webvowl.js
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlflowstav.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/use_instruction.txt
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/meta.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/AIProvider
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/EnergyConsumption
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.user
+-rw-r--r--   0        0        0  2246897 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf
+-rw-r--r--   0        0        0  3015403 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
+-rw-r--r--   0        0        0   828085 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/oss_na24_template.pptx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/~$ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/__about__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/eu/__init__.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/eu/aia/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 stav-0.2.dev5/tests/__init__.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 stav-0.2.dev5/tools/ttltopy.ipynb
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 stav-0.2.dev5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stav-0.2.dev5/LICENSE.txt
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 stav-0.2.dev5/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 stav-0.2.dev5/pyproject.toml
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 stav-0.2.dev5/PKG-INFO
```

### Comparing `stav-0.2.dev4/ai-stakeholders.drawio` & `stav-0.2.dev5/ai-stakeholders.drawio`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/catalog-v001.xml` & `stav-0.2.dev5/catalog-v001.xml`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/stav-eu-aia.ttl` & `stav-0.2.dev5/stav-eu-aia.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/stav-th-aisbd.ttl` & `stav-0.2.dev5/stav-th-aisbd.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/stav-us-aaa.ttl` & `stav-0.2.dev5/stav-us-aaa.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/stav.ttl` & `stav-0.2.dev5/stav.ttl`

 * *Files 0% similar despite different names*

```diff
@@ -202,23 +202,23 @@
                                           [ rdf:type owl:Restriction ;
                                             owl:onProperty odrl:partOf ;
                                             owl:someValuesFrom :SystemGeneralDescription
                                           ] ;
                           rdfs:label "Installation Instructions"@en .
 
 
-###  https://w3id.org/stav#InstructionsOfUse
+###  https://w3id.org/stav#InstructionsForUse
 :InstructionsOfUse rdf:type owl:Class ;
                    rdfs:subClassOf odrl:Asset ,
                                    [ rdf:type owl:Restriction ;
                                      owl:onProperty odrl:partOf ;
                                      owl:someValuesFrom :SystemGeneralDescription
                                    ] ;
-                   rdfs:label "Instructions of Use"@en ;
-                   skos:definition "‘instructions for use’ means the information provided by the provider to inform the user of in particular an AI system’s intended purpose and proper use, inclusive of the specific geographical, behavioural or functional setting within which the high-risk AI system is intended to be used."@en ;
+                   rdfs:label "Instructions for Use"@en ;
+                   skos:definition "‘instructions for use’ or ‘instructions of use’ means the information provided by the provider to inform the user of in particular an AI system’s intended purpose and proper use, inclusive of the specific geographical, behavioural or functional setting within which the high-risk AI system is intended to be used."@en ;
                    skos:note "Article 3 (15)" ;
                    odrl:source "https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:52021PC0206&from=EN" .
 
 
 ###  https://w3id.org/stav#IntendedBenefitsOverPreviouslyExistingProcess
 :IntendedBenefitsOverPreviouslyExistingProcess rdf:type owl:Class ;
                                                rdfs:subClassOf odrl:Asset ;
```

### Comparing `stav-0.2.dev4/docs/.htaccess` & `stav-0.2.dev5/docs/.htaccess`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/index.html` & `stav-0.2.dev5/docs/index.html`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/ontology.jsonld` & `stav-0.2.dev5/docs/ontology.jsonld`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/ontology.nt` & `stav-0.2.dev5/docs/ontology.nt`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/ontology.owl` & `stav-0.2.dev5/docs/ontology.owl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/ontology.ttl` & `stav-0.2.dev5/docs/ontology.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/readme.md` & `stav-0.2.dev5/docs/readme.md`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/resources/extra.css` & `stav-0.2.dev5/docs/resources/extra.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/resources/jquery.js` & `stav-0.2.dev5/docs/resources/jquery.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/resources/marked.min.js` & `stav-0.2.dev5/docs/resources/marked.min.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/resources/owl.css` & `stav-0.2.dev5/docs/resources/owl.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/resources/primer.css` & `stav-0.2.dev5/docs/resources/primer.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/resources/rec.css` & `stav-0.2.dev5/docs/resources/rec.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/favicon.ico` & `stav-0.2.dev5/docs/webvowl/favicon.ico`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/index.html` & `stav-0.2.dev5/docs/webvowl/index.html`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/license.txt` & `stav-0.2.dev5/docs/webvowl/license.txt`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/css/webvowl.app.css` & `stav-0.2.dev5/docs/webvowl/css/webvowl.app.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/css/webvowl.css` & `stav-0.2.dev5/docs/webvowl/css/webvowl.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/data/foaf.json` & `stav-0.2.dev5/docs/webvowl/data/foaf.json`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/data/ontology.json` & `stav-0.2.dev5/docs/webvowl/data/ontology.json`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/data/template.json` & `stav-0.2.dev5/docs/webvowl/data/template.json`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/js/d3.min.js` & `stav-0.2.dev5/docs/webvowl/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/js/webvowl.app.js` & `stav-0.2.dev5/docs/webvowl/js/webvowl.app.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/docs/webvowl/js/webvowl.js` & `stav-0.2.dev5/docs/webvowl/js/webvowl.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf` & `stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx` & `stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/presentations/oss_na24_template.pptx` & `stav-0.2.dev5/presentations/oss_na24_template.pptx`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/src/stav/__init__.py` & `stav-0.2.dev5/src/stav/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,94 @@
 # SPDX-FileCopyrightText: 2023 Arthit Suriyawongkul <suriyawa@tcd.ie>
 # SPDX-License-Identifier: Apache-2.0
 
 __stav_namespace__ = ""
 
 from stav.eu.aia import LogRecord, TechnicalDocumentation
 
+# Obligations
+INFORMATION_CREATION_OBLIGATION = "InformationCreationObligation"
+INFORMATION_SUBMISSION_OBLIGATION = "InformationSubmissionObligation"
+QUALITY_MANAGEMENT_SYSTEM_DOCUMENTATION_OBLIGATION = "QualityManagementSystemDocumentationObligation"
+REGISTERATION_OBLIGATION = "RegisterationObligation"
+TECHNICAL_DOCUMENTATION_OBLIGATION = "TechnicalDocumentationObligation"
+
+# System information
+INSTRUCTIONS_FOR_USE = "InstructionsForUse"
+INSTRUCTIONS_INSTALLATION = "InstallationInstructions"
+INTENDED_PURPOSES = "IntendedPurposes"
+SYSTEM_GENERAL_DESCRIPTION = "SystemGeneralDescription"
+
+# Stakeholders
 AI_PROVIDER = "AIProvider"
 AI_DEPLOYER = "AIDeployer"
+MARKET_SURVEILLENCE_AUTHORITY = "MarketSurveillenceAuthority"
 
+# Documentation
+PREVIOUSLY_EXISTING_PROCESS_DOCUMENTATION = "PreviouslyExistingProcessDocumentation"
 PREVIOUSLY_EXISTING_PROCESS_EVALUATION_DOCUMENTATION = "PreviouslyExistingProcessEvaluationDocumentation"
-TECHNICAL_DOCUMENTATION_OBLIGATION = "TechnicalDocumentationObligation"
-BASELINE_PROCESS_DESCRIPTION = "BaselineProcessDescription"
-INSTRUCTIONS_OF_USE = "InstructionsOfUse"
-MAKING_AVAILABLE_ON_THE_MARKET = "MakingAvailableOnTheMarket"
-MARKET_SURVEILLENCE_AUTHORITY = "MarketSurveillenceAuthority"
-SYSTEM_GENERAL_DESCRIPTION = "SystemGeneralDescription"
+PREVIOUSLY_EXISTING_PROCESS_KNOWN_NEGATIVE_IMPACT_INFORMATION = (
+    "PreviouslyExistingProcessKnownNegativeImpactInformation"
+)
+INTENDED_BENEFITS_OVER_PREVIOUSLY_EXISTING_PROCESS = "IntendedBenefitsOverPreviouslyExistingProcess"
 CURRENT_AND_POTENTIAL_FUTURE_IMPACTS = "CurrentAndPotentialFutureImpacts"
 TECHNICAL_DOCUMENTATION = "TechnicalDocumentation"
-QUALITY_MANAGEMENT_SYSTEM_DOCUMENTATION_OBLIGATION = "QualityManagementSystemDocumentationObligation"
-PUTTING_INTO_SERVICE = "PuttingIntoService"
-INTENDED_PURPOSES = "IntendedPurposes"
-DATA_MINIMIZATION_PRACTICES = "DataMinimizationPractices"
 PRIVACY_RISKS_AND_PRIVACY_MEASURES_EVALUATION_DOCUMENTATION = "PrivacyRisksAndPrivacyMeasuresEvaluationDocumentation"
-PLACING_ON_THE_MARKET = "PlacingOnTheMarket"
-INSTALLATION_INSTRUCTIONS = "InstallationInstructions"
 SYSTEM_EVALUATION_DOCUMENTATION = "SystemEvaluationDocumentation"
-PREVIOUSLY_EXISTING_PROCESS_KNOWN_NEGATIVE_IMPACT_INFORMATION = (
-    "PreviouslyExistingProcessKnownNegativeImpactInformation"
-)
-PREVIOUSLY_EXISTING_PROCESS_DOCUMENTATION = "PreviouslyExistingProcessDocumentation"
 CONSUMER_RIGHTS_EVALUATION_INFORMATION = "ConsumerRightsEvaluationInformation"
-INFORMATION_CREATION_OBLIGATION = "InformationCreationObligation"
 IMPACT_ASSESSMENT_DOCUMENTATION = "ImpactAssessmentDocumentation"
-INTENDED_BENEFITS_OVER_PREVIOUSLY_EXISTING_PROCESS = "IntendedBenefitsOverPreviouslyExistingProcess"
-INFORMATION_SUBMISSION_OBLIGATION = "InformationSubmissionObligation"
-LOG = "Log"
+BASELINE_PROCESS_DESCRIPTION = "BaselineProcessDescription"
+DATA_MINIMIZATION_PRACTICES = "DataMinimizationPractices"
+
+# Actions / Verbs
+MAKING_AVAILABLE_ON_THE_MARKET = "MakingAvailableOnTheMarket"
+PLACING_ON_THE_MARKET = "PlacingOnTheMarket"
+PUTTING_INTO_SERVICE = "PuttingIntoService"
+
+# Measures
 INFORMATION_SECURITY_MEASURES = "InformationSecurityMeasures"
-REGISTERATION_OBLIGATION = "RegisterationObligation"
 
+# Metrics
 METRICS_RECALL = "MetricsRecall"
 METRICS_PRECISION = "MetricsPrecision"
 METRICS_F1 = "MetricsF1"
 METRICS_R2 = "MetricsR2"
 METRICS_RMSE = "MetricsRMSE"
 METRICS_MAE = "MetricsMAE"
-
 METRICS_ENERGY = "MetricsEnergy"
 
+LOG = "Log"
 DATASET_SIZE = "DatasetSize"
 
-ENERGY_CONSUMPTION = "EnergyConsumption"  # SPDX AI Profile
-AUTONOMY_TYPE = "AutonomyType"  # SPDX AI Profile
+# SPDX AI Profile
+AUTONOMY_TYPE = "autonomyType"
+DOMAIN = "domain"
+ENERGY_CONSUMPTION = "energyConsumption"
+HYPERPARAMETER = "hyperparameter"
+INFO_APP = "informationAboutApplication"
+INFO_TRAINING = "informationAboutTraining"
+LIMITATION = "limitation"
+METRIC = "metric"
+METRIC_DECISION_THRESHOLD = "metricDecisionThreshold"
+MODEL_DATA_PROCESSING = "modelDataPreprocessing"
+MODEL_EXPLAINABILITY = "modelExplainability"
+SAFETY_RISK_ASSESSMENT = "safetyRiskAssessment"
+STANDARD_COMPLIANCE = "standardCompliance"
+MODEL_TYPE = "typeOfModel"
+USE_SENSITIVE_PERSONAL_INFO = "useSensitivePersonalInformation"
 
 __all__ = [
     "LogRecord",
     "TechnicalDocumentation",
     "AI_PROVIDER",
     "AI_DEPLOYER",
     "PREVIOUSLY_EXISTING_PROCESS_EVALUATION_DOCUMENTATION",
     "TECHNICAL_DOCUMENTATION_OBLIGATION",
     "BASELINE_PROCESS_DESCRIPTION",
-    "INSTRUCTIONS_OF_USE",
+    "INSTRUCTIONS_FOR_USE",
     "MAKING_AVAILABLE_ON_THE_MARKET",
     "MARKET_SURVEILLENCE_AUTHORITY",
     "SYSTEM_GENERAL_DESCRIPTION",
     "CURRENT_AND_POTENTIAL_FUTURE_IMPACTS",
     "TECHNICAL_DOCUMENTATION",
     "QUALITY_MANAGEMENT_SYSTEM_DOCUMENTATION_OBLIGATION",
     "PUTTING_INTO_SERVICE",
@@ -90,10 +114,23 @@
     "METRICS_PRECISION",
     "METRICS_F1",
     "METRICS_R2",
     "METRICS_RMSE",
     "METRICS_MAE",
     "METRICS_ENERGY",
     "DATASET_SIZE",
-    "ENERGY_CONSUMPTION",
     "AUTONOMY_TYPE",
+    "DOMAIN",
+    "ENERGY_CONSUMPTION",
+    "HYPERPARAMETER",
+    "INFO_APP",
+    "INFO_TRAINING",
+    "LIMITATION",
+    "METRIC",
+    "METRIC_DECISION_THRESHOLD",
+    "MODEL_DATA_PROCESSING",
+    "MODEL_EXPLAINABILITY",
+    "SAFETY_RISK_ASSESSMENT",
+    "STANDARD_COMPLIANCE",
+    "MODEL_TYPE",
+    "USE_SENSITIVE_PERSONAL_INFO",
 ]
```

### Comparing `stav-0.2.dev4/src/stav/eu/aia/__init__.py` & `stav-0.2.dev5/src/stav/eu/aia/__init__.py`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/tools/ttltopy.ipynb` & `stav-0.2.dev5/tools/ttltopy.ipynb`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/.gitignore` & `stav-0.2.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/LICENSE.txt` & `stav-0.2.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/README.md` & `stav-0.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/pyproject.toml` & `stav-0.2.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev4/PKG-INFO` & `stav-0.2.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stav
-Version: 0.2.dev4
+Version: 0.2.dev5
 Summary: System Trustworthiness and Accountability Vocabulary
 Project-URL: Documentation, https://github.com/unknown/stav#readme
 Project-URL: Issues, https://github.com/unknown/stav/issues
 Project-URL: Source, https://github.com/unknown/stav
 Author-email: Arthit Suriyawongkul <arthit@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

