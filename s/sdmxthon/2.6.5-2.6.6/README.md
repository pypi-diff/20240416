# Comparing `tmp/sdmxthon-2.6.5.tar.gz` & `tmp/sdmxthon-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmxthon-2.6.5.tar", last modified: Mon Apr 15 14:10:11 2024, max compression
+gzip compressed data, was "sdmxthon-2.6.6.tar", last modified: Tue Apr 16 08:06:46 2024, max compression
```

## Comparing `sdmxthon-2.6.5.tar` & `sdmxthon-2.6.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.745608 sdmxthon-2.6.5/
--rw-rw-rw-   0        0        0      143 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2753 2024-04-15 14:10:11.745608 sdmxthon-2.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     1685 2024-01-16 10:41:25.000000 sdmxthon-2.6.5/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.653986 sdmxthon-2.6.5/sdmxthon/
--rw-rw-rw-   0        0        0      467 2024-02-22 15:21:47.000000 sdmxthon-2.6.5/sdmxthon/__init__.py
--rw-rw-rw-   0        0        0      801 2024-04-15 13:35:59.000000 sdmxthon-2.6.5/sdmxthon/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.659556 sdmxthon-2.6.5/sdmxthon/api/
--rw-rw-rw-   0        0        0     9095 2024-04-12 09:53:28.000000 sdmxthon-2.6.5/sdmxthon/api/api.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.672808 sdmxthon-2.6.5/sdmxthon/model/
--rw-rw-rw-   0        0        0        0 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/model/__init__.py
--rw-rw-rw-   0        0        0    21941 2023-12-05 11:29:36.000000 sdmxthon-2.6.5/sdmxthon/model/base.py
--rw-rw-rw-   0        0        0    17061 2024-01-17 11:00:45.000000 sdmxthon-2.6.5/sdmxthon/model/component.py
--rw-rw-rw-   0        0        0    23526 2024-04-11 19:56:52.000000 sdmxthon-2.6.5/sdmxthon/model/dataset.py
--rw-rw-rw-   0        0        0    35951 2024-01-17 11:00:45.000000 sdmxthon-2.6.5/sdmxthon/model/definitions.py
--rw-rw-rw-   0        0        0     6074 2024-02-22 15:21:47.000000 sdmxthon-2.6.5/sdmxthon/model/descriptors.py
--rw-rw-rw-   0        0        0      871 2023-11-10 12:25:07.000000 sdmxthon-2.6.5/sdmxthon/model/error.py
--rw-rw-rw-   0        0        0     2118 2021-11-10 17:15:12.000000 sdmxthon-2.6.5/sdmxthon/model/extras.py
--rw-rw-rw-   0        0        0    15563 2023-12-29 12:06:57.000000 sdmxthon-2.6.5/sdmxthon/model/header.py
--rw-rw-rw-   0        0        0    22774 2023-12-29 12:06:57.000000 sdmxthon-2.6.5/sdmxthon/model/itemScheme.py
--rw-rw-rw-   0        0        0     7691 2024-04-12 09:53:28.000000 sdmxthon-2.6.5/sdmxthon/model/message.py
--rw-rw-rw-   0        0        0     4230 2021-12-01 12:46:51.000000 sdmxthon-2.6.5/sdmxthon/model/representation.py
--rw-rw-rw-   0        0        0      773 2023-11-10 12:25:07.000000 sdmxthon-2.6.5/sdmxthon/model/submission.py
--rw-rw-rw-   0        0        0     7155 2023-12-29 12:06:57.000000 sdmxthon-2.6.5/sdmxthon/model/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.680338 sdmxthon-2.6.5/sdmxthon/parsers/
--rw-rw-rw-   0        0        0       36 2021-03-22 11:19:58.000000 sdmxthon-2.6.5/sdmxthon/parsers/__init__.py
--rw-rw-rw-   0        0        0     6586 2024-02-23 16:27:37.000000 sdmxthon-2.6.5/sdmxthon/parsers/data_read.py
--rw-rw-rw-   0        0        0    25740 2023-12-01 14:23:07.000000 sdmxthon-2.6.5/sdmxthon/parsers/data_validations.py
--rw-rw-rw-   0        0        0    27381 2024-04-15 14:09:30.000000 sdmxthon-2.6.5/sdmxthon/parsers/metadata_read.py
--rw-rw-rw-   0        0        0    12189 2024-04-12 09:53:28.000000 sdmxthon-2.6.5/sdmxthon/parsers/read.py
--rw-rw-rw-   0        0        0     5170 2024-01-17 11:00:45.000000 sdmxthon-2.6.5/sdmxthon/parsers/reader_input_processor.py
--rw-rw-rw-   0        0        0    20871 2024-02-23 16:10:14.000000 sdmxthon-2.6.5/sdmxthon/parsers/write.py
--rw-rw-rw-   0        0        0     9682 2024-02-09 12:34:50.000000 sdmxthon-2.6.5/sdmxthon/parsers/writer_aux.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.735365 sdmxthon-2.6.5/sdmxthon/schemas/
--rw-rw-rw-   0        0        0   113624 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXCommon.xsd
--rw-rw-rw-   0        0        0   278665 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXCommonReferences.xsd
--rw-rw-rw-   0        0        0      805 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataGeneric.xsd
--rw-rw-rw-   0        0        0    24835 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataGenericBase.xsd
--rw-rw-rw-   0        0        0     9579 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd
--rw-rw-rw-   0        0        0     1156 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataStructureSpecific.xsd
--rw-rw-rw-   0        0        0    41262 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd
--rw-rw-rw-   0        0        0     8408 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd
--rw-rw-rw-   0        0        0    81157 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXMessage.xsd
--rw-rw-rw-   0        0        0     3624 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXMessageFooter.xsd
--rw-rw-rw-   0        0        0    16072 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXMetadataGeneric.xsd
--rw-rw-rw-   0        0        0    30613 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd
--rw-rw-rw-   0        0        0     2172 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQuery.xsd
--rw-rw-rw-   0        0        0    46248 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryBase.xsd
--rw-rw-rw-   0        0        0     6558 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryCategorisation.xsd
--rw-rw-rw-   0        0        0     5726 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryCategory.xsd
--rw-rw-rw-   0        0        0     5284 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryCodelist.xsd
--rw-rw-rw-   0        0        0     6473 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryConcept.xsd
--rw-rw-rw-   0        0        0    11540 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryConstraint.xsd
--rw-rw-rw-   0        0        0    34427 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryData.xsd
--rw-rw-rw-   0        0        0    19416 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryDataStructure.xsd
--rw-rw-rw-   0        0        0     4184 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryDataflow.xsd
--rw-rw-rw-   0        0        0     5308 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd
--rw-rw-rw-   0        0        0    25651 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryMetadata.xsd
--rw-rw-rw-   0        0        0    14717 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd
--rw-rw-rw-   0        0        0     4352 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryMetadataflow.xsd
--rw-rw-rw-   0        0        0     7463 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryOrganisation.xsd
--rw-rw-rw-   0        0        0     9459 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryProcess.xsd
--rw-rw-rw-   0        0        0     5669 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd
--rw-rw-rw-   0        0        0     7677 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd
--rw-rw-rw-   0        0        0     5305 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQuerySchema.xsd
--rw-rw-rw-   0        0        0    10154 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryStructureSet.xsd
--rw-rw-rw-   0        0        0     3709 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryStructures.xsd
--rw-rw-rw-   0        0        0     1009 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistry.xsd
--rw-rw-rw-   0        0        0    14238 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistryBase.xsd
--rw-rw-rw-   0        0        0    19745 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistryRegistration.xsd
--rw-rw-rw-   0        0        0    10271 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistryStructure.xsd
--rw-rw-rw-   0        0        0    63155 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistrySubscription.xsd
--rw-rw-rw-   0        0        0    41096 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructure.xsd
--rw-rw-rw-   0        0        0    39172 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureBase.xsd
--rw-rw-rw-   0        0        0     2069 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureCategorisation.xsd
--rw-rw-rw-   0        0        0     4767 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureCategory.xsd
--rw-rw-rw-   0        0        0     4930 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureCodelist.xsd
--rw-rw-rw-   0        0        0     7866 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureConcept.xsd
--rw-rw-rw-   0        0        0    28760 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureConstraint.xsd
--rw-rw-rw-   0        0        0    52702 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureDataStructure.xsd
--rw-rw-rw-   0        0        0     2167 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureDataflow.xsd
--rw-rw-rw-   0        0        0    23519 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd
--rw-rw-rw-   0        0        0    37058 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd
--rw-rw-rw-   0        0        0     2265 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureMetadataflow.xsd
--rw-rw-rw-   0        0        0    19113 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureOrganisation.xsd
--rw-rw-rw-   0        0        0    14460 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureProcess.xsd
--rw-rw-rw-   0        0        0     2597 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd
--rw-rw-rw-   0        0        0     6218 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd
--rw-rw-rw-   0        0        0    34361 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureStructureSet.xsd
--rw-rw-rw-   0        0        0     3363 2021-05-28 09:14:58.000000 sdmxthon-2.6.5/sdmxthon/schemas/xml.xsd
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.741158 sdmxthon-2.6.5/sdmxthon/utils/
--rw-rw-rw-   0        0        0        0 2021-03-22 11:19:40.000000 sdmxthon-2.6.5/sdmxthon/utils/__init__.py
--rw-rw-rw-   0        0        0      522 2023-12-29 12:06:57.000000 sdmxthon-2.6.5/sdmxthon/utils/enums.py
--rw-rw-rw-   0        0        0     1025 2023-12-29 12:06:57.000000 sdmxthon-2.6.5/sdmxthon/utils/handlers.py
--rw-rw-rw-   0        0        0     6303 2024-04-11 19:56:52.000000 sdmxthon-2.6.5/sdmxthon/utils/mappings.py
--rw-rw-rw-   0        0        0     4460 2024-04-15 11:05:46.000000 sdmxthon-2.6.5/sdmxthon/utils/parsing_words.py
--rw-rw-rw-   0        0        0      125 2023-03-14 10:20:20.000000 sdmxthon-2.6.5/sdmxthon/utils/xml_allowed_errors.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.745608 sdmxthon-2.6.5/sdmxthon/webservices/
--rw-rw-rw-   0        0        0        0 2023-09-13 11:19:02.000000 sdmxthon-2.6.5/sdmxthon/webservices/__init__.py
--rw-rw-rw-   0        0        0    11091 2024-04-11 19:56:52.000000 sdmxthon-2.6.5/sdmxthon/webservices/fmr.py
--rw-rw-rw-   0        0        0   575935 2024-04-12 09:53:28.000000 sdmxthon-2.6.5/sdmxthon/webservices/query_builder.py
--rw-rw-rw-   0        0        0    12147 2024-04-12 09:53:28.000000 sdmxthon-2.6.5/sdmxthon/webservices/webservices.py
-drwxrwxrwx   0        0        0        0 2024-04-15 14:10:11.659053 sdmxthon-2.6.5/sdmxthon.egg-info/
--rw-rw-rw-   0        0        0     2753 2024-04-15 14:10:11.000000 sdmxthon-2.6.5/sdmxthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3606 2024-04-15 14:10:11.000000 sdmxthon-2.6.5/sdmxthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 14:10:11.000000 sdmxthon-2.6.5/sdmxthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-15 14:10:11.000000 sdmxthon-2.6.5/sdmxthon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 14:10:11.000000 sdmxthon-2.6.5/sdmxthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 14:10:11.746884 sdmxthon-2.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1598 2023-10-24 10:13:00.000000 sdmxthon-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.916329 sdmxthon-2.6.6/
+-rw-rw-rw-   0        0        0      143 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2753 2024-04-16 08:06:46.917328 sdmxthon-2.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1685 2024-01-16 10:41:25.000000 sdmxthon-2.6.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.816489 sdmxthon-2.6.6/sdmxthon/
+-rw-rw-rw-   0        0        0      467 2024-02-22 15:21:47.000000 sdmxthon-2.6.6/sdmxthon/__init__.py
+-rw-rw-rw-   0        0        0      801 2024-04-16 08:05:51.000000 sdmxthon-2.6.6/sdmxthon/__version__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.823632 sdmxthon-2.6.6/sdmxthon/api/
+-rw-rw-rw-   0        0        0     9095 2024-04-12 09:53:28.000000 sdmxthon-2.6.6/sdmxthon/api/api.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.838560 sdmxthon-2.6.6/sdmxthon/model/
+-rw-rw-rw-   0        0        0        0 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/model/__init__.py
+-rw-rw-rw-   0        0        0    21941 2023-12-05 11:29:36.000000 sdmxthon-2.6.6/sdmxthon/model/base.py
+-rw-rw-rw-   0        0        0    17061 2024-01-17 11:00:45.000000 sdmxthon-2.6.6/sdmxthon/model/component.py
+-rw-rw-rw-   0        0        0    23526 2024-04-11 19:56:52.000000 sdmxthon-2.6.6/sdmxthon/model/dataset.py
+-rw-rw-rw-   0        0        0    35951 2024-01-17 11:00:45.000000 sdmxthon-2.6.6/sdmxthon/model/definitions.py
+-rw-rw-rw-   0        0        0     6074 2024-02-22 15:21:47.000000 sdmxthon-2.6.6/sdmxthon/model/descriptors.py
+-rw-rw-rw-   0        0        0      871 2023-11-10 12:25:07.000000 sdmxthon-2.6.6/sdmxthon/model/error.py
+-rw-rw-rw-   0        0        0     2118 2021-11-10 17:15:12.000000 sdmxthon-2.6.6/sdmxthon/model/extras.py
+-rw-rw-rw-   0        0        0    15563 2023-12-29 12:06:57.000000 sdmxthon-2.6.6/sdmxthon/model/header.py
+-rw-rw-rw-   0        0        0    22774 2023-12-29 12:06:57.000000 sdmxthon-2.6.6/sdmxthon/model/itemScheme.py
+-rw-rw-rw-   0        0        0     7691 2024-04-12 09:53:28.000000 sdmxthon-2.6.6/sdmxthon/model/message.py
+-rw-rw-rw-   0        0        0     4230 2021-12-01 12:46:51.000000 sdmxthon-2.6.6/sdmxthon/model/representation.py
+-rw-rw-rw-   0        0        0      773 2023-11-10 12:25:07.000000 sdmxthon-2.6.6/sdmxthon/model/submission.py
+-rw-rw-rw-   0        0        0     7155 2023-12-29 12:06:57.000000 sdmxthon-2.6.6/sdmxthon/model/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.846703 sdmxthon-2.6.6/sdmxthon/parsers/
+-rw-rw-rw-   0        0        0       36 2021-03-22 11:19:58.000000 sdmxthon-2.6.6/sdmxthon/parsers/__init__.py
+-rw-rw-rw-   0        0        0     6586 2024-02-23 16:27:37.000000 sdmxthon-2.6.6/sdmxthon/parsers/data_read.py
+-rw-rw-rw-   0        0        0    25740 2023-12-01 14:23:07.000000 sdmxthon-2.6.6/sdmxthon/parsers/data_validations.py
+-rw-rw-rw-   0        0        0    27381 2024-04-15 14:09:30.000000 sdmxthon-2.6.6/sdmxthon/parsers/metadata_read.py
+-rw-rw-rw-   0        0        0    12189 2024-04-12 09:53:28.000000 sdmxthon-2.6.6/sdmxthon/parsers/read.py
+-rw-rw-rw-   0        0        0     5170 2024-01-17 11:00:45.000000 sdmxthon-2.6.6/sdmxthon/parsers/reader_input_processor.py
+-rw-rw-rw-   0        0        0    20871 2024-02-23 16:10:14.000000 sdmxthon-2.6.6/sdmxthon/parsers/write.py
+-rw-rw-rw-   0        0        0     9682 2024-02-09 12:34:50.000000 sdmxthon-2.6.6/sdmxthon/parsers/writer_aux.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.904227 sdmxthon-2.6.6/sdmxthon/schemas/
+-rw-rw-rw-   0        0        0   113624 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXCommon.xsd
+-rw-rw-rw-   0        0        0   278665 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXCommonReferences.xsd
+-rw-rw-rw-   0        0        0      805 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataGeneric.xsd
+-rw-rw-rw-   0        0        0    24835 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataGenericBase.xsd
+-rw-rw-rw-   0        0        0     9579 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd
+-rw-rw-rw-   0        0        0     1156 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataStructureSpecific.xsd
+-rw-rw-rw-   0        0        0    41262 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd
+-rw-rw-rw-   0        0        0     8408 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd
+-rw-rw-rw-   0        0        0    81157 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXMessage.xsd
+-rw-rw-rw-   0        0        0     3624 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXMessageFooter.xsd
+-rw-rw-rw-   0        0        0    16072 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXMetadataGeneric.xsd
+-rw-rw-rw-   0        0        0    30613 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd
+-rw-rw-rw-   0        0        0     2172 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQuery.xsd
+-rw-rw-rw-   0        0        0    46248 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryBase.xsd
+-rw-rw-rw-   0        0        0     6558 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryCategorisation.xsd
+-rw-rw-rw-   0        0        0     5726 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryCategory.xsd
+-rw-rw-rw-   0        0        0     5284 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryCodelist.xsd
+-rw-rw-rw-   0        0        0     6473 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryConcept.xsd
+-rw-rw-rw-   0        0        0    11540 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryConstraint.xsd
+-rw-rw-rw-   0        0        0    34427 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryData.xsd
+-rw-rw-rw-   0        0        0    19416 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryDataStructure.xsd
+-rw-rw-rw-   0        0        0     4184 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryDataflow.xsd
+-rw-rw-rw-   0        0        0     5308 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd
+-rw-rw-rw-   0        0        0    25651 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryMetadata.xsd
+-rw-rw-rw-   0        0        0    14717 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd
+-rw-rw-rw-   0        0        0     4352 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryMetadataflow.xsd
+-rw-rw-rw-   0        0        0     7463 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryOrganisation.xsd
+-rw-rw-rw-   0        0        0     9459 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryProcess.xsd
+-rw-rw-rw-   0        0        0     5669 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd
+-rw-rw-rw-   0        0        0     7677 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd
+-rw-rw-rw-   0        0        0     5305 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQuerySchema.xsd
+-rw-rw-rw-   0        0        0    10154 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryStructureSet.xsd
+-rw-rw-rw-   0        0        0     3709 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryStructures.xsd
+-rw-rw-rw-   0        0        0     1009 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistry.xsd
+-rw-rw-rw-   0        0        0    14238 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistryBase.xsd
+-rw-rw-rw-   0        0        0    19745 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistryRegistration.xsd
+-rw-rw-rw-   0        0        0    10271 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistryStructure.xsd
+-rw-rw-rw-   0        0        0    63155 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistrySubscription.xsd
+-rw-rw-rw-   0        0        0    41096 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructure.xsd
+-rw-rw-rw-   0        0        0    39172 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureBase.xsd
+-rw-rw-rw-   0        0        0     2069 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureCategorisation.xsd
+-rw-rw-rw-   0        0        0     4767 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureCategory.xsd
+-rw-rw-rw-   0        0        0     4930 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureCodelist.xsd
+-rw-rw-rw-   0        0        0     7866 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureConcept.xsd
+-rw-rw-rw-   0        0        0    28760 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureConstraint.xsd
+-rw-rw-rw-   0        0        0    52702 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureDataStructure.xsd
+-rw-rw-rw-   0        0        0     2167 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureDataflow.xsd
+-rw-rw-rw-   0        0        0    23519 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd
+-rw-rw-rw-   0        0        0    37058 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd
+-rw-rw-rw-   0        0        0     2265 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureMetadataflow.xsd
+-rw-rw-rw-   0        0        0    19113 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureOrganisation.xsd
+-rw-rw-rw-   0        0        0    14460 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureProcess.xsd
+-rw-rw-rw-   0        0        0     2597 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd
+-rw-rw-rw-   0        0        0     6218 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd
+-rw-rw-rw-   0        0        0    34361 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureStructureSet.xsd
+-rw-rw-rw-   0        0        0     3363 2021-05-28 09:14:58.000000 sdmxthon-2.6.6/sdmxthon/schemas/xml.xsd
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.910226 sdmxthon-2.6.6/sdmxthon/utils/
+-rw-rw-rw-   0        0        0        0 2021-03-22 11:19:40.000000 sdmxthon-2.6.6/sdmxthon/utils/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-12-29 12:06:57.000000 sdmxthon-2.6.6/sdmxthon/utils/enums.py
+-rw-rw-rw-   0        0        0     1025 2023-12-29 12:06:57.000000 sdmxthon-2.6.6/sdmxthon/utils/handlers.py
+-rw-rw-rw-   0        0        0     6313 2024-04-16 08:02:20.000000 sdmxthon-2.6.6/sdmxthon/utils/mappings.py
+-rw-rw-rw-   0        0        0     4460 2024-04-15 11:05:46.000000 sdmxthon-2.6.6/sdmxthon/utils/parsing_words.py
+-rw-rw-rw-   0        0        0      125 2023-03-14 10:20:20.000000 sdmxthon-2.6.6/sdmxthon/utils/xml_allowed_errors.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.915321 sdmxthon-2.6.6/sdmxthon/webservices/
+-rw-rw-rw-   0        0        0        0 2023-09-13 11:19:02.000000 sdmxthon-2.6.6/sdmxthon/webservices/__init__.py
+-rw-rw-rw-   0        0        0    11091 2024-04-11 19:56:52.000000 sdmxthon-2.6.6/sdmxthon/webservices/fmr.py
+-rw-rw-rw-   0        0        0   575935 2024-04-12 09:53:28.000000 sdmxthon-2.6.6/sdmxthon/webservices/query_builder.py
+-rw-rw-rw-   0        0        0    12147 2024-04-12 09:53:28.000000 sdmxthon-2.6.6/sdmxthon/webservices/webservices.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:06:46.822624 sdmxthon-2.6.6/sdmxthon.egg-info/
+-rw-rw-rw-   0        0        0     2753 2024-04-16 08:06:46.000000 sdmxthon-2.6.6/sdmxthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3606 2024-04-16 08:06:46.000000 sdmxthon-2.6.6/sdmxthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:06:46.000000 sdmxthon-2.6.6/sdmxthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-16 08:06:46.000000 sdmxthon-2.6.6/sdmxthon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 08:06:46.000000 sdmxthon-2.6.6/sdmxthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:06:46.917328 sdmxthon-2.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1598 2023-10-24 10:13:00.000000 sdmxthon-2.6.6/setup.py
```

### Comparing `sdmxthon-2.6.5/PKG-INFO` & `sdmxthon-2.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmxthon
-Version: 2.6.5
+Version: 2.6.6
 Summary: Library with SDMX to Pandas, Pandas to SDMX, SDMX validation and SDMX metadata validation
 Author: Francisco Javier Hernandez del Cano
 Author-email: javier.hernandez@meaningfuldata.eu
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Meaningful-Data/sdmxthon/issues
 Project-URL: Documentation, https://docs.sdmxthon.meaningfuldata.eu
 Project-URL: Source Code, https://github.com/Meaningful-Data/sdmxthon
