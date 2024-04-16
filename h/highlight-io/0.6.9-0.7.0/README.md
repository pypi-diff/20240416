# Comparing `tmp/highlight_io-0.6.9.tar.gz` & `tmp/highlight_io-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.6.9.tar", max compression
+gzip compressed data, was "highlight_io-0.7.0.tar", max compression
```

## Comparing `highlight_io-0.6.9.tar` & `highlight_io-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0      867 2023-12-19 18:36:44.660250 highlight_io-0.6.9/README.md
--rw-r--r--   0        0        0       64 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1662 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/django.py
--rw-r--r--   0        0        0     2191 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1549 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1327 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/requests.py
--rw-r--r--   0        0        0     1072 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0    15118 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/sdk.py
--rw-r--r--   0        0        0        0 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/utils/__init__.py
--rw-r--r--   0        0        0     1150 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/utils/lru_cache.py
--rw-r--r--   0        0        0      500 2023-12-19 18:36:44.660250 highlight_io-0.6.9/highlight_io/utils/utils.py
--rw-r--r--   0        0        0     1740 2023-12-19 18:36:44.664250 highlight_io-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 highlight_io-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1340 2024-04-16 19:50:41.352277 highlight_io-0.7.0/README.md
+-rw-r--r--   0        0        0       64 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0      516 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/boto.py
+-rw-r--r--   0        0        0      541 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/boto3sqs.py
+-rw-r--r--   0        0        0      530 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/celery.py
+-rw-r--r--   0        0        0     1911 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     2224 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1688 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0      523 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/redis.py
+-rw-r--r--   0        0        0      544 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/requests.py
+-rw-r--r--   0        0        0     1072 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0      558 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/integrations/sqlalchemy.py
+-rw-r--r--   0        0        0    19222 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/sdk.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/utils/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-16 19:50:41.356277 highlight_io-0.7.0/highlight_io/utils/lru_cache.py
+-rw-r--r--   0        0        0     2674 2024-04-16 19:50:41.356277 highlight_io-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 highlight_io-0.7.0/PKG-INFO
```

### Comparing `highlight_io-0.6.9/highlight_io/integrations/aws.py` & `highlight_io-0.7.0/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.6.9/highlight_io/integrations/azure.py` & `highlight_io-0.7.0/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.6.9/highlight_io/integrations/django.py` & `highlight_io-0.7.0/highlight_io/integrations/django.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,21 @@
             try:
                 session_id, request_id = str(
                     environ[DjangoIntegration.HIGHLIGHT_HEADER]
                 ).split("/")
             except (KeyError, ValueError):
                 pass
 
-            with highlight_io.H.get_instance().trace(session_id, request_id):
+            span_name = f"{environ.get('REQUEST_METHOD')} {environ.get('PATH_INFO')}"
+            qs = environ.get("QUERY_STRING")
+            if qs:
+                span_name = f"{span_name}?{qs}"
+            with highlight_io.H.get_instance().trace(
+                session_id, request_id, span_name=span_name
+            ):
                 return self._orig_django(app, environ, start_response)
 
         WSGIHandler.__call__ = wrapped_call
 
         signals.got_request_exception.connect(self._exception_handler)
 
     def disable(self):
```

### Comparing `highlight_io-0.6.9/highlight_io/integrations/fastapi.py` & `highlight_io-0.7.0/highlight_io/integrations/fastapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,18 @@
         try:
             session_id, request_id = request.headers.get(
                 FastAPIMiddleware.HIGHLIGHT_HEADER
             ).split("/")
         except (AttributeError, KeyError, ValueError):
             pass
 
-        with highlight_io.H.get_instance().trace(session_id, request_id):
+        span_name = f"{request.method} {request.base_url}"
+        with highlight_io.H.get_instance().trace(
+            session_id, request_id, span_name=span_name
+        ):
             resp = await call_next(request)
             # if the request raises an `HTTPException`, the exception isn't propagated.
             # we detect this by checking the status code and recording a special type of error
             if resp.status_code >= 400:
                 body = b""
                 if hasattr(resp, "body"):
                     body = resp.body
