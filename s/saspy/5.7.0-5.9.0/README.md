# Comparing `tmp/saspy-5.7.0.tar.gz` & `tmp/saspy-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saspy-5.7.0.tar", last modified: Tue Mar 19 14:58:34 2024, max compression
+gzip compressed data, was "saspy-5.9.0.tar", last modified: Mon Apr  8 19:58:15 2024, max compression
```

## Comparing `saspy-5.7.0.tar` & `saspy-5.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.058898 saspy-5.7.0/
--rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2024-03-19 14:58:21.000000 saspy-5.7.0/LICENSE.md
--rw-r--r--   0 sastpw     (894) r&d        (100)       18 2024-03-19 14:58:21.000000 saspy-5.7.0/MANIFEST.in
--rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-03-19 14:58:34.057898 saspy-5.7.0/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2024-03-19 14:58:21.000000 saspy-5.7.0/README.md
--rw-r--r--   0 sastpw     (894) r&d        (100)      173 2024-03-19 14:58:21.000000 saspy-5.7.0/pyproject.toml
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.033897 saspy-5.7.0/saspy/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/SASLogLexer.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/__init__.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/autocfg.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.035897 saspy-5.7.0/saspy/java/
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.045898 saspy-5.7.0/saspy/java/iomclient/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-api-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-api-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-core-2.12.4.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/log4j-core-2.17.1.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/sas.core.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/sas.security.sspi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/iomclient/sas.svc.connection.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.050898 saspy-5.7.0/saspy/java/pyiom/
--rw-r--r--   0 sastpw     (894) r&d        (100)     1095 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/cancel.class
--rw-r--r--   0 sastpw     (894) r&d        (100)     1332 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/cancel.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    18884 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/saspy2j.class
--rw-r--r--   0 sastpw     (894) r&d        (100)    34685 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/pyiom/saspy2j.java
--rw-r--r--   0 sastpw     (894) r&d        (100)    15824 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/saspyiom.jar
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.056898 saspy-5.7.0/saspy/java/thirdparty/
--rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/NOTICE.md
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-orb.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/pfl-basic.jar
--rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/java/thirdparty/pfl-tf.jar
--rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/libname_gen.sas
--rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasViyaML.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sas_magic.py
--rw-r--r--   0 sastpw     (894) r&d        (100)   136277 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasbase.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10965 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sascfg.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasdata.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasdecorator.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasets.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     3905 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasexceptions.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    35993 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasiocom.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    88492 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasiohttp.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    89012 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasioiom.py
--rwxr-xr-x   0 sastpw     (894) r&d        (100)   101414 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasiostdio.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasml.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasproccommons.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasqc.py
--rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasresults.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasstat.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sastabulate.py
--rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/sasutil.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.056898 saspy-5.7.0/saspy/scripts/
--rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/scripts/run_sas.py
--rw-r--r--   0 sastpw     (894) r&d        (100)       22 2024-03-19 14:58:21.000000 saspy-5.7.0/saspy/version.py
-drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-03-19 14:58:34.056898 saspy-5.7.0/saspy.egg-info/
--rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/PKG-INFO
--rw-r--r--   0 sastpw     (894) r&d        (100)     1451 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/SOURCES.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        1 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/dependency_links.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       41 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/requires.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)        6 2024-03-19 14:58:34.000000 saspy-5.7.0/saspy.egg-info/top_level.txt
--rw-r--r--   0 sastpw     (894) r&d        (100)       38 2024-03-19 14:58:34.058898 saspy-5.7.0/setup.cfg
--rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2024-03-19 14:58:21.000000 saspy-5.7.0/setup.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.498511 saspy-5.9.0/
+-rw-r--r--   0 sastpw     (894) r&d        (100)    16774 2024-04-08 19:58:03.000000 saspy-5.9.0/LICENSE.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)       18 2024-04-08 19:58:03.000000 saspy-5.9.0/MANIFEST.in
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-04-08 19:58:15.498511 saspy-5.9.0/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3502 2024-04-08 19:58:03.000000 saspy-5.9.0/README.md
+-rw-r--r--   0 sastpw     (894) r&d        (100)      173 2024-04-08 19:58:03.000000 saspy-5.9.0/pyproject.toml
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.470508 saspy-5.9.0/saspy/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1985 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/SASLogLexer.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2275 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/__init__.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3343 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/autocfg.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.473509 saspy-5.9.0/saspy/java/
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.485509 saspy-5.9.0/saspy/java/iomclient/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    67163 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   208005 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   276756 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/log4j-api-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   301873 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/log4j-api-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1682736 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/log4j-core-2.12.4.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1790452 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/log4j-core-2.17.1.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   997855 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/sas.core.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     6589 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/sas.security.sspi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  2289298 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/iomclient/sas.svc.connection.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.489510 saspy-5.9.0/saspy/java/pyiom/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1095 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/pyiom/cancel.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1332 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/pyiom/cancel.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    18884 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/pyiom/saspy2j.class
+-rw-r--r--   0 sastpw     (894) r&d        (100)    34685 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/pyiom/saspy2j.java
+-rw-r--r--   0 sastpw     (894) r&d        (100)    15824 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/saspyiom.jar
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.496510 saspy-5.9.0/saspy/java/thirdparty/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     2155 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/thirdparty/NOTICE.md
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    28157 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1376212 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)  1624797 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/thirdparty/glassfish-corba-orb.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   197485 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/thirdparty/pfl-basic.jar
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)    93886 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/java/thirdparty/pfl-tf.jar
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3529 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/libname_gen.sas
+-rw-r--r--   0 sastpw     (894) r&d        (100)    26811 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasViyaML.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     7181 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sas_magic.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)   136277 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasbase.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10965 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sascfg.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    70625 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasdata.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5338 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasdecorator.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    24448 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasets.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     3905 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasexceptions.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    35993 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasiocom.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    88541 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasiohttp.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    89813 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasioiom.py
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)   101414 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasiostdio.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    13996 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasml.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    37444 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasproccommons.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    10214 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasqc.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)     5022 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasresults.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    29545 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasstat.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    11192 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sastabulate.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)    12143 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/sasutil.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.496510 saspy-5.9.0/saspy/scripts/
+-rwxr-xr-x   0 sastpw     (894) r&d        (100)     3366 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/scripts/run_sas.py
+-rw-r--r--   0 sastpw     (894) r&d        (100)       22 2024-04-08 19:58:03.000000 saspy-5.9.0/saspy/version.py
+drwxr-xr-x   0 sastpw     (894) r&d        (100)        0 2024-04-08 19:58:15.497511 saspy-5.9.0/saspy.egg-info/
+-rw-r--r--   0 sastpw     (894) r&d        (100)     4096 2024-04-08 19:58:15.000000 saspy-5.9.0/saspy.egg-info/PKG-INFO
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1451 2024-04-08 19:58:15.000000 saspy-5.9.0/saspy.egg-info/SOURCES.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        1 2024-04-08 19:58:15.000000 saspy-5.9.0/saspy.egg-info/dependency_links.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       41 2024-04-08 19:58:15.000000 saspy-5.9.0/saspy.egg-info/requires.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)        6 2024-04-08 19:58:15.000000 saspy-5.9.0/saspy.egg-info/top_level.txt
+-rw-r--r--   0 sastpw     (894) r&d        (100)       38 2024-04-08 19:58:15.498511 saspy-5.9.0/setup.cfg
+-rw-r--r--   0 sastpw     (894) r&d        (100)     1666 2024-04-08 19:58:03.000000 saspy-5.9.0/setup.py
```

### Comparing `saspy-5.7.0/LICENSE.md` & `saspy-5.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/PKG-INFO` & `saspy-5.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.7.0
+Version: 5.9.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.7.0/README.md` & `saspy-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/SASLogLexer.py` & `saspy-5.9.0/saspy/SASLogLexer.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/__init__.py` & `saspy-5.9.0/saspy/__init__.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/autocfg.py` & `saspy-5.9.0/saspy/autocfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar` & `saspy-5.9.0/saspy/java/iomclient/log4j-1.2-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar` & `saspy-5.9.0/saspy/java/iomclient/log4j-1.2-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/log4j-api-2.12.4.jar` & `saspy-5.9.0/saspy/java/iomclient/log4j-api-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/log4j-api-2.17.1.jar` & `saspy-5.9.0/saspy/java/iomclient/log4j-api-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/log4j-core-2.12.4.jar` & `saspy-5.9.0/saspy/java/iomclient/log4j-core-2.12.4.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/log4j-core-2.17.1.jar` & `saspy-5.9.0/saspy/java/iomclient/log4j-core-2.17.1.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/sas.core.jar` & `saspy-5.9.0/saspy/java/iomclient/sas.core.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/sas.security.sspi.jar` & `saspy-5.9.0/saspy/java/iomclient/sas.security.sspi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/iomclient/sas.svc.connection.jar` & `saspy-5.9.0/saspy/java/iomclient/sas.svc.connection.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/pyiom/cancel.class` & `saspy-5.9.0/saspy/java/pyiom/cancel.class`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/pyiom/cancel.java` & `saspy-5.9.0/saspy/java/pyiom/cancel.java`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/pyiom/saspy2j.class` & `saspy-5.9.0/saspy/java/pyiom/saspy2j.class`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/pyiom/saspy2j.java` & `saspy-5.9.0/saspy/java/pyiom/saspy2j.java`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/saspyiom.jar` & `saspy-5.9.0/saspy/java/saspyiom.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/thirdparty/NOTICE.md` & `saspy-5.9.0/saspy/java/thirdparty/NOTICE.md`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar` & `saspy-5.9.0/saspy/java/thirdparty/glassfish-corba-internal-api.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar` & `saspy-5.9.0/saspy/java/thirdparty/glassfish-corba-omgapi.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/thirdparty/glassfish-corba-orb.jar` & `saspy-5.9.0/saspy/java/thirdparty/glassfish-corba-orb.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/thirdparty/pfl-basic.jar` & `saspy-5.9.0/saspy/java/thirdparty/pfl-basic.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/java/thirdparty/pfl-tf.jar` & `saspy-5.9.0/saspy/java/thirdparty/pfl-tf.jar`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/libname_gen.sas` & `saspy-5.9.0/saspy/libname_gen.sas`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasViyaML.py` & `saspy-5.9.0/saspy/sasViyaML.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sas_magic.py` & `saspy-5.9.0/saspy/sas_magic.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasbase.py` & `saspy-5.9.0/saspy/sasbase.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sascfg.py` & `saspy-5.9.0/saspy/sascfg.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasdata.py` & `saspy-5.9.0/saspy/sasdata.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasdecorator.py` & `saspy-5.9.0/saspy/sasdecorator.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasets.py` & `saspy-5.9.0/saspy/sasets.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasexceptions.py` & `saspy-5.9.0/saspy/sasexceptions.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasiocom.py` & `saspy-5.9.0/saspy/sasiocom.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasiohttp.py` & `saspy-5.9.0/saspy/sasiohttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -819,26 +819,28 @@
          conn = self.sascfg.HTTPConn; conn.connect()
          headers={"Accept":"application/json","Authorization":"Bearer "+self.sascfg._token}
          conn.request('DELETE', self._uri_del, headers=headers)
          req = conn.getresponse()
          resp = req.read()
          conn.close()
 
-         self._refthd.join(5)
+         self._refthd.join(1)
 
          if self.sascfg.verbose:
             logger.info("SAS server terminated for SESSION_ID="+self._session.get('id'))
          self._session   = None
          self.pid        = None
          self._sb.SASpid = None
       return rc
 
    def _refresh_thread(self):
       while True:
          sleep(3000)
+         if self.pid is None:
+            return
          self._refresh_token()
 
    def _refresh_token(self):
       if not self.sascfg._refresh:
          return
       d1      = ("grant_type=refresh_token&refresh_token="+self.sascfg._refresh).encode(self.sascfg.encoding)
       client  = "Basic "+base64.encodebytes(("SASPy:").encode(self.sascfg.encoding)).splitlines()[0].decode(self.sascfg.encoding)
```

