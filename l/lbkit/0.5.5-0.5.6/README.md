# Comparing `tmp/lbkit-0.5.5.tar.gz` & `tmp/lbkit-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbkit-0.5.5.tar", last modified: Sat Apr 13 15:08:04 2024, max compression
+gzip compressed data, was "lbkit-0.5.6.tar", last modified: Tue Apr 16 16:17:49 2024, max compression
```

## Comparing `lbkit-0.5.5.tar` & `lbkit-0.5.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.931476 lbkit-0.5.5/
--rw-rw-r--   0 root         (0) root         (0)      122 2024-04-13 15:07:56.000000 lbkit-0.5.5/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)    11357 2024-04-13 15:07:56.000000 lbkit-0.5.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      149 2024-04-13 15:07:56.000000 lbkit-0.5.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-13 15:08:04.927476 lbkit-0.5.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      388 2024-04-13 15:07:56.000000 lbkit-0.5.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.923476 lbkit-0.5.5/lbkit/
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-13 15:07:57.000000 lbkit-0.5.5/lbkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.923476 lbkit-0.5.5/lbkit/ci_robot/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/ci_robot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12840 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/ci_robot/gitee.py
--rw-rw-r--   0 root         (0) root         (0)     8454 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/codegen/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3881 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/codegen.py
--rw-rw-r--   0 root         (0) root         (0)     7893 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/ctype_defination.py
--rw-rw-r--   0 root         (0) root         (0)    23132 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/idf_interface.py
--rw-rw-r--   0 root         (0) root         (0)      287 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/codegen/template/
--rw-rw-r--   0 root         (0) root         (0)     5781 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/client.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2888 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/client.h.mako
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/interface.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2297 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/interface.introspect.xml.mako
--rw-rw-r--   0 root         (0) root         (0)    26271 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/public.c.mako
--rw-rw-r--   0 root         (0) root         (0)     8106 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/public.h.mako
--rw-rw-r--   0 root         (0) root         (0)    12974 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/server.c.mako
--rw-rw-r--   0 root         (0) root         (0)     1492 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/codegen/template/server.h.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/component/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2155 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/arg_parser.py
--rw-rw-r--   0 root         (0) root         (0)    10709 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/component/template/
--rw-rw-r--   0 root         (0) root         (0)     9157 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/template/conanbase.mako
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/template/deploy.mako
--rw-rw-r--   0 root         (0) root         (0)     5554 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/component/test.py
--rw-rw-r--   0 root         (0) root         (0)     1886 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/errors.py
--rw-rw-r--   0 root         (0) root         (0)      829 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2762 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/build_manifest.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/build_prepare.py
--rw-rw-r--   0 root         (0) root         (0)     8475 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/build_rootfs.py
--rw-rw-r--   0 root         (0) root         (0)     2890 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/config.py
--rw-rw-r--   0 root         (0) root         (0)     4637 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit/integration/template/
--rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/integration/template/conanfile.py.mako
--rw-rw-r--   0 root         (0) root         (0)      114 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/lbkit.py
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/log.py
--rw-rw-r--   0 root         (0) root         (0)     3180 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/misc.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-13 15:07:56.000000 lbkit-0.5.5/lbkit/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 15:08:04.927476 lbkit-0.5.5/lbkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1268 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 15:08:04.000000 lbkit-0.5.5/lbkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 15:08:04.931476 lbkit-0.5.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1295 2024-04-13 15:07:56.000000 lbkit-0.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-04-16 16:17:40.000000 lbkit-0.5.6/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)    11357 2024-04-16 16:17:40.000000 lbkit-0.5.6/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      149 2024-04-16 16:17:40.000000 lbkit-0.5.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-16 16:17:49.214934 lbkit-0.5.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-04-16 16:17:40.000000 lbkit-0.5.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 16:17:41.000000 lbkit-0.5.6/lbkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/ci_robot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/ci_robot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12840 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/ci_robot/gitee.py
+-rw-rw-r--   0 root         (0) root         (0)     8483 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/codegen/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4241 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/codegen.py
+-rw-rw-r--   0 root         (0) root         (0)    17074 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/ctype_defination.py
+-rw-rw-r--   0 root         (0) root         (0)    30770 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/idf_interface.py
+-rw-rw-r--   0 root         (0) root         (0)      287 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/codegen/template/
+-rw-rw-r--   0 root         (0) root         (0)     5781 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/client.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2888 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/client.h.mako
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/interface.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2297 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/interface.introspect.xml.mako
+-rw-rw-r--   0 root         (0) root         (0)    26271 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/public.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     8106 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/public.h.mako
+-rw-rw-r--   0 root         (0) root         (0)    12974 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/server.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     1492 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/codegen/template/server.h.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/component/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2155 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/arg_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    13224 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.210934 lbkit-0.5.6/lbkit/component/template/
+-rw-rw-r--   0 root         (0) root         (0)     9157 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/template/conanbase.mako
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/template/deploy.mako
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/component/test.py
+-rw-rw-r--   0 root         (0) root         (0)     2119 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/errors.py
+-rw-rw-r--   0 root         (0) root         (0)      829 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/lbkit/integration/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2762 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/build_manifest.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/build_prepare.py
+-rw-rw-r--   0 root         (0) root         (0)     8475 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/build_rootfs.py
+-rw-rw-r--   0 root         (0) root         (0)     2890 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4637 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/lbkit/integration/template/
+-rw-rw-r--   0 root         (0) root         (0)     1276 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/integration/template/conanfile.py.mako
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/lbkit.py
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/log.py
+-rw-rw-r--   0 root         (0) root         (0)     3561 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-04-16 16:17:40.000000 lbkit-0.5.6/lbkit/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 16:17:49.214934 lbkit-0.5.6/lbkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-16 16:17:49.000000 lbkit-0.5.6/lbkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 16:17:49.214934 lbkit-0.5.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1295 2024-04-16 16:17:40.000000 lbkit-0.5.6/setup.py
```

### Comparing `lbkit-0.5.5/LICENSE` & `lbkit-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/PKG-INFO` & `lbkit-0.5.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.5/lbkit/ci_robot/gitee.py` & `lbkit-0.5.6/lbkit/ci_robot/gitee.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/cli.py` & `lbkit-0.5.6/lbkit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         except KeyboardInterrupt as exc:
             log.error(exc)
             ret_code = 0
         except SystemExit as exc:
             if exc.code != 0:
                 log.error("Exiting with code: %d" % exc.code)
             ret_code = exc.code
