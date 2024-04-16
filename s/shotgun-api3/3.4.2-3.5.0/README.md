# Comparing `tmp/shotgun_api3-3.4.2.tar.gz` & `tmp/shotgun_api3-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shotgun_api3-3.4.2.tar", last modified: Sat Feb 17 02:18:44 2024, max compression
+gzip compressed data, was "shotgun_api3-3.5.0.tar", last modified: Tue Apr 16 01:43:10 2024, max compression
```

## Comparing `shotgun_api3-3.4.2.tar` & `shotgun_api3-3.5.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.228095 shotgun_api3-3.4.2/shotgun_api3/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.228095 shotgun_api3-3.4.2/shotgun_api3/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.232095 shotgun_api3-3.4.2/shotgun_api3/lib/certifi/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/certifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/certifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   281617 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/certifi/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/certifi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/certifi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.232095 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   137365 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/cacerts.txt
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/iri2uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.232095 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/
--rw-r--r--   0 runner    (1001) docker     (127)    74660 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   137365 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/cacerts.txt
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/iri2uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/socks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/
--rw-r--r--   0 runner    (1001) docker     (127)    69389 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   137365 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/cacerts.txt
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/iri2uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/mimetypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    35381 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/mockgun.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)   273322 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/sgsix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/sgtimezone.py
--rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/lib/six.py
--rw-r--r--   0 runner    (1001) docker     (127)   196024 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/shotgun_api3/shotgun.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/shotgun_api3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-02-17 02:18:44.000000 shotgun_api3-3.4.2/shotgun_api3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-02-17 02:18:44.000000 shotgun_api3-3.4.2/shotgun_api3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 02:18:44.000000 shotgun_api3-3.4.2/shotgun_api3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 02:18:44.000000 shotgun_api3-3.4.2/shotgun_api3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-17 02:18:44.000000 shotgun_api3-3.4.2/shotgun_api3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 02:18:44.236095 shotgun_api3-3.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   118919 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/tests/test_api_long.py
--rw-r--r--   0 runner    (1001) docker     (127)    28007 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/tests/test_mockgun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-02-17 02:18:36.000000 shotgun_api3-3.4.2/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.150931 shotgun_api3-3.5.0/shotgun_api3/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.154931 shotgun_api3-3.5.0/shotgun_api3/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.154931 shotgun_api3-3.5.0/shotgun_api3/lib/certifi/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/certifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/certifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   281617 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/certifi/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/certifi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/certifi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.158931 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137365 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/cacerts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/iri2uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.158931 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/
+-rw-r--r--   0 runner    (1001) docker     (127)    74660 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137365 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/cacerts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/iri2uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/socks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/
+-rw-r--r--   0 runner    (1001) docker     (127)    69389 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137365 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/cacerts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/iri2uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/mimetypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35413 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/mockgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)   273322 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/sgsix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/sgtimezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/lib/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196127 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/shotgun_api3/shotgun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/shotgun_api3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-16 01:43:10.000000 shotgun_api3-3.5.0/shotgun_api3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-16 01:43:10.000000 shotgun_api3-3.5.0/shotgun_api3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:43:10.000000 shotgun_api3-3.5.0/shotgun_api3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:43:09.000000 shotgun_api3-3.5.0/shotgun_api3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 01:43:10.000000 shotgun_api3-3.5.0/shotgun_api3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:43:10.162931 shotgun_api3-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   118928 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/tests/test_api_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28009 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/tests/test_mockgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-04-16 01:43:06.000000 shotgun_api3-3.5.0/tests/test_unit.py
```

### Comparing `shotgun_api3-3.4.2/LICENSE` & `shotgun_api3-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/PKG-INFO` & `shotgun_api3-3.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shotgun_api3
-Version: 3.4.2
-Summary: ShotGrid Python API 
+Version: 3.5.0
+Summary: Flow Production Tracking Python API 
 Home-page: https://github.com/shotgunsoftware/python-api
-Author: ShotGrid Software
+Author: Autodesk
 License: Copyright (c) 2009-2011, Shotgun Software Inc
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
          - Redistributions of source code must retain the above copyright notice, this
