# Comparing `tmp/danidisp-0.0.7.tar.gz` & `tmp/danidisp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danidisp-0.0.7.tar", last modified: Fri Feb 23 14:31:12 2024, max compression
+gzip compressed data, was "danidisp-0.0.8.tar", last modified: Tue Apr 16 17:23:56 2024, max compression
```

## Comparing `danidisp-0.0.7.tar` & `danidisp-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2024-02-23 14:31:12.653389 danidisp-0.0.7/
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1096 2023-03-29 13:33:14.000000 danidisp-0.0.7/LICENSE
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      495 2024-02-23 14:31:12.653389 danidisp-0.0.7/PKG-INFO
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1200 2024-02-23 14:28:47.000000 danidisp-0.0.7/README.md
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)       38 2024-02-23 14:31:12.663404 danidisp-0.0.7/setup.cfg
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      590 2024-02-23 14:21:13.000000 danidisp-0.0.7/setup.py
-drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2024-02-23 14:31:12.399952 danidisp-0.0.7/src/
-drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2024-02-23 14:31:12.572100 danidisp-0.0.7/src/danidisp.egg-info/
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      495 2024-02-23 14:31:11.000000 danidisp-0.0.7/src/danidisp.egg-info/PKG-INFO
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      186 2024-02-23 14:31:11.000000 danidisp-0.0.7/src/danidisp.egg-info/SOURCES.txt
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        1 2024-02-23 14:31:11.000000 danidisp-0.0.7/src/danidisp.egg-info/dependency_links.txt
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        9 2024-02-23 14:31:11.000000 danidisp-0.0.7/src/danidisp.egg-info/top_level.txt
--rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1494 2024-02-23 14:24:09.000000 danidisp-0.0.7/src/danidisp.py
+drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2024-04-16 17:23:56.718578 danidisp-0.0.8/
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1096 2023-03-29 13:33:14.000000 danidisp-0.0.8/LICENSE
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      612 2024-04-16 17:23:56.715159 danidisp-0.0.8/PKG-INFO
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1200 2024-02-23 14:28:47.000000 danidisp-0.0.8/README.md
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)       38 2024-04-16 17:23:56.719837 danidisp-0.0.8/setup.cfg
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      711 2024-04-16 17:21:57.000000 danidisp-0.0.8/setup.py
+drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2024-04-16 17:23:56.494145 danidisp-0.0.8/src/
+drwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        0 2024-04-16 17:23:56.667346 danidisp-0.0.8/src/danidisp.egg-info/
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      612 2024-04-16 17:23:55.000000 danidisp-0.0.8/src/danidisp.egg-info/PKG-INFO
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)      186 2024-04-16 17:23:55.000000 danidisp-0.0.8/src/danidisp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        1 2024-04-16 17:23:55.000000 danidisp-0.0.8/src/danidisp.egg-info/dependency_links.txt
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)        9 2024-04-16 17:23:55.000000 danidisp-0.0.8/src/danidisp.egg-info/top_level.txt
+-rwxrwxrwx   0 danieledisp  (1000) danieledisp  (1000)     1864 2024-04-16 17:23:22.000000 danidisp-0.0.8/src/danidisp.py
```

### Comparing `danidisp-0.0.7/LICENSE` & `danidisp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `danidisp-0.0.7/README.md` & `danidisp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `danidisp-0.0.7/setup.py` & `danidisp-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup
 
 setup(
     name="danidisp",
-    version='0.0.7',
+    version='0.0.8',
     description='My own package: every useful function I want to use',
     py_modules=['danidisp'],
     package_dir={'': 'src'},
     url="https://github.com/DanieleDiSpirito/danidisp",
     author="Daniele Di Spirito",
     author_email="danieledisp@proton.me",
     long_description='''
         Package contains:\n
         - xor(a: bytes, b: bytes) -> bytes
         - dlog(n: int, b: int, mod: int) -> int
         - base_conv(n: str, bs: int = 10, be: int = 10) -> str
         - @clock
+        - sprint(string: str, gap: float = 0.03, new_line: bool = True) -> None
+        - sinput(prompt: str) -> str
     '''
-)
+)
```

### Comparing `danidisp-0.0.7/src/danidisp.py` & `danidisp-0.0.8/src/danidisp.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,7 +43,22 @@
 def clock(func):
 	def _clock():
 		start = perf_counter()
 		func()
 		end = perf_counter()
 		print('{func.__name__} took {0:.8f}s'.format(end-start))
 	return _clock
+
+GAP_TIME = 0.03
+
+def sprint(string: str, gap: float = GAP_TIME, new_line: bool = True) -> None:
+    for ch in string:
+        stdout.write(ch)
+        stdout.flush()
+        sleep(gap)
+    if ch != '\n' and new_line:
+        stdout.write('\n')
+        stdout.flush()
+
+def sinput(prompt: str) -> str:
+    sprint(prompt, new_line=False)
+    return input()
```