```

### Comparing `sdmxthon-2.6.5/README.rst` & `sdmxthon-2.6.6/README.rst`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/__version__.py` & `sdmxthon-2.6.6/sdmxthon/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #   |___/   |___/ |_|__|_| /_/\_\   _\__|  |_||_|   \___/  |_||_|
 # _|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|
 # "`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'
 project = 'sdmxthon'
 description = ('Library with SDMX to Pandas, Pandas to SDMX, '
                'SDMX validation and SDMX metadata validation')
 url = 'https://github.com/Meaningful-Data/sdmxthon'
-version = '2.6.5'
+version = '2.6.6'
 author = 'Francisco Javier Hernandez del Cano'
 author_email = 'javier.hernandez@meaningfuldata.eu'
 copyright = '2024 MeaningfulData. All Rights Reserved'
```

### Comparing `sdmxthon-2.6.5/sdmxthon/api/api.py` & `sdmxthon-2.6.6/sdmxthon/api/api.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/base.py` & `sdmxthon-2.6.6/sdmxthon/model/base.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/component.py` & `sdmxthon-2.6.6/sdmxthon/model/component.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/dataset.py` & `sdmxthon-2.6.6/sdmxthon/model/dataset.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/definitions.py` & `sdmxthon-2.6.6/sdmxthon/model/definitions.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/descriptors.py` & `sdmxthon-2.6.6/sdmxthon/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/error.py` & `sdmxthon-2.6.6/sdmxthon/model/error.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/extras.py` & `sdmxthon-2.6.6/sdmxthon/model/extras.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/header.py` & `sdmxthon-2.6.6/sdmxthon/model/header.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/itemScheme.py` & `sdmxthon-2.6.6/sdmxthon/model/itemScheme.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/message.py` & `sdmxthon-2.6.6/sdmxthon/model/message.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/representation.py` & `sdmxthon-2.6.6/sdmxthon/model/representation.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/submission.py` & `sdmxthon-2.6.6/sdmxthon/model/submission.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/model/utils.py` & `sdmxthon-2.6.6/sdmxthon/model/utils.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/data_read.py` & `sdmxthon-2.6.6/sdmxthon/parsers/data_read.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/data_validations.py` & `sdmxthon-2.6.6/sdmxthon/parsers/data_validations.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/metadata_read.py` & `sdmxthon-2.6.6/sdmxthon/parsers/metadata_read.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/read.py` & `sdmxthon-2.6.6/sdmxthon/parsers/read.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/reader_input_processor.py` & `sdmxthon-2.6.6/sdmxthon/parsers/reader_input_processor.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/write.py` & `sdmxthon-2.6.6/sdmxthon/parsers/write.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/parsers/writer_aux.py` & `sdmxthon-2.6.6/sdmxthon/parsers/writer_aux.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXCommon.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXCommon.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXCommonReferences.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXCommonReferences.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataGeneric.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataGenericBase.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataGenericBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataGenericTimeSeries.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataStructureSpecific.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataStructureSpecificBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXDataStructureSpecificTimeSeries.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXMessage.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXMessage.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXMessageFooter.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXMessageFooter.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXMetadataGeneric.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXMetadataGeneric.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXMetadataStructureSpecific.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQuery.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQuery.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryBase.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryCategorisation.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryCategory.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryCodelist.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryConcept.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryConstraint.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryData.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryData.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryDataStructure.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryDataflow.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryMetadata.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryMetadata.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryMetadataflow.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryOrganisation.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryProcess.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQuerySchema.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQuerySchema.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryStructureSet.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryStructureSet.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXQueryStructures.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXQueryStructures.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistry.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistry.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistryBase.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistryBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistryRegistration.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistryRegistration.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistryStructure.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistryStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXRegistrySubscription.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXRegistrySubscription.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructure.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureBase.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureBase.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureCategorisation.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureCategorisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureCategory.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureCategory.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureCodelist.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureConcept.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureConcept.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureConstraint.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureConstraint.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureDataStructure.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureDataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureDataflow.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureDataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureHierarchicalCodelist.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureMetadataStructure.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureMetadataflow.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureMetadataflow.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureOrganisation.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureOrganisation.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureProcess.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureProcess.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureProvisionAgreement.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureReportingTaxonomy.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/SDMXStructureStructureSet.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/SDMXStructureStructureSet.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/schemas/xml.xsd` & `sdmxthon-2.6.6/sdmxthon/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/utils/enums.py` & `sdmxthon-2.6.6/sdmxthon/utils/enums.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/utils/handlers.py` & `sdmxthon-2.6.6/sdmxthon/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/utils/mappings.py` & `sdmxthon-2.6.6/sdmxthon/utils/mappings.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,30 +29,30 @@
     "Double": "Number",
     "Boolean": "Boolean",
     "URI": "String",
     "Count": "Integer",
     "InclusiveValueRange": "Number",
     "ExclusiveValueRange": "Number",
     "Incremental": "Number",