### Comparing `saspy-5.7.0/saspy/sasioiom.py` & `saspy-5.9.0/saspy/sasioiom.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from time import sleep
 import socket as socks
 import tempfile as tf
 import codecs
 import warnings
 import io
 import atexit
+from threading import Thread
 
 import logging
 logger = logging.getLogger('saspy')
 
 from saspy.sasexceptions import (SASDFNamesToLongError,
                                  SASIOConnectionTerminated
                                 )
@@ -67,14 +68,18 @@
       self.sspi      = cfg.get('sspi', False)
       self.javaparms = cfg.get('javaparms', '')
       self.lrecl     = cfg.get('lrecl', None)
       self.reconnect = cfg.get('reconnect', True)
       self.reconuri  = cfg.get('reconuri', None)
       self.logbufsz  = cfg.get('logbufsz', None)
       self.log4j     = cfg.get('log4j', '2.12.4')
+      self.keep      = cfg.get('keepalive', None)
+
+      if self.keep:
+         self.keep = int(self.keep)
 
       try:
          self.outopts = getattr(SAScfg, "SAS_output_options")
          self.output  = self.outopts.get('output', 'html5')
       except:
          self.output  = 'html5'
 
@@ -257,14 +262,21 @@
       inlogsz = kwargs.get('logbufsz', None)
       if inlogsz:
          if inlogsz < 32:
             self.logbufsz = 32
          else:
             self.logbufsz = inlogsz
 
