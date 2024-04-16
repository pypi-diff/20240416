# Comparing `tmp/rats_apps-0.1.2.dev9-py3-none-any.whl.zip` & `tmp/rats_apps-0.1.3.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 6696 bytes, number of entries: 13
--rw-r--r--  2.0 unx      857 b- defN 80-Jan-01 00:00 rats/apps/__init__.py
--rw-r--r--  2.0 unx     5124 b- defN 80-Jan-01 00:00 rats/apps/_annotations.py
+-rw-r--r--  2.0 unx      858 b- defN 80-Jan-01 00:00 rats/apps/__init__.py
+-rw-r--r--  2.0 unx     5125 b- defN 80-Jan-01 00:00 rats/apps/_annotations.py
 -rw-r--r--  2.0 unx      553 b- defN 80-Jan-01 00:00 rats/apps/_composite_container.py
--rw-r--r--  2.0 unx     3131 b- defN 80-Jan-01 00:00 rats/apps/_container.py
+-rw-r--r--  2.0 unx     3129 b- defN 80-Jan-01 00:00 rats/apps/_container.py
 -rw-r--r--  2.0 unx      457 b- defN 80-Jan-01 00:00 rats/apps/_ids.py
 -rw-r--r--  2.0 unx      188 b- defN 80-Jan-01 00:00 rats/apps/_namespaces.py
 -rw-r--r--  2.0 unx      853 b- defN 80-Jan-01 00:00 rats/apps/_plugin_container.py
--rw-r--r--  2.0 unx     1304 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
+-rw-r--r--  2.0 unx     1305 b- defN 80-Jan-01 00:00 rats/apps/_scoping.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 rats/apps/py.typed
--rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/WHEEL
--rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.2.dev9.dist-info/RECORD
-13 files, 14402 bytes uncompressed, 4944 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx      716 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       86 b- defN 80-Jan-01 00:00 rats_apps-0.1.3.dev1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1045 b- defN 16-Jan-01 00:00 rats_apps-0.1.3.dev1.dist-info/RECORD
+13 files, 14403 bytes uncompressed, 4944 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: rats/apps/_scoping.py
 Comment: 
 
 Filename: rats/apps/py.typed
 Comment: 
 
-Filename: rats_apps-0.1.2.dev9.dist-info/METADATA
+Filename: rats_apps-0.1.3.dev1.dist-info/METADATA
 Comment: 
 
-Filename: rats_apps-0.1.2.dev9.dist-info/WHEEL
+Filename: rats_apps-0.1.3.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: rats_apps-0.1.2.dev9.dist-info/entry_points.txt
+Filename: rats_apps-0.1.3.dev1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rats_apps-0.1.2.dev9.dist-info/RECORD
+Filename: rats_apps-0.1.3.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rats/apps/__init__.py

```diff
@@ -1,13 +1,14 @@
 """
 Provides a small set of libraries to help create new applications.
 
 Applications give you the ability to define a development experience to match your project's
 domain.
 """
+
 from ._annotations import (
     AnnotatedContainer,
     config,
     container,
     fallback_config,
     fallback_group,
     fallback_service,
```

## rats/apps/_annotations.py

```diff
@@ -15,25 +15,27 @@
 class GroupAnnotations(NamedTuple):
     """
     The list of service ids attached to a given function.
 
     The `name` attribute is the name of the function, and the `namespace` attribute represents a
     specific meaning for the group of services.
     """
+
     name: str
     namespace: str
     groups: tuple[ServiceId[Any], ...]
 
 
 class FunctionAnnotations(NamedTuple):
     """
     Holds metadata about the annotated service provider.
 
     Loosely inspired by: https://peps.python.org/pep-3107/.
     """
+
     providers: tuple[GroupAnnotations, ...]
 
     def group_in_namespace(
         self,
         namespace: str,
         group_id: ServiceId[T_ServiceType],
     ) -> tuple[GroupAnnotations, ...]:
@@ -61,15 +63,14 @@
                 GroupAnnotations(name=name, namespace=namespace, groups=tuple(services))
                 for namespace, services in self._service_ids.items()
             ]
         )
 
 
 class AnnotatedContainer(Container):
-
     def get_namespaced_group(
         self,
         namespace: str,
         group_id: ServiceId[T_ServiceType],
     ) -> Iterator[T_ServiceType]:
         annotations = _extract_class_annotations(type(self))
         containers = annotations.with_namespace(ProviderNamespaces.CONTAINERS)
```

## rats/apps/_container.py