-    "ObservationalTimePeriod": "TimePeriod",
-    "StandardTimePeriod": "TimePeriod",
+    "ObservationalTimePeriod": "Time_Period",
+    "StandardTimePeriod": "Time_Period",
     "BasicTimePeriod": "Date",
     "GregorianTimePeriod": "Date",
     "GregorianYear": "Date",
     "GregorianYearMonth": "Date",
     "GregorianMonth": "Date",
     "GregorianDay": "Date",
-    "ReportingTimePeriod": "TimePeriod",
-    "ReportingYear": "TimePeriod",
-    "ReportingSemester": "TimePeriod",
-    "ReportingTrimester": "TimePeriod",
-    "ReportingQuarter": "TimePeriod",
-    "ReportingMonth": "TimePeriod",
-    "ReportingWeek": "TimePeriod",
-    "ReportingDay": "TimePeriod",
+    "ReportingTimePeriod": "Time_Period",
+    "ReportingYear": "Time_Period",
+    "ReportingSemester": "Time_Period",
+    "ReportingTrimester": "Time_Period",
+    "ReportingQuarter": "Time_Period",
+    "ReportingMonth": "Time_Period",
+    "ReportingWeek": "Time_Period",
+    "ReportingDay": "Time_Period",
     "DateTime": "Date",
     "TimeRange": "Time",
     "Month": "String",
     "MonthDay": "String",
     "Day": "String",
     "Time": "String",
     "Duration": "Duration"
