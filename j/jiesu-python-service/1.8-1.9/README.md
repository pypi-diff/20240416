# Comparing `tmp/jiesu-python-service-1.8.tar.gz` & `tmp/jiesu-python-service-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiesu-python-service-1.8.tar", last modified: Sat Mar 19 01:44:03 2022, max compression
+gzip compressed data, was "jiesu-python-service-1.9.tar", last modified: Sun Mar 20 20:54:29 2022, max compression
```

## Comparing `jiesu-python-service-1.8.tar` & `jiesu-python-service-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jie       (1000) jie       (1000)        0 2022-03-19 01:44:03.853590 jiesu-python-service-1.8/
--rw-rw-r--   0 jie       (1000) jie       (1000)      200 2022-03-19 01:44:03.853590 jiesu-python-service-1.8/PKG-INFO
-drwxrwxr-x   0 jie       (1000) jie       (1000)        0 2022-03-19 01:44:03.853590 jiesu-python-service-1.8/jiesu_python_service.egg-info/
--rw-rw-r--   0 jie       (1000) jie       (1000)      200 2022-03-19 01:44:03.000000 jiesu-python-service-1.8/jiesu_python_service.egg-info/PKG-INFO
--rw-rw-r--   0 jie       (1000) jie       (1000)      333 2022-03-19 01:44:03.000000 jiesu-python-service-1.8/jiesu_python_service.egg-info/SOURCES.txt
--rw-rw-r--   0 jie       (1000) jie       (1000)        1 2022-03-19 01:44:03.000000 jiesu-python-service-1.8/jiesu_python_service.egg-info/dependency_links.txt
--rw-rw-r--   0 jie       (1000) jie       (1000)        1 2022-03-16 21:49:03.000000 jiesu-python-service-1.8/jiesu_python_service.egg-info/not-zip-safe
--rw-rw-r--   0 jie       (1000) jie       (1000)       23 2022-03-19 01:44:03.000000 jiesu-python-service-1.8/jiesu_python_service.egg-info/requires.txt
--rw-rw-r--   0 jie       (1000) jie       (1000)       15 2022-03-19 01:44:03.000000 jiesu-python-service-1.8/jiesu_python_service.egg-info/top_level.txt
-drwxrwxr-x   0 jie       (1000) jie       (1000)        0 2022-03-19 01:44:03.853590 jiesu-python-service-1.8/python_service/
--rw-rw-r--   0 jie       (1000) jie       (1000)        0 2022-03-17 20:47:57.000000 jiesu-python-service-1.8/python_service/__init__.py
--rw-rw-r--   0 jie       (1000) jie       (1000)     7156 2022-03-19 01:43:32.000000 jiesu-python-service-1.8/python_service/service.py
--rw-rw-r--   0 jie       (1000) jie       (1000)      128 2022-03-19 01:44:03.853590 jiesu-python-service-1.8/setup.cfg
--rw-rw-r--   0 jie       (1000) jie       (1000)      261 2022-03-19 01:43:59.000000 jiesu-python-service-1.8/setup.py
+drwxrwxr-x   0 jie       (1000) jie       (1000)        0 2022-03-20 20:54:29.468079 jiesu-python-service-1.9/
+-rw-rw-r--   0 jie       (1000) jie       (1000)      200 2022-03-20 20:54:29.468079 jiesu-python-service-1.9/PKG-INFO
+drwxrwxr-x   0 jie       (1000) jie       (1000)        0 2022-03-20 20:54:29.464079 jiesu-python-service-1.9/jiesu_python_service.egg-info/
+-rw-rw-r--   0 jie       (1000) jie       (1000)      200 2022-03-20 20:54:29.000000 jiesu-python-service-1.9/jiesu_python_service.egg-info/PKG-INFO
+-rw-rw-r--   0 jie       (1000) jie       (1000)      333 2022-03-20 20:54:29.000000 jiesu-python-service-1.9/jiesu_python_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 jie       (1000) jie       (1000)        1 2022-03-20 20:54:29.000000 jiesu-python-service-1.9/jiesu_python_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 jie       (1000) jie       (1000)        1 2022-03-16 21:49:03.000000 jiesu-python-service-1.9/jiesu_python_service.egg-info/not-zip-safe
+-rw-rw-r--   0 jie       (1000) jie       (1000)       23 2022-03-20 20:54:29.000000 jiesu-python-service-1.9/jiesu_python_service.egg-info/requires.txt
+-rw-rw-r--   0 jie       (1000) jie       (1000)       15 2022-03-20 20:54:29.000000 jiesu-python-service-1.9/jiesu_python_service.egg-info/top_level.txt
+drwxrwxr-x   0 jie       (1000) jie       (1000)        0 2022-03-20 20:54:29.468079 jiesu-python-service-1.9/python_service/
+-rw-rw-r--   0 jie       (1000) jie       (1000)        0 2022-03-17 20:47:57.000000 jiesu-python-service-1.9/python_service/__init__.py
+-rw-rw-r--   0 jie       (1000) jie       (1000)     7219 2022-03-20 20:51:44.000000 jiesu-python-service-1.9/python_service/service.py
+-rw-rw-r--   0 jie       (1000) jie       (1000)      128 2022-03-20 20:54:29.468079 jiesu-python-service-1.9/setup.cfg
+-rw-rw-r--   0 jie       (1000) jie       (1000)      261 2022-03-20 20:54:07.000000 jiesu-python-service-1.9/setup.py
```

### Comparing `jiesu-python-service-1.8/python_service/service.py` & `jiesu-python-service-1.9/python_service/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,28 +207,28 @@
         self.port: int = self.args.port
         self.eureka_server: str = self.args.eureka
         self.log_file: PurePath = get_log_file(
             self.args.log, self.name + "_" + self.instance
         )
         self.log: logging.Logger = setup_log(self.log_file)
 
-    def start(self, httpHandler: BaseHttpHandler):
+    def start(self, create_handler: Callable[[], BaseHttpHandler]):
         eureka_client = register_eureka(
             self.eureka_server, self.name, self.port, self.instance
         )
 
         def unregister_eureka(signal: Any, frame: Any):
             self.cleanup()
             eureka_client.stop()
             sys.exit(0)
 
         signal.signal(signal.SIGINT, unregister_eureka)
         signal.signal(signal.SIGTERM, unregister_eureka)
 
-        httpHandler.set_log(self.log)
-
         def handler(*args: Any) -> BaseHTTPRequestHandler:
+            httpHandler = create_handler()
+            httpHandler.set_log(self.log)
             return HttpRequestHandler(httpHandler, self.log, *args)
 
         httpServer = ThreadingHTTPServer(("", self.port), handler)
         self.log.info("Serving at " + str(self.port))
         httpServer.serve_forever()
```