+      inkeep = kwargs.get('keepalive', None)
+      if inkeep:
+         if lock and self.keep:
+            logger.warning("Parameter 'keepalive' passed to SAS_session was ignored due to configuration restriction.")
+         else:
+            self.keep = int(inkeep)
+
       self._prompt = session._sb.sascfg._prompt
 
       return
 
 class SASsessionIOM():
    """
    The SASsession object is the main object to instantiate and provides access to the rest of the functionality.
@@ -572,14 +584,19 @@
          if zero:
             logger.fatal("Be sure the path to sspiauth.dll is in your System PATH"+"\n")
          return None
 
       if self.sascfg.verbose:
          logger.info("SAS Connection established. Subprocess id is "+str(pid)+"\n")
 
+      if self.sascfg.keep:
+         self._keep = Thread(target=self._keepalive_thread, args=())
+         self._keep.daemon = True
+         self._keep.start()
+
       atexit.register(self._endsas)
 
       return self.pid
 
    def _endsas(self):
       rc = 0
       if self.pid:
@@ -632,14 +649,17 @@
                else:
                   if self.sascfg.verbose:
                      logger.info("SAS didn't shutdown w/in 5 seconds; killing it to be sure")
                   os.kill(self.pid, signal.SIGKILL)
          except:
             pass
 
+         if self.sascfg.keep:
+            self._keep.join(1)
+
          try: # Mac OS Python has bugs with this call
             self.stdin[0].shutdown(socks.SHUT_RDWR)
          except:
             pass
          self.stdin[0].close()
          self.sockin.close()
 
@@ -659,14 +679,20 @@
 
          if self.sascfg.verbose:
             logger.info("SAS Connection terminated. Subprocess id was "+str(pid))
          self.pid        = None
          self._sb.SASpid = None
       return
 
+   def _keepalive_thread(self):
+      while True:
+         sleep(self.sascfg.keep * 60)
+         if self.pid is None:
+            return
+         self.submit('', results='text')
 
    """
    def _getlog(self, wait=5, jobid=None):
       logf   = b''
       quit   = wait * 2
       logn   = self._logcnt(False)
       code1  = "%put E3969440A681A24088859985"+logn+";\nE3969440A681A24088859985"+logn
