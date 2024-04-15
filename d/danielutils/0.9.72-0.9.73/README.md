# Comparing `tmp/danielutils-0.9.72.tar.gz` & `tmp/danielutils-0.9.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.72.tar", last modified: Wed Apr  3 22:26:23 2024, max compression
+gzip compressed data, was "danielutils-0.9.73.tar", last modified: Mon Apr 15 22:44:53 2024, max compression
```

## Comparing `danielutils-0.9.72.tar` & `danielutils-0.9.73.tar`

### file list

```diff
@@ -1,136 +1,134 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.940152 danielutils-0.9.72/
--rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.72/LICENSE
--rw-rw-rw-   0        0        0     4499 2024-04-03 22:26:23.937017 danielutils-0.9.72/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2024-03-21 23:41:27.000000 danielutils-0.9.72/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.825463 danielutils-0.9.72/danielutils/
--rw-rw-rw-   0        0        0     1423 2024-03-30 13:12:04.000000 danielutils-0.9.72/danielutils/__init__.py
--rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/aliases.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.840384 danielutils-0.9.72/danielutils/classes/
--rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/Convenience.py
--rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/Counter.py
--rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/Tree.py
--rw-rw-rw-   0        0        0      159 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/__init__.py
--rw-rw-rw-   0        0        0     3776 2024-04-03 22:23:41.000000 danielutils-0.9.72/danielutils/classes/frange.py
--rw-rw-rw-   0        0        0     3045 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/classes/repl.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.842325 danielutils-0.9.72/danielutils/classes/sorted_builtins/
--rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/sorted_builtins/__init__.py
--rw-rw-rw-   0        0        0      112 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/sorted_builtins/sset.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.849092 danielutils-0.9.72/danielutils/classes/typed_builtins/
--rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/__init__.py
--rw-rw-rw-   0        0        0     4730 2024-03-29 00:29:43.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/factory.py
--rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/tdict.py
--rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/tlist.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/tset.py
--rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/classes/typed_builtins/ttuple.py
--rw-rw-rw-   0        0        0     5434 2024-03-29 22:03:21.000000 danielutils-0.9.72/danielutils/colors.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.851163 danielutils-0.9.72/danielutils/conversions/
--rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/__init__.py
--rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/main_conversions.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.854164 danielutils-0.9.72/danielutils/conversions/specialized_conversions/
--rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/specialized_conversions/__init__.py
--rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.72/danielutils/conversions/specialized_conversions/to_hex.py
--rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/conversions/specialized_conversions/to_int.py
--rw-rw-rw-   0        0        0     2800 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/d_print.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.862272 danielutils-0.9.72/danielutils/data_structures/
--rw-rw-rw-   0        0        0     1228 2024-03-28 19:48:44.000000 danielutils-0.9.72/danielutils/data_structures/Comparer.py
--rw-rw-rw-   0        0        0     1860 2024-03-28 19:42:06.000000 danielutils-0.9.72/danielutils/data_structures/Stack.py
--rw-rw-rw-   0        0        0      161 2024-03-30 20:21:37.000000 danielutils-0.9.72/danielutils/data_structures/__init__.py
--rw-rw-rw-   0        0        0      261 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/data_structures/default_dict.py
--rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.72/danielutils/data_structures/functions.py
--rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.72/danielutils/date.py
--rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.72/danielutils/date_time.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.881632 danielutils-0.9.72/danielutils/decorators/
--rw-rw-rw-   0        0        0      413 2024-03-27 18:54:28.000000 danielutils-0.9.72/danielutils/decorators/__init__.py
--rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/atomic.py
--rw-rw-rw-   0        0        0     1555 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/attach.py
--rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/chain_decorators.py
--rw-rw-rw-   0        0        0     1016 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0     1192 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/delay_call.py
--rw-rw-rw-   0        0        0     1469 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/deprecate.py
--rw-rw-rw-   0        0        0     1877 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/limit_recursion.py
--rw-rw-rw-   0        0        0     1034 2024-03-29 21:27:58.000000 danielutils-0.9.72/danielutils/decorators/memo.py
--rw-rw-rw-   0        0        0     7511 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/overload.py
--rw-rw-rw-   0        0        0     1012 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/partially_implemented.py
--rw-rw-rw-   0        0        0     1753 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/processify.py
--rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/decorators/property.py
--rw-rw-rw-   0        0        0      916 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/threadify.py
--rw-rw-rw-   0        0        0     2131 2024-04-03 22:25:29.000000 danielutils-0.9.72/danielutils/decorators/timeout.py
--rw-rw-rw-   0        0        0    10013 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/decorators/validate.py
--rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/exceptions.py
--rw-rw-rw-   0        0        0    11820 2024-03-14 21:24:08.000000 danielutils-0.9.72/danielutils/files_and_folders.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.889164 danielutils-0.9.72/danielutils/functions/
--rw-rw-rw-   0        0        0      160 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/functions/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/functions/check_foreach.py
--rw-rw-rw-   0        0        0     9027 2024-03-29 00:10:11.000000 danielutils-0.9.72/danielutils/functions/isoftype.py
--rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/functions/isoneof.py
--rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/functions/powerset.py
--rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/functions/types_subseteq.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.895523 danielutils-0.9.72/danielutils/generators/
--rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/generators/__init__.py
--rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/generators/conditional_generator.py
--rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2827 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/generators/join_generators.py
--rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/internet.py
--rw-rw-rw-   0        0        0     2005 2024-02-19 17:33:20.000000 danielutils-0.9.72/danielutils/loops.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.901722 danielutils-0.9.72/danielutils/math/
--rw-rw-rw-   0        0        0       80 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/__init__.py
--rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/constants.py
--rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/functions.py
--rw-rw-rw-   0        0        0     1062 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/math/math_print.py
--rw-rw-rw-   0        0        0     4051 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/math/math_symbols.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.910246 danielutils-0.9.72/danielutils/metaclasses/
--rw-rw-rw-   0        0        0    10944 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/metaclasses/Interface.py
--rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.72/danielutils/metaclasses/__init__.py
--rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/atomic_class_meta.py
--rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/implicit_data_deleter_meta.py
--rw-rw-rw-   0        0        0     1487 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/instance_cache_meta.py
--rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/metaclasses/overload_meta.py
--rw-rw-rw-   0        0        0      202 2024-03-10 17:39:29.000000 danielutils-0.9.72/danielutils/multi_x.py
--rw-rw-rw-   0        0        0     1419 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/my_tqdm.py
--rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/path.py
--rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.72/danielutils/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.919207 danielutils-0.9.72/danielutils/reflection/
--rw-rw-rw-   0        0        0     1655 2024-03-29 21:36:20.000000 danielutils-0.9.72/danielutils/reflection/__init__.py
--rw-rw-rw-   0        0        0      736 2024-03-29 21:51:07.000000 danielutils-0.9.72/danielutils/reflection/class_reflection.py
--rw-rw-rw-   0        0        0     1133 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/reflection/file_reflection.py
--rw-rw-rw-   0        0        0     5055 2024-03-29 21:50:42.000000 danielutils-0.9.72/danielutils/reflection/function_reflections.py
--rw-rw-rw-   0        0        0      748 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/reflection/get_prev_frame.py
--rw-rw-rw-   0        0        0      444 2024-03-29 21:51:07.000000 danielutils-0.9.72/danielutils/reflection/get_traceback.py
--rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/reflection/module_reflections.py
--rw-rw-rw-   0        0        0      639 2024-03-29 21:49:46.000000 danielutils-0.9.72/danielutils/reflection/system_reflections.py
--rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/relations.py
--rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.922437 danielutils-0.9.72/danielutils/snippets/
--rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/snippets/try_get.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.924440 danielutils-0.9.72/danielutils/system/
--rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/__init__.py
--rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/system/independent.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.926852 danielutils-0.9.72/danielutils/system/windows/
--rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.930339 danielutils-0.9.72/danielutils/system/windows/utils/
--rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/utils/__init__.py
--rw-rw-rw-   0        0        0      477 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/utils/filetime.py
--rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/win32_ctime.py
--rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/system/windows/windows.py
--rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/text.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.932925 danielutils-0.9.72/danielutils/threads/
--rw-rw-rw-   0        0        0       51 2023-08-15 21:20:20.000000 danielutils-0.9.72/danielutils/threads/__init__.py
--rw-rw-rw-   0        0        0     2416 2024-03-29 22:01:24.000000 danielutils-0.9.72/danielutils/threads/worker.py
--rw-rw-rw-   0        0        0     2319 2024-03-27 18:52:27.000000 danielutils-0.9.72/danielutils/threads/worker_pool.py
--rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/time.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.933925 danielutils-0.9.72/danielutils/university/
--rw-rw-rw-   0        0        0       54 2024-03-30 12:00:49.000000 danielutils-0.9.72/danielutils/university/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.935975 danielutils-0.9.72/danielutils/university/databases/
--rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/university/databases/__init__.py
--rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.72/danielutils/university/databases/all.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:26:23.831342 danielutils-0.9.72/danielutils.egg-info/
--rw-rw-rw-   0        0        0     4499 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4191 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 22:26:23.000000 danielutils-0.9.72/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      934 2024-04-03 22:26:22.000000 danielutils-0.9.72/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 22:26:23.941071 danielutils-0.9.72/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-03 22:26:22.000000 danielutils-0.9.72/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.177250 danielutils-0.9.73/
+-rw-rw-rw-   0        0        0     1091 2023-05-29 13:19:53.000000 danielutils-0.9.73/LICENSE
+-rw-rw-rw-   0        0        0     4478 2024-04-15 22:44:53.175932 danielutils-0.9.73/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2024-03-21 23:41:27.000000 danielutils-0.9.73/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.061297 danielutils-0.9.73/danielutils/
+-rw-rw-rw-   0        0        0     1474 2024-04-15 22:00:00.000000 danielutils-0.9.73/danielutils/__init__.py
+-rw-rw-rw-   0        0        0     5663 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/aliases.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.075708 danielutils-0.9.73/danielutils/classes/
+-rw-rw-rw-   0        0        0      210 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/Convenience.py
+-rw-rw-rw-   0        0        0     1221 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/Counter.py
+-rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/Tree.py
+-rw-rw-rw-   0        0        0      159 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/__init__.py
+-rw-rw-rw-   0        0        0     7286 2024-04-15 22:37:37.000000 danielutils-0.9.73/danielutils/classes/frange.py
+-rw-rw-rw-   0        0        0     3169 2024-04-15 22:24:58.000000 danielutils-0.9.73/danielutils/classes/repl.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.078293 danielutils-0.9.73/danielutils/classes/sorted_builtins/
+-rw-rw-rw-   0        0        0        0 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/sorted_builtins/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/sorted_builtins/sset.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.088155 danielutils-0.9.73/danielutils/classes/typed_builtins/
+-rw-rw-rw-   0        0        0       88 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/typed_builtins/__init__.py
+-rw-rw-rw-   0        0        0     4730 2024-04-09 22:20:09.000000 danielutils-0.9.73/danielutils/classes/typed_builtins/factory.py
+-rw-rw-rw-   0        0        0      913 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/typed_builtins/tdict.py
+-rw-rw-rw-   0        0        0     7214 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/typed_builtins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/typed_builtins/tset.py
+-rw-rw-rw-   0        0        0      294 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/classes/typed_builtins/ttuple.py
+-rw-rw-rw-   0        0        0     5457 2024-04-15 22:08:50.000000 danielutils-0.9.73/danielutils/colors.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.090176 danielutils-0.9.73/danielutils/conversions/
+-rw-rw-rw-   0        0        0       73 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/conversions/__init__.py
+-rw-rw-rw-   0        0        0     2227 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/conversions/main_conversions.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.092394 danielutils-0.9.73/danielutils/conversions/specialized_conversions/
+-rw-rw-rw-   0        0        0       46 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/conversions/specialized_conversions/__init__.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 23:16:41.000000 danielutils-0.9.73/danielutils/conversions/specialized_conversions/to_hex.py
+-rw-rw-rw-   0        0        0      549 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/conversions/specialized_conversions/to_int.py
+-rw-rw-rw-   0        0        0     2800 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/d_print.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.098616 danielutils-0.9.73/danielutils/data_structures/
+-rw-rw-rw-   0        0        0     1224 2024-04-15 22:24:58.000000 danielutils-0.9.73/danielutils/data_structures/Comparer.py
+-rw-rw-rw-   0        0        0     2143 2024-04-15 22:26:05.000000 danielutils-0.9.73/danielutils/data_structures/Stack.py
+-rw-rw-rw-   0        0        0      163 2024-04-15 22:26:05.000000 danielutils-0.9.73/danielutils/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      273 2024-04-15 22:24:58.000000 danielutils-0.9.73/danielutils/data_structures/default_dict.py
+-rw-rw-rw-   0        0        0      632 2023-09-25 13:19:42.000000 danielutils-0.9.73/danielutils/data_structures/functions.py
+-rw-rw-rw-   0        0        0      631 2023-09-25 13:20:33.000000 danielutils-0.9.73/danielutils/date.py
+-rw-rw-rw-   0        0        0      232 2023-08-07 20:06:13.000000 danielutils-0.9.73/danielutils/date_time.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.120299 danielutils-0.9.73/danielutils/decorators/
+-rw-rw-rw-   0        0        0      446 2024-04-09 22:04:07.000000 danielutils-0.9.73/danielutils/decorators/__init__.py
+-rw-rw-rw-   0        0        0      912 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/decorators/atomic.py
+-rw-rw-rw-   0        0        0     1538 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1074 2024-04-10 11:18:47.000000 danielutils-0.9.73/danielutils/decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1175 2024-04-15 22:37:37.000000 danielutils-0.9.73/danielutils/decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1452 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1860 2024-04-15 22:37:37.000000 danielutils-0.9.73/danielutils/decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0     1017 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/decorators/memo.py
+-rw-rw-rw-   0        0        0     7785 2024-04-15 22:37:37.000000 danielutils-0.9.73/danielutils/decorators/overload.py
+-rw-rw-rw-   0        0        0      995 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/decorators/partially_implemented.py
+-rw-rw-rw-   0        0        0     1709 2024-04-09 23:09:17.000000 danielutils-0.9.73/danielutils/decorators/processify.py
+-rw-rw-rw-   0        0        0     1095 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/decorators/property.py
+-rw-rw-rw-   0        0        0      899 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/decorators/threadify.py
+-rw-rw-rw-   0        0        0     2157 2024-04-15 22:37:37.000000 danielutils-0.9.73/danielutils/decorators/timeout.py
+-rw-rw-rw-   0        0        0     9996 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/exceptions.py
+-rw-rw-rw-   0        0        0    12002 2024-04-15 21:39:53.000000 danielutils-0.9.73/danielutils/files_and_folders.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.128972 danielutils-0.9.73/danielutils/functions/
+-rw-rw-rw-   0        0        0      160 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/functions/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/functions/check_foreach.py
+-rw-rw-rw-   0        0        0     9027 2024-03-29 00:10:11.000000 danielutils-0.9.73/danielutils/functions/isoftype.py
+-rw-rw-rw-   0        0        0     1598 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/functions/isoneof.py
+-rw-rw-rw-   0        0        0      639 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/functions/powerset.py
+-rw-rw-rw-   0        0        0     1016 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.134461 danielutils-0.9.73/danielutils/generators/
+-rw-rw-rw-   0        0        0      108 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      463 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2861 2024-04-10 15:54:43.000000 danielutils-0.9.73/danielutils/generators/join_generators.py
+-rw-rw-rw-   0        0        0     2051 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/internet.py
+-rw-rw-rw-   0        0        0     2005 2024-02-19 17:33:20.000000 danielutils-0.9.73/danielutils/loops.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.141232 danielutils-0.9.73/danielutils/math/
+-rw-rw-rw-   0        0        0       80 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/math/__init__.py
+-rw-rw-rw-   0        0        0     7682 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/math/constants.py
+-rw-rw-rw-   0        0        0      627 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/math/functions.py
+-rw-rw-rw-   0        0        0     1062 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/math/math_print.py
+-rw-rw-rw-   0        0        0     4051 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/math/math_symbols.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.147665 danielutils-0.9.73/danielutils/metaclasses/
+-rw-rw-rw-   0        0        0    10944 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/metaclasses/Interface.py
+-rw-rw-rw-   0        0        0      169 2024-03-21 23:16:41.000000 danielutils-0.9.73/danielutils/metaclasses/__init__.py
+-rw-rw-rw-   0        0        0      695 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/metaclasses/atomic_class_meta.py
+-rw-rw-rw-   0        0        0     2511 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/metaclasses/implicit_data_deleter_meta.py
+-rw-rw-rw-   0        0        0     1487 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/metaclasses/instance_cache_meta.py
+-rw-rw-rw-   0        0        0     1754 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/metaclasses/overload_meta.py
+-rw-rw-rw-   0        0        0      374 2024-04-15 21:39:53.000000 danielutils-0.9.73/danielutils/multi_x.py
+-rw-rw-rw-   0        0        0     1733 2024-04-15 22:27:00.000000 danielutils-0.9.73/danielutils/my_tqdm.py
+-rw-rw-rw-   0        0        0     1032 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/path.py
+-rw-rw-rw-   0        0        0        0 2023-08-09 09:08:58.000000 danielutils-0.9.73/danielutils/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.155655 danielutils-0.9.73/danielutils/reflection/
+-rw-rw-rw-   0        0        0     1650 2024-04-09 23:20:42.000000 danielutils-0.9.73/danielutils/reflection/__init__.py
+-rw-rw-rw-   0        0        0     1063 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/reflection/class_reflection.py
+-rw-rw-rw-   0        0        0     1192 2024-04-15 22:37:38.000000 danielutils-0.9.73/danielutils/reflection/file_reflection.py
+-rw-rw-rw-   0        0        0     4480 2024-04-15 21:50:16.000000 danielutils-0.9.73/danielutils/reflection/function_reflections.py
+-rw-rw-rw-   0        0        0      444 2024-03-29 21:51:07.000000 danielutils-0.9.73/danielutils/reflection/get_traceback.py
+-rw-rw-rw-   0        0        0      507 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/reflection/module_reflections.py
+-rw-rw-rw-   0        0        0      622 2024-04-15 21:50:16.000000 danielutils-0.9.73/danielutils/reflection/system_reflections.py
+-rw-rw-rw-   0        0        0      288 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/relations.py
+-rw-rw-rw-   0        0        0      489 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.158659 danielutils-0.9.73/danielutils/snippets/
+-rw-rw-rw-   0        0        0       24 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/snippets/try_get.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.161087 danielutils-0.9.73/danielutils/system/
+-rw-rw-rw-   0        0        0       52 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/system/__init__.py
+-rw-rw-rw-   0        0        0     6844 2024-03-27 18:52:27.000000 danielutils-0.9.73/danielutils/system/independent.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.163806 danielutils-0.9.73/danielutils/system/windows/
+-rw-rw-rw-   0        0        0       50 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/system/windows/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.165818 danielutils-0.9.73/danielutils/system/windows/utils/
+-rw-rw-rw-   0        0        0       25 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/system/windows/utils/__init__.py
+-rw-rw-rw-   0        0        0      499 2024-04-15 21:50:16.000000 danielutils-0.9.73/danielutils/system/windows/utils/filetime.py
+-rw-rw-rw-   0        0        0     6064 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/system/windows/win32_ctime.py
+-rw-rw-rw-   0        0        0     2253 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/system/windows/windows.py
+-rw-rw-rw-   0        0        0     4093 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/text.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.169999 danielutils-0.9.73/danielutils/threads/
+-rw-rw-rw-   0        0        0       51 2023-08-15 21:20:20.000000 danielutils-0.9.73/danielutils/threads/__init__.py
+-rw-rw-rw-   0        0        0     2397 2024-04-15 22:40:32.000000 danielutils-0.9.73/danielutils/threads/worker.py
+-rw-rw-rw-   0        0        0     2425 2024-04-15 22:40:32.000000 danielutils-0.9.73/danielutils/threads/worker_pool.py
+-rw-rw-rw-   0        0        0     1399 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/time.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.171032 danielutils-0.9.73/danielutils/university/
+-rw-rw-rw-   0        0        0       74 2024-04-15 21:59:15.000000 danielutils-0.9.73/danielutils/university/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.174647 danielutils-0.9.73/danielutils/university/databases/
+-rw-rw-rw-   0        0        0       20 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/university/databases/__init__.py
+-rw-rw-rw-   0        0        0    24942 2024-03-21 20:59:13.000000 danielutils-0.9.73/danielutils/university/databases/all.py
+drwxrwxrwx   0        0        0        0 2024-04-15 22:44:53.067144 danielutils-0.9.73/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     4478 2024-04-15 22:44:52.000000 danielutils-0.9.73/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4116 2024-04-15 22:44:52.000000 danielutils-0.9.73/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 22:44:52.000000 danielutils-0.9.73/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 22:44:52.000000 danielutils-0.9.73/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      928 2024-04-15 22:44:52.000000 danielutils-0.9.73/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 22:44:53.178750 danielutils-0.9.73/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-15 22:44:51.000000 danielutils-0.9.73/setup.py
```

### Comparing `danielutils-0.9.72/LICENSE` & `danielutils-0.9.73/LICENSE`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/PKG-INFO` & `danielutils-0.9.73/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.72
+Version: 0.9.73
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,14 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tqdm
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
```