-        except (errors.LiteBmcException, errors.RunCommandException, errors.ArgException, errors.PackageConfigException, Exception) as exc:
+        except (errors.LiteBmcException, errors.RunCommandException, errors.ArgException, errors.PackageConfigException, Exception, errors.OdfValidateException) as exc:
             if os.environ.get("LOG"):
                 print(traceback.format_exc())
             ret_code = -1
             msg = str(exc)
             log.error(misc.Color.RED + msg + misc.Color.RESET_ALL)
 
         return ret_code
```

### Comparing `lbkit-0.5.5/lbkit/codegen/codegen.py` & `lbkit-0.5.6/lbkit/codegen/codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
     DBus接口代码自动生成
 """
 import os
 import sys
+import json
 import yaml
 import argparse
 from lbkit.codegen.idf_interface import IdfInterface
 
 from mako.lookup import TemplateLookup
 from lbkit.log import Logger
 from lbkit.helper import Helper
@@ -41,14 +42,21 @@
         data = {
             "version": interface.version,
             "name": interface.name
         }
         with open(json_file, "w", encoding="utf-8") as fp:
             yaml.dump(data, fp, encoding='utf-8', allow_unicode=True)
 
+        # 生成接口schema文件
+        odf_file = os.path.join(directory, "server", "schema", f"{interface.name}.json")
+        os.makedirs(os.path.dirname(odf_file), exist_ok=True)
+        odf_data = interface.odf_schema
+        with open(odf_file, "w", encoding="utf-8") as fp:
+            json.dump(odf_data, fp, sort_keys=False, indent=4)
+
 
     def run(self, package_yml=None):
         """
         代码自动生成.
 
         支持自动生成服务端和客户端C代码
         """
```

### Comparing `lbkit-0.5.5/lbkit/codegen/idf_interface.py` & `lbkit-0.5.6/lbkit/codegen/idf_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import yaml
 import os
 import re
 import hashlib
 from lbkit.log import Logger
 from lbkit.codegen.renderer import Renderer
-from lbkit.codegen.ctype_defination import CTYPE_OBJS
+from lbkit.codegen.ctype_defination import CTYPE_OBJS, RefObjArrayValidator, RefObjValidator
 from lbkit.misc import validate_yml_with_json_schema
 
 log = Logger("gen_interface")
 
 class IDFException(Exception):
     pass
 
@@ -122,22 +122,96 @@
             return sig_prefix + dictionary.signature
 
 
 class IdfCtypeRender():
     intf: IdfInterfaceBase = None
     ctype: str = None
     name: str = ""
+    flags: list[str] = []
 
     def __init__(self):
         # 非基础类型
         match = re.match(f"^(set\[enum\[(.*)\]\])$", self.ctype)
         # 如果set类型由转换成数组，当前不具备对set类型独立处理能力
         if match:
             self.ctype = f"array[enum[{match.group(1)}]]"
 
+    def odf_schema(self, allow_ref):
+        log.debug(f"Get odf schema info, name: {self.name}, ctype: {self.ctype}")
+        if "variant" == self.ctype:
+            return None
+        match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
+        if match:
+            if "refobj" in self.flags:
+                valiator = RefObjArrayValidator()
+                return valiator.odf_schema(allow_ref, {})
+            ctype_obj = CTYPE_OBJS.get(self.ctype)
+            return ctype_obj.validator.odf_schema(allow_ref, {})
+        match = re.match(f"^({CTYPE_BASE_REG})$", self.ctype)
+        if match:
+            if "refobj" in self.flags:
+                valiator = RefObjValidator()
+                return valiator.odf_schema(allow_ref, {})
+            ctype_obj = CTYPE_OBJS.get(self.ctype)
+            return ctype_obj.validator.odf_schema(allow_ref, {})
+        # 非基础类型
+        is_array = False
+        ctype = self.ctype
+        match = re.match(f"^array\[(.*)\]$", ctype)
+        if match:
+            is_array = True
+            ctype = match.group(1)
+        match = re.match(f"^(struct|enum|dict)\[(.*)\]$", ctype)
+        _, stru_name = get_intfname_and_ctype(match.group(2))
+        if match.group(1) == "struct":
+            stru = self.intf.structures.get(stru_name)
+            if stru is None:
+                raise IDFException(f"Structurer {stru_name} is not found, generate odf for {self.name} failed")
+            schema = stru.odf_schema()
+        elif match.group(1) == "enum":
+            enum = self.intf.enumerations.get(stru_name)
+            if enum is None:
+                raise IDFException(f"Enumerate {stru_name} is not found, generate odf for {self.name} failed")
+            schema = enum.odf_schema()
+        else:
+            dict_cls = self.intf.dictionaries.get(stru_name)
+            if dict_cls is None:
+                raise IDFException(f"Dictionary {stru_name} is not found, generate odf for {self.name} failed")
+            schema = dict_cls.odf_schema()
+        if is_array:
+            # 结构体数组初始化时为二级空指针，以空指针结束
+            if allow_ref:
+                return {
+                        "type": "array",
+                        "item": schema
+                    }
+            return  {
+                "oneOf": [
+                    {
+                        "$ref": "#/$defs/ref_value"
+                    },
+                    {
+                        "type": "array",
+                        "item": schema
+                    }
+                ]
+            }
+        else:
+            # 结构体成员初始化时为空结构体，由反序列化时填充内容
+            if allow_ref:
+                return {
+                    "oneOf": [
+                        {
+                            "$ref": "#/$defs/ref_value"
+                        },
+                        schema
+                    ]
+                }
+            return schema
+
     def declare(self):
         """变量申明，用于结构体（接口类、方法请求和响应、信号消息等）申明"""
         log.debug(f"Get declare info, name: {self.name}, ctype: {self.ctype}")
         match = re.match(f"^array\[({CTYPE_BASE_REG})\]$", self.ctype)
         if match:
             ctype_obj = CTYPE_OBJS.get(self.ctype)
             return ctype_obj.declare
@@ -435,23 +509,50 @@
         super().__init__(intf, stru_data)
         self.values: IdfParameters = IdfParameters(intf, stru_data.get(propety_key, []))
 
     @property
     def signature(self):
         return "(" + self.values.signature+ ")"
 
+    def odf_schema(self):
+        schema = {}
+        for prop in self.values.parameters:
+            odf = prop.odf_schema(False)
+            if odf is not None:
+                schema[prop.name] = odf
+            else:
+                log.warning(f"the schema of prop {prop.name} is None")
+        odf = {
+            "type": "object",
+            "additionalProperties": False,
+            # "required": [],
+            "properties": schema
+        }
+        return odf
+
 class IdfEnumeration(IdfBase):
     def __init__(self, intf: IdfInterfaceBase, enum_data):
         super().__init__(intf, enum_data)
         self.values: list[IdfParameter] = IdfParameters(intf, enum_data.get("values", []))
 
     @property
     def signature(self):
         return "s"
 
+    def odf_schema(self):
+        values = []
+        for prop in self.values.parameters:
+            val = self.intf.name + "." + self.name + "." + prop.name
+            values.append(val)
+
+        odf = {
+            "enum": values
+        }
+        return odf
+
 
 class IdfDictionary():
     def __init__(self, intf: IdfInterfaceBase, dict_data):
         self.intf = intf
         self.annotations: list[IdfAnnotation] = []
         self.name = dict_data.get("name")
         self.key = dict_data.get("key")
@@ -500,14 +601,45 @@
     @property
     def key_free(self):
         if self.key_is_string:
             return "g_free"
         else:
             return "NULL"
 
+    def odf_schema(self):
+        schema = {}
+        for prop in self.values.parameters:
+            odf = prop.odf_schema(False)
+            if odf is not None:
+                schema[prop.name] = odf
+            else:
+                log.warning(f"the schema of prop {prop.name} is None")
+        key_schema = self.key_obj.odf_schema(False)
+        odf = {
+            "type": "array",
+            "description": "dictionary schema#",
+            "items": {
+                "type": "object",
+                "additionalProperties": False,
+                "required": [
+                    "key",
+                    "properties"
+                ],
+                "properties": {
+                    "key": key_schema,
+                    "properties": {
+                        "type": "object",
+                        "additionalProperties": False,
+                        "properties": schema
+                    }
+                }
+            }
+        }
+        return odf
+
 
 class IdfInterface(IdfInterfaceBase):
     def __init__(self, lookup, idf_file):
         if not idf_file.endswith(".yaml"):
             raise IDFException(f"IDF file {idf_file} not endswith .yaml")
         super().__init__()
         self.lookup = lookup
@@ -528,14 +660,71 @@
     @property
     def signature(self):
         sig = ""
         for prop in self.properties:
             sig += prop.signature
         return "(" + sig + ")"
 
+    @property
+    def odf_schema(self):
+        schema = {}
+        with_schema_prop_cnt = 0
+        for prop in self.properties:
+            odf = prop.odf_schema(True)
+            if odf is not None:
+                schema[prop.name] = odf
+                with_schema_prop_cnt += 1
+            else:
+                log.warning(f"the schema of prop {prop.name} is None")
+            # 顶层属性可以有一个flags标记属性
+            schema[f"_{prop.name}_flags"] =  {
+                "type": "string",
+                "pattern": "^(per_save|per_power_off|per_reboot)*$"
+            }
+        odf = {
+            "$schema": "http://json-schema.org/draft-07/schema#",
+            "title": self.name + " schema#",
+            "description": f"schema of the interface " + self.name,
+            "type": "object",
+            "additionalProperties": False
+        }
+        if with_schema_prop_cnt > 0:
+            odf["properties"] = schema
+            odf["$defs"] = {
+                "ref_value": {
+                    "type": "string",
+                    "description": "Property reference syntax. The format must be `\\$\\{([<]*|:)<interface>:<object_path>.<property name>\\}`",
+                    "pattern": "^\\$\\{([<]*|:)(([a-zA-Z_][A-Za-z0-9_]*)(\\.[a-zA-Z_][A-Za-z0-9_]*)+:)[/]?[A-Z0-9a-z_]+(/[A-Z0-9a-z_]+)*\\.[A-Za-z][a-zA-Z0-9_-]*\\}$"
+                },
+                "ref_obj": {
+                    "type": "string",
+                    "description": "Property reference syntax. The format must be `\\$\\{([<]*|:)<interface>:<object_path>.<property name>\\}`",
+                    "pattern": "^\\$\\{([<]*|:)(([a-zA-Z_][A-Za-z0-9_]*)(\\.[a-zA-Z_][A-Za-z0-9_]*)+:)[/]?[A-Z0-9a-z_]+(/[A-Z0-9a-z_]+)*\\}$"
+                },
+                "ref_obj_array": {
+                    "type": "array",
+                    "description": "String array, each item is described using the object reference syntax",
+                    "items": {
+                        "anyOf": [
+                            {
+                                "type": "string",
+                                "description": "Object reference syntax. The format must be `\\$\\{([<]*|:)<interface>:<object_path>\\}`",
+                                "pattern": "^\\$\\{([<]*|:)(([a-zA-Z_][A-Za-z0-9_]*)(\\.[a-zA-Z_][A-Za-z0-9_]*)+:)[/]?[A-Z0-9a-z_]+(/[A-Z0-9a-z_]+)*\\}$"
+                            },
+                            {
+                                "type": "string",
+                                "description": "Plain string format, if the string start with `$` must add `\\` before `$` to escape; If the string is empty it must be surrounded by `\"`",
+                                "pattern": "^[/]?[A-Z0-9a-z_]+(/[A-Z0-9a-z_]+)*$"
+                            }
+                        ]
+                    }
+                }
+            }
+        return odf
+
     def load_elements(self):
         # 使用schema校验数据，确保IDF文件符合格式要求，减少程序处理过程中的异常处理
         # 验证失败时抛异常，此处不用处理，由外层处理
         validate_yml_with_json_schema(self.file, "/usr/share/litebmc/schema/idf.v1.json")
         log.info(f"validate {self.file} successfully")
         with open(self.file, "r") as fp:
             idf = yaml.load(fp, yaml.FullLoader)
```

### Comparing `lbkit-0.5.5/lbkit/codegen/template/client.c.mako` & `lbkit-0.5.6/lbkit/codegen/template/client.c.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/codegen/template/client.h.mako` & `lbkit-0.5.6/lbkit/codegen/template/client.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/codegen/template/interface.introspect.xml.mako` & `lbkit-0.5.6/lbkit/codegen/template/interface.introspect.xml.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/codegen/template/public.c.mako` & `lbkit-0.5.6/lbkit/codegen/template/public.c.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/codegen/template/public.h.mako` & `lbkit-0.5.6/lbkit/codegen/template/public.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/codegen/template/server.c.mako` & `lbkit-0.5.6/lbkit/codegen/template/server.c.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/codegen/template/server.h.mako` & `lbkit-0.5.6/lbkit/codegen/template/server.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/component/arg_parser.py` & `lbkit-0.5.6/lbkit/component/arg_parser.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/component/template/conanbase.mako` & `lbkit-0.5.6/lbkit/component/template/conanbase.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/component/template/deploy.mako` & `lbkit-0.5.6/lbkit/component/template/deploy.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/component/test.py` & `lbkit-0.5.6/lbkit/component/test.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/errors.py` & `lbkit-0.5.6/lbkit/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,15 @@
          Http request exception
     """
     def __init__(self, *args, **kwargs):
         super(HttpRequestException, self).__init__(*args, **kwargs)
 
     def __str__(self):
         return super(HttpRequestException, self).__str__()
