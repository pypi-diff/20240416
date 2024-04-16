# Comparing `tmp/secure_sedge-1.8.2.tar.gz` & `tmp/secure_sedge-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_sedge-1.8.2.tar", last modified: Sun Feb 11 20:09:20 2024, max compression
+gzip compressed data, was "secure_sedge-1.8.3.tar", last modified: Tue Apr 16 16:02:31 2024, max compression
```

## Comparing `secure_sedge-1.8.2.tar` & `secure_sedge-1.8.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-11 20:09:20.869598 secure_sedge-1.8.2/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       86 2022-07-30 10:57:45.000000 secure_sedge-1.8.2/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6006 2024-02-11 20:09:20.869598 secure_sedge-1.8.2/PKG-INFO
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-11 20:09:20.869598 secure_sedge-1.8.2/docs/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     5165 2023-01-24 17:30:51.000000 secure_sedge-1.8.2/docs/index.rst
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-11 20:09:20.869598 secure_sedge-1.8.2/secure_sedge.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6006 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/secure_sedge.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      391 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/secure_sedge.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/secure_sedge.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       49 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/secure_sedge.egg-info/entry_points.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      160 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/secure_sedge.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/secure_sedge.egg-info/top_level.txt
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-02-11 20:09:20.869598 secure_sedge-1.8.2/sedge/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     4461 2023-02-21 19:50:49.000000 secure_sedge-1.8.2/sedge/README.md
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2021-08-03 07:09:12.000000 secure_sedge-1.8.2/sedge/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    34078 2024-02-11 20:07:35.000000 secure_sedge-1.8.2/sedge/cert_tasks.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    20131 2023-10-11 07:56:27.000000 secure_sedge-1.8.2/sedge/installers.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1217 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/sedge/main.py
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     6373 2023-12-02 09:35:36.000000 secure_sedge-1.8.2/sedge/sedge_client.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        6 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/sedge/version.txt
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       84 2024-02-11 20:09:20.869598 secure_sedge-1.8.2/setup.cfg
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2673 2024-02-11 20:09:20.000000 secure_sedge-1.8.2/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-04-16 16:02:31.026298 secure_sedge-1.8.3/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       86 2022-07-30 10:57:45.000000 secure_sedge-1.8.3/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     6006 2024-04-16 16:02:31.026298 secure_sedge-1.8.3/PKG-INFO
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-04-16 16:02:31.026298 secure_sedge-1.8.3/docs/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     5165 2023-01-24 17:30:51.000000 secure_sedge-1.8.3/docs/index.rst
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-04-16 16:02:31.026298 secure_sedge-1.8.3/secure_sedge.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     6006 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/secure_sedge.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      391 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/secure_sedge.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/secure_sedge.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       49 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/secure_sedge.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      160 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/secure_sedge.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        6 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/secure_sedge.egg-info/top_level.txt
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2024-04-16 16:02:31.026298 secure_sedge-1.8.3/sedge/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     4461 2023-02-21 19:50:49.000000 secure_sedge-1.8.3/sedge/README.md
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2021-08-03 07:09:12.000000 secure_sedge-1.8.3/sedge/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    34358 2024-04-16 16:01:49.000000 secure_sedge-1.8.3/sedge/cert_tasks.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)    20131 2023-10-11 07:56:27.000000 secure_sedge-1.8.3/sedge/installers.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1217 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/sedge/main.py
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     6373 2023-12-02 09:35:36.000000 secure_sedge-1.8.3/sedge/sedge_client.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        6 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/sedge/version.txt
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       84 2024-04-16 16:02:31.026298 secure_sedge-1.8.3/setup.cfg
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2673 2024-04-16 16:02:30.000000 secure_sedge-1.8.3/setup.py
```

### Comparing `secure_sedge-1.8.2/PKG-INFO` & `secure_sedge-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_sedge
-Version: 1.8.2
+Version: 1.8.3
 Summary: a helpful set of convocations to create certs
 Home-page: https://bitbucket.org/dbuy/secure_sedge
 Author: 2ps
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `secure_sedge-1.8.2/docs/index.rst` & `secure_sedge-1.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.8.2/secure_sedge.egg-info/PKG-INFO` & `secure_sedge-1.8.3/secure_sedge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-sedge
-Version: 1.8.2
+Version: 1.8.3
 Summary: a helpful set of convocations to create certs
 Home-page: https://bitbucket.org/dbuy/secure_sedge
 Author: 2ps
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `secure_sedge-1.8.2/sedge/README.md` & `secure_sedge-1.8.3/sedge/README.md`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.8.2/sedge/cert_tasks.py` & `secure_sedge-1.8.3/sedge/cert_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,14 +387,15 @@
                     break
             if not included:
                 domains.append({
                     'name': hostname,
                     'profile': profile,
                 })
         else:
+            domains = []
             included = False
             for x in alt_domains:
                 domains.append({ 'name': x, 'profile': profile })
                 if x == hostname:
                     included = True
             if not included:
                 domains.append({
@@ -471,15 +472,15 @@
     save_to_temp(tmp_dir, filename, content)
     if isinstance(content, str):
         content = content.encode('utf-8')
     s3_key = posixpath.join(ns, filename)
     s3.put_object(Bucket=bucket, Key=s3_key, Body=content, ACL='bucket-owner-full-control')
 
 
-def full_pfx(ctx, certificate, key, password=None, chain=None, legacy=False):
+def full_pfx(ctx, certificate, key, password=None, chain=None, legacy=False, include_chain=True):
     from cryptography.x509 import load_pem_x509_certificates
     from cryptography.hazmat.primitives import hashes
     from cryptography.hazmat.primitives.serialization import (
         BestAvailableEncryption,
         load_pem_private_key,
         NoEncryption,
         pkcs12,
@@ -491,14 +492,16 @@
         certs = load_pem_x509_certificates(certificate.encode('utf-8'))
     else:
         certs = [ certificate ]
         if chain:
             certs += chain
     if isinstance(key, str):
         key = load_pem_private_key(key.encode('utf-8'), password=None)
+    if not include_chain:
+        certs = certs[:1]
     encryption = NoEncryption()
     if password:
         if legacy:
             alg = pkcs12.PBES.PBESv1SHA1And3KeyTripleDESCBC
             encryption = PrivateFormat.PKCS12.encryption_builder()
             encryption = encryption.kdf_rounds(50000)
             encryption = encryption.key_cert_algorithm(alg)
@@ -673,18 +676,22 @@
     """
     extensions = [ '', '.alt', '.02', '.03', '.04', '.05', ]
     session = Session(profile_name=profile)
     if role:
         session = assume_role(session, role)
     s3 = session.client('s3')
     for i, certificate in enumerate(certificates):
-        pfx_content = full_pfx(ctx, certificate, key, pfx_password)
+        pfx_content = full_pfx(
+            ctx, certificate, key, pfx_password,
+            include_chain=False, legacy=True)
+        modern_pfx_content = full_pfx(ctx, certificate, key, pfx_password)
         contents = [
             (f'{extensions[i]}.crt', certificate),
             ('.pfx', pfx_content),
+            ('.modern.pfx', modern_pfx_content),
         ]
         for extension, content in contents:
             filename = f'{hostname}{extension}'
             filename = filename.replace('*', 'star')
             filename = posixpath.join(ns, filename)
             log.info('saving s3://%s/%s', bucket, filename)
             if isinstance(content, str):
```