### Comparing `danielutils-0.9.72/README.md` & `danielutils-0.9.73/README.md`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/__init__.py` & `danielutils-0.9.73/danielutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from .date_time import *
 from .multi_x import *
 from .loops import *
 from .signals import *
 from .aliases import *
 from .exceptions import PrintCatchOne
 from .snippets import *
-
+from .abstractions import *
+from .imports import *
 # =================================================================
 # ========================= ORDER MATTERS =========================
 # =================================================================
 
 from .reflection import *
 from .decorators import *
```

### Comparing `danielutils-0.9.72/danielutils/aliases.py` & `danielutils-0.9.73/danielutils/aliases.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/classes/Counter.py` & `danielutils-0.9.73/danielutils/classes/Counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/classes/repl.py` & `danielutils-0.9.73/danielutils/classes/repl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import copy
 from typing import Any, Callable, Union, Tuple as t_tuple, List as t_list, Dict as t_dict
 import re
-from ..reflection import get_python_version
+from ..reflection import get_python_version  # pylint :disable=relative-beyond-top-level
+
 if get_python_version() >= (3, 9):
     from builtins import tuple as t_tuple, list as t_list, dict as t_dict  # type:ignore
 
 
 class Argument:
     """a class to wrap an argument"""
 
@@ -35,17 +37,18 @@
         return self.callback(*args, **kwargs)
 
 
 class REPL:
     """a class to easily create a shell application and get functionality for free
     """
 