```

### Comparing `saspy-5.7.0/saspy/sasiostdio.py` & `saspy-5.9.0/saspy/sasiostdio.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasml.py` & `saspy-5.9.0/saspy/sasml.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasproccommons.py` & `saspy-5.9.0/saspy/sasproccommons.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasqc.py` & `saspy-5.9.0/saspy/sasqc.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasresults.py` & `saspy-5.9.0/saspy/sasresults.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasstat.py` & `saspy-5.9.0/saspy/sasstat.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sastabulate.py` & `saspy-5.9.0/saspy/sastabulate.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/sasutil.py` & `saspy-5.9.0/saspy/sasutil.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy/scripts/run_sas.py` & `saspy-5.9.0/saspy/scripts/run_sas.py`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/saspy.egg-info/PKG-INFO` & `saspy-5.9.0/saspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saspy
-Version: 5.7.0
+Version: 5.9.0
 Summary: A Python interface to SAS
 Home-page: https://github.com/sassoftware/saspy
 Author: Tom Weber
 Author-email: Tom.Weber@sas.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `saspy-5.7.0/saspy.egg-info/SOURCES.txt` & `saspy-5.9.0/saspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saspy-5.7.0/setup.py` & `saspy-5.9.0/setup.py`

 * *Files identical despite different names*