@@ -34,15 +37,14 @@
                         body += chunk
                 highlight_io.H.get_instance().record_http_error(
                     status_code=resp.status_code,
                     detail=body.decode(),
                     attributes={
                         "http.response.headers": resp.headers,
                         "http.request.headers": request.headers,
-                        "http.request.detail": await request.body(),
                         SpanAttributes.HTTP_METHOD: request.method,
                         SpanAttributes.HTTP_URL: str(request.url),
                     },
                 )
                 return Response(
                     content=body,
                     status_code=resp.status_code,
```

### Comparing `highlight_io-0.6.9/highlight_io/integrations/flask.py` & `highlight_io-0.7.0/highlight_io/integrations/flask.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,15 +32,18 @@
             try:
                 session_id, request_id = str(
                     environ[FlaskIntegration.HIGHLIGHT_HEADER]
                 ).split("/")
             except (KeyError, ValueError):
                 pass
 
-            with highlight_io.H.get_instance().trace(session_id, request_id):
+            span_name = f"{environ.get('REQUEST_METHOD')} {environ.get('REQUEST_URI')}"
+            with highlight_io.H.get_instance().trace(
+                session_id, request_id, span_name=span_name
+            ):
                 return self._orig_flask(app, environ, start_response)
 
         Flask.__call__ = wrapped_call
 
         got_request_exception.connect(self.exception_handler)
 
     def disable(self):
```

### Comparing `highlight_io-0.6.9/highlight_io/integrations/gcp.py` & `highlight_io-0.7.0/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.6.9/highlight_io/integrations/serverless.py` & `highlight_io-0.7.0/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.6.9/highlight_io/sdk.py` & `highlight_io-0.7.0/highlight_io/sdk.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,86 @@
 import contextlib
 import http
 import json
 import logging
+import sys
 import traceback
 import typing
 
 from opentelemetry import trace, _logs
 from opentelemetry._logs.severity import std_to_otel
+from opentelemetry.baggage import set_baggage, get_baggage
+from opentelemetry.context import Context, attach
 from opentelemetry.exporter.otlp.proto.http import Compression
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
-from opentelemetry.sdk._logs import LoggerProvider, LogRecord
+from opentelemetry.sdk._logs import (
+    LoggerProvider,
+    LogRecord,
+)
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.trace import TracerProvider, Span
+from opentelemetry.sdk.trace import TracerProvider, Span, SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import INVALID_SPAN
 
 from highlight_io.integrations import Integration
-from highlight_io.utils.lru_cache import LRUCache
+from highlight_io.integrations.boto import BotoIntegration
+from highlight_io.integrations.boto3sqs import Boto3SQSIntegration
+from highlight_io.integrations.celery import CeleryIntegration
+from highlight_io.integrations.redis import RedisIntegration
 from highlight_io.integrations.requests import RequestsIntegration
+from highlight_io.integrations.sqlalchemy import SQLAlchemyIntegration
+from highlight_io.utils.lru_cache import LRUCache
 
-DEFAULT_INTEGRATIONS = [RequestsIntegration]
+DEFAULT_INTEGRATIONS = [
+    BotoIntegration,
+    Boto3SQSIntegration,
+    CeleryIntegration,
+    RedisIntegration,
+    RequestsIntegration,
+    SQLAlchemyIntegration,
+]
 
 
 class LogHandler(logging.Handler):
     def __init__(self, highlight: "H", level=logging.NOTSET):
+        """Create a `logging.Handler` that ships data to highlight.
+        :param highlight: Highlight object
+        :param level: Log level
+
+        Example:
+            # define the formatting for logs sent to highlight
+            formatter = logging.Formatter(' %(name)s :: %(levelname)-8s :: %(message)s')
+            handler = LogHandler(H)
+            handler.setFormatter(formatter)
+            # create the logger object with a custom logger module name
+            lg = logging.getLogger("my.logger")
+            lg.addHandler(handler)
+
+            lg.warning("oh, no!")
+        """
         self.highlight = highlight
         super(LogHandler, self).__init__(level=level)
 
     def emit(self, record: logging.LogRecord):
         ctx = contextlib.nullcontext
         span = trace.get_current_span()
 
         if span is None or not span.is_recording():
             ctx = self.highlight.trace
 
         with ctx():
-            self.highlight.log_hook(trace.get_current_span(), record)
+            if self.filter(record):
+                self.highlight.log_hook(
+                    trace.get_current_span(), record, formatted=self.format(record)
+                )
 
 
 class H(object):
     REQUEST_HEADER = "X-Highlight-Request"
     OTLP_HTTP = "https://otel.highlight.io:4318"
     _instance: "H" = None
     _logging_instrumented = False
@@ -68,14 +104,16 @@
         disabled_integrations: typing.List[str] = None,
         otlp_endpoint: str = "",
         instrument_logging: bool = True,
         log_level=logging.DEBUG,
         service_name: str = "",
         service_version: str = "",
         environment: str = "",
+        debug: bool = False,
+        **kwargs,
     ):
         """
         Setup Highlight backend instrumentation.
 
         Example:
             import highlight_io
             H = highlight_io.H('project_id', ...)
@@ -85,55 +123,113 @@
         :param integrations: a list of Integrations that allow connecting with your framework, like Flask or Django.
         :param disabled_integrations: a list of integrations to disable.
         :param instrument_logging: defaults to True. set False to disable auto-instrumentation of python `logging` methods.
         :param otlp_endpoint: set to a custom otlp destination
         :param service_name: a string to name this app
         :param service_version: a string to set this app's version (typically a Git deploy sha).
         :param environment: a string to set this app's environment (e.g. 'production', 'development').
+        :param debug: a boolean to turn on debug logging.
+        :param **kwargs: optional kwargs passed to the BatchLogRecordProcessor and BatchSpanProcessor.
         :return: a configured H instance
         """