@@ -63,17 +63,17 @@
 
 [![VFX Platform](https://img.shields.io/badge/vfxplatform-2024%20%7C%202023%20%7C%202022%20%7C%202021-blue.svg)](http://www.vfxplatform.com/)
 [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/)
 [![Reference Documentation](http://img.shields.io/badge/doc-reference-blue.svg)](http://developer.shotgridsoftware.com/python-api)
 [![Build Status](https://dev.azure.com/shotgun-ecosystem/Python%20API/_apis/build/status/shotgunsoftware.python-api?branchName=master)](https://dev.azure.com/shotgun-ecosystem/Python%20API/_build/latest?definitionId=108&branchName=master)
 [![Coverage Status](https://coveralls.io/repos/github/shotgunsoftware/python-api/badge.svg?branch=master)](https://coveralls.io/github/shotgunsoftware/python-api?branch=master)
 
-# ShotGrid Python API
+# Flow Production Tracking Python API
 
-ShotGrid provides a simple Python-based API for accessing ShotGrid and integrating with other tools. This is the official API that is maintained by ShotGrid Software (https://knowledge.autodesk.com/contact-support)
+Autodesk provides a simple Python-based API for accessing Flow Production Tracking and integrating with other tools. This is the official API that is maintained by Autodesk (https://knowledge.autodesk.com/contact-support)
 
 The latest version can always be found at http://github.com/shotgunsoftware/python-api
 
 ## Minimum Requirements
 
 * Python v3.7
 
@@ -107,16 +107,16 @@
 - All tests require:
     - The [nose unit testing tools](http://nose.readthedocs.org),
     - The [nose-exclude nose plugin](https://pypi.org/project/nose-exclude/)
     - (Note: Running `pip install -r tests/ci_requirements.txt` will install this package)
 - A `tests/config` file (you can copy an example from `tests/example_config`).
 - Tests can be run individually like this: `nosetests --config="nose.cfg" tests/test_client.py`
     - Make sure to not forget the `--config="nose.cfg"` option. This option tells nose to use our config file.  This will exclude python 2- and 3-specific files in the `/lib` directory, preventing a failure from being reported by nose for compilation due to incompatible syntax in those files.
-- `test_client` and `tests_unit` use mock server interaction and do not require a ShotGrid instance to be available (no modifications to `tests/config` are necessary).
-- `test_api` and `test_api_long` *do* require a ShotGrid instance, with a script key available for the tests. The server and script user values must be supplied in the `tests/config` file. The tests will add test data to your server based on information in your config. This data will be manipulated by the tests, and should not be used for other purposes.
+- `test_client` and `tests_unit` use mock server interaction and do not require a Flow Production Tracking instance to be available (no modifications to `tests/config` are necessary).
+- `test_api` and `test_api_long` *do* require a Flow Production Tracking instance, with a script key available for the tests. The server and script user values must be supplied in the `tests/config` file. The tests will add test data to your server based on information in your config. This data will be manipulated by the tests, and should not be used for other purposes.
 - To run all of the tests, use the shell script `run-tests`.
 
 ## Release process
 
 ### Packaging up new release
 
 1) Update the Changelog in the `HISTORY.rst` file
```

### Comparing `shotgun_api3-3.4.2/README.md` & `shotgun_api3-3.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [![VFX Platform](https://img.shields.io/badge/vfxplatform-2024%20%7C%202023%20%7C%202022%20%7C%202021-blue.svg)](http://www.vfxplatform.com/)
 [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/)
 [![Reference Documentation](http://img.shields.io/badge/doc-reference-blue.svg)](http://developer.shotgridsoftware.com/python-api)
 [![Build Status](https://dev.azure.com/shotgun-ecosystem/Python%20API/_apis/build/status/shotgunsoftware.python-api?branchName=master)](https://dev.azure.com/shotgun-ecosystem/Python%20API/_build/latest?definitionId=108&branchName=master)
 [![Coverage Status](https://coveralls.io/repos/github/shotgunsoftware/python-api/badge.svg?branch=master)](https://coveralls.io/github/shotgunsoftware/python-api?branch=master)
 
-# ShotGrid Python API
+# Flow Production Tracking Python API
 
-ShotGrid provides a simple Python-based API for accessing ShotGrid and integrating with other tools. This is the official API that is maintained by ShotGrid Software (https://knowledge.autodesk.com/contact-support)
+Autodesk provides a simple Python-based API for accessing Flow Production Tracking and integrating with other tools. This is the official API that is maintained by Autodesk (https://knowledge.autodesk.com/contact-support)
 
 The latest version can always be found at http://github.com/shotgunsoftware/python-api
 
 ## Minimum Requirements
 
 * Python v3.7
 
@@ -44,16 +44,16 @@
 - All tests require:
     - The [nose unit testing tools](http://nose.readthedocs.org),
     - The [nose-exclude nose plugin](https://pypi.org/project/nose-exclude/)
     - (Note: Running `pip install -r tests/ci_requirements.txt` will install this package)
 - A `tests/config` file (you can copy an example from `tests/example_config`).
 - Tests can be run individually like this: `nosetests --config="nose.cfg" tests/test_client.py`
     - Make sure to not forget the `--config="nose.cfg"` option. This option tells nose to use our config file.  This will exclude python 2- and 3-specific files in the `/lib` directory, preventing a failure from being reported by nose for compilation due to incompatible syntax in those files.
-- `test_client` and `tests_unit` use mock server interaction and do not require a ShotGrid instance to be available (no modifications to `tests/config` are necessary).
-- `test_api` and `test_api_long` *do* require a ShotGrid instance, with a script key available for the tests. The server and script user values must be supplied in the `tests/config` file. The tests will add test data to your server based on information in your config. This data will be manipulated by the tests, and should not be used for other purposes.
+- `test_client` and `tests_unit` use mock server interaction and do not require a Flow Production Tracking instance to be available (no modifications to `tests/config` are necessary).
+- `test_api` and `test_api_long` *do* require a Flow Production Tracking instance, with a script key available for the tests. The server and script user values must be supplied in the `tests/config` file. The tests will add test data to your server based on information in your config. This data will be manipulated by the tests, and should not be used for other purposes.
 - To run all of the tests, use the shell script `run-tests`.
 
 ## Release process
 
 ### Packaging up new release
 
 1) Update the Changelog in the `HISTORY.rst` file
```

### Comparing `shotgun_api3-3.4.2/setup.py` & `shotgun_api3-3.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 if (sys.version_info[0] <= 2) or (sys.version_info[0] == 2 and sys.version_info[1] <= 5):
     if 'install' in script_args and '--no-compile' not in script_args:
         script_args.append('--no-compile')
 
 
 setup(
     name='shotgun_api3',
-    version='3.4.2',
-    description='ShotGrid Python API ',
+    version='3.5.0',
+    description='Flow Production Tracking Python API ',
     long_description=readme,
     long_description_content_type='text/markdown',
-    author='ShotGrid Software',
+    author='Autodesk',
     url='https://github.com/shotgunsoftware/python-api',
     license=license,
     packages=find_packages(exclude=('tests',)),
     script_args=script_args,
     include_package_data=True,
     package_data={'': ['cacerts.txt', 'cacert.pem']},
     zip_safe=False,
```

### Comparing `shotgun_api3-3.4.2/shotgun_api3/__init__.py` & `shotgun_api3-3.5.0/shotgun_api3/__init__.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/certifi/cacert.pem` & `shotgun_api3-3.5.0/shotgun_api3/lib/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/certifi/core.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/certifi/core.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/__init__.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/auth.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/auth.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/cacerts.txt` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/certs.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/certs.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/error.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/error.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/iri2uri.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/__init__.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/__init__.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/auth.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/auth.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/cacerts.txt` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/certs.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/certs.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/error.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/error.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/iri2uri.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python2/socks.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python2/socks.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/__init__.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/__init__.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/auth.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/auth.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/cacerts.txt` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/cacerts.txt`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/certs.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/certs.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/error.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/error.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/iri2uri.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/iri2uri.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/python3/socks.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/python3/socks.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/httplib2/socks.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/mimetypes.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/mimetypes.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/__init__.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/__init__.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/errors.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/errors.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/mockgun.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/mockgun.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
         # load in the shotgun schema to associate with this Shotgun
         (schema_path, schema_entity_path) = self.get_schema_paths()
 
         if schema_path is None or schema_entity_path is None:
             raise MockgunError("Cannot create Mockgun instance because no schema files have been defined. "
                                "Before creating a Mockgun instance, please call Mockgun.set_schema_paths() "
-                               "in order to specify which ShotGrid schema Mockgun should operate against.")
+                               "in order to specify which Flow Production Tracking schema Mockgun should operate against.")
 
         self._schema, self._schema_entity = SchemaFactory.get_schemas(schema_path, schema_entity_path)
 
         # initialize the "database"
         self._db = dict((entity, {}) for entity in self._schema)
 
         # set some basic public members that exist in the Shotgun API
@@ -500,15 +500,15 @@
                                    "date": datetime.date,
                                    "date_time": datetime.datetime,
                                    "list": six.string_types,
                                    "status_list": six.string_types,
                                    "url": dict}[sg_type]
                 except KeyError:
                     raise ShotgunError(
-                        "Field %s.%s: Handling for ShotGrid type %s is not implemented" %
+                        "Field %s.%s: Handling for Flow Production Tracking type %s is not implemented" %
                         (entity_type, field, sg_type)
                     )
 
                 if not isinstance(item, python_type):
                     raise ShotgunError(
                         "%s.%s is of type %s, but data %s is not of type %s" %
                         (entity_type, field, type(item), sg_type, python_type)
```

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/mockgun/schema.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/mockgun/schema.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/pyparsing.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/pyparsing.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/sgsix.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/sgsix.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/sgtimezone.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/sgtimezone.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/lib/six.py` & `shotgun_api3-3.5.0/shotgun_api3/lib/six.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/shotgun_api3/shotgun.py` & `shotgun_api3-3.5.0/shotgun_api3/shotgun.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         raise ImportError("%s. SHOTGUN_FORCE_CERTIFICATE_VALIDATION environment variable prevents "
                           "disabling SSL certificate validation." % e)
     LOG.debug("ssl not found, disabling certificate validation")
     NO_SSL_VALIDATION = True
 
 # ----------------------------------------------------------------------------
 # Version
-__version__ = "3.4.2"
+__version__ = "3.5.0"
 
 # ----------------------------------------------------------------------------
 # Errors
 
 
 class ShotgunError(Exception):
     """
@@ -220,18 +220,18 @@
         # Version from server is major.minor.rev or major.minor.rev."Dev"
         # Store version as tuple and check dev flag
         try:
             self.version = meta.get("version", None)
         except AttributeError:
             self.version = None
         if not self.version:
-            raise ShotgunError("The ShotGrid Server didn't respond with a version number. "
+            raise ShotgunError("The Flow Production Tracking Server didn't respond with a version number. "
                                "This may be because you are running an older version of "
-                               "ShotGrid against a more recent version of the ShotGrid API. "
-                               "For more information, please contact ShotGrid Support.")
+                               "Flow Production Tracking against a more recent version of the Flow Production Tracking API. "
+                               "For more information, please contact the Autodesk support.")
 
         if len(self.version) > 3 and self.version[3] == "Dev":
             self.is_dev = True
         else:
             self.is_dev = False
 
         self.version = tuple(self.version[:3])
@@ -335,15 +335,15 @@
     .. warning::
 
         This class is part of the internal API and its interfaces may change at any time in
         the future. Therefore, usage of this class is discouraged.
 
     :ivar str platform: The current client platform. Valid values are ``mac``, ``linux``,
         ``windows``, or ``None`` (if the current platform couldn't be determined).
-    :ivar str local_path_field: The SG field used for local file paths. This is calculated using
+    :ivar str local_path_field: The PTR field used for local file paths. This is calculated using
         the value of ``platform``. Ex. ``local_path_mac``.
     :ivar str py_version: Simple version of Python executable as a string. Eg. ``2.7``.
     :ivar str ssl_version: Version of OpenSSL installed. Eg. ``OpenSSL 1.0.2g  1 Mar 2016``. This
         info is only available in Python 2.7+ if the ssl module was imported successfully.
         Defaults to ``unknown``
     """
 
@@ -3437,16 +3437,16 @@
             LOG.debug("Completed rpc call to %s" % (method))
 
             try:
                 self._parse_http_status(http_status)
             except ProtocolError as e:
                 e.headers = resp_headers
 
-                # We've seen some rare instances of SG returning 502 for issues that
-                # appear to be caused by something internal to SG. We're going to
+                # We've seen some rare instances of PTR returning 502 for issues that
+                # appear to be caused by something internal to PTR. We're going to
                 # allow for limited retries for those specifically.
                 if attempt != max_attempts and e.errcode in [502, 504]:
                     LOG.debug("Got a 502 or 504 response. Waiting and retrying...")
                     time.sleep(float(attempt) * backoff)
                     attempt += 1
                     continue
                 elif e.errcode == 403:
@@ -3675,15 +3675,15 @@
         """
         error_code = status[0]
         errmsg = status[1]
 
         if status[0] >= 300:
             headers = "HTTP error from server"
             if status[0] == 503:
-                errmsg = "ShotGrid is currently down for maintenance or too busy to reply. Please try again later."
+                errmsg = "Flow Production Tracking is currently down for maintenance or too busy to reply. Please try again later."
             raise ProtocolError(self.config.server,
                                 error_code,
                                 errmsg,
                                 headers)
 
         return
 
@@ -3761,20 +3761,20 @@
                 raise MissingTwoFactorAuthenticationFault(
                     sg_response.get("message", "Unknown 2FA Authentication Error")
                 )
             elif sg_response.get("error_code") == ERR_SSO:
                 raise UserCredentialsNotAllowedForSSOAuthenticationFault(
                     sg_response.get("message",
                                     "Authentication using username/password is not "
-                                    "allowed for an SSO-enabled ShotGrid site")
+                                    "allowed for an SSO-enabled Flow Production Tracking site")
                 )
             elif sg_response.get("error_code") == ERR_OXYG:
                 raise UserCredentialsNotAllowedForOxygenAuthenticationFault(
                     sg_response.get("message", "Authentication using username/password is not "
-                                    "allowed for an Autodesk Identity enabled ShotGrid site")
+                                    "allowed for an Autodesk Identity enabled Flow Production Tracking site")
                 )
             else:
                 # raise general Fault
                 raise Fault(sg_response.get("message", "Unknown Error"))
         return
 
     def _visit_data(self, data, visitor):
```

### Comparing `shotgun_api3-3.4.2/shotgun_api3.egg-info/PKG-INFO` & `shotgun_api3-3.5.0/shotgun_api3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shotgun_api3
-Version: 3.4.2
-Summary: ShotGrid Python API 
+Version: 3.5.0
+Summary: Flow Production Tracking Python API 
 Home-page: https://github.com/shotgunsoftware/python-api
-Author: ShotGrid Software
+Author: Autodesk
 License: Copyright (c) 2009-2011, Shotgun Software Inc
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
          - Redistributions of source code must retain the above copyright notice, this
@@ -63,17 +63,17 @@
 
 [![VFX Platform](https://img.shields.io/badge/vfxplatform-2024%20%7C%202023%20%7C%202022%20%7C%202021-blue.svg)](http://www.vfxplatform.com/)
 [![Python](https://img.shields.io/badge/python-3.7%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/)
 [![Reference Documentation](http://img.shields.io/badge/doc-reference-blue.svg)](http://developer.shotgridsoftware.com/python-api)
 [![Build Status](https://dev.azure.com/shotgun-ecosystem/Python%20API/_apis/build/status/shotgunsoftware.python-api?branchName=master)](https://dev.azure.com/shotgun-ecosystem/Python%20API/_build/latest?definitionId=108&branchName=master)
 [![Coverage Status](https://coveralls.io/repos/github/shotgunsoftware/python-api/badge.svg?branch=master)](https://coveralls.io/github/shotgunsoftware/python-api?branch=master)
 
-# ShotGrid Python API
+# Flow Production Tracking Python API
 
-ShotGrid provides a simple Python-based API for accessing ShotGrid and integrating with other tools. This is the official API that is maintained by ShotGrid Software (https://knowledge.autodesk.com/contact-support)
+Autodesk provides a simple Python-based API for accessing Flow Production Tracking and integrating with other tools. This is the official API that is maintained by Autodesk (https://knowledge.autodesk.com/contact-support)
 
 The latest version can always be found at http://github.com/shotgunsoftware/python-api
 
 ## Minimum Requirements
 
 * Python v3.7
 
@@ -107,16 +107,16 @@
 - All tests require:
     - The [nose unit testing tools](http://nose.readthedocs.org),
     - The [nose-exclude nose plugin](https://pypi.org/project/nose-exclude/)
     - (Note: Running `pip install -r tests/ci_requirements.txt` will install this package)
 - A `tests/config` file (you can copy an example from `tests/example_config`).
 - Tests can be run individually like this: `nosetests --config="nose.cfg" tests/test_client.py`
     - Make sure to not forget the `--config="nose.cfg"` option. This option tells nose to use our config file.  This will exclude python 2- and 3-specific files in the `/lib` directory, preventing a failure from being reported by nose for compilation due to incompatible syntax in those files.
-- `test_client` and `tests_unit` use mock server interaction and do not require a ShotGrid instance to be available (no modifications to `tests/config` are necessary).
-- `test_api` and `test_api_long` *do* require a ShotGrid instance, with a script key available for the tests. The server and script user values must be supplied in the `tests/config` file. The tests will add test data to your server based on information in your config. This data will be manipulated by the tests, and should not be used for other purposes.
+- `test_client` and `tests_unit` use mock server interaction and do not require a Flow Production Tracking instance to be available (no modifications to `tests/config` are necessary).
+- `test_api` and `test_api_long` *do* require a Flow Production Tracking instance, with a script key available for the tests. The server and script user values must be supplied in the `tests/config` file. The tests will add test data to your server based on information in your config. This data will be manipulated by the tests, and should not be used for other purposes.
 - To run all of the tests, use the shell script `run-tests`.
 
 ## Release process
 
 ### Packaging up new release
 
 1) Update the Changelog in the `HISTORY.rst` file
```

### Comparing `shotgun_api3-3.4.2/shotgun_api3.egg-info/SOURCES.txt` & `shotgun_api3-3.5.0/shotgun_api3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/tests/test_api.py` & `shotgun_api3-3.5.0/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1733,15 +1733,15 @@
             self.assertEqual(1, len(result))
             self.assertEqual(human_user['id'], result[0]['id'])
 
     def test_following(self):
         '''Test following method'''
 
         if not self.sg.server_caps.version or self.sg.server_caps.version < (7, 0, 12):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         with self.gen_entity(
             "HumanUser",
             projects=[self.project],
         ) as human_user, self.gen_entity(
             "Shot",
@@ -2603,15 +2603,15 @@
 class TestReadAdditionalFilterPresets(base.LiveTestBase):
     """
     Unit tests for the additional_filter_presets read parameter
     """
 
     def test_simple_case(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2622,15 +2622,15 @@
         versions = self.sg.find("Version", filters, fields=fields, additional_filter_presets=additional_filters)
         version = versions[0]
         self.assertEqual("Version", version["type"])
         self.assertEqual(self.version["id"], version["id"])
 
     def test_find_one(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2640,15 +2640,15 @@
 
         version = self.sg.find_one("Version", filters, fields=fields, additional_filter_presets=additional_filters)
         self.assertEqual("Version", version["type"])
         self.assertEqual(self.version["id"], version["id"])
 
     def test_filter_with_no_name(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2658,15 +2658,15 @@
 
         self.assertRaises(shotgun_api3.Fault,
                           self.sg.find,
                           "Version", filters, fields=fields, additional_filter_presets=additional_filters)
 
     def test_invalid_filter(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2676,15 +2676,15 @@
 
         self.assertRaises(shotgun_api3.Fault,
                           self.sg.find,
                           "Version", filters, fields=fields, additional_filter_presets=additional_filters)
 
     def test_filter_not_iterable(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2694,15 +2694,15 @@
 
         self.assertRaises(shotgun_api3.Fault,
                           self.sg.find,
                           "Version", filters, fields=fields, additional_filter_presets=additional_filters)
 
     def test_filter_not_list_of_iterable(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2712,15 +2712,15 @@
 
         self.assertRaises(shotgun_api3.Fault,
                           self.sg.find,
                           "Version", filters, fields=fields, additional_filter_presets=additional_filters)
 
     def test_multiple_latest_filters(self):
         if self.sg_version < (7, 0, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         filters = [
             ["project", "is", self.project],
             ["id", "is", self.version["id"]]
         ]
 
@@ -2736,15 +2736,15 @@
     def test_modify_visibility(self):
         """
         Ensure the visibility of a field can be edited via the API.
         """
         # If the version of Shotgun is too old, do not run this test.
         # TODO: Update this with the real version number once the feature is released.
         if self.sg_version < (8, 5, 0):
-            warnings.warn("Test bypassed because SG server used does not support this feature.", FutureWarning)
+            warnings.warn("Test bypassed because PTR server used does not support this feature.", FutureWarning)
             return
 
         field_display_name = "Project Visibility Test"
         field_name = "sg_{0}".format(field_display_name.lower().replace(" ", "_"))
 
         schema = self.sg.schema_field_read("Asset")
         # Ensure the custom field exists.
```

### Comparing `shotgun_api3-3.4.2/tests/test_api_long.py` & `shotgun_api3-3.5.0/tests/test_api_long.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/tests/test_client.py` & `shotgun_api3-3.5.0/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,25 +240,25 @@
         args, _ = self.sg._http_request.call_args
         verb, path, body, headers = args
 
         expected = "Basic " + b64encode(urllib.parse.unquote(login_password)).strip()
         self.assertEqual(expected, headers.get("Authorization"))
 
     def test_localization_header_default(self):
-        """Localization header not passed to server without explicitly setting SG localization config to True"""
+        """Localization header not passed to server without explicitly setting PTR localization config to True"""
         self.sg.info()
 
         args, _ = self.sg._http_request.call_args
         (_, _, _, headers) = args
         expected_header_value = "auto"
 
         self.assertEqual(None, headers.get("locale"))
 
     def test_localization_header_when_localized(self):
-        """Localization header passed to server when setting SG localization config to True"""
+        """Localization header passed to server when setting PTR localization config to True"""
         self.sg.config.localized = True
 
         self.sg.info()
 
         args, _ = self.sg._http_request.call_args
         (_, _, _, headers) = args
         expected_header_value = "auto"
```

### Comparing `shotgun_api3-3.4.2/tests/test_mockgun.py` & `shotgun_api3-3.5.0/tests/test_mockgun.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/tests/test_proxy.py` & `shotgun_api3-3.5.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `shotgun_api3-3.4.2/tests/test_unit.py` & `shotgun_api3-3.5.0/tests/test_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         http = Http(ca_certs=certs)
         return http.request(url)
 
     def _check_url_with_urllib(self, url):
         """
         Given a url it will perform a simple request and return a result.
         """
-        # create a request using the opener generated by the SG API.
+        # create a request using the opener generated by the PTR API.
         # The `_build_opener` method internally should use the correct certs.
         opener = self.sg._build_opener(urllib.request.HTTPHandler)
         request = urllib.request.Request(url)
         return opener.open(request)
 
     def test_found_correct_cert(self):
         """
@@ -456,15 +456,15 @@
         cert_path = os.path.normpath(
             # Get the path relative to where we picked up the API and not relative
             # to file on disk. On CI we pip install the API to run the tests
             # so we have to pick the location from the installed copy.
             # Call dirname to remove from __init__.py
             os.path.join(os.path.dirname(api.__file__), "lib", "certifi", "cacert.pem")
         )
-        # Now ensure that the path the SG API has found is correct.
+        # Now ensure that the path the PTR API has found is correct.
         self.assertEqual(cert_path, self.certs)
         self.assertTrue(os.path.isfile(self.certs))
 
     def test_httplib(self):
         """
         Checks that we can access the amazon urls using our bundled
         certificate with httplib.
```

