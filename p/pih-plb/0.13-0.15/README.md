# Comparing `tmp/pih-plb-0.13.tar.gz` & `tmp/pih-plb-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.13.tar", last modified: Mon Apr 15 00:50:49 2024, max compression
+gzip compressed data, was "pih-plb-0.15.tar", last modified: Tue Apr 16 02:00:00 2024, max compression
```

## Comparing `pih-plb-0.13.tar` & `pih-plb-0.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 00:50:49.804860 pih-plb-0.13/
--rw-rw-rw-   0        0        0      293 2024-04-15 00:50:49.773592 pih-plb-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 00:50:48.986924 pih-plb-0.13/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.13/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.13/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45675 2024-02-27 00:56:04.000000 pih-plb-0.13/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3553 2024-04-15 00:49:47.000000 pih-plb-0.13/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14584 2024-02-27 00:46:55.000000 pih-plb-0.13/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 00:50:49.379652 pih-plb-0.13/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-04-15 00:50:47.000000 pih-plb-0.13/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-15 00:50:48.000000 pih-plb-0.13/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 00:50:48.000000 pih-plb-0.13/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-15 00:50:48.000000 pih-plb-0.13/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 00:50:48.000000 pih-plb-0.13/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 00:50:48.000000 pih-plb-0.13/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 00:50:49.820466 pih-plb-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 02:00:00.522837 pih-plb-0.15/
+-rw-rw-rw-   0        0        0      293 2024-04-16 02:00:00.491587 pih-plb-0.15/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 01:59:59.722820 pih-plb-0.15/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.15/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.15/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    44594 2024-04-15 05:12:25.000000 pih-plb-0.15/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3553 2024-04-16 01:59:05.000000 pih-plb-0.15/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14584 2024-02-27 00:46:55.000000 pih-plb-0.15/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:00:00.444714 pih-plb-0.15/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 01:59:59.000000 pih-plb-0.15/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 02:00:00.585365 pih-plb-0.15/setup.cfg
```

### Comparing `pih-plb-0.13/PolibaseService/api.py` & `pih-plb-0.15/PolibaseService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     ne,
     nl,
     one,
     esc,
     escs,
     BitMask as BM,
     while_not_do,
-    
 )
 
 from typing import Any, Callable
 import re
 
 
 def get_host(test: bool) -> str:
@@ -952,50 +951,55 @@
             )  # type: ignore
         return one(result, {})  # type: ignore
 
     @staticmethod
     def get_person_pin_list_by_visit_date(
         date: str, only_operation_department: bool = False, test: bool | None = None
     ) -> list[int]:
-        complete_list_part: str = """OJBS_COMPLETE_LIST as (
-                                                            select
-                                                            DIV_NAME,
-                                                            DIV_NOTES DEPARTMENT,
-                                                            JOB_NO,
-                                                            JOB_NAME,
-                                                            ORD_PAT_NO,
-                                                            PATIENT.PER_FULL_NAME,
-                                                            PATIENT.PER_NO,
-                                                            OJB_DOC_NO as DOC_NO,
-                                                            DOCTOR.PER_FULL_NAME as DOCTOR,
-                                                            OJB_MED_NO as MED_NO,
-                                                            DOCTOR.PER_PLI_NO as DOC_PLI_NO,
-                                                            OJB_NO,
-                                                            OJB_ORD_NO ORDER_NO,
-                                                            ORD_STRT CREATE_AT,
-                                                            ORD_PAID PAID_AT,
-                                                            ORD_TOTAL_PRICE TOTAL_PRICE,
-                                                            OJB_JOB_PRC,
-                                                            OJB_JOB_QNT,
-                                                            OJB_JOB_KO,
-                                                            OJB_DOC_PRC DOC_RATE,
-                                                            OJB_MED_PRC MED_RATE,
-                                                            JSL_COST_DOC,
-                                                            JSL_NO,
-                                                            JSL_TRF_NO
-                                                            from DIVS_ALL
-                                                            left outer join JOBLISTS on JLI_DIV_NO=DIV_NO
-                                                            left outer join JOBLIS on JIL_JLI_NO=JLI_NO
-                                                            left outer join JOBS on JIL_JOB_NO=JOB_NO
-                                                            left outer join OJBS on OJB_JOB_NO=JOB_NO
-                                                            left outer join PERSONS DOCTOR on OJB_DOC_NO=DOCTOR.PER_NO
-                                                            left outer join PERSONS PATIENT on OJB_PAT_NO=PATIENT.PER_NO
-                                                            left outer join JOBSALS ON JSL_JOB_NO=OJB_JOB_NO and DOCTOR.PER_PLI_NO=JSL_PLI_NO
-                                                        )"""
+        complete_list_part: str = """
+                            OJBS_COMPLETE_LIST as (
+                            select
+                            DIV_NAME,
+                            DIV_NOTES DEPARTMENT,
+                            JOB_NO,
+                            JOB_NAME,
+                            ORD_PAT_NO,
+                            PATIENT.PER_FULL_NAME,
+                            PATIENT.PER_NO,
+                            OJB_DOC_NO as DOC_NO,
+                            DOCTOR.PER_FULL_NAME as DOCTOR,
+                            OJB_MED_NO as MED_NO,
+                            DOCTOR.PER_PLI_NO as DOC_PLI_NO,
+                            OJB_NO,
+                            OJB_ORD_NO ORDER_NO,
+                            ORD_STRT CREATE_AT,
+                            ORD_PAID PAID_AT,
+                            ORD_TOTAL_PRICE TOTAL_PRICE,
+                            OJB_JOB_PRC,
+                            OJB_JOB_QNT,
+                            OJB_JOB_KO,
+                            OJB_DOC_PRC DOC_RATE,
+                            OJB_MED_PRC MED_RATE,
+                            JSL_COST_DOC,
+                            JSL_NO,
+                            JSL_TRF_NO
+                            from DIVS_ALL
+                            left outer join JOBLISTS on JLI_DIV_NO=DIV_NO
+                            left outer join JOBLIS on JIL_JLI_NO=JLI_NO
+                            left outer join JOBS on JIL_JOB_NO=JOB_NO
+                            left outer join OJBS on OJB_JOB_NO=JOB_NO
+                            left outer join PERSONS DOCTOR on OJB_DOC_NO=DOCTOR.PER_NO
+                            left outer join PERSONS PATIENT on OJB_PAT_NO=PATIENT.PER_NO
+                            left outer join JOBSALS ON JSL_JOB_NO=OJB_JOB_NO and DOCTOR.PER_PLI_NO=JSL_PLI_NO
+                        )
+                        """
 
+        pin_list: list[int] = A.S.get(
+            A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST
+        )
         query: str = js(
             (
                 (
                     j(
                         (
                             """with DIVS_ALL as (
                             select DIV_NO, DIV_NAME, DIV_NOTES from DIVISIONS where DIV_NOTES is not NULL
@@ -1073,23 +1077,19 @@
                             complete_list_part,
                             "select distinct PER_NO from OJBS_COMPLETE_LIST where (DEPARTMENT not like '%---%---%' or DEPARTMENT is NULL)",
                         )
                     )
                 ),
                 (
                     None
-                    if only_operation_department
+                    if only_operation_department or e(pin_list)
                     else j(
                         (
                             "and DOC_NO IN(",
-                            A.D.list_to_string(
-                                A.S.get(
-                                    A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_DOCTOR_PERSON_PIN_LIST
-                                )
-                            ),
+                            A.D.list_to_string(A.D.map(str, pin_list)),
                             ")",
                         )
                     )
                 ),
                 " and CREATE_AT like TO_DATE(",
                 escs(date),
                 ", 'DD.MM.YY')",
```

### Comparing `pih-plb-0.13/PolibaseService/const.py` & `pih-plb-0.15/PolibaseService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.13"
+VERSION: str = "0.15"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
```

### Comparing `pih-plb-0.13/PolibaseService/service.py` & `pih-plb-0.15/PolibaseService/service.py`

 * *Files identical despite different names*