+    # pylint: disable=dangerous-default-value
     def __init__(self, routes: t_list[Command], *, prompt_symbol: str = ">>> ", exit_keywords: set = {"exit", "quit"}):
         self.prompt_symbol = prompt_symbol
-        self.exit_keywords = exit_keywords
+        self.exit_keywords = copy.copy(exit_keywords)
         self.routes: t_dict[str, Command] = {
             com.command.name: com for com in routes}
 
     def run(self) -> None:
         """runs the main loop for the shell
 
         Raises:
@@ -54,29 +57,29 @@
         while True:
             prompt = input(self.prompt_symbol)
             if prompt in self.exit_keywords:
                 break
 
             if prompt == "help":
                 print("Available commands:")
-                for com in list(self.routes.keys())+list(self.exit_keywords):
+                for com in list(self.routes.keys()) + list(self.exit_keywords):
                     print(f"\t{com}")
                 continue
 
             prompt_parts = prompt.split()
             command = prompt_parts[0]
             if command in self.routes:
                 try:
                     self.routes[command](*prompt_parts[1:])
                 except TypeError as e:
                     msg = str(e)
                     if re.match(r".*missing.*required.*argument.*", msg):
-                        print(f"'{command}' "+msg[msg.find("missing"):])
+                        print(f"'{command}' " + msg[msg.find("missing"):])
                     elif re.match(r".*takes.*arguments but.*given", msg):
-                        print(f"'{command}' "+msg[msg.find("takes"):])
+                        print(f"'{command}' " + msg[msg.find("takes"):])
                     else:
                         raise e
 
             else:
                 print(
                     "Invalid command. for help type 'help'.\nOr additionally you may try a command and then 'help'")
```

### Comparing `danielutils-0.9.72/danielutils/classes/typed_builtins/factory.py` & `danielutils-0.9.73/danielutils/classes/typed_builtins/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import types
 from abc import abstractmethod
 from typing import Any, Iterable, List as t_list, Set as t_set, Dict as t_dict, Tuple as t_tuple
 from ...functions import types_subseteq, isoftype
 from ...reflection import get_caller_name, get_python_version
+
 if get_python_version() >= (3, 9):
     from builtins import list as t_list, set as t_set, dict as t_dict, tuple as t_tuple  # type:ignore
 # needed for python 3.8
 class_to_type = {
     list: t_list,
     set: t_set,
     dict: t_dict,
@@ -35,27 +36,26 @@
     cls = types.new_class(name, (fallback_class,), {})
 
     def __class_getitem__(cls, item: type):
         return cls(item)
 
     def __instancecheck__(self, instance: Any) -> bool:
         if isinstance(instance, cls):
-
             return types_subseteq(
                 instance.get_params(),  # type:ignore
                 self.get_params()
             )
 
         return isoftype(
             instance,
             class_to_type[fallback_class][self.get_params()]  # type:ignore
         )
 
     def __init__(self, item) -> None:
-        if not get_caller_name(0) == "__class_getitem__":
+        if not get_caller_name(1) == "__class_getitem__":
             raise ValueError(
                 f"Can't instantiate {self.__class__.__name__} without a supplied type")
         fallback_class.__init__(self)  # type: ignore
         # pylint: disable=protected-access
         self._params = (item,) if not isinstance(
             item, Iterable) else tuple(item)
         self._inited = False
```

### Comparing `danielutils-0.9.72/danielutils/classes/typed_builtins/tdict.py` & `danielutils-0.9.73/danielutils/classes/typed_builtins/tdict.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/classes/typed_builtins/tlist.py` & `danielutils-0.9.73/danielutils/classes/typed_builtins/tlist.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/classes/typed_builtins/tset.py` & `danielutils-0.9.73/danielutils/classes/typed_builtins/tset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/colors.py` & `danielutils-0.9.73/danielutils/colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Optional, IO
 from .decorators import validate
 
-
 RESET = "\033[0m"
 
 
 class ColoredText:
     """static utility class with static functions:\n
         from_rgb,
         green,
         red,
         blue,
         red,
         yellow,
         white,
         black
     """
-    @staticmethod
+
+    @staticmethod  # type:ignore
     @validate
     def from_rgb(red: int, green: int, blue: int, text: str) -> str:
         """Applies an RGB color to the given text.
 
         Args:
-            r (int): The red component of the color.
-            g (int): The green component of the color.
-            b (int): The blue component of the color.
+            red (int): The red component of the color.
+            green (int): The green component of the color.
+            blue (int): The blue component of the color.
             text (str): The text to apply the color to.
 
         Returns:
             str: The given text with an RGB color applied to it.
         """
         return f"\033[38;2;{red};{green};{blue}m{text}{RESET}"
 
@@ -174,15 +174,15 @@
         end (str, optional): print endline. Defaults to "\\n".
     """
     __special_print(*args, sep=sep, end=end,
                     start_with=ColoredText.red("ERROR"))
 
 
 def info(*args, sep: str = " ", end: str = "\n"):
-    """print an error message
+    """print an info message
 
     Args:
         sep (str, optional): print separator. Defaults to " ".
         end (str, optional): print endline. Defaults to "\\n".
     """
     __special_print(*args, sep=sep, end=end,
                     start_with=ColoredText.yellow("INFO"))
```

### Comparing `danielutils-0.9.72/danielutils/conversions/main_conversions.py` & `danielutils-0.9.73/danielutils/conversions/main_conversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/conversions/specialized_conversions/to_int.py` & `danielutils-0.9.73/danielutils/conversions/specialized_conversions/to_int.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/d_print.py` & `danielutils-0.9.73/danielutils/d_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/data_structures/Comparer.py` & `danielutils-0.9.73/danielutils/data_structures/Comparer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Comparer class"""
-from typing import Callable, Any, Union, Generic, TypeVar
+from typing import Callable,  Union, Generic, TypeVar
 from .functions import default_weight_function
 
 U = TypeVar("U")
 V = TypeVar("V")
 
 
 class Comparer(Generic[U, V]):
