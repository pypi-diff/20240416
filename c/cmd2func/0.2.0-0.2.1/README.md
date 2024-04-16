# Comparing `tmp/cmd2func-0.2.0.tar.gz` & `tmp/cmd2func-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmd2func-0.2.0.tar", last modified: Tue Mar 12 14:25:54 2024, max compression
+gzip compressed data, was "cmd2func-0.2.1.tar", last modified: Tue Apr 16 07:57:09 2024, max compression
```

## Comparing `cmd2func-0.2.0.tar` & `cmd2func-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:25:54.988030 cmd2func-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-03-12 14:25:47.000000 cmd2func-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 14:25:47.000000 cmd2func-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-12 14:25:47.000000 cmd2func-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-12 14:25:54.988030 cmd2func-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-12 14:25:47.000000 cmd2func-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:25:54.984030 cmd2func-0.2.0/cmd2func/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-12 14:25:47.000000 cmd2func-0.2.0/cmd2func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-12 14:25:47.000000 cmd2func-0.2.0/cmd2func/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-12 14:25:47.000000 cmd2func-0.2.0/cmd2func/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-12 14:25:47.000000 cmd2func-0.2.0/cmd2func/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-12 14:25:47.000000 cmd2func-0.2.0/cmd2func/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-12 14:25:47.000000 cmd2func-0.2.0/cmd2func/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:25:54.984030 cmd2func-0.2.0/cmd2func.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-12 14:25:54.000000 cmd2func-0.2.0/cmd2func.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-12 14:25:54.000000 cmd2func-0.2.0/cmd2func.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 14:25:54.000000 cmd2func-0.2.0/cmd2func.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 14:25:54.000000 cmd2func-0.2.0/cmd2func.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 14:25:54.000000 cmd2func-0.2.0/cmd2func.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 14:25:54.000000 cmd2func-0.2.0/cmd2func.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 14:25:54.988030 cmd2func-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-12 14:25:47.000000 cmd2func-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 14:25:54.984030 cmd2func-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-12 14:25:47.000000 cmd2func-0.2.0/tests/test_cmd2func.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-12 14:25:47.000000 cmd2func-0.2.0/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-12 14:25:47.000000 cmd2func-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:57:09.420849 cmd2func-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-16 07:56:58.000000 cmd2func-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 07:56:58.000000 cmd2func-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 07:56:58.000000 cmd2func-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-16 07:57:09.420849 cmd2func-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-16 07:56:58.000000 cmd2func-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:57:09.416849 cmd2func-0.2.1/cmd2func/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 07:56:58.000000 cmd2func-0.2.1/cmd2func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-16 07:56:58.000000 cmd2func-0.2.1/cmd2func/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-16 07:56:58.000000 cmd2func-0.2.1/cmd2func/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-16 07:56:58.000000 cmd2func-0.2.1/cmd2func/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-16 07:56:58.000000 cmd2func-0.2.1/cmd2func/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 07:56:58.000000 cmd2func-0.2.1/cmd2func/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:57:09.416849 cmd2func-0.2.1/cmd2func.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-16 07:57:09.000000 cmd2func-0.2.1/cmd2func.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-16 07:57:09.000000 cmd2func-0.2.1/cmd2func.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:57:09.000000 cmd2func-0.2.1/cmd2func.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:57:09.000000 cmd2func-0.2.1/cmd2func.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 07:57:09.000000 cmd2func-0.2.1/cmd2func.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 07:57:09.000000 cmd2func-0.2.1/cmd2func.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:57:09.420849 cmd2func-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-16 07:56:58.000000 cmd2func-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:57:09.416849 cmd2func-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-16 07:56:58.000000 cmd2func-0.2.1/tests/test_cmd2func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-16 07:56:58.000000 cmd2func-0.2.1/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-16 07:56:58.000000 cmd2func-0.2.1/tests/test_utils.py
```

### Comparing `cmd2func-0.2.0/CONTRIBUTING.md` & `cmd2func-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cmd2func-0.2.0/LICENSE` & `cmd2func-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmd2func-0.2.0/PKG-INFO` & `cmd2func-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd2func
-Version: 0.2.0
+Version: 0.2.1
 Summary: Convert command to callable Python object.
 Home-page: https://github.com/Nanguage/cmd2func
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT license
 Keywords: cmd2func
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cmd2func-0.2.0/README.md` & `cmd2func-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cmd2func-0.2.0/cmd2func/cmd.py` & `cmd2func-0.2.1/cmd2func/cmd.py`

 * *Files identical despite different names*

### Comparing `cmd2func-0.2.0/cmd2func/config.py` & `cmd2func-0.2.1/cmd2func/config.py`

 * *Files identical despite different names*

### Comparing `cmd2func-0.2.0/cmd2func/core.py` & `cmd2func-0.2.1/cmd2func/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     def __init__(
             self, cmd_or_func: T.Union[str, StrFunc, StrGenFunc],
             config: T.Optional[CLIConfig] = None,
             print_cmd=True,
             out_stream=sys.stdout,
             err_stream=sys.stderr,
             conda_env: T.Optional[str] = None,
+            flush_streams_each_time=False,
             popen_kwargs: T.Optional[dict] = None,):
         """Convert a command to a function.
 
         Args:
             cmd_or_func: The command string or a function that returns the
                 command string or a generator that yields the command string.
             config: The config of the command. If not provided, it will be
@@ -82,14 +83,16 @@
                 default: True.
             out_stream: The stream to print the output of the command.
                 default: sys.stdout.
             err_stream: The stream to print the error of the command.
                 default: sys.stderr.
             conda_env: The conda environment to run the command.
                 default: None.
+            flush_streams_each_time: Whether to flush the streams each time
+                after writing to them. default: False.
             popen_kwargs: The keyword arguments for subprocess.Popen.
                 default: None.
 
         Attributes:
             lastest_cmd_str: The lastest command string that is run.
         """
         self.get_cmd_str: T.Union[StrFunc, StrGenFunc]
