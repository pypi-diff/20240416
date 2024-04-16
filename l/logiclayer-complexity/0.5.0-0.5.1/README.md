# Comparing `tmp/logiclayer_complexity-0.5.0.tar.gz` & `tmp/logiclayer_complexity-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer_complexity-0.5.0.tar", max compression
+gzip compressed data, was "logiclayer_complexity-0.5.1.tar", max compression
```

## Comparing `logiclayer_complexity-0.5.0.tar` & `logiclayer_complexity-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1093 2022-08-10 00:34:08.071136 logiclayer_complexity-0.5.0/LICENSE
--rw-r--r--   0        0        0      292 2024-04-08 21:02:29.621542 logiclayer_complexity-0.5.0/logiclayer_complexity/__init__.py
--rw-r--r--   0        0        0     1686 2024-04-08 19:52:31.149383 logiclayer_complexity-0.5.0/logiclayer_complexity/common.py
--rw-r--r--   0        0        0      184 2023-12-07 21:31:37.974492 logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/__init__.py
--rw-r--r--   0        0        0     3409 2024-02-09 22:30:54.554079 logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/dependencies.py
--rw-r--r--   0        0        0     5576 2024-04-08 20:57:25.893205 logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/structs.py
--rw-r--r--   0        0        0     4721 2024-02-27 19:14:50.359214 logiclayer_complexity-0.5.0/logiclayer_complexity/dependencies.py
--rw-r--r--   0        0        0    15938 2024-04-08 20:30:18.639653 logiclayer_complexity-0.5.0/logiclayer_complexity/module.py
--rw-r--r--   0        0        0     2912 2024-02-09 22:30:54.588648 logiclayer_complexity-0.5.0/logiclayer_complexity/opportunity_gain.py
--rw-r--r--   0        0        0      279 2024-04-03 16:43:40.886690 logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/__init__.py
--rw-r--r--   0        0        0     4565 2024-04-08 18:59:34.649911 logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/peii.py
--rw-r--r--   0        0        0     4302 2024-04-08 18:59:50.506445 logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/pgi.py
--rw-r--r--   0        0        0      134 2023-12-07 21:02:11.815737 logiclayer_complexity-0.5.0/logiclayer_complexity/rca/__init__.py
--rw-r--r--   0        0        0     6425 2024-02-09 19:43:15.189094 logiclayer_complexity-0.5.0/logiclayer_complexity/rca/dependencies.py
--rw-r--r--   0        0        0     6105 2024-03-25 19:51:09.834805 logiclayer_complexity-0.5.0/logiclayer_complexity/rca/structs.py
--rw-r--r--   0        0        0      359 2024-02-02 19:36:49.968808 logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/__init__.py
--rw-r--r--   0        0        0     2705 2024-02-09 22:30:54.589330 logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/dependencies.py
--rw-r--r--   0        0        0     4124 2024-02-02 21:19:27.228036 logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/structs.py
--rw-r--r--   0        0        0     3040 2024-04-08 19:17:16.727139 logiclayer_complexity-0.5.0/logiclayer_complexity/response.py
--rw-r--r--   0        0        0     2660 2024-04-08 19:17:07.621358 logiclayer_complexity-0.5.0/logiclayer_complexity/wdi.py
--rw-r--r--   0        0        0     1658 2022-08-10 00:46:00.273578 logiclayer_complexity-0.5.0/PACKAGE.md
--rw-r--r--   0        0        0     1078 2024-04-08 21:02:20.533797 logiclayer_complexity-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 logiclayer_complexity-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-08-10 00:34:08.071136 logiclayer_complexity-0.5.1/LICENSE
+-rw-r--r--   0        0        0      292 2024-04-16 21:36:35.493903 logiclayer_complexity-0.5.1/logiclayer_complexity/__init__.py
+-rw-r--r--   0        0        0     1686 2024-04-08 19:52:31.149383 logiclayer_complexity-0.5.1/logiclayer_complexity/common.py
+-rw-r--r--   0        0        0      184 2023-12-07 21:31:37.974492 logiclayer_complexity-0.5.1/logiclayer_complexity/complexity/__init__.py
+-rw-r--r--   0        0        0     3409 2024-02-09 22:30:54.554079 logiclayer_complexity-0.5.1/logiclayer_complexity/complexity/dependencies.py
+-rw-r--r--   0        0        0     5495 2024-04-16 20:43:40.161855 logiclayer_complexity-0.5.1/logiclayer_complexity/complexity/structs.py
+-rw-r--r--   0        0        0     5580 2024-04-16 20:24:41.153018 logiclayer_complexity-0.5.1/logiclayer_complexity/dependencies.py
+-rw-r--r--   0        0        0    18414 2024-04-16 20:53:44.612929 logiclayer_complexity-0.5.1/logiclayer_complexity/module.py
+-rw-r--r--   0        0        0     2831 2024-04-16 20:35:52.218592 logiclayer_complexity-0.5.1/logiclayer_complexity/opportunity_gain.py
+-rw-r--r--   0        0        0      279 2024-04-03 16:43:40.886690 logiclayer_complexity-0.5.1/logiclayer_complexity/pmi/__init__.py
+-rw-r--r--   0        0        0     4607 2024-04-16 20:39:23.329720 logiclayer_complexity-0.5.1/logiclayer_complexity/pmi/peii.py
+-rw-r--r--   0        0        0     4344 2024-04-16 20:37:17.082156 logiclayer_complexity-0.5.1/logiclayer_complexity/pmi/pgi.py
+-rw-r--r--   0        0        0      134 2023-12-07 21:02:11.815737 logiclayer_complexity-0.5.1/logiclayer_complexity/rca/__init__.py
+-rw-r--r--   0        0        0     6425 2024-02-09 19:43:15.189094 logiclayer_complexity-0.5.1/logiclayer_complexity/rca/dependencies.py
+-rw-r--r--   0        0        0     6147 2024-04-16 20:31:54.241321 logiclayer_complexity-0.5.1/logiclayer_complexity/rca/structs.py
+-rw-r--r--   0        0        0      359 2024-02-02 19:36:49.968808 logiclayer_complexity-0.5.1/logiclayer_complexity/relatedness/__init__.py
+-rw-r--r--   0        0        0     2705 2024-02-09 22:30:54.589330 logiclayer_complexity-0.5.1/logiclayer_complexity/relatedness/dependencies.py
+-rw-r--r--   0        0        0     4043 2024-04-16 20:35:27.465692 logiclayer_complexity-0.5.1/logiclayer_complexity/relatedness/structs.py
+-rw-r--r--   0        0        0     3040 2024-04-08 19:17:16.727139 logiclayer_complexity-0.5.1/logiclayer_complexity/response.py
+-rw-r--r--   0        0        0     2660 2024-04-08 19:17:07.621358 logiclayer_complexity-0.5.1/logiclayer_complexity/wdi.py
+-rw-r--r--   0        0        0     1658 2022-08-10 00:46:00.273578 logiclayer_complexity-0.5.1/PACKAGE.md
+-rw-r--r--   0        0        0     1078 2024-04-16 21:36:29.600736 logiclayer_complexity-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 logiclayer_complexity-0.5.1/PKG-INFO
```

### Comparing `logiclayer_complexity-0.5.0/LICENSE` & `logiclayer_complexity-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/common.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/common.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/dependencies.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/complexity/dependencies.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/complexity/structs.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/complexity/structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,14 @@
 class ComplexityParameters:
     rca_params: "RcaParameters"
     cutoff: float = 1
     iterations: int = 20
     rank: bool = False
     sort_ascending: Optional[bool] = None
 