```

### Comparing `danielutils-0.9.72/danielutils/data_structures/Stack.py` & `danielutils-0.9.73/danielutils/data_structures/Stack.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,61 @@
-from typing import Optional, Generator, Any, cast, TypeVar, Generic
+from typing import Optional, Generator, TypeVar, Generic
 from .graph import Node
 
 T = TypeVar('T')
 
 
 class Stack(Generic[T]):
     """A classic Stack class
     """
 
     def __init__(self) -> None:
         self.head: Optional[Node[T]] = None
         self.size = 0
 
-    def push(self, value: Node[T]):
+    def push(self, value: T):
         """push an item to the stack
 
         Args:
             value (Any): item to push
         """
         if self.head is None:
             self.head = Node(value)
         else:
             new_head = Node(value, self.head)
             self.head = new_head
         self.size += 1
 
-    def pop(self) -> Node[T]:
+    def pop(self) -> T:
         """pop an item from the stack
 
         Returns:
             Any: poped item
         """
         if not self.is_empty():
-            self.head = cast(Node, self.head)
-            res = self.head.data
+            res = self.head.data  # type:ignore
             self.size -= 1
-            self.head = self.head.next
+            self.head = self.head.next  # type:ignore
             return res
+        raise RuntimeError("Can't pop from an empty stack")
+
+    def peek(self) -> Optional[T]:
+        """
+        Returns the top element of the stack
+        Returns:
+            Optional[T]
+        """
+        if self.is_empty():
+            return None
+        return self.head.data
 
     def __len__(self) -> int:
         return self.size
 
-    def __iter__(self) -> Generator[Node[T], None, None]:
+    def __iter__(self) -> Generator[T, None, None]:
         while self:
             yield self.pop()
 
     def is_empty(self) -> bool:
         """return whether the stack is empty
         """
         return len(self) == 0
@@ -54,14 +64,15 @@
         return not self.is_empty()
 
     def __contains__(self, value: T) -> bool:
         curr = self.head
         while curr is not None:
             if curr.data == value:
                 return True
+            curr = curr.next
         return False
 
     def __str__(self) -> str:
         values = []
         curr = self.head
         while curr:
             values.append(str(curr.data))
```

### Comparing `danielutils-0.9.72/danielutils/data_structures/functions.py` & `danielutils-0.9.73/danielutils/data_structures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/date.py` & `danielutils-0.9.73/danielutils/date.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/decorators/atomic.py` & `danielutils-0.9.73/danielutils/decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/decorators/attach.py` & `danielutils-0.9.73/danielutils/decorators/attach.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import functools
 from typing import Callable, Optional, TypeVar
-import platform
 from .validate import validate
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
 T = TypeVar("T")
```

### Comparing `danielutils-0.9.72/danielutils/decorators/chain_decorators.py` & `danielutils-0.9.73/danielutils/decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/decorators/delay_call.py` & `danielutils-0.9.73/danielutils/decorators/delay_call.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Callable, TypeVar, Union
-import platform
 import time
 import functools
 from .decorate_conditionally import decorate_conditionally
 from .threadify import threadify
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
```

### Comparing `danielutils-0.9.72/danielutils/decorators/deprecate.py` & `danielutils-0.9.73/danielutils/decorators/deprecate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import platform
 from typing import Callable, TypeVar
 from ..colors import warning, ColoredText
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
```

### Comparing `danielutils-0.9.72/danielutils/decorators/limit_recursion.py` & `danielutils-0.9.73/danielutils/decorators/limit_recursion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import functools
 import re
 import traceback
-import platform
 from typing import Any, Callable, TypeVar
 from .validate import validate
 from ..colors import warning
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
```

### Comparing `danielutils-0.9.72/danielutils/decorators/memo.py` & `danielutils-0.9.73/danielutils/decorators/memo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Callable, Any, TypeVar, Dict as t_dict
 import functools
-import platform
+from typing import Callable, Any, TypeVar, Dict as t_dict
+from copy import deepcopy
 from .validate import validate
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
     from builtins import dict as t_dict
     from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
-from copy import deepcopy
 T = TypeVar("T")
 P = ParamSpec("P")
 FuncT = Callable[P, T]  # type:ignore
 
 
 @validate
 def memo(func: FuncT) -> FuncT:
```

### Comparing `danielutils-0.9.72/danielutils/decorators/overload.py` & `danielutils-0.9.73/danielutils/decorators/overload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable, cast, Any, TypeVar, Dict as t_dict, List as t_list
 import inspect
-import platform
 import functools
 from ..reflection import is_function_annotated_properly
 from ..functions import isoftype, isoneof, isoneof_strict
 from ..exceptions import OverloadDuplication, OverloadNotFound
 from .deprecate import deprecate
 from ..reflection import get_python_version
+
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec  # type:ignore# pylint: disable=ungrouped-imports
     from builtins import dict as t_dict, list as t_list
 T = TypeVar("T")
 P = ParamSpec("P")
@@ -75,15 +75,15 @@
         if types in __overload_dict[name]:
             # raise if current overload already exists for current function
             raise OverloadDuplication(
                 f"{name} has duplicate overloading for type(s): {types}")
 
         __overload_dict[name][types] = func
 