+        kwargs.update(
+            {
+                "schedule_delay_millis": 1000,
+                "max_export_batch_size": 1024 * 1024,
+                "max_queue_size": 1024 * 1024,
+            }
+        )
+
+        if debug:
+            root = logging.getLogger()
+            root.setLevel(logging.DEBUG)
+            handler = logging.StreamHandler(sys.stdout)
+            handler.setLevel(logging.DEBUG)
+            formatter = logging.Formatter(
+                "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+            )
+            handler.setFormatter(formatter)
+            root.addHandler(handler)
+
+        logger = logging.getLogger("highlight_io")
+
         H._instance = self
         self._project_id = project_id
         self._integrations = integrations or []
         self._disabled_integrations = disabled_integrations or []
         self._otlp_endpoint = otlp_endpoint or H.OTLP_HTTP
+        logger.debug(
+            "Highlight initializing: %s %s %s",
+            self._otlp_endpoint,
+            self._project_id,
+            kwargs,
+        )
         self._log_handler = LogHandler(self, level=log_level)
         if instrument_logging:
             self._instrument_logging()
 
+        class HighlightSpanProcessor(SpanProcessor):
+            def on_start(
+                self, span: Span, parent_context: typing.Optional[Context] = None
+            ) -> None:
+                session_id, request_id = "", ""
+                try:
+                    header_value = str(
+                        get_baggage(H._instance.REQUEST_HEADER, parent_context)
+                    )
+                    session_id, request_id = header_value.split("/")
+                except (AttributeError, KeyError, ValueError):
+                    pass
+                if not session_id or not request_id:
+                    session_id, request_id = H._instance.get_highlight_context(
+                        span.context.trace_id
+                    )
+
+                span.set_attributes(
+                    {
+                        "highlight.project_id": H._instance._project_id,
+                        "highlight.trace_id": request_id,
+                        "highlight.session_id": session_id,
+                    }
+                )
+                attach(
+                    set_baggage(
+                        H._instance.REQUEST_HEADER, f"{session_id}/{request_id}"
+                    )
+                )
+
+                return super().on_start(span, parent_context)
+
         resource = _build_resource(
             service_name=service_name,
             service_version=service_version,
             environment=environment,
         )
         self._trace_provider = TracerProvider(resource=resource)
+        self._trace_provider.add_span_processor(HighlightSpanProcessor())
         self._trace_provider.add_span_processor(
             BatchSpanProcessor(
                 OTLPSpanExporter(
                     f"{self._otlp_endpoint}/v1/traces", compression=Compression.Gzip
                 ),
-                schedule_delay_millis=1000,
-                max_export_batch_size=128,
-                max_queue_size=1024,
+                **kwargs,
             )
         )
         trace.set_tracer_provider(self._trace_provider)
         self.tracer = trace.get_tracer(__name__)
 
         self._log_provider = LoggerProvider(
             resource=resource,
         )
         self._log_provider.add_log_record_processor(
             BatchLogRecordProcessor(
                 OTLPLogExporter(
                     f"{self._otlp_endpoint}/v1/logs", compression=Compression.Gzip
                 ),
-                schedule_delay_millis=1000,
-                max_export_batch_size=128,
-                max_queue_size=1024,
+                **kwargs,
             )
         )
         _logs.set_logger_provider(self._log_provider)
         self.log = self._log_provider.get_logger(__name__)
 
         skip_disabled_integrations = self._disabled_integrations.copy()
 
@@ -150,14 +246,15 @@
         self._log_provider.force_flush()
 
     @contextlib.contextmanager
     def trace(
         self,
         session_id: typing.Optional[str] = "",
         request_id: typing.Optional[str] = "",
+        span_name: typing.Optional[str] = "highlight-ctx",
         attributes: typing.Optional[typing.Dict[str, any]] = None,
     ) -> Span:
         """
         Catch exceptions raised by your app using this context manager.
         Exceptions will be recorded with the Highlight project and
         associated with a frontend session when headers are provided.
 
@@ -169,23 +266,24 @@
                 with H.trace(headers={'X-Highlight-Request': '...'}):
                     raise Exception('fake error!')
 
 
         :param session_id: the highlight session that initiated this network request.
         :param request_id: the identifier of the current network request.
         :param attributes: additional attributes to attribute to this error.
+        :param span_name: span name to record.
         :return: Span
         """
         # in case the otel library is in a non-recording context, do nothing
         if not hasattr(self, "tracer") or not self.tracer:
             yield
             return
 
         with self.tracer.start_as_current_span(
-            "highlight-ctx", record_exception=False, set_status_on_exception=False
+            span_name, record_exception=False, set_status_on_exception=False
         ) as span:
             span.set_attributes({"highlight.project_id": self._project_id})
             span.set_attributes({"highlight.session_id": session_id})
             span.set_attributes({"highlight.trace_id": request_id})
 
             self._context_map.put(span.context.trace_id, (session_id, request_id))
 
@@ -310,27 +408,37 @@
                 format="{message}",
                 level="INFO",
                 backtrace=True,
             )
         """
         return self._log_handler
 
-    def log_hook(self, span: Span, record: logging.LogRecord):
+    def log_hook(self, span: Span, record: logging.LogRecord, formatted: str = ""):
         if span and span.is_recording():
             ctx = span.get_span_context()
+            session_id, request_id = H._instance.get_highlight_context(
+                span.context.trace_id
+            )
             # record.created is sec but timestamp should be ns
             ts = int(record.created * 1000.0 * 1000.0 * 1000.0)
             attributes = span.attributes.copy()
             attributes[SpanAttributes.CODE_FUNCTION] = record.funcName
             attributes[SpanAttributes.CODE_NAMESPACE] = record.module
             attributes[SpanAttributes.CODE_FILEPATH] = record.pathname
             attributes[SpanAttributes.CODE_LINENO] = record.lineno
-            attributes.update(record.args or {})
+            attributes["highlight.trace_id"] = request_id
+            attributes["highlight.session_id"] = session_id
+            if isinstance(record.args, dict):
+                attributes.update(record.args)
+            elif isinstance(record.args, list):
+                attributes["args"] = record.args
+            elif record.args:
+                attributes["args"] = str(record.args)
 
-            message = record.getMessage()
+            message = formatted or record.getMessage()
             try:
                 # Handle loguru's serialize=True format
                 # See: https://loguru.readthedocs.io/en/stable/api/logger.html#record
                 obj = json.loads(message)
                 extra = obj["record"]["extra"]
                 message = obj["text"]
```

### Comparing `highlight_io-0.6.9/highlight_io/utils/lru_cache.py` & `highlight_io-0.7.0/highlight_io/utils/lru_cache.py`

 * *Files identical despite different names*

