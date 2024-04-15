# Comparing `tmp/snapshooter-1.0.4.tar.gz` & `tmp/snapshooter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapshooter-1.0.4.tar", last modified: Mon Apr 15 21:32:43 2024, max compression
+gzip compressed data, was "snapshooter-1.0.5.tar", last modified: Mon Apr 15 21:50:34 2024, max compression
```

## Comparing `snapshooter-1.0.4.tar` & `snapshooter-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:32:26.000000 snapshooter-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:32:43.290494 snapshooter-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-15 21:32:26.000000 snapshooter-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:32:43.290494 snapshooter-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 21:32:26.000000 snapshooter-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/snapshooter/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 21:32:35.000000 snapshooter-1.0.4/snapshooter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/jsonl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34032 2024-04-15 21:32:26.000000 snapshooter-1.0.4/snapshooter/snapshooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/snapshooter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:32:43.000000 snapshooter-1.0.4/snapshooter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:43.290494 snapshooter-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/test_fsspec_snapshooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:32:26.000000 snapshooter-1.0.4/tests/test_fsspec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:50:34.350508 snapshooter-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 21:50:18.000000 snapshooter-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:50:34.350508 snapshooter-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-15 21:50:18.000000 snapshooter-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:50:34.350508 snapshooter-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-15 21:50:18.000000 snapshooter-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:50:34.346508 snapshooter-1.0.5/snapshooter/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 21:50:27.000000 snapshooter-1.0.5/snapshooter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-15 21:50:18.000000 snapshooter-1.0.5/snapshooter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-15 21:50:18.000000 snapshooter-1.0.5/snapshooter/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 21:50:18.000000 snapshooter-1.0.5/snapshooter/jsonl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 21:50:18.000000 snapshooter-1.0.5/snapshooter/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34733 2024-04-15 21:50:18.000000 snapshooter-1.0.5/snapshooter/snapshooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:50:34.350508 snapshooter-1.0.5/snapshooter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-15 21:50:34.000000 snapshooter-1.0.5/snapshooter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-15 21:50:34.000000 snapshooter-1.0.5/snapshooter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:50:34.000000 snapshooter-1.0.5/snapshooter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-15 21:50:34.000000 snapshooter-1.0.5/snapshooter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:50:34.000000 snapshooter-1.0.5/snapshooter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 21:50:34.000000 snapshooter-1.0.5/snapshooter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:50:34.350508 snapshooter-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:50:18.000000 snapshooter-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-15 21:50:18.000000 snapshooter-1.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-15 21:50:18.000000 snapshooter-1.0.5/tests/test_fsspec_snapshooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 21:50:18.000000 snapshooter-1.0.5/tests/test_fsspec_utils.py
```

### Comparing `snapshooter-1.0.4/LICENSE` & `snapshooter-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/PKG-INFO` & `snapshooter-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-1.0.4/README.md` & `snapshooter-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/setup.py` & `snapshooter-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/snapshooter/cli.py` & `snapshooter-1.0.5/snapshooter/cli.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/snapshooter/fsspec_utils.py` & `snapshooter-1.0.5/snapshooter/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/snapshooter/jsonl_utils.py` & `snapshooter-1.0.5/snapshooter/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/snapshooter/snapshooter.py` & `snapshooter-1.0.5/snapshooter/snapshooter.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,14 +551,58 @@
         old_is_interrupted = self._is_interrupted
         self._is_interrupted = True
         # Wake up all threads waiting on the queue by putting None as a special value
         if not old_is_interrupted:
             for _ in range(self.parallel_listers):
                 self.dir_queue.put(None)
 
+    def list_files(self):
+        # remark: first connection and root check in main thread improves error handling
+        try:
+            root_exists = self.fs.exists(self.root)
+        except Exception as e:
+            raise Exception(f"Error verifying root folder '{self.root}' in {self.fs}: {e}") from e
+
+        if not root_exists:
+            raise Exception(f"Root folder '{self.root}' does not exist in {self.fs}")
+        else:
+            log.info(f"Root folder '{self.root}' exists in {self.fs}. Now listing files...")
+
+        tic = time.monotonic()
+        # even first root dir search in main threa ensures that access rights are ok
+        try:
+            self._list_dir(self.root)
+        except Exception as e:
+            raise Exception(f"Error listing files of root folder '{self.root}' in {self.fs}: {e}") from e
+            
+        # start parallelized listing
+        with concurrent.futures.ThreadPoolExecutor(max_workers=self.parallel_listers) as executor:
+            for _ in range(self.parallel_listers):
+                executor.submit(self._process_queue)
+
+            log_thread = threading.Thread(target=self._log_progress, daemon=True)
+            log_thread.start()
+
+            # Add root and wait for the directory listing tasks to complete
+            self.dir_queue.join()
+
+            # for logger
+            self.interrupt()
+
+        # Check if there were any errors during listing
+        if self.errors:
+            error_summary = "\n---------------------------\n".join(self.errors)
+            raise Exception(f"Errors occurred during file listing:\n{error_summary}")
+        else:
+            elapsed_time = time.monotonic() - tic
+            files_per_seconds = len(self.result) / elapsed_time
+            log.info(f"Listed {len(self.result)} files in {elapsed_time:.2f} seconds ({files_per_seconds:.2f} files/s)")
+
+        return self.result
+
     def _list_dir(self, directory: str):
             # all_details  = self.fs.find(directory, detail=True, withdirs=True, maxdepth=0).values()
             # all_details  = list(all_details)
             all_details    = self.fs.ls(directory, detail=True)
             all_details    = [d for d in all_details if d["name"] != directory]  # avoid endless loop
             sub_dir_infos  = [d for d in all_details if d['type'] == 'directory']
             src_file_infos = [d for d in all_details if d['type'] == 'file']