```

### Comparing `sdmxthon-2.6.5/sdmxthon/utils/parsing_words.py` & `sdmxthon-2.6.6/sdmxthon/utils/parsing_words.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/webservices/fmr.py` & `sdmxthon-2.6.6/sdmxthon/webservices/fmr.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/webservices/query_builder.py` & `sdmxthon-2.6.6/sdmxthon/webservices/query_builder.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon/webservices/webservices.py` & `sdmxthon-2.6.6/sdmxthon/webservices/webservices.py`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/sdmxthon.egg-info/PKG-INFO` & `sdmxthon-2.6.6/sdmxthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdmxthon
-Version: 2.6.5
+Version: 2.6.6
 Summary: Library with SDMX to Pandas, Pandas to SDMX, SDMX validation and SDMX metadata validation
 Author: Francisco Javier Hernandez del Cano
 Author-email: javier.hernandez@meaningfuldata.eu
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Meaningful-Data/sdmxthon/issues
 Project-URL: Documentation, https://docs.sdmxthon.meaningfuldata.eu
 Project-URL: Source Code, https://github.com/Meaningful-Data/sdmxthon
```

### Comparing `sdmxthon-2.6.5/sdmxthon.egg-info/SOURCES.txt` & `sdmxthon-2.6.6/sdmxthon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdmxthon-2.6.5/setup.py` & `sdmxthon-2.6.6/setup.py`

 * *Files identical despite different names*

