# Comparing `tmp/ycls-1.0.6.tar.gz` & `tmp/ycls-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ycls-1.0.6.tar", last modified: Wed Apr 10 14:47:37 2024, max compression
+gzip compressed data, was "ycls-1.0.7.tar", last modified: Tue Apr 16 11:05:05 2024, max compression
```

## Comparing `ycls-1.0.6.tar` & `ycls-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:47:37.224489 ycls-1.0.6/
--rw-rw-rw-   0        0        0     3059 2024-04-10 14:47:37.224489 ycls-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2738 2024-04-10 14:30:08.000000 ycls-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 14:47:37.224489 ycls-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      688 2024-04-10 14:43:21.000000 ycls-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:47:37.224489 ycls-1.0.6/ycls/
--rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.6/ycls/__init__.py
--rw-rw-rw-   0        0        0     1419 2024-04-10 14:43:07.000000 ycls-1.0.6/ycls/ycls.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:47:37.224489 ycls-1.0.6/ycls.egg-info/
--rw-rw-rw-   0        0        0     3059 2024-04-10 14:47:37.000000 ycls-1.0.6/ycls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-10 14:47:37.000000 ycls-1.0.6/ycls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:47:37.000000 ycls-1.0.6/ycls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-10 14:47:37.000000 ycls-1.0.6/ycls.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 14:47:37.000000 ycls-1.0.6/ycls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 14:47:37.000000 ycls-1.0.6/ycls.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 11:05:05.240847 ycls-1.0.7/
+-rw-rw-rw-   0        0        0     3059 2024-04-16 11:05:05.240847 ycls-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2738 2024-04-10 14:30:08.000000 ycls-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:05:05.240847 ycls-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      688 2024-04-16 10:48:58.000000 ycls-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:05:05.228847 ycls-1.0.7/ycls/
+-rw-rw-rw-   0        0        0      107 2024-04-10 11:01:36.000000 ycls-1.0.7/ycls/__init__.py
+-rw-rw-rw-   0        0        0     1506 2024-04-16 10:55:14.000000 ycls-1.0.7/ycls/ycls.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:05:05.239848 ycls-1.0.7/ycls.egg-info/
+-rw-rw-rw-   0        0        0     3059 2024-04-16 11:05:05.000000 ycls-1.0.7/ycls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-16 11:05:05.000000 ycls-1.0.7/ycls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:05:05.000000 ycls-1.0.7/ycls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-16 11:05:05.000000 ycls-1.0.7/ycls.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-16 11:05:05.000000 ycls-1.0.7/ycls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-16 11:05:05.000000 ycls-1.0.7/ycls.egg-info/top_level.txt
```

### Comparing `ycls-1.0.6/PKG-INFO` & `ycls-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.6
+Version: 1.0.7
 Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
```

### Comparing `ycls-1.0.6/README.md` & `ycls-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ycls-1.0.6/setup.py` & `ycls-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ycls",
-    version="1.0.6",
+    version="1.0.7",
     description="YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.",
     packages=find_packages(),
     install_requires=requirements,
     long_description=description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
```

### Comparing `ycls-1.0.6/ycls/ycls.py` & `ycls-1.0.7/ycls/ycls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import r128gain
 import typer
 
-def calculate_loudness_lufs(input_file):
+def calculate_loudness_lufs(input_file: str) -> float:
     '''Calculates the loudness level of the input audio (or video) file in LUFS (Loudness Units Full Scale) using the r128gain library.'''
     return r128gain.get_r128_loudness([input_file])[0]
 
-def calculate_youtube_content_loudness(input_file):
+def calculate_youtube_content_loudness(input_file: str) -> float:
     '''Calculates the adjusted loudness suitable for YouTube content based on the input audio (or video) file. It adds 14 dB to the loudness level calculated by calculate_loudness_lufs.'''
     return round(calculate_loudness_lufs(input_file) + 14, 1)
 
-def calculate_peak_dbfs(input_file):
+def calculate_peak_dbfs(input_file: str) -> float:
     '''Calculates the peak loudness in dBFS (decibels relative to full scale) of the input audio (or video) file using the r128gain library.'''
     return round(r128gain.scale_to_gain(r128gain.get_r128_loudness([input_file])[1]), 1)
 
 
 def main(input_file: str = typer.Option(None, "-i", help="Input file path.")):
     if not input_file:
         print("Please enter input file, --help to view commands.")
@@ -25,8 +25,11 @@
 
     print(f"File Loudness: {lufs} LUFS")
     print(f"Peak Loudness: {peak} dBFS")
     print(f"Youtube Content Loudness: {youtube_content_loudness} dB")
 
 
 def run_cli():
-    typer.run(main)
+    typer.run(main)
+
+if __name__ == "__main__":
+    run_cli()
```

### Comparing `ycls-1.0.6/ycls.egg-info/PKG-INFO` & `ycls-1.0.7/ycls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ycls
-Version: 1.0.6
+Version: 1.0.7
 Summary: YCLS is a Python module for calculating loudness metrics for audio (or video) files, particularly aimed at determining the loudness level suitable for YouTube content.
 Description-Content-Type: text/markdown
 Requires-Dist: r128gain
 Requires-Dist: typer
 
 # YCLS (YouTube Content Loudness Scanner)
```