@@ -590,53 +634,14 @@
                 time.sleep(10)
                 self.check_interrupted()
                 log.info(f"Progress: {len(self.result)} files listed.")
         except InterruptedError:
             # some tools log error is thread die because of exception, but we want to ignore this excepted case
             log.debug("ParallelLister: Logging thread interrupted properly.")
 
-    def list_files(self):
-        # remark: first connection and root check in main thread improves error handling
-        try:
-            root_exists = self.fs.exists(self.root)
-        except Exception as e:
-            raise Exception(f"Error verifying root folder '{self.root}' in {self.fs}: {e}") from e
-
-        if not root_exists:
-            raise Exception(f"Root folder '{self.root}' does not exist in {self.fs}")
-        else:
-            log.info(f"Root folder '{self.root}' exists in {self.fs}. Now listing files...")
-            
-        # even first root dir search in main threa ensures that access rights are ok
-        try:
-            self._list_dir(self.root)
-        except Exception as e:
-            raise Exception(f"Error listing files of root folder '{self.root}' in {self.fs}: {e}") from e
-            
-        # start parallelized listing
-        with concurrent.futures.ThreadPoolExecutor(max_workers=self.parallel_listers) as executor:
-            for _ in range(self.parallel_listers):
-                executor.submit(self._process_queue)
-
-            log_thread = threading.Thread(target=self._log_progress, daemon=True)
-            log_thread.start()
-
-            # Add root and wait for the directory listing tasks to complete
-            self.dir_queue.join()
-
-            # for logger
-            self.interrupt()
-
-        # Check if there were any errors during listing
-        if self.errors:
-            error_summary = "\n---------------------------\n".join(self.errors)
-            raise Exception(f"Errors occurred during file listing:\n{error_summary}")
-
-        return self.result
-
 
 class ParallelFileProcessor:
     """Abstract class for parallel file processing."""
     def __init__(
         self,
         file_fs                : AbstractFileSystem,
         file_root              : str,
@@ -659,14 +664,15 @@
             raise InterruptedError(f"{self.__class__.__name__}: Interrupted properly")
 
     def interrupt(self):
         self._is_interrupted = True
 
     def process_files(self):
         log.info(f"{self.__class__.__name__}: Processing {len(self.relative_paths_to_process)} files with {self.parallelization} workers")
+        tic = time.monotonic()
         with concurrent.futures.ThreadPoolExecutor(max_workers=self.parallelization) as executor:
             log_thread = threading.Thread(target=self._log_progress, daemon=True)
             log_thread.start()
 
             # Submit all download tasks to the executor
             futures = [executor.submit(self._process_file, file_relative_path) for file_relative_path in self.relative_paths_to_process]
 
@@ -682,14 +688,21 @@
         # Ensures the logging thread also completes
         self.interrupt()
 
         # Check if there were any errors during downloads
         if self.errors:
             error_summary = "\n---------------------------\n".join(self.errors)
             raise Exception(f"{self.__class__.__name__}: Errors occurred during files processing:\n{error_summary}")
+        else:
+            elapsed_time = time.monotonic() - tic
+            files_per_second = len(self.relative_paths_to_process) / elapsed_time
+            log.info(
+                f"{self.__class__.__name__}: Processing {len(self.relative_paths_to_process)} files with {self.parallelization} workers "
+                f"in {elapsed_time:.2f} seconds ({files_per_second:.2f} files/s)"
+            )
 
     @abstractmethod
     def _process_file(self, file_relative_path):
         ...
 
     def _log_progress(self):
         try:
```

### Comparing `snapshooter-1.0.4/snapshooter.egg-info/PKG-INFO` & `snapshooter-1.0.5/snapshooter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapshooter
-Version: 1.0.4
+Version: 1.0.5
 Summary: Provides a set of utilities for comparing and backing up data on different filesystems
 Home-page: https://github.com/jeromerg/snapshooter
 Author: jeromerg
 Author-email: jeromerg@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snapshooter-1.0.4/tests/test_fsspec_snapshooter.py` & `snapshooter-1.0.5/tests/test_fsspec_snapshooter.py`

 * *Files identical despite different names*

### Comparing `snapshooter-1.0.4/tests/test_fsspec_utils.py` & `snapshooter-1.0.5/tests/test_fsspec_utils.py`

 * *Files identical despite different names*

