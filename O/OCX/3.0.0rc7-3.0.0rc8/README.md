# Comparing `tmp/ocx-3.0.0rc7.tar.gz` & `tmp/ocx-3.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocx-3.0.0rc7.tar", max compression
+gzip compressed data, was "ocx-3.0.0rc8.tar", max compression
```

## Comparing `ocx-3.0.0rc7.tar` & `ocx-3.0.0rc8.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     2305 2024-04-09 11:41:22.639758 ocx-3.0.0rc7/DATABINDING.md
--rw-r--r--   0        0        0    11359 2024-04-09 11:41:22.639758 ocx-3.0.0rc7/LICENSE
--rw-r--r--   0        0        0   253332 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/OCX_Schema.xsd
--rw-r--r--   0        0        0       25 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/__init__.py
--rw-r--r--   0        0        0    10427 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/ocx_286/__init__.py
--rw-r--r--   0        0        0   347292 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/ocx_286/ocx_286.py
--rw-r--r--   0        0        0    10426 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/ocx_286_fix/__init__.py
--rw-r--r--   0        0        0   370511 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/ocx_286_fix/ocx_286_fix.py
--rw-r--r--   0        0        0    10269 2024-04-09 11:41:22.643758 ocx-3.0.0rc7/ocx/ocx_300b0/__init__.py
--rw-r--r--   0        0        0   359814 2024-04-09 11:41:22.647758 ocx-3.0.0rc7/ocx/ocx_300b0/ocx_300b0.py
--rw-r--r--   0        0        0    10269 2024-04-09 11:41:22.647758 ocx-3.0.0rc7/ocx/ocx_300b3/__init__.py
--rw-r--r--   0        0        0   360029 2024-04-09 11:41:22.647758 ocx-3.0.0rc7/ocx/ocx_300b3/ocx_300b3.py
--rw-r--r--   0        0        0    10269 2024-04-09 11:41:22.647758 ocx-3.0.0rc7/ocx/ocx_300b4/__init__.py
--rw-r--r--   0        0        0   360028 2024-04-09 11:41:22.647758 ocx-3.0.0rc7/ocx/ocx_300b4/ocx_300b4.py
--rw-r--r--   0        0        0    10269 2024-04-09 11:41:22.647758 ocx-3.0.0rc7/ocx/ocx_300b5/__init__.py
--rw-r--r--   0        0        0   359068 2024-04-09 11:41:22.651758 ocx-3.0.0rc7/ocx/ocx_300b5/ocx_300b5.py
--rw-r--r--   0        0        0    10017 2024-04-09 11:41:22.651758 ocx-3.0.0rc7/ocx/ocx_300b6/__init__.py
--rw-r--r--   0        0        0   368690 2024-04-09 11:41:22.651758 ocx-3.0.0rc7/ocx/ocx_300b6/ocx_300b6.py
--rw-r--r--   0        0        0    10200 2024-04-09 11:41:22.651758 ocx-3.0.0rc7/ocx/ocx_300b7/__init__.py
--rw-r--r--   0        0        0   364833 2024-04-09 11:41:22.651758 ocx-3.0.0rc7/ocx/ocx_300b7/ocx_300b7.py
--rw-r--r--   0        0        0    10278 2024-04-09 11:41:22.651758 ocx-3.0.0rc7/ocx/ocx_300rc1/__init__.py
--rw-r--r--   0        0        0   359787 2024-04-09 11:41:22.655758 ocx-3.0.0rc7/ocx/ocx_300rc1/ocx_300rc1.py
--rw-r--r--   0        0        0    10297 2024-04-09 11:41:22.655758 ocx-3.0.0rc7/ocx/ocx_300rc2/__init__.py
--rw-r--r--   0        0        0   359310 2024-04-09 11:41:22.655758 ocx-3.0.0rc7/ocx/ocx_300rc2/ocx_300rc2.py
--rw-r--r--   0        0        0    10315 2024-04-09 11:41:22.655758 ocx-3.0.0rc7/ocx/ocx_300rc3/__init__.py
--rw-r--r--   0        0        0   360787 2024-04-09 11:41:22.655758 ocx-3.0.0rc7/ocx/ocx_300rc3/ocx_300rc3.py
--rw-r--r--   0        0        0    10315 2024-04-09 11:41:22.655758 ocx-3.0.0rc7/ocx/ocx_300rc4/__init__.py
--rw-r--r--   0        0        0   360787 2024-04-09 11:41:22.659758 ocx-3.0.0rc7/ocx/ocx_300rc4/ocx_300rc4.py
--rw-r--r--   0        0        0    10219 2024-04-09 11:41:22.659758 ocx-3.0.0rc7/ocx/ocx_300rc5/__init__.py
--rw-r--r--   0        0        0   362169 2024-04-09 11:41:22.659758 ocx-3.0.0rc7/ocx/ocx_300rc5/ocx_300rc5.py
--rw-r--r--   0        0        0    10219 2024-04-09 11:41:22.659758 ocx-3.0.0rc7/ocx/ocx_300rc6/__init__.py
--rw-r--r--   0        0        0   364284 2024-04-09 11:41:22.659758 ocx-3.0.0rc7/ocx/ocx_300rc6/ocx_300rc6.py
--rw-r--r--   0        0        0    10219 2024-04-09 11:41:22.659758 ocx-3.0.0rc7/ocx/ocx_300rc7/__init__.py
--rw-r--r--   0        0        0   363034 2024-04-09 11:41:22.663758 ocx-3.0.0rc7/ocx/ocx_300rc7/ocx_300rc7.py
--rw-r--r--   0        0        0     2438 2024-04-09 11:41:22.663758 ocx-3.0.0rc7/pyproject.toml
--rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 ocx-3.0.0rc7/PKG-INFO
+-rw-r--r--   0        0        0    11359 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/LICENSE
+-rw-r--r--   0        0        0     4513 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/README.md
+-rw-r--r--   0        0        0   253328 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/ocx/OCX_Schema.xsd
+-rw-r--r--   0        0        0       25 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/ocx/__init__.py
+-rw-r--r--   0        0        0    10427 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/ocx/ocx_286/__init__.py
+-rw-r--r--   0        0        0   347292 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/ocx/ocx_286/ocx_286.py
+-rw-r--r--   0        0        0    10426 2024-04-16 13:56:10.298734 ocx-3.0.0rc8/ocx/ocx_286_fix/__init__.py
+-rw-r--r--   0        0        0   370511 2024-04-16 13:56:10.302734 ocx-3.0.0rc8/ocx/ocx_286_fix/ocx_286_fix.py
+-rw-r--r--   0        0        0    10269 2024-04-16 13:56:10.302734 ocx-3.0.0rc8/ocx/ocx_300b0/__init__.py
+-rw-r--r--   0        0        0   359814 2024-04-16 13:56:10.302734 ocx-3.0.0rc8/ocx/ocx_300b0/ocx_300b0.py
+-rw-r--r--   0        0        0    10269 2024-04-16 13:56:10.302734 ocx-3.0.0rc8/ocx/ocx_300b3/__init__.py
+-rw-r--r--   0        0        0   360029 2024-04-16 13:56:10.302734 ocx-3.0.0rc8/ocx/ocx_300b3/ocx_300b3.py
+-rw-r--r--   0        0        0    10269 2024-04-16 13:56:10.306734 ocx-3.0.0rc8/ocx/ocx_300b4/__init__.py
+-rw-r--r--   0        0        0   360028 2024-04-16 13:56:10.306734 ocx-3.0.0rc8/ocx/ocx_300b4/ocx_300b4.py
+-rw-r--r--   0        0        0    10269 2024-04-16 13:56:10.306734 ocx-3.0.0rc8/ocx/ocx_300b5/__init__.py
+-rw-r--r--   0        0        0   359068 2024-04-16 13:56:10.306734 ocx-3.0.0rc8/ocx/ocx_300b5/ocx_300b5.py
+-rw-r--r--   0        0        0    10017 2024-04-16 13:56:10.306734 ocx-3.0.0rc8/ocx/ocx_300b6/__init__.py
+-rw-r--r--   0        0        0   368690 2024-04-16 13:56:10.310734 ocx-3.0.0rc8/ocx/ocx_300b6/ocx_300b6.py
+-rw-r--r--   0        0        0    10200 2024-04-16 13:56:10.310734 ocx-3.0.0rc8/ocx/ocx_300b7/__init__.py
+-rw-r--r--   0        0        0   364833 2024-04-16 13:56:10.310734 ocx-3.0.0rc8/ocx/ocx_300b7/ocx_300b7.py
+-rw-r--r--   0        0        0    10278 2024-04-16 13:56:10.310734 ocx-3.0.0rc8/ocx/ocx_300rc1/__init__.py
+-rw-r--r--   0        0        0   359787 2024-04-16 13:56:10.310734 ocx-3.0.0rc8/ocx/ocx_300rc1/ocx_300rc1.py
+-rw-r--r--   0        0        0    10297 2024-04-16 13:56:10.310734 ocx-3.0.0rc8/ocx/ocx_300rc2/__init__.py
+-rw-r--r--   0        0        0   359310 2024-04-16 13:56:10.314735 ocx-3.0.0rc8/ocx/ocx_300rc2/ocx_300rc2.py
+-rw-r--r--   0        0        0    10315 2024-04-16 13:56:10.314735 ocx-3.0.0rc8/ocx/ocx_300rc3/__init__.py
+-rw-r--r--   0        0        0   360787 2024-04-16 13:56:10.314735 ocx-3.0.0rc8/ocx/ocx_300rc3/ocx_300rc3.py
+-rw-r--r--   0        0        0    10315 2024-04-16 13:56:10.314735 ocx-3.0.0rc8/ocx/ocx_300rc4/__init__.py
+-rw-r--r--   0        0        0   360787 2024-04-16 13:56:10.314735 ocx-3.0.0rc8/ocx/ocx_300rc4/ocx_300rc4.py
+-rw-r--r--   0        0        0    10219 2024-04-16 13:56:10.314735 ocx-3.0.0rc8/ocx/ocx_300rc5/__init__.py
+-rw-r--r--   0        0        0   362169 2024-04-16 13:56:10.318735 ocx-3.0.0rc8/ocx/ocx_300rc5/ocx_300rc5.py
+-rw-r--r--   0        0        0    10219 2024-04-16 13:56:10.318735 ocx-3.0.0rc8/ocx/ocx_300rc6/__init__.py
+-rw-r--r--   0        0        0   364284 2024-04-16 13:56:10.318735 ocx-3.0.0rc8/ocx/ocx_300rc6/ocx_300rc6.py
+-rw-r--r--   0        0        0    10219 2024-04-16 13:56:10.318735 ocx-3.0.0rc8/ocx/ocx_300rc7/__init__.py
+-rw-r--r--   0        0        0   363034 2024-04-16 13:56:10.318735 ocx-3.0.0rc8/ocx/ocx_300rc7/ocx_300rc7.py
+-rw-r--r--   0        0        0    10219 2024-04-16 13:56:10.318735 ocx-3.0.0rc8/ocx/ocx_300rc8/__init__.py
+-rw-r--r--   0        0        0   357212 2024-04-16 13:56:10.322734 ocx-3.0.0rc8/ocx/ocx_300rc8/ocx_300rc8.py
+-rw-r--r--   0        0        0     2419 2024-04-16 13:56:10.322734 ocx-3.0.0rc8/pyproject.toml
+-rw-r--r--   0        0        0     4967 1970-01-01 00:00:00.000000 ocx-3.0.0rc8/PKG-INFO
```

### Comparing `ocx-3.0.0rc7/LICENSE` & `ocx-3.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/OCX_Schema.xsd` & `ocx-3.0.0rc8/ocx/OCX_Schema.xsd`

 * *Files 0% similar despite different names*

#### Comparing `ocx-3.0.0rc7/ocx/OCX_Schema.xsd` & `ocx-3.0.0rc8/ocx/OCX_Schema.xsd`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- edited with XMLSpy v2024 (x64) (http://www.altova.com) by Astrup, Ole Christian (DNV AS) -->
 <!-- Copyright 2024 Open Class 3D Exchange (OCX) Consortium (https://3docx.org)			Licensed under the Apache License, Version 2.0 (the "License"); 			You may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0			Unless required by applicable law or agreed to in writing, the 3Docx standard and software distributed under the License is distributed on an 			"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either expressed or implied.			The OCX Consortium is not liable to any use whatsoever of the distributed standard or software based on the standard.			See the License for the specific language governing permissions and limitations under the License.  -->
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:vc="http://www.w3.org/2007/XMLSchema-versioning" xmlns:ocx="https://3docx.org/fileadmin//ocx_schema//V300rc7//OCX_Schema.xsd" xmlns:unitsml="urn:oasis:names:tc:unitsml:schema:xsd:UnitsMLSchema_lite-0.9.18" targetNamespace="https://3docx.org/fileadmin//ocx_schema//V300rc7//OCX_Schema.xsd" elementFormDefault="qualified" attributeFormDefault="unqualified" vc:minVersion="1.0">
+<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:vc="http://www.w3.org/2007/XMLSchema-versioning" xmlns:ocx="https://3docx.org/fileadmin//ocx_schema//V300rc8//OCX_Schema.xsd" xmlns:unitsml="urn:oasis:names:tc:unitsml:schema:xsd:UnitsMLSchema_lite-0.9.18" targetNamespace="https://3docx.org/fileadmin//ocx_schema//V300rc8//OCX_Schema.xsd" elementFormDefault="qualified" attributeFormDefault="unqualified" vc:minVersion="1.0">
   <!-- Import the NIST unitsML lite schema -->
   <xs:import namespace="urn:oasis:names:tc:unitsml:schema:xsd:UnitsMLSchema_lite-0.9.18" schemaLocation="https://3docx.org/fileadmin/ocx_schema/unitsml/unitsmlSchema_lite-0.9.18.xsd"/>
   <xs:annotation>
     <xs:documentation>Copyright 2024 Open Class 3D Exchange (OCX) Consortium (https://3docx.org). Licensed under the Apache License, Version 2.0 (the &quot;License&quot;); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0. Unless required by applicable law or agreed to in writing, the 3Docx standard and software distributed under the License is distributed on an &quot;AS IS&quot; BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either expressed or implied.	The OCX Consortium is not liable to any use whatsoever of the distributed standard or software based on the standard. See the License for the specific language governing permissions and limitations under the License.</xs:documentation>
   </xs:annotation>
   <xs:element name="Header" type="ocx:Header_T">
     <xs:annotation>
@@ -66,15 +66,15 @@
   <xs:complexType name="DocumentBase_T" abstract="true">
     <xs:annotation>
       <xs:documentation>Type definition of the abstract base class for the XML document defined in this schema.</xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element ref="ocx:Header"/>
     </xs:sequence>
-    <xs:attribute name="schemaVersion" type="xs:string" use="required" fixed="3.0.0rc7">
+    <xs:attribute name="schemaVersion" type="xs:string" use="required" fixed="3.0.0rc8">
       <xs:annotation>
         <xs:documentation>Current XML schema version (Format - x.y.z) x : Incremented for backward incompatible changes ( Ex - Adding a required attribute, etc.) y : Major backward compatible changes [ Ex - Adding a new node ,fixing major CRs,etc..] z : Minor backward compatible changes (Ex - adding an optional attribute, etc).</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="language" type="xs:language" use="optional" default="en">
       <xs:annotation>
         <xs:documentation>Language used by the application.</xs:documentation>
@@ -602,25 +602,25 @@
     <xs:annotation>
       <xs:documentation>Type definition</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="ocx:StructureRef_T"/>
     </xs:complexContent>
   </xs:complexType>
-  <xs:element name="EdgeReinforcementRef" type="ocx:EdgeReinforcementRef_T" substitutionGroup="ocx:StructureRef">
+  <xs:element name="EdgeReinforcementRef" type="ocx:EdgeReinforcementRef_T" substitutionGroup="ocx:BoundedRef">
     <xs:annotation>
       <xs:documentation>A  reference to an EdgeReinforcement.</xs:documentation>
     </xs:annotation>
   </xs:element>
   <xs:complexType name="EdgeReinforcementRef_T">
     <xs:annotation>
       <xs:documentation>Type definition</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
-      <xs:extension base="ocx:StructureRef_T">
+      <xs:extension base="ocx:BoundedRef_T">
         <xs:attribute ref="ocx:refType" use="required" fixed="ocx:EdgeReinforcement"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <!-- References to structure concept instances without geometry-->
   <xs:element name="EndCutRef" substitutionGroup="ocx:ReferenceBase">
     <xs:annotation>
```

