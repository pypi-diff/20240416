# Comparing `tmp/ome-model-6.3.4.tar.gz` & `tmp/ome-model-6.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ome-model-6.3.4.tar", last modified: Thu Dec  7 13:23:05 2023, max compression
+gzip compressed data, was "ome-model-6.3.5.tar", last modified: Tue Apr 16 14:59:35 2024, max compression
```

## Comparing `ome-model-6.3.4.tar` & `ome-model-6.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:23:05.352965 ome-model-6.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-12-07 13:23:02.000000 ome-model-6.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-07 13:23:02.000000 ome-model-6.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-12-07 13:23:05.352965 ome-model-6.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-12-07 13:23:02.000000 ome-model-6.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:23:05.352965 ome-model-6.3.4/ome_model/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-07 13:23:05.000000 ome-model-6.3.4/ome_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2023-12-07 13:23:02.000000 ome-model-6.3.4/ome_model/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 13:23:05.352965 ome-model-6.3.4/ome_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-12-07 13:23:05.000000 ome-model-6.3.4/ome_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-07 13:23:05.000000 ome-model-6.3.4/ome_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 13:23:05.000000 ome-model-6.3.4/ome_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 13:23:05.000000 ome-model-6.3.4/ome_model.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-07 13:23:05.000000 ome-model-6.3.4/ome_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2023-12-07 13:23:02.000000 ome-model-6.3.4/pom.xml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 13:23:05.352965 ome-model-6.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-12-07 13:23:02.000000 ome-model-6.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:35.905288 ome-model-6.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-16 14:59:33.000000 ome-model-6.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 14:59:33.000000 ome-model-6.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-16 14:59:35.905288 ome-model-6.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-16 14:59:33.000000 ome-model-6.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:35.901288 ome-model-6.3.5/ome_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 14:59:35.000000 ome-model-6.3.5/ome_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-04-16 14:59:33.000000 ome-model-6.3.5/ome_model/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:59:35.905288 ome-model-6.3.5/ome_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-16 14:59:35.000000 ome-model-6.3.5/ome_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 14:59:35.000000 ome-model-6.3.5/ome_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:59:35.000000 ome-model-6.3.5/ome_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:59:35.000000 ome-model-6.3.5/ome_model.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 14:59:35.000000 ome-model-6.3.5/ome_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-16 14:59:33.000000 ome-model-6.3.5/pom.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:59:35.905288 ome-model-6.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-16 14:59:33.000000 ome-model-6.3.5/setup.py
```

### Comparing `ome-model-6.3.4/LICENSE.md` & `ome-model-6.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ome-model-6.3.4/PKG-INFO` & `ome-model-6.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ome-model
-Version: 6.3.4
+Version: 6.3.5
 Summary: Core OME model library (EXPERIMENTAL)
 Home-page: https://github.com/ome/ome-model/
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPL-2.0+
-Download-URL: https://github.com/ome/ome-model//v6.3.4.tar.gz
+Download-URL: https://github.com/ome/ome-model//v6.3.5.tar.gz
 Keywords: OME,Model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `ome-model-6.3.4/README.md` & `ome-model-6.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ome-model-6.3.4/ome_model/experimental.py` & `ome-model-6.3.5/ome_model/experimental.py`

 * *Files identical despite different names*

### Comparing `ome-model-6.3.4/ome_model.egg-info/PKG-INFO` & `ome-model-6.3.5/ome_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ome-model
-Version: 6.3.4
+Version: 6.3.5
 Summary: Core OME model library (EXPERIMENTAL)
 Home-page: https://github.com/ome/ome-model/
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPL-2.0+
-Download-URL: https://github.com/ome/ome-model//v6.3.4.tar.gz
+Download-URL: https://github.com/ome/ome-model//v6.3.5.tar.gz
 Keywords: OME,Model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `ome-model-6.3.4/pom.xml` & `ome-model-6.3.5/pom.xml`

 * *Files 2% similar despite different names*

#### Comparing `ome-model-6.3.4/pom.xml` & `ome-model-6.3.5/pom.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0     http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>org.openmicroscopy</groupId>
   <artifactId>ome-model</artifactId>
-  <version>6.3.4</version>
+  <version>6.3.5</version>
   <packaging>pom</packaging>
   <name>OME Model</name>
   <description>Contains the OME imaging metadata model specification, code generator and implementation</description>
   <url>http://www.openmicroscopy.org/site/products/bio-formats</url>
   <inceptionYear>2005</inceptionYear>
   <organization>
     <name>Open Microscopy Environment</name>
@@ -135,16 +135,15 @@
          same dependency, behavior is inconsistent at best, and often broken.
          The following properties facilitate consistency of dependency
          versions between various projects in the SciJava software stack.
          When possible, we advise using the relevant groupId and version
          properties for your dependencies rather than hardcoding them. -->
     <logback.version>1.3.14</logback.version>
     <slf4j.version>2.0.9</slf4j.version>
-    <testng.version>6.8</testng.version>
-    <ome_common.version>6.0.21</ome_common.version>
+    <ome_common.version>6.0.22</ome_common.version>
     <ome-common.version>${ome_common.version}</ome-common.version>
     <ome.model.schemaver>2016-06</ome.model.schemaver>
     <ome.model.schemapath>specification/src/main/resources/released-schema/${ome.model.schemaver}</ome.model.schemapath>
     <ome.model.omeschema>${ome.model.schemapath}/ome.xsd</ome.model.omeschema>
     <!-- NB: Avoid platform encoding warning when copying resources. -->
     <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
     <project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>
@@ -399,9 +398,27 @@
                 </goals>
               </execution>
             </executions>
           </plugin>
         </plugins>
       </build>
     </profile>
+    <profile>
+      <id>jdk8-only</id>
+      <activation>
+        <jdk>(,11)</jdk>
+      </activation>
+      <properties>
+        <testng.version>7.5</testng.version>
+      </properties>
+    </profile>
+    <profile>
+      <id>jdk11+</id>
+      <activation>
+        <jdk>[11,)</jdk>
+      </activation>
+      <properties>
+        <testng.version>7.9.0</testng.version>
+      </properties>
+    </profile>
   </profiles>
 </project>
```

### Comparing `ome-model-6.3.4/setup.py` & `ome-model-6.3.5/setup.py`

 * *Files identical despite different names*