### Comparing `secure_sedge-1.8.2/sedge/installers.py` & `secure_sedge-1.8.3/sedge/installers.py`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.8.2/sedge/main.py` & `secure_sedge-1.8.3/sedge/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
             'handlers': [ 'console-brief', ],
             'propagate': False,
         }
     }
 ))
 ns = Collection.from_module(cert_tasks)
 ns.add_collection(installers.installers_collection, 'install')
-program = Program(version='1.8.2', namespace=ns)
+program = Program(version='1.8.3', namespace=ns)
```

### Comparing `secure_sedge-1.8.2/sedge/sedge_client.py` & `secure_sedge-1.8.3/sedge/sedge_client.py`

 * *Files identical despite different names*

### Comparing `secure_sedge-1.8.2/setup.py` & `secure_sedge-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     from pkg_resources import resource_string
     readme_text = resource_string('sedge', 'README.md')
     readme_text = readme_text.decode('utf-8')
 
 # Version info -- read without importing
 _locals = {}
-version = '1.8.2'
+version = '1.8.3'
 
 
 # PyYAML ships a split Python 2/3 codebase. Unfortunately, some pip versions
 # attempt to interpret both halves of PyYAML, yielding SyntaxErrors. Thus, we
 # exclude whichever appears inappropriate for the installing interpreter.
 exclude = ['*.yaml2', 'tests']
```

