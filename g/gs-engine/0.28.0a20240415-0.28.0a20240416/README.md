# Comparing `tmp/gs_engine-0.28.0a20240415-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.28.0a20240416-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12626 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 24-Apr-15 19:01 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      593 b- defN 24-Apr-15 19:01 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 24-Apr-15 19:01 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-15 19:01 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-15 19:01 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    23179 b- defN 24-Apr-15 20:00 gs_engine-0.28.0a20240415.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-15 20:00 gs_engine-0.28.0a20240415.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Apr-15 20:00 gs_engine-0.28.0a20240415.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 24-Apr-15 20:00 gs_engine-0.28.0a20240415.dist-info/RECORD
-9 files, 27601 bytes uncompressed, 11164 bytes compressed:  59.6%
+Zip file size: 12699 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 24-Apr-16 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      593 b- defN 24-Apr-16 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 24-Apr-16 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-16 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-16 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    23359 b- defN 24-Apr-16 20:03 gs_engine-0.28.0a20240416.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-16 20:03 gs_engine-0.28.0a20240416.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-16 20:03 gs_engine-0.28.0a20240416.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-Apr-16 20:03 gs_engine-0.28.0a20240416.dist-info/RECORD
+9 files, 27781 bytes uncompressed, 11237 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.28.0a20240415.dist-info/METADATA
+Filename: gs_engine-0.28.0a20240416.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.28.0a20240415.dist-info/WHEEL
+Filename: gs_engine-0.28.0a20240416.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.28.0a20240415.dist-info/top_level.txt
+Filename: gs_engine-0.28.0a20240416.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.28.0a20240415.dist-info/RECORD
+Filename: gs_engine-0.28.0a20240416.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.28.0a20240415.dist-info/METADATA` & `gs_engine-0.28.0a20240416.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.28.0a20240415
+Version: 0.28.0a20240416
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,15 @@
 🎉 See our ongoing [GraphScope Flex](https://github.com/alibaba/GraphScope/tree/main/flex): a LEGO-inspired, modular, and user-friendly GraphScope evolution. 🎉
 
 GraphScope is a unified distributed graph computing platform that provides a one-stop environment for performing diverse graph operations on a cluster of computers through a user-friendly Python interface. GraphScope makes multi-staged processing of large-scale graph data on compute clusters simply by combining several important pieces of Alibaba technology: including [GRAPE](https://github.com/alibaba/libgrape-lite), [MaxGraph](interactive_engine/), and [Graph-Learn](https://github.com/alibaba/graph-learn) (GL) for analytics, interactive, and graph neural networks (GNN) computation, respectively, and the [Vineyard](https://github.com/v6d-io/v6d) store that offers efficient in-memory data transfers.
 
 Visit our website at [graphscope.io](https://graphscope.io) to learn more.
 
 ## Latest News
+- [25/03/2024] 🙌🏻 We donated the graph file format [GraphAr](https://graphar.apache.org/) to [Apache Software Foundation](https://www.apache.org/) as an Incubating Project. 
 - [05/02/2024] 🎉 GraphScope Flex [paper](https://arxiv.org/abs/2312.12107) was accepted by [SIGMOD 2024](https://2024.sigmod.org/) Industry Track. See you in 🇨🇱!
 - [19/12/2023] 📑 A paper introducing GraphScope Flex released on [arXiv.org](https://arxiv.org/abs/2312.12107).
 - [20/07/2023] 🏆 GraphScope achieved record-breaking results on the [LDBC Social Network Benchmark Interactive workload](https://ldbcouncil.org/benchmarks/snb-interactive/), with a 2.45× higher throughput on SF300 than the previous record holder! 🏆
 - [04/07/2023] 🚀 GraphScope Flex tech preview released with [v0.23.0](https://github.com/alibaba/GraphScope/releases/tag/v0.23.0).
   
 ## Table of Contents
```