### Comparing `ocx-3.0.0rc7/ocx/ocx_286/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_286/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_286/ocx_286.py` & `ocx-3.0.0rc8/ocx/ocx_286/ocx_286.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_286_fix/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_286_fix/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_286_fix/ocx_286_fix.py` & `ocx-3.0.0rc8/ocx/ocx_286_fix/ocx_286_fix.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b0/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300b0/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b0/ocx_300b0.py` & `ocx-3.0.0rc8/ocx/ocx_300b0/ocx_300b0.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b3/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300b3/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b3/ocx_300b3.py` & `ocx-3.0.0rc8/ocx/ocx_300b3/ocx_300b3.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b4/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300b4/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b4/ocx_300b4.py` & `ocx-3.0.0rc8/ocx/ocx_300b4/ocx_300b4.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b5/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300b5/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b5/ocx_300b5.py` & `ocx-3.0.0rc8/ocx/ocx_300b5/ocx_300b5.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b6/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300b6/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b6/ocx_300b6.py` & `ocx-3.0.0rc8/ocx/ocx_300b6/ocx_300b6.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b7/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300b7/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300b7/ocx_300b7.py` & `ocx-3.0.0rc8/ocx/ocx_300b7/ocx_300b7.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc1/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc1/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc1/ocx_300rc1.py` & `ocx-3.0.0rc8/ocx/ocx_300rc1/ocx_300rc1.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc2/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc2/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc2/ocx_300rc2.py` & `ocx-3.0.0rc8/ocx/ocx_300rc2/ocx_300rc2.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc3/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc3/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc3/ocx_300rc3.py` & `ocx-3.0.0rc8/ocx/ocx_300rc3/ocx_300rc3.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc4/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc4/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc4/ocx_300rc4.py` & `ocx-3.0.0rc8/ocx/ocx_300rc4/ocx_300rc4.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc5/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc5/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc5/ocx_300rc5.py` & `ocx-3.0.0rc8/ocx/ocx_300rc5/ocx_300rc5.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc6/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc6/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc6/ocx_300rc6.py` & `ocx-3.0.0rc8/ocx/ocx_300rc6/ocx_300rc6.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc7/__init__.py` & `ocx-3.0.0rc8/ocx/ocx_300rc7/__init__.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/ocx/ocx_300rc7/ocx_300rc7.py` & `ocx-3.0.0rc8/ocx/ocx_300rc7/ocx_300rc7.py`

 * *Files identical despite different names*

### Comparing `ocx-3.0.0rc7/pyproject.toml` & `ocx-3.0.0rc8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "OCX"
-version = "3.0.0rc7"
+version = "3.0.0rc8"
 description = ""
 authors = ["ocastrup <ole.christain.astrup@dnv.com>"]
-readme = "DATABINDING.md"
+readme = "README.md"
 packages = [{include = "ocx"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-xsdata = "*"
+python = "^3.9"
 packaging = "^23.1"
 tbump = "*"
-ocx_databinding = "^2.6"
+ocx_databinding = "^2.7"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/OCXStandard/OCX_Schema"
 
 [tool.tbump.version]
-current = "3.0.0rc7"
+current = "3.0.0rc8"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