+
+
+class OdfValidateException(Exception):
+    def __init__(self, *args, **kwargs):
+        super(OdfValidateException, self).__init__(*args, **kwargs)
+
+    def __str__(self):
+        return super(OdfValidateException, self).__str__()
```

### Comparing `lbkit-0.5.5/lbkit/helper.py` & `lbkit-0.5.6/lbkit/helper.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/integration/build_manifest.py` & `lbkit-0.5.6/lbkit/integration/build_manifest.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/integration/build_prepare.py` & `lbkit-0.5.6/lbkit/integration/build_prepare.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/integration/build_rootfs.py` & `lbkit-0.5.6/lbkit/integration/build_rootfs.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/integration/config.py` & `lbkit-0.5.6/lbkit/integration/config.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/integration/task.py` & `lbkit-0.5.6/lbkit/integration/task.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/integration/template/conanfile.py.mako` & `lbkit-0.5.6/lbkit/integration/template/conanfile.py.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/log.py` & `lbkit-0.5.6/lbkit/log.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit/misc.py` & `lbkit-0.5.6/lbkit/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,38 +46,46 @@
 class SmartFormatter(argparse.HelpFormatter):
     """重写HelpFormatter"""
     def _fill_text(self, text, width, indent):
         """重写HelpFormatter"""
         text = textwrap.dedent(text)
         return ''.join(indent + line for line in text.splitlines(True))
 