@@ -101,14 +104,15 @@
             self.get_cmd_str = cmd_or_func
             functools.update_wrapper(self, cmd_or_func)
 
         self.is_print_cmd = print_cmd
         self.out_stream = out_stream
         self.err_stream = err_stream
         self.conda_env = conda_env
+        self.flush_streams_each_time = flush_streams_each_time
         self.kwargs_popen = popen_kwargs or dict()
         self.lastest_cmd_str: T.Optional[str] = None
 
     def process_cmd_str(self, cmd_str: str) -> str:
         if self.conda_env is not None:
             cmd_str = "conda run --no-capture-output " + \
                 f"-n {self.conda_env} {cmd_str}"
@@ -119,15 +123,16 @@
         cmd_str = self.process_cmd_str(cmd_str)
         self.lastest_cmd_str = cmd_str
         if self.is_print_cmd:
             print(f"Run command: {cmd_str}")
         runner = ProcessRunner(cmd_str)
         runner.run(**self.kwargs_popen)
         ret_code = runner.write_stream_until_stop(
-            self.out_stream, self.err_stream)
+            self.out_stream, self.err_stream,
+            self.flush_streams_each_time)
         return ret_code
 
     def iter_and_run(self, generator: CmdGen) -> T.Any:
         cmd = next(generator)
         while True:
             ret_code = self.run_cmd(cmd)
             try:
@@ -147,22 +152,25 @@
 def cmd2func(
         cmd_or_func: T.Union[str, StrFunc, StrGenFunc, None] = None,
         config: T.Optional[CLIConfig] = None,
         print_cmd=True,
         out_stream=sys.stdout,
         err_stream=sys.stderr,
         conda_env: T.Optional[str] = None,
+        flush_streams_each_time=False,
         popen_kwargs: T.Optional[dict] = None,
         ) -> Cmd2Func:
     if cmd_or_func is None:
         return functools.partial(  # type: ignore
             cmd2func, config=config, print_cmd=print_cmd,
             out_stream=out_stream, err_stream=err_stream,
-            conda_env=conda_env, popen_kwargs=popen_kwargs)
+            conda_env=conda_env,
+            flush_streams_each_time=flush_streams_each_time,
+            popen_kwargs=popen_kwargs)
     else:
         return Cmd2Func(
             cmd_or_func, config, print_cmd, out_stream, err_stream,
-            conda_env, popen_kwargs
+            conda_env, flush_streams_each_time, popen_kwargs
         )
 
 
 cmd2func.__doc__ = Cmd2Func.__init__.__doc__
```

### Comparing `cmd2func-0.2.0/cmd2func/runner.py` & `cmd2func-0.2.1/cmd2func/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,21 +70,27 @@
                 line_decoded = line.decode()
                 yield src, line_decoded
         return self.proc.wait()
 
     def write_stream_until_stop(
             self,
             out_file: T.TextIO,
-            err_file: T.TextIO) -> int:
+            err_file: T.TextIO,
+            flush_streams_each_time: bool = False,
+            ) -> int:
         g = self.stream()
         retcode = None
         while True:
             try:
                 src, line = next(g)
                 if src == 'stdout':
-                    out_file.write(line)
-                elif src == 'stderr':
-                    err_file.write(line)
+                    ofile = out_file
+                else:
+                    assert src == 'stderr'
+                    ofile = err_file
+                ofile.write(line)
+                if flush_streams_each_time:
+                    ofile.flush()
             except StopIteration as e:
                 retcode = e.value
                 break
         return retcode
```

### Comparing `cmd2func-0.2.0/cmd2func.egg-info/PKG-INFO` & `cmd2func-0.2.1/cmd2func.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd2func
-Version: 0.2.0
+Version: 0.2.1
 Summary: Convert command to callable Python object.
 Home-page: https://github.com/Nanguage/cmd2func
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT license
 Keywords: cmd2func
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cmd2func-0.2.0/setup.py` & `cmd2func-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `cmd2func-0.2.0/tests/test_cmd2func.py` & `cmd2func-0.2.1/tests/test_cmd2func.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,7 +162,21 @@
     @cmd2func(conda_env="test")
     def test1():
         return cmd
 
     new_cmd = test1.process_cmd_str(cmd)
     assert new_cmd.startswith(
         "conda run --no-capture-output -n test")
+
+
+def test_flush_streams_each_time():
+    out = io.StringIO()
+
+    @cmd2func(
+        out_stream=out,
+        flush_streams_each_time=True,
+    )
+    def test1():
+        return "python -c 'print(1)'"
+
+    test1()
+    assert out.getvalue().strip() == "1"
```

### Comparing `cmd2func-0.2.0/tests/test_runner.py` & `cmd2func-0.2.1/tests/test_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     runner = ProcessRunner("python -c 'print(1)'")
     runner.run(capture_stdout=False)  # Don't capture stdout
     out = list(runner.stream())
     assert len(out) == 0
 
 
 def test_runner_shell():
-    runner = ProcessRunner("python -c 'print(1)'")
+    runner = ProcessRunner("python -c \"print(1)\"")
     runner.run(shell=True)
     out = list(runner.stream())
     assert len(out) == 1
```