-        @ functools.wraps(func)
+        @functools.wraps(func)
         def wrapper(*args, **kwargs) -> Any:
             default_func = None
             # select correct overload
             for variable_types, curr_func in __overload_dict[f"{func.__module__}.{func.__qualname__}"].items():
                 if len(variable_types) == 0:
                     if default_func is None:
                         default_func = curr_func
@@ -108,14 +108,15 @@
             if default_func is not None:
                 return default_func(*args, **kwargs)
             # or raise exception if no overload exists for current arguments
             raise OverloadNotFound(
                 f"function {func.__module__}.{func.__qualname__} is not overloaded with {[type(v) for v in args]}")
 
         return wrapper
+
     return deco
 
 
 class overload:
     """this class create an object to manage the overloads for a given function.\n
     will only match a specific resolution and won't infer best guess for types
     """
@@ -156,38 +157,49 @@
         k = overload._get_key(func)
         if k not in self._functions:
             self._functions[k] = []
         self._functions[k].append(func)
         return self
 
     def __call__(self, *args, **kwargs):
-        num_args = len(args)+len(kwargs.keys())
+        num_args = len(args) + len(kwargs.keys())
         if num_args not in self._functions:
             raise AttributeError(
                 f"No overload with {num_args} argument found for {self._moudle}.{self._qualname}")
-        selected_func = None
-        if len(self._functions[num_args]) == 1:
-            selected_func = self._functions[num_args][0]
-        else:
-            for func in self._functions[num_args]:
-                signature = inspect.signature(func)
-                for i, tup in enumerate(signature.parameters.items()):
-                    param_name, param_type = tup
-                    if param_name in overload.__SKIP_SET:
-                        continue
 
-                    if not isoftype(args[i], param_type.annotation):
-                        break
+        if num_args == 0:
+            return self._functions[num_args][0](*args, **kwargs)
+
+        max_score = 0
+        winner = self._functions[num_args][0]
+        EXACT_MATCH = 1 / num_args
+        SUBCLASS = 1 / num_args
+        for func in self._functions[num_args]:
+            score = 0
+            signature = inspect.signature(func)
+            for i, tup in enumerate(signature.parameters.items()):
+                param_name, param_type = tup
+                if param_name in overload.__SKIP_SET:
+                    continue
+
+                if type(args[i]) == param_type.annotation:  # pylint :disable=unidiomatic-typecheck
+                    score += EXACT_MATCH
+
+                elif isoftype(args[i], param_type.annotation):
+                    score += SUBCLASS
                 else:
-                    # reaching here means current function matches perfectly the annotation
-                    selected_func = func
                     break
+
             else:
-                raise AttributeError("No overload found")
+                # reaching here means current function matches perfectly the annotation
+                if score > max_score:
+                    max_score = score
+                    winner = func
+        # raise AttributeError("No overload found")
 
-        return selected_func(*args, **kwargs)
+        return winner(*args, **kwargs)
 
 
 __all__ = [
     "explicit_global_overload",
     "overload"
 ]
```

### Comparing `danielutils-0.9.72/danielutils/decorators/partially_implemented.py` & `danielutils-0.9.73/danielutils/decorators/partially_implemented.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Callable, Any, TypeVar
 import functools
-import platform
 from .validate import validate
 from ..colors import warning
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
```

### Comparing `danielutils-0.9.72/danielutils/decorators/processify.py` & `danielutils-0.9.73/danielutils/decorators/processify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import functools
 import multiprocessing
 
-from ..reflection import get_n_caller_func, get_current_frame, get_n_prev_frame
+from ..reflection import get_prev_frame
 from ..multi_x import process_id
 import pickle
 
 
 def processify(func):
     """Modifies the function so that when calling it, a new process
     will start to run it with provided arguments. Note that no return
@@ -20,15 +20,15 @@
     """
     multiprocessing.freeze_support()
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         main_pid = kwargs.get("__main_pid", process_id())
         if process_id() == main_pid:
-            frame = get_n_prev_frame(2)
+            frame = get_prev_frame(2)
             dct = {k: v for k, v in frame.f_globals.items() if type(v) != type(inspect)}
             p = multiprocessing.Process(target=_run_func, args=(main_pid, dct, func.__name__, args, kwargs))
             p.start()
             p.join()  # Optionally wait for the process to finish
         else:
             del kwargs["__main_pid"]
             return func(*args, **kwargs)
@@ -37,15 +37,15 @@
 
 
 
 def _run_func(main_pid: int, dct: dict, func_name: str, args, kwargs) -> None:
     return dct[func_name](*args, __main_pid=main_pid, **kwargs)
 
 def debug_info(include_builtins: bool = False) -> dict:
-    f = get_n_prev_frame(2)
+    f = get_prev_frame(2)
     g = {k: v for k, v in f.f_globals.items() if k != "__builtins__"} if not include_builtins else dict(f.f_globals)
     return {
         "file": f.f_code.co_filename,
         "function": f.f_code.co_qualname,
         "line": f.f_lineno,
         "globals": g,
         "locals": dict(f.f_locals)
```

### Comparing `danielutils-0.9.72/danielutils/decorators/property.py` & `danielutils-0.9.73/danielutils/decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/decorators/threadify.py` & `danielutils-0.9.73/danielutils/decorators/threadify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Callable, TypeVar
-import platform
 import functools
 import threading
 
 from ..reflection import get_python_version
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
```

### Comparing `danielutils-0.9.72/danielutils/decorators/timeout.py` & `danielutils-0.9.73/danielutils/decorators/timeout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import threading
 import functools
-import platform
 from typing import Callable, TypeVar, Union
 from .validate import validate
 from ..reflection import get_python_version
 
 if get_python_version() < (3, 9):
     from typing_extensions import ParamSpec
 else:
@@ -40,15 +39,15 @@
         def wrapper(*args, **kwargs):
             res: list = [
                 TimeoutError(f'{func.__module__}.{func.__qualname__} timed out after {duration} seconds!')]
 
             def timeout_wrapper() -> None:
                 try:
                     res[0] = func(*args, **kwargs)
-                except Exception as function_error:
+                except Exception as function_error:  # pylint : disable=broad-exception-caught
                     res[0] = function_error
 
             t = threading.Thread(target=timeout_wrapper, daemon=True)
             try:
                 t.start()
                 t.join(duration)
             except Exception as thread_error:
```

### Comparing `danielutils-0.9.72/danielutils/decorators/validate.py` & `danielutils-0.9.73/danielutils/decorators/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import platform
 import functools
 import inspect
 from typing import Callable, get_type_hints, cast, TypeVar, Union
 from ..functions.isoftype import isoftype
 from ..reflection import get_function_return_type
 from ..exceptions import EmptyAnnotationException,\
     InvalidDefaultValueException, ValidationException, InvalidReturnValueException
```

### Comparing `danielutils-0.9.72/danielutils/exceptions.py` & `danielutils-0.9.73/danielutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/files_and_folders.py` & `danielutils-0.9.73/danielutils/files_and_folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,21 @@
     """
     if not directory_exists(path):
         os.makedirs(path)
 
 
 @validate
 def create_file(path: str) -> None:
+    """
+    Will create a file at the specified path if it doesn't already exists
+    Args:
+        path (str): the path to create a file at
+    Returns:
+        None
+    """
     if not file_exists(path):
         with open(path, "w", encoding='utf8') as f:
             pass
 
 
 @validate
 def get_file_type_from_directory(path: str, file_type: str) -> Iterator[str]:
```

### Comparing `danielutils-0.9.72/danielutils/functions/areoneof.py` & `danielutils-0.9.73/danielutils/functions/areoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/functions/check_foreach.py` & `danielutils-0.9.73/danielutils/functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/functions/isoftype.py` & `danielutils-0.9.73/danielutils/functions/isoftype.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/functions/isoneof.py` & `danielutils-0.9.73/danielutils/functions/isoneof.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/functions/powerset.py` & `danielutils-0.9.73/danielutils/functions/powerset.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/functions/types_subseteq.py` & `danielutils-0.9.73/danielutils/functions/types_subseteq.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/generators/conditional_generator.py` & `danielutils-0.9.73/danielutils/generators/conditional_generator.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/generators/join_generators.py` & `danielutils-0.9.73/danielutils/generators/join_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Generator, Any, Tuple as t_tuple
 from threading import Semaphore  # , Condition
 from ..decorators import threadify
 from ..data_structures import AtomicQueue, Queue
 from ..classes import AtomicCounter
 # from ..Print import aprint
 from ..reflection import get_python_version
+
 if get_python_version() >= (3, 9):
     from builtins import tuple as t_tuple  # type:ignore
 
 
 def join_generators_busy_waiting(*generators) -> Generator[t_tuple[int, Any], None, None]:
     """joins an arbitrary amount of generators to yield objects as soon someone yield an object
 
     Yields:
         Generator[tuple[int, Any], None, None]: resulting generator
     """
-    q = AtomicQueue()
+    q: AtomicQueue[t_tuple[int, Any]] = AtomicQueue()
     threads_status = [False for _ in range(len(generators))]
 
     @threadify
     def yield_from_one(thread_id: int, generator: Generator):
         nonlocal threads_status
         for v in generator:
             q.push((thread_id, v))
```

### Comparing `danielutils-0.9.72/danielutils/internet.py` & `danielutils-0.9.73/danielutils/internet.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/loops.py` & `danielutils-0.9.73/danielutils/loops.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/math/constants.py` & `danielutils-0.9.73/danielutils/math/constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/math/functions.py` & `danielutils-0.9.73/danielutils/math/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/math/math_print.py` & `danielutils-0.9.73/danielutils/math/math_print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/math/math_symbols.py` & `danielutils-0.9.73/danielutils/math/math_symbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/metaclasses/Interface.py` & `danielutils-0.9.73/danielutils/metaclasses/Interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/metaclasses/atomic_class_meta.py` & `danielutils-0.9.73/danielutils/metaclasses/atomic_class_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/metaclasses/implicit_data_deleter_meta.py` & `danielutils-0.9.73/danielutils/metaclasses/implicit_data_deleter_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/metaclasses/instance_cache_meta.py` & `danielutils-0.9.73/danielutils/metaclasses/instance_cache_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/metaclasses/overload_meta.py` & `danielutils-0.9.73/danielutils/metaclasses/overload_meta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/my_tqdm.py` & `danielutils-0.9.73/danielutils/my_tqdm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-from typing import Optional
-from tqdm import tqdm
+from typing import Optional, List as t_list
 from .reflection import get_python_version
+
 if get_python_version() >= (3, 9):
     from builtins import list as t_list  # type:ignore
-else:
-    from typing import List as t_list
+try:
+    from tqdm import tqdm
+except ImportError:
+    from .imports import MockImportObject
+
+    tqdm = MockImportObject("`tqdm` is not installed")  # type:ignore
 
 
 class ProgressBarPool:
-    def __init__(self, num_of_bars: int = 1, *, global_options: Optional[dict] = None, individual_options: Optional[t_list[Optional[dict]]] = None) -> None:
+    """
+    My attempt at creating a progress bar pool using tqdm
+    """
+
+    def __init__(self, num_of_bars: int = 1, *, global_options: Optional[dict] = None,
+                 individual_options: Optional[t_list[Optional[dict]]] = None) -> None:
         self.bars: t_list[tqdm] = []
         if global_options is None:
             global_options = {}
         if individual_options is None:
             individual_options = [{} for _ in range(num_of_bars)]
         if len(individual_options) != num_of_bars:
             raise ValueError("")
@@ -27,13 +36,16 @@
             t = tqdm(
                 position=i,
                 **final_options
             )
             self.bars.append(t)
 
     def write(self, *args, sep=" ", end="\n") -> None:
+        """
+        prints texts to the console **while** using tqdm progress bars
+        """
         self.bars[0].write(sep.join((str(a) for a in args)), end=end)
 
 
 __all__ = [
     "ProgressBarPool"
 ]
```

### Comparing `danielutils-0.9.72/danielutils/path.py` & `danielutils-0.9.73/danielutils/path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/reflection/__init__.py` & `danielutils-0.9.73/danielutils/reflection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .system_reflections import *  # this has to be first, the order matters!
 from .file_reflection import *
 from .function_reflections import *
 from .get_traceback import *
 from .module_reflections import *
 from .class_reflection import *
-from .get_prev_frame import *
+from .callstack import *
 from .interpreter import *
 # def get_class(module_name: str, class_name: str) -> type:
 #     """dynammically loads the module and returns the class from this file
 
 #     Args:
 #         module_name (str): name of python module, (typically a file name without extention)
 #         class_name (str): the name of the wanted class
```

### Comparing `danielutils-0.9.72/danielutils/reflection/class_reflection.py` & `danielutils-0.9.73/danielutils/reflection/class_reflection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
+from typing import Any, List as t_list
 from .interpreter import get_python_version
+
 if get_python_version() >= (3, 9):
     from builtins import list as t_list  # type:ignore
-else:
-    from typing import List as t_list
 
 
 def get_explicitly_declared_functions(cls: type) -> t_list[str]:
     """
     Returns the names of the functions that are explicitly declared in a class.
 
     This function does not return inherited functions.
@@ -17,10 +17,25 @@
 
     Returns:
         list[str]: A list of names of the functions explicitly declared in the class.
     """
     return [func for func, val in inspect.getmembers(cls, predicate=inspect.isfunction)]
 
 
+def get_mro(obj: Any) -> t_list[type]:
+    """returns the mro of an object
+
+    Args:
+        obj (Any): any object, instance or class
+
+    Returns:
+        list[type]: the resulting mro for the object
+    """
+    if isinstance(obj, type):
+        return obj.mro()
+    return get_mro(obj.__class__)
+
+
 __all__ = [
-    "get_explicitly_declared_functions"
+    "get_explicitly_declared_functions",
+    "get_mro"
 ]
```

### Comparing `danielutils-0.9.72/danielutils/reflection/file_reflection.py` & `danielutils-0.9.73/danielutils/reflection/file_reflection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import inspect
 import os
 from typing import Optional, cast
 from types import FrameType
-from .get_prev_frame import get_prev_frame_from
+from .callstack import _get_prev_frame_from
 
 
 def get_filename() -> Optional[str]:
     """returns the name of the file that this functions is called from
 
     Returns:
         Optional[str]: name of file
     """
-    frame = get_prev_frame_from(inspect.currentframe())
+    frame = _get_prev_frame_from(inspect.currentframe())
     if frame is None:
         return None
     frame = cast(FrameType, frame)
     return frame.f_code.co_filename
 
 
 def get_caller_filename() -> Optional[str]:
     """return the name of the file that the caller of the 
     function that's using this function is in
 
     Returns:
         Optional[str]: name of file
     """
-    frame = get_prev_frame_from(get_prev_frame_from(inspect.currentframe()))
+    frame = _get_prev_frame_from(_get_prev_frame_from(inspect.currentframe()))
     if frame is None:
         return None
     frame = cast(FrameType, frame)
     return frame.f_code.co_filename
 
 
 def get_current_directory() -> str:
+    """returns the name of the directory of main script"""
     return os.path.dirname(os.path.abspath(get_caller_filename()))  # type:ignore # noqa
 
 
 __all__ = [
     "get_filename",
     "get_caller_filename",
     'get_current_directory',
```

### Comparing `danielutils-0.9.72/danielutils/reflection/system_reflections.py` & `danielutils-0.9.73/danielutils/reflection/system_reflections.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-import platform
 from enum import Enum
 
 
 class OSType(Enum):
     """enum result for possible results of get_os()
     """
     LINUX = "Linux"
```

### Comparing `danielutils-0.9.72/danielutils/system/independent.py` & `danielutils-0.9.73/danielutils/system/independent.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/system/windows/win32_ctime.py` & `danielutils-0.9.73/danielutils/system/windows/win32_ctime.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/system/windows/windows.py` & `danielutils-0.9.73/danielutils/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/text.py` & `danielutils-0.9.73/danielutils/text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/threads/worker.py` & `danielutils-0.9.73/danielutils/threads/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from threading import Thread
 from abc import ABC, abstractmethod
-from typing import Optional, Any
+from typing import Optional, Any,Tuple as t_tuple
 from logging import error
 import danielutils # this is explicitly this way to prevent circular import
 from ..reflection import get_python_version
 if get_python_version() >= (3, 9):
     from builtins import tuple as t_tuple  # type:ignore
-else:
-    from typing import Tuple as t_tuple
 
 
 class Worker(ABC):
     """A Worker Interface
     """
 
     def __init__(self, id: int, pool: "danielutils.Threading.worker_pool.WorkerPool") -> None:  # pylint: disable=redefined-builtin #noqa
@@ -55,15 +53,15 @@
         self._notify()
 
     def _notify(self) -> None:
         """utility method to be called on the end of each iteration of work 
         to signal actions if needed
         will call 'notification_function'
         """
-        self.pool._notify()  # pylint: disable=protected-access
+        self.pool._notify_subscribers()  # pylint: disable=protected-access
 
     def acquire(self) -> Optional[t_tuple[Any]]:
         """acquire a new job object to work on from the pool
         will return a tuple of only one object (the job) or None if there are no more jobs
         Returns:
             Optional[tuple[Any]]: tuple of job object or None
         """
```

### Comparing `danielutils-0.9.72/danielutils/threads/worker_pool.py` & `danielutils-0.9.73/danielutils/threads/worker_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from queue import Queue
-from typing import Optional, Any
+from typing import Optional, Any, Type as t_type, Tuple as t_tuple, List as t_list
 from threading import Semaphore
 from .worker import Worker
 from ..reflection import get_python_version
+
 if get_python_version() >= (3, 9):
     from builtins import type as t_type, tuple as t_tuple, list as t_list  # type:ignore
-else:
-    from typing import Type as t_type, Tuple as t_tuple, List as t_list
 
 
 class WorkerPool:
     """A worker pool class
     """
 
     def __init__(self, num_workers: int, worker_class: t_type[Worker], w_kwargs: dict, global_variables: dict) -> None:
@@ -59,14 +58,19 @@
         this function is called automatically from Worker.work()
         """
         self.q.task_done()
         if self.q.unfinished_tasks <= 0:
             self.sem.release(self.num_workers)
 
     def join(self) -> None:
+        """
+        waits for all the workers to finish and will return afterwards
+        Returns:
+            None
+        """
         for w in self.workers:
             w.thread.join()
 
 
 __all__ = [
     "WorkerPool"
 ]
```

### Comparing `danielutils-0.9.72/danielutils/time.py` & `danielutils-0.9.73/danielutils/time.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils/university/databases/all.py` & `danielutils-0.9.73/danielutils/university/databases/all.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.72/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.73/danielutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.72
+Version: 0.9.73
 Summary: A python utils library for things I find useful
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 danielnachumdev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,15 +30,14 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tqdm
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
```

### Comparing `danielutils-0.9.72/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.73/danielutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 danielutils/relations.py
 danielutils/signals.py
 danielutils/text.py
 danielutils/time.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
-danielutils.egg-info/requires.txt
 danielutils.egg-info/top_level.txt
 danielutils/classes/Convenience.py
 danielutils/classes/Counter.py
 danielutils/classes/Tree.py
 danielutils/classes/__init__.py
 danielutils/classes/convenience.py
 danielutils/classes/counter.py
@@ -95,15 +94,14 @@
 danielutils/metaclasses/instance_cache_meta.py
 danielutils/metaclasses/interface.py
 danielutils/metaclasses/overload_meta.py
 danielutils/reflection/__init__.py
 danielutils/reflection/class_reflection.py
 danielutils/reflection/file_reflection.py
 danielutils/reflection/function_reflections.py
-danielutils/reflection/get_prev_frame.py
 danielutils/reflection/get_traceback.py
 danielutils/reflection/module_reflections.py
 danielutils/reflection/system_reflections.py
 danielutils/snippets/__init__.py
 danielutils/snippets/try_get.py
 danielutils/system/__init__.py
 danielutils/system/independent.py
```

### Comparing `danielutils-0.9.72/pyproject.toml` & `danielutils-0.9.73/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "danielutils"
-version = "0.9.72"
+version = "0.9.73"
 authors = [
     { name = "danielnachumdev", email = "danielnachumdev@gmail.com" },
 ]
-dependencies = ['tqdm']
+dependencies = []
 keywords = ['functions', 'decorators', 'methods', 'classes', 'metaclasses']
 license = { "file" = "./LICENSE" }
 description = "A python utils library for things I find useful"
 readme = "./README.md"
 requires-python = ">=3.8.0"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