-
-def validate_yml_with_json_schema(yml_file, default_json_schema_file):
+def get_json_schema_file(yml_file, default_json_schema_file):
     """使用json schema文件校验yml_file配置文件"""
-    schema_file = None
     with open(yml_file, "r") as fp:
         for line in fp:
             match = re.search(r"#[ ]*yaml-language-server:[ ]*\$schema=(.*)\n", line)
             if match is not None:
-                schema_file = match.group(1)
-                break
-    if schema_file is None:
-        schema_file = default_json_schema_file
+                return match.group(1)
+    return default_json_schema_file
+
+def load_json_schema(schema_file):
+    """使用json schema文件校验yml_file配置文件"""
     if schema_file.startswith("https://litebmc.com/"):
         resp = requests.get(schema_file)
         if resp.status_code != 200:
             raise HttpRequestException(f"Get {schema_file} failed, status code: {resp.status_code}")
-        schema = json.loads(resp.content)
+        return json.loads(resp.content)
     elif not os.path.isfile(schema_file):
         raise FileNotFoundError(f"schemafile {schema_file} not exist")
     else:
         with open(schema_file, "r") as fp:
             tmp = fp.read()
-            schema = json.loads(tmp)
+            return json.loads(tmp)
+
+def validate_yml_with_json_schema(yml_file, default_json_schema_file):
+    """使用json schema文件校验yml_file配置文件"""
+    schema_file = get_json_schema_file(yml_file, default_json_schema_file)
+    if schema_file is None:
+        raise FileNotFoundError(f"Can't found invalid schema file in {yml_file}")
+
+    schema = load_json_schema(schema_file)
     try:
         fp = open(yml_file, "r")
         data = yaml.safe_load(fp)
+        fp.close()
         validate(data, schema)
     except ValidationError as exc:
         raise PackageConfigException(f"validate {yml_file} failed, schema file is {schema_file}, "
                                      f"message: {exc.message}\n"
-                                     "installing redhat.vscode-yaml plugin in vscode will help you write odf files")
+                                     "installing redhat.vscode-yaml plugin in vscode will help you write odf files") from exec
```

### Comparing `lbkit-0.5.5/lbkit/tools.py` & `lbkit-0.5.6/lbkit/tools.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/lbkit.egg-info/PKG-INFO` & `lbkit-0.5.6/lbkit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.5/lbkit.egg-info/SOURCES.txt` & `lbkit-0.5.6/lbkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.5/setup.py` & `lbkit-0.5.6/setup.py`

 * *Files identical despite different names*