-    @property
-    def request(self):
-        return self.rca_params.request
-
     def _calculate(self, rca: pd.Series, kind: Literal["ECI", "PCI"]) -> pd.Series:
         df_rca = rca.unstack()
         eci, pci = ec.complexity(df_rca, cutoff=self.cutoff, iterations=self.iterations)
 
         if kind == "ECI":
             return eci
         if kind == "PCI":
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/module.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/module.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 """
 
 from typing import Dict, List, Mapping, Optional, Tuple
 
 import logiclayer as ll
 import pandas as pd
 import polars as pl
-from fastapi import Depends, Header, HTTPException, Request, status
+from fastapi import Depends, Header, HTTPException, Request
 from fastapi.responses import JSONResponse, RedirectResponse
-from tesseract_olap import DataRequest, OlapServer, PublicCube, PublicSchema
+from tesseract_olap import (
+    DataRequest,
+    NotAuthorized,
+    OlapServer,
+    TesseractCube,
+    TesseractSchema,
+)
 from tesseract_olap.backend import Session
 from tesseract_olap.exceptions import QueryError, TesseractError
 from typing_extensions import Annotated
 
 from . import __title__, __version__
 from .complexity import (
     ComplexityParameters,
     ComplexitySubnationalParameters,
     prepare_complexity_params,
     prepare_complexity_subnational_params,
 )
-from .dependencies import parse_alias, parse_filter
+from .dependencies import auth_token, parse_alias, parse_filter
 from .opportunity_gain import OpportunityGainParameters, prepare_opportunity_gain_params
 from .pmi import (
     PEIIParameters,
     PGIParameters,
     prepare_peii_params,
     prepare_pgi_params,
 )
@@ -56,15 +62,15 @@
     def __init__(
         self,
         olap: "OlapServer",
         wdi: Optional["WdiReferenceSchema"] = None,
         **kwargs,
     ):
         """Setups the server for this instance."""
-        super().__init__()
+        super().__init__(**kwargs)
 
         if olap is None:
             raise ValueError(
                 "EconomicComplexityModule requires a tesseract_olap.OlapServer instance"
             )
 
         self.debug = kwargs.get("debug", False)
@@ -101,250 +107,276 @@
         """Retrieves the data from the backend, and handles related errors."""
         query = self.olap.build_query(request)
         result = session.fetch_dataframe(query)
         return result.data
 
     @ll.route("GET", "/")
     def route_status(self) -> ComplexityStatus:
+        """Retrieves the current status of the module."""
         return ComplexityStatus(
             module=__title__,
             version=__version__,
             debug=False,
             extras={
                 "wdi": "disabled" if self.wdi is None else "enabled",
             },
         )
 
     @ll.route("GET", "/cubes")
-    def route_schema(self, locale: Optional[str] = None) -> PublicSchema:
-        roles = []
+    def route_schema(
+        self,
+        locale: Optional[str] = None,
+        token: Optional[ll.AuthToken] = Depends(auth_token),
+    ) -> TesseractSchema:
+        """Returns the public schema, available for this module's instance."""
+        roles = self.auth.get_roles(token)
         locale = self.olap.schema.default_locale if locale is None else locale