```diff
@@ -3,22 +3,20 @@
 from typing import Generic, Protocol
 
 from ._ids import ServiceId, T_ServiceType, Tco_ConfigType, Tco_ServiceType
 from ._namespaces import ProviderNamespaces
 
 
 class ServiceProvider(Protocol[Tco_ServiceType]):
-
     @abstractmethod
     def __call__(self) -> Tco_ServiceType:
         """Return the service instance."""
 
 
 class ConfigProvider(ServiceProvider[Tco_ConfigType], Protocol[Tco_ConfigType]):
-
     @abstractmethod
     def __call__(self) -> Tco_ConfigType:
         """Return the config instance."""
 
 
 class Container(Protocol):
     """Main interface for service containers."""
```

## rats/apps/_scoping.py

```diff
@@ -11,14 +11,15 @@
 def autoscope(cls: type[T]) -> type[T]:
     """
     Decorator that replaces all ServiceId instances in the class with scoped ServiceId instances.
 
     The scoped ServiceId instances have a prefix to eliminate the chance of conflicts across
     packages.
     """
+
     def wrap(func: Callable[..., Any]) -> Callable[..., Any]:
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> ServiceId[Any]:
             result = func(*args, **kwargs)
             if not isinstance(result, ServiceId):
                 return result
 
             return ServiceId[Any](f"{cls.__module__}:{cls.__name__}[{result.name}]")
```

## Comparing `rats_apps-0.1.2.dev9.dist-info/METADATA` & `rats_apps-0.1.3.dev1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rats-apps
-Version: 0.1.2.dev9
+Version: 0.1.3.dev1
 Summary: research analysis tools for building applications
 Home-page: https://github.com/microsoft/rats/
 License: MIT
 Keywords: pipelines,machine learning,research
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rats_apps-0.1.2.dev9.dist-info/RECORD` & `rats_apps-0.1.3.dev1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-rats/apps/__init__.py,sha256=EHza57K66uM7w8pFBJBqMWaJ7Xn_7E4hn0xA7k8Ag5U,857
-rats/apps/_annotations.py,sha256=V6sNsvh66VGB6ciog0AwPgXwTjBrtlIZXT-ZZx_LpdY,5124
+rats/apps/__init__.py,sha256=JYVss3L2R4uxdOp4Ozfg_cHWgRvCWq79OyVZefFw9wY,858
+rats/apps/_annotations.py,sha256=NGCw1JMZdPMoK_pE61iXgjeI1Xn7P5WXLt7t8zWligg,5125
 rats/apps/_composite_container.py,sha256=wSWVQWPin2xxIlEoSgk_D1rlc3N2gpTxQ2y9UFdqXy0,553
-rats/apps/_container.py,sha256=JSmO4x0JcnM9gQP0ki9JcGzYqbjmgAj79lZw5YfBrqI,3131
+rats/apps/_container.py,sha256=5uiCyxN6HS2z97XcTOFP-t72cNoB1U1sJMkMcfSfDps,3129
 rats/apps/_ids.py,sha256=dxWCPMpMA_vpaTDJEKNByIBJaX97Db203XqWLhaOezo,457
 rats/apps/_namespaces.py,sha256=THUV_Xj5PtweC23Ob-zsSpk8exC4fT-qRwjpQ6IDm0U,188
 rats/apps/_plugin_container.py,sha256=W_xQD2btc0N2dEb3c5tXM-ZZ4A4diMpkCjbOZdlXYuI,853
-rats/apps/_scoping.py,sha256=-5hl0RoOdQGkxWLIn42hthMUyX8_84sV8H3u40y-gIU,1304
+rats/apps/_scoping.py,sha256=lRV1DDq-U4mr4WOQhvFjTiCQe2dKY95LNn6b0RXRjFA,1305
 rats/apps/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rats_apps-0.1.2.dev9.dist-info/METADATA,sha256=-WiawuBlYmLlPdFLoWa8DvkM1-9Dcn57jNmoJRZIX_4,716
-rats_apps-0.1.2.dev9.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-rats_apps-0.1.2.dev9.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
-rats_apps-0.1.2.dev9.dist-info/RECORD,,
+rats_apps-0.1.3.dev1.dist-info/METADATA,sha256=zRGXo26P57Mt62Y19aR13fsMl7CvBQnIZnGkUdGOswE,716
+rats_apps-0.1.3.dev1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+rats_apps-0.1.3.dev1.dist-info/entry_points.txt,sha256=Vu1IgAPQvL4xMJzW_OG2JSPFac7HalCHyXiRr0-OfCI,86
+rats_apps-0.1.3.dev1.dist-info/RECORD,,
```