-        return PublicSchema.from_entity(self.olap.schema, locale=locale, roles=roles)
+        return TesseractSchema.from_entity(self.olap.schema, locale=locale, roles=roles)
 
     @ll.route("GET", "/cubes/{cube_name}")
-    def route_schema_cube(self, cube_name: str, locale: Optional[str] = None):
-        roles = []
+    def route_schema_cube(
+        self,
+        cube_name: str,
+        locale: Optional[str] = None,
+        token: Optional[ll.AuthToken] = Depends(auth_token),
+    ) -> TesseractCube:
+        """Returns the public schema for a single cube, available for this module's instance."""
+        roles = self.auth.get_roles(token)
         cube = self.olap.schema.get_cube(cube_name)
         if not cube.is_authorized(roles):
-            raise HTTPException(
-                status.HTTP_403_FORBIDDEN,
-                "You don't have authorization to access this cube. "
-                "Check your credentials and try again.",
-            )
+            raise NotAuthorized(f"Cube({cube.name})", roles)
         locale = self.olap.schema.default_locale if locale is None else locale
-        return PublicCube.from_entity(cube, locale=locale)
+        return TesseractCube.from_entity(cube, locale=locale)
 
     @ll.route("GET", "/rca.{extension}")
     def route_rca(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RcaParameters = Depends(prepare_rca_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
         wdi: List[WdiParameters] = Depends(parse_wdi),
     ):
         """RCA calculation endpoint."""
+        request = params.build_request(self.auth.get_roles(token))
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params, wdi=wdi)
 
         df_rca = params.calculate(df)
 
         return extension.serialize(df_rca, aliases, filters)
 
     @ll.route("GET", "/eci.{extension}")
     def route_eci(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexityParameters = Depends(prepare_complexity_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
         wdi: List[WdiParameters] = Depends(parse_wdi),
     ):
         """ECI calculation endpoint."""
+        request = params.rca_params.build_request(self.auth.get_roles(token))
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params.rca_params, wdi=wdi)
 
         df_eci = params.calculate(df, "ECI")
 
         return extension.serialize(df_eci, aliases, filters)
 
     @ll.route("GET", "/pci.{extension}")
     def route_pci(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexityParameters = Depends(prepare_complexity_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
         wdi: List[WdiParameters] = Depends(parse_wdi),
     ):
         """PCI calculation endpoint."""
+        request = params.rca_params.build_request(self.auth.get_roles(token))
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params.rca_params, wdi=wdi)
 
         df_pci = params.calculate(df, "PCI")
 
         return extension.serialize(df_pci, aliases, filters)
 
     @ll.route("GET", "/relatedness.{extension}")
     def route_relatedness(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RelatednessParameters = Depends(prepare_relatedness_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """Relatedness calculation endpoint."""
+        request = params.rca_params.build_request(self.auth.get_roles(token))
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params.rca_params)
 
         df_reltd = params.calculate(df)
 
         return extension.serialize(df_reltd, aliases, filters)
 
     @ll.route("GET", "/opportunity_gain.{extension}")
     def route_opportunity_gain(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: OpportunityGainParameters = Depends(prepare_opportunity_gain_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """Opportunity Gain calculation endpoint."""
+        request = params.rca_params.build_request(self.auth.get_roles(token))
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params.rca_params)
 
         df_opgain = params.calculate(df)
 
         return extension.serialize(df_opgain, aliases, filters)
 
     @ll.route("GET", "/pgi.{extension}")
     def route_pgi(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: PGIParameters = Depends(prepare_pgi_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """PGI calculation endpoint."""
+        roles = self.auth.get_roles(token)
+        request = params.rca_params.build_request(roles)
+        request_gini = params.build_request(roles)
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.rca_params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params.rca_params)
-            df_gini = self.fetch_data(session, params.request).to_pandas()
+            df_gini = self.fetch_data(session, request_gini).to_pandas()
 
         df_pgi = params.calculate(df, df_gini)
 
         return extension.serialize(df_pgi, aliases, filters)
 
     @ll.route("GET", "/peii.{extension}")
     def route_peii(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: PEIIParameters = Depends(prepare_peii_params),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """PEII calculation endpoint."""
+        roles = self.auth.get_roles(token)
+        request = params.rca_params.build_request(roles)
+        request_emissions = params.build_request(roles)
         with self.olap.session() as session:
-            df = self.fetch_data(session, params.rca_params.request)
+            df = self.fetch_data(session, request)
             df = self.apply_threshold(session, df, rca=params.rca_params)
-            df_emissions = self.fetch_data(session, params.request).to_pandas()
+            df_emissions = self.fetch_data(session, request_emissions).to_pandas()
 
         df_peii = params.calculate(df, df_emissions)
 
         return extension.serialize(df_peii, aliases, filters)
 
     @ll.route("GET", "/rca_subnational.{extension}")
     def route_rca_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
         params: RcaSubnationalParameters = Depends(prepare_subnatrca_params),
     ):
+        roles = self.auth.get_roles(token)
+        req_subnat = params.subnat_params.build_request(roles)
+        req_global = params.global_params.build_request(roles)
         with self.olap.session() as session:
-            df_subnat = self.fetch_data(
-                session, params.subnat_params.request
-            ).to_pandas()
-            df_global = self.fetch_data(
-                session, params.global_params.request
-            ).to_pandas()
+            df_subnat = self.fetch_data(session, req_subnat).to_pandas()
+            df_global = self.fetch_data(session, req_global).to_pandas()
 
         df_rca = params.calculate(df_subnat, df_global)
 
         return extension.serialize(df_rca, aliases, filters)
 
     @ll.route("GET", "/eci_subnational.{extension}")
     def route_eci_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexitySubnationalParameters = Depends(
             prepare_complexity_subnational_params
         ),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """ECI calculation endpoint."""
+        roles = self.auth.get_roles(token)
+        req_subnat = params.rca_params.subnat_params.build_request(roles)
+        req_global = params.rca_params.global_params.build_request(roles)
         with self.olap.session() as session:
-            df_subnat = self.fetch_data(
-                session, params.rca_params.subnat_params.request
-            ).to_pandas()
-            df_global = self.fetch_data(
-                session, params.rca_params.global_params.request
-            ).to_pandas()
+            df_subnat = self.fetch_data(session, req_subnat).to_pandas()
+            df_global = self.fetch_data(session, req_global).to_pandas()
 
         df_eci = params.calculate(df_subnat, df_global, "ECI")
 
         return extension.serialize(df_eci, aliases, filters)
 
     @ll.route("GET", "/pci_subnational.{extension}")
     def route_pci_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: ComplexitySubnationalParameters = Depends(
             prepare_complexity_subnational_params
         ),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """PCI calculation endpoint."""
+        roles = self.auth.get_roles(token)
+        req_subnat = params.rca_params.subnat_params.build_request(roles)
+        req_global = params.rca_params.global_params.build_request(roles)
         with self.olap.session() as session:
-            df_subnat = self.fetch_data(
-                session, params.rca_params.subnat_params.request
-            ).to_pandas()
-            df_global = self.fetch_data(
-                session, params.rca_params.global_params.request
-            ).to_pandas()
+            df_subnat = self.fetch_data(session, req_subnat).to_pandas()
+            df_global = self.fetch_data(session, req_global).to_pandas()
 
         df_pci = params.calculate(df_subnat, df_global, "PCI")
 
         return extension.serialize(df_pci, aliases, filters)
 
     @ll.route("GET", "/relatedness_subnational.{extension}")
     def route_relatedness_subnational(
         self,
         extension: ResponseFormat,
         aliases: Dict[str, str] = Depends(parse_alias),
         filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
         params: RelatednessSubnationalParameters = Depends(
             prepare_relatedness_subnational_params
         ),
+        token: Optional[ll.AuthToken] = Depends(auth_token),
     ):
         """Relatedness calculation endpoint."""
+        roles = self.auth.get_roles(token)
+        req_subnat = params.rca_params.subnat_params.build_request(roles)
+        req_global = params.rca_params.global_params.build_request(roles)
         with self.olap.session() as session:
-            df_subnat = self.fetch_data(
-                session, params.rca_params.subnat_params.request
-            ).to_pandas()
-            df_global = self.fetch_data(
-                session, params.rca_params.global_params.request
-            ).to_pandas()
+            df_subnat = self.fetch_data(session, req_subnat).to_pandas()
+            df_global = self.fetch_data(session, req_global).to_pandas()
 
         df_reltd = params.calculate(df_subnat, df_global)
 
         return extension.serialize(df_reltd, aliases, filters)
 
     @ll.route("GET", "/{endpoint}", response_class=RedirectResponse)
     def route_redirect(
@@ -370,14 +402,24 @@
 
         url = request.url
         path, endpoint = url.path.rsplit("/", maxsplit=1)
         return f"{path}/{endpoint}.{extension}?{url.query}"
 
     @ll.exception_handler(TesseractError)
     def exc_tesseracterror(self, request: Request, exc: TesseractError):
+        if isinstance(exc, NotAuthorized):
+            if self.debug:
+                detail = (
+                    f"Requested resource '{exc.resource}' is not allowed for the roles "
+                    f"provided by authorization credentials: '{', '.join(exc.request_roles)}'"
+                )
+                content = {"error": True, "type": "NotAuthorized", "detail": detail}
+            else:
+                content = {"error": True, "detail": exc.message}
+
         if self.debug or isinstance(exc, QueryError):
             content = {"error": True, "type": type(exc).__name__, "detail": exc.message}
         else:
             content = {"error": True, "detail": "Backend error"}
         return JSONResponse(content, status_code=exc.code)
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/opportunity_gain.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/opportunity_gain.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,14 @@
     rank: bool = False
     sort_ascending: Optional[bool] = None
 
     @property
     def column_name(self):
         return f"{self.rca_params.measure} Opportunity Gain"
 
-    @property
-    def request(self):
-        return self.rca_params.request
-
     def _calculate(self, rca: pd.Series) -> pd.Series:
         df_rca = rca.unstack()
         eci, pci = ec.complexity(df_rca, cutoff=self.cutoff, iterations=self.iterations)
         df_opgain = ec.opportunity_gain(df_rca, pci=pci, cutoff=self.cutoff)
         opgain: pd.Series = df_opgain.stack()  # type: ignore
         return opgain.rename(self.column_name)
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/peii.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/pmi/peii.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Set
 
 import economic_complexity as ec
 import pandas as pd
 from fastapi import Depends, Query
 from tesseract_olap import DataRequest, DataRequestParams
 from typing_extensions import Annotated
 
@@ -20,19 +20,19 @@
     rank: bool = False
     sort_ascending: Optional[bool] = None
 
     @property
     def column_name(self):
         return f"{self.rca_params.measure} PEII"
 
-    @property
-    def request(self) -> DataRequest:
+    def build_request(self, roles: Set[str]) -> DataRequest:
         params: DataRequestParams = {
             "drilldowns": [self.emissions_location],
             "measures": [self.emissions_measure],
+            "roles": roles,
         }
 
         locale = self.rca_params.locale
         if locale is not None:
             params["locale"] = locale
 
         return DataRequest.new(self.emissions_cube, params)
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/pmi/pgi.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/pmi/pgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Set
 
 import economic_complexity as ec
 import pandas as pd
 from fastapi import Depends, Query
 from tesseract_olap import DataRequest, DataRequestParams
 from typing_extensions import Annotated
 
@@ -20,19 +20,19 @@
     rank: bool = False
     sort_ascending: Optional[bool] = None
 
     @property
     def column_name(self):
         return f"{self.rca_params.measure} PGI"
 
-    @property
-    def request(self) -> DataRequest:
+    def build_request(self, roles: Set[str]) -> DataRequest:
         params: DataRequestParams = {
             "drilldowns": [self.gini_location],
             "measures": [self.gini_measure],
+            "roles": roles,
         }
 
         locale = self.rca_params.locale
         if locale is not None:
             params["locale"] = locale
 
         return DataRequest.new(self.gini_cube, params)
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/rca/dependencies.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/rca/dependencies.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/rca/structs.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/rca/structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Mapping, Optional, Tuple
+from typing import Mapping, Optional, Set, Tuple
 
 import economic_complexity as ec
 import pandas as pd
 from tesseract_olap import DataRequest, DataRequestParams
 
 from logiclayer_complexity.common import df_melt, df_pivot, series_compare
 
@@ -27,21 +27,21 @@
     def location_id(self):
         return self.location + " ID"
 
     @property
     def column_name(self):
         return f"{self.measure} RCA"
 
-    @property
-    def request(self) -> DataRequest:
+    def build_request(self, roles: Set[str]) -> DataRequest:
         params: DataRequestParams = {
             "drilldowns": (self.location, self.activity),
             "measures": (self.measure,),
             "cuts_include": {**self.cuts},
             "parents": self.parents,
+            "roles": roles,
         }
 
         if self.locale is not None:
             params["locale"] = self.locale
 
         return DataRequest.new(self.cube, params)
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/dependencies.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/relatedness/dependencies.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/relatedness/structs.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/relatedness/structs.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,14 @@
     rank: bool = False
     sort_ascending: Optional[bool] = None
 
     @property
     def column_name(self):
         return f"{self.rca_params.measure} Relatedness"
 
-    @property
-    def request(self):
-        return self.rca_params.request
-
     def _calculate(self, rca: pd.Series) -> pd.Series:
         df_rca = rca.unstack()
         df_relatd = ec.relatedness(df_rca, cutoff=self.cutoff)
         relatd: pd.Series = df_relatd.stack()  # type: ignore
         return relatd.rename(self.column_name)
 
     def calculate(self, df: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/response.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/response.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/logiclayer_complexity/wdi.py` & `logiclayer_complexity-0.5.1/logiclayer_complexity/wdi.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/PACKAGE.md` & `logiclayer_complexity-0.5.1/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.5.0/pyproject.toml` & `logiclayer_complexity-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "logiclayer-complexity"
-version = "0.5.0"
+version = "0.5.1"
 description = "LogicLayer module to enable Economic Complexity calculations, using data from a tesseract-olap server."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
   "Jelmy Hermosilla <jelmy@datawheel.us>",
   "Samuel Osorio <samuel@datawheel.us>",
   "Nicolás Netz <nicolas.netz@datawheel.us>",
 ]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/logiclayer-complexity"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 economic-complexity = "^0.2.1"
-logiclayer = "^0.3.0"
+logiclayer = "^0.3.2"
 orjson = "^3.8.0"
 pandas = ">=1.5.0"
 polars = "^0.20.0"
 pyarrow = "^15.0.0"
-tesseract-olap = ">=0.9.2"
+tesseract-olap = ">=0.9.3"
 
 [tool.poetry.group.dev.dependencies]
 granian = {extras = ["reload"], version = "^1.2.0"}
 ipykernel = "^6.0.0"
 pandas = "^1.5.3"
 pyinstrument = "^4.6.1"
 pytest = "^7.2.0"
 ruff = "^0.3.4"
 snakeviz = "^2.2.0"
-tesseract-olap = {version = "^0.9.2", extras = ["clickhouse"]}
+tesseract-olap = {version = "^0.9.3", extras = ["clickhouse"]}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `logiclayer_complexity-0.5.0/PKG-INFO` & `logiclayer_complexity-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: logiclayer-complexity
-Version: 0.5.0
+Version: 0.5.1
 Summary: LogicLayer module to enable Economic Complexity calculations, using data from a tesseract-olap server.
 Home-page: https://github.com/Datawheel/logiclayer-complexity
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: economic-complexity (>=0.2.1,<0.3.0)
-Requires-Dist: logiclayer (>=0.3.0,<0.4.0)
+Requires-Dist: logiclayer (>=0.3.2,<0.4.0)
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: pandas (>=1.5.0)
 Requires-Dist: polars (>=0.20.0,<0.21.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
-Requires-Dist: tesseract-olap (>=0.9.2)
+Requires-Dist: tesseract-olap (>=0.9.3)
 Project-URL: Repository, https://github.com/Datawheel/logiclayer-complexity
 Description-Content-Type: text/markdown
 
 <p>
 <a href="https://github.com/Datawheel/logiclayer-complexity/releases"><img src="https://flat.badgen.net/github/release/Datawheel/logiclayer-complexity" /></a>
 <a href="https://github.com/Datawheel/logiclayer-complexity/blob/master/LICENSE"><img src="https://flat.badgen.net/github/license/Datawheel/logiclayer-complexity" /></a>
 <a href="https://github.com/Datawheel/logiclayer-complexity/"><img src="https://flat.badgen.net/github/checks/Datawheel/logiclayer-complexity" /></a>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: logiclayer-complexity Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: logiclayer-complexity Version: 0.5.1 Summary:
 LogicLayer module to enable Economic Complexity calculations, using data from a
 tesseract-olap server. Home-page: https://github.com/Datawheel/logiclayer-
 complexity License: MIT Author: Francisco Abarzua Author-email:
 francisco@datawheel.us Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: economic-complexity (>=0.2.1,<0.3.0)
-Requires-Dist: logiclayer (>=0.3.0,<0.4.0) Requires-Dist: orjson
+Requires-Dist: logiclayer (>=0.3.2,<0.4.0) Requires-Dist: orjson
 (>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1.5.0) Requires-Dist: polars
 (>=0.20.0,<0.21.0) Requires-Dist: pyarrow (>=15.0.0,<16.0.0) Requires-Dist:
-tesseract-olap (>=0.9.2) Project-URL: Repository, https://github.com/Datawheel/
+tesseract-olap (>=0.9.3) Project-URL: Repository, https://github.com/Datawheel/
 logiclayer-complexity Description-Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:
 _/_/_f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:_/_/
 _f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_c_h_e_c_k_s_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]_[_h_t_t_p_s_:_/_/
 _f_l_a_t_._b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/_D_a_t_a_w_h_e_e_l_/_l_o_g_i_c_l_a_y_e_r_-_c_o_m_p_l_e_x_i_t_y_]
 ## Getting started This module must be used with LogicLayer. An instance of
 `OlapServer` from the `tesseract_olap` package is also required to retrieve the
```

