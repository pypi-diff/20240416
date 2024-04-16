# Comparing `tmp/mat-model-0.1b11.tar.gz` & `tmp/mat_model-0.1b12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat-model-0.1b11.tar", last modified: Wed Apr 10 16:18:46 2024, max compression
+gzip compressed data, was "mat_model-0.1b12.tar", last modified: Tue Apr 16 12:52:26 2024, max compression
```

## Comparing `mat-model-0.1b11.tar` & `mat_model-0.1b12.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-10 16:18:46.027019 mat-model-0.1b11/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat-model-0.1b11/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat-model-0.1b11/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat-model-0.1b11/MANIFEST.in
--rw-------   0 tarlisportela   (501) staff       (20)    30233 2024-04-10 16:01:18.000000 mat-model-0.1b11/MAT-Tools.drawio
--rwx------   0 tarlisportela   (501) staff       (20)    44191 2024-04-10 16:08:37.000000 mat-model-0.1b11/MAT-model-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5040 2024-04-10 16:18:46.026812 mat-model-0.1b11/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat-model-0.1b11/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat-model-0.1b11/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-10 16:18:46.026125 mat-model-0.1b11/mat_model.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5040 2024-04-10 16:18:46.000000 mat-model-0.1b11/mat_model.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      606 2024-04-10 16:18:46.000000 mat-model-0.1b11/mat_model.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-10 16:18:46.000000 mat-model-0.1b11/mat_model.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      148 2024-04-10 16:18:46.000000 mat-model-0.1b11/mat_model.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-10 16:18:46.000000 mat-model-0.1b11/mat_model.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-10 16:18:46.023604 mat-model-0.1b11/matmodel/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat-model-0.1b11/matmodel/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat-model-0.1b11/matmodel/README.md
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-10 16:18:46.025953 mat-model-0.1b11/matmodel/classes/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3749 2023-09-03 21:43:34.000000 mat-model-0.1b11/matmodel/classes/Aspect.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     8987 2023-09-03 21:18:52.000000 mat-model-0.1b11/matmodel/classes/Comparator.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      814 2023-09-03 21:44:18.000000 mat-model-0.1b11/matmodel/classes/Feature.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1277 2023-09-02 21:37:48.000000 mat-model-0.1b11/matmodel/classes/Movelet.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3657 2023-09-02 21:09:06.000000 mat-model-0.1b11/matmodel/classes/MultipleAspectSequence.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-09-02 21:02:56.000000 mat-model-0.1b11/matmodel/classes/Quality.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4223 2023-09-02 21:46:34.000000 mat-model-0.1b11/matmodel/classes/Subtrajectory.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      784 2023-09-02 21:46:47.000000 mat-model-0.1b11/matmodel/classes/Trajectory.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-05-02 00:25:10.000000 mat-model-0.1b11/matmodel/classes/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2134 2024-04-10 16:10:37.000000 mat-model-0.1b11/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-10 16:18:46.027056 mat-model-0.1b11/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat-model-0.1b11/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 12:52:26.548844 mat_model-0.1b12/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b12/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b12/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b12/MANIFEST.in
+-rw-------   0 tarlisportela   (501) staff       (20)    31070 2024-04-15 18:13:37.000000 mat_model-0.1b12/MAT-Tools.drawio
+-rwx------   0 tarlisportela   (501) staff       (20)     3231 2024-04-10 16:28:00.000000 mat_model-0.1b12/MAT-model-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5040 2024-04-16 12:52:26.548648 mat_model-0.1b12/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b12/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b12/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 12:52:26.547916 mat_model-0.1b12/mat_model.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5040 2024-04-16 12:52:26.000000 mat_model-0.1b12/mat_model.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      605 2024-04-16 12:52:26.000000 mat_model-0.1b12/mat_model.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-16 12:52:26.000000 mat_model-0.1b12/mat_model.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      148 2024-04-16 12:52:26.000000 mat_model-0.1b12/mat_model.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-16 12:52:26.000000 mat_model-0.1b12/mat_model.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 12:52:26.545529 mat_model-0.1b12/matmodel/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b12/matmodel/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b12/matmodel/README.md
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 12:52:26.547119 mat_model-0.1b12/matmodel/base/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3749 2023-09-03 21:43:34.000000 mat_model-0.1b12/matmodel/base/Aspect.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      811 2024-04-16 12:05:57.000000 mat_model-0.1b12/matmodel/base/Feature.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1271 2024-04-16 12:05:30.000000 mat_model-0.1b12/matmodel/base/Movelet.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3654 2024-04-16 12:06:50.000000 mat_model-0.1b12/matmodel/base/MultipleAspectSequence.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4220 2024-04-16 12:05:44.000000 mat_model-0.1b12/matmodel/base/Subtrajectory.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      781 2024-04-16 12:05:49.000000 mat_model-0.1b12/matmodel/base/Trajectory.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-05-02 00:25:10.000000 mat_model-0.1b12/matmodel/base/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 12:52:26.547242 mat_model-0.1b12/matmodel/distance/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     8987 2023-09-03 21:18:52.000000 mat_model-0.1b12/matmodel/distance/Comparator.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-16 12:52:26.547741 mat_model-0.1b12/matmodel/evaluation/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-09-02 21:02:56.000000 mat_model-0.1b12/matmodel/evaluation/Quality.py
+-rw-------   0 tarlisportela   (501) staff       (20)    58933 2024-04-12 14:57:32.000000 mat_model-0.1b12/matmodel.drawio
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2134 2024-04-16 12:52:00.000000 mat_model-0.1b12/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-16 12:52:26.548885 mat_model-0.1b12/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b12/setup.py
```

### Comparing `mat-model-0.1b11/LICENSE` & `mat_model-0.1b12/LICENSE`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/MAT-Tools.drawio` & `mat_model-0.1b12/MAT-Tools.drawio`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-<mxfile host="app.diagrams.net" modified="2024-04-10T16:01:18.310Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36" etag="ZwS9_k6pSJtNATrDpxDf" version="23.1.5" type="device">
+<mxfile host="app.diagrams.net" modified="2024-04-15T18:13:37.867Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36" etag="GOhE4i7AqAaWFN0QtzYx" version="23.1.5" type="device">
   <diagram name="Página-1" id="NjSdwOmiIwXVztQAF8Lo">
-    <mxGraphModel dx="1781" dy="615" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
+    <mxGraphModel dx="1156" dy="212" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
       <root>
         <mxCell id="0" />
         <mxCell id="1" parent="0" />
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-61" value="&lt;h4&gt;Trajectory Input&lt;/h4&gt;" style="rounded=1;whiteSpace=wrap;html=1;fillColor=none;verticalAlign=top;labelPosition=right;verticalLabelPosition=bottom;align=left;spacing=-15;spacingTop=0;spacingLeft=-100;spacingRight=0;fontColor=#0000CC;labelBorderColor=none;strokeColor=#0000CC;arcSize=5;" parent="1" vertex="1">
-          <mxGeometry x="1340" y="224" width="180" height="240" as="geometry" />
+          <mxGeometry x="2170" y="168" width="180" height="240" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-62" value="&lt;h4&gt;Mixed Input / Ensemble&lt;/h4&gt;" style="rounded=1;whiteSpace=wrap;html=1;fillColor=none;verticalAlign=top;labelPosition=center;verticalLabelPosition=bottom;align=center;spacing=-15;spacingTop=1;spacingLeft=0;spacingRight=0;fontColor=#EBC75E;labelBorderColor=none;strokeColor=#EBC75E;arcSize=12;" parent="1" vertex="1">
-          <mxGeometry x="1166" y="310" width="140" height="154" as="geometry" />
+          <mxGeometry x="1996" y="254" width="140" height="154" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-60" value="&lt;h4&gt;Feature Input&lt;/h4&gt;" style="rounded=1;whiteSpace=wrap;html=1;fillColor=none;verticalAlign=top;labelPosition=left;verticalLabelPosition=bottom;align=right;spacing=-15;spacingTop=1;spacingLeft=0;spacingRight=-80;fontColor=#009900;labelBorderColor=none;strokeColor=#009900;arcSize=6;" parent="1" vertex="1">
-          <mxGeometry x="840" y="303" width="300" height="160" as="geometry" />
+          <mxGeometry x="1670" y="247" width="300" height="160" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-5" value="methods" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=14;tabPosition=left;html=1;whiteSpace=wrap;horizontal=1;verticalAlign=top;fillColor=none;" parent="1" vertex="1">
           <mxGeometry x="260" y="307" width="160" height="436" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-2" value="mat-data" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
           <mxGeometry x="150" y="20" width="170" height="190" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-4" value="preprocess" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
           <mxGeometry x="170" y="96" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-5" value="generator" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
           <mxGeometry x="170" y="60" width="130" height="30" as="geometry" />
         </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-6" value="mat-view" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-6" value="mat-view" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=26;" parent="1" vertex="1">
           <mxGeometry x="-160" y="274" width="170" height="130" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-7" value="web-app &lt;br&gt;&lt;i&gt;(Movelets &amp;amp; MAT)&lt;/i&gt;" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
           <mxGeometry x="-140" y="350" width="130" height="41" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-8" value="graphics" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
           <mxGeometry x="-140" y="314" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-35" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;exitX=0.512;exitY=0;exitDx=0;exitDy=0;exitPerimeter=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-9" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="ncjso_DGpGOnADHclqbK-1" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;dashed=1;strokeColor=default;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=open;endFill=0;" edge="1" parent="1" source="n9qyGrMY-b-BzYaa1yog-9" target="BebV0c_RTAwMKaFlxQ5s-1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-9" value="movelets" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
-          <mxGeometry x="480" y="273" width="170" height="190" as="geometry" />
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-9" value="movelets" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=25;" parent="1" vertex="1">
+          <mxGeometry x="490" y="285.5" width="170" height="190" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-10" value="MLP (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
           <mxGeometry x="270" y="599" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-8" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=1;entryY=0.5;entryDx=0;entryDy=0;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-11" target="n9qyGrMY-b-BzYaa1yog-21" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
@@ -78,15 +78,15 @@
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-23" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-12" target="n9qyGrMY-b-BzYaa1yog-6" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-33" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-12" target="n9qyGrMY-b-BzYaa1yog-19" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-12" value="automatize" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-12" value="automatize" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=120;height=27;" parent="1" vertex="1">
           <mxGeometry x="40" y="273" width="170" height="235" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-13" value="run" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
           <mxGeometry x="60" y="350" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-14" value="results" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;" parent="1" vertex="1">
           <mxGeometry x="60" y="313" width="130" height="30" as="geometry" />
@@ -99,15 +99,15 @@
             <mxPoint x="460" y="362.1250000000001" as="sourcePoint" />
             <mxPoint x="502.70491803278696" y="297" as="targetPoint" />
           </mxGeometry>
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-34" style="rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;dashed=1;endFill=0;" parent="1" source="n9qyGrMY-b-BzYaa1yog-19" target="n9qyGrMY-b-BzYaa1yog-2" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
-        <mxCell id="n9qyGrMY-b-BzYaa1yog-19" value="mat-analysis" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
+        <mxCell id="n9qyGrMY-b-BzYaa1yog-19" value="mat-classification" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=130;height=27;" parent="1" vertex="1">
           <mxGeometry x="250" y="273" width="190" height="520" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-20" value="POI-S" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
           <mxGeometry x="271" y="562" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="n9qyGrMY-b-BzYaa1yog-21" value="MARC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
           <mxGeometry x="271" y="525" width="130" height="30" as="geometry" />
@@ -150,185 +150,194 @@
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-7" value="scripts" style="shape=folder;fontStyle=1;spacingTop=10;tabWidth=40;tabHeight=10;tabPosition=left;html=1;whiteSpace=wrap;" parent="1" vertex="1">
           <mxGeometry x="65" y="469" width="125" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-38" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-11" target="mgZLQg_ETMRa4hPbAOP7-26" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1150" y="327" />
+              <mxPoint x="1980" y="271" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-11" value="MLP (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="1004" y="311.5" width="130" height="30" as="geometry" />
+          <mxGeometry x="1834" y="255.5" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-12" value="TEC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#fff2cc;strokeColor=#d6b656;" parent="1" vertex="1">
-          <mxGeometry x="1171" y="322.5" width="130" height="30" as="geometry" />
+          <mxGeometry x="2001" y="266.5" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-36" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-13" target="mgZLQg_ETMRa4hPbAOP7-26" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1150" y="368" />
+              <mxPoint x="1980" y="312" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-13" value="POI-S" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="1004" y="352.5" width="130" height="30" as="geometry" />
+          <mxGeometry x="1834" y="296.5" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-39" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-14" target="mgZLQg_ETMRa4hPbAOP7-27" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1500" y="118" />
+              <mxPoint x="2330" y="62" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-14" value="MARC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="1380" y="417" width="130" height="30" as="geometry" />
+          <mxGeometry x="2210" y="361" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-32" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;entryX=0;entryY=0.5;entryDx=0;entryDy=0;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-15" target="mgZLQg_ETMRa4hPbAOP7-22" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="990" y="330" />
-              <mxPoint x="990" y="200" />
+              <mxPoint x="1820" y="274" />
+              <mxPoint x="1820" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-15" value="RFHP&amp;nbsp; (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="844" y="314" width="130" height="30" as="geometry" />
+          <mxGeometry x="1674" y="258" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-33" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-47" target="mgZLQg_ETMRa4hPbAOP7-22" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="990" y="365" />
-              <mxPoint x="990" y="200" />
+              <mxPoint x="1820" y="309" />
+              <mxPoint x="1820" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-48" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-16" target="mgZLQg_ETMRa4hPbAOP7-22" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="990" y="401" />
-              <mxPoint x="990" y="200" />
+              <mxPoint x="1820" y="345" />
+              <mxPoint x="1820" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-16" value="SVM&amp;nbsp;(movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="844" y="386" width="130" height="30" as="geometry" />
+          <mxGeometry x="1674" y="330" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-40" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-17" target="mgZLQg_ETMRa4hPbAOP7-28" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1330" y="247" />
-              <mxPoint x="1330" y="200" />
+              <mxPoint x="2160" y="191" />
+              <mxPoint x="2160" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-17" value="DeepestST" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="1350" y="232" width="130" height="30" as="geometry" />
+          <mxGeometry x="2180" y="176" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-41" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-18" target="mgZLQg_ETMRa4hPbAOP7-28" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1330" y="284" />
-              <mxPoint x="1330" y="200" />
+              <mxPoint x="2160" y="228" />
+              <mxPoint x="2160" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-18" value="MAT RF" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="1350" y="269" width="130" height="30" as="geometry" />
+          <mxGeometry x="2180" y="213" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-42" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-19" target="mgZLQg_ETMRa4hPbAOP7-28" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1330" y="320" />
-              <mxPoint x="1330" y="200" />
+              <mxPoint x="2160" y="264" />
+              <mxPoint x="2160" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-19" value="MAT XGBoost" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="1350" y="305" width="130" height="30" as="geometry" />
+          <mxGeometry x="2180" y="249" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-43" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-20" target="mgZLQg_ETMRa4hPbAOP7-28" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1330" y="357" />
-              <mxPoint x="1330" y="200" />
+              <mxPoint x="2160" y="301" />
+              <mxPoint x="2160" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-20" value="TULVAE" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="1350" y="342" width="130" height="30" as="geometry" />
+          <mxGeometry x="2180" y="286" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-44" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-21" target="mgZLQg_ETMRa4hPbAOP7-28" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1330" y="394" />
-              <mxPoint x="1330" y="200" />
+              <mxPoint x="2160" y="338" />
+              <mxPoint x="2160" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-21" value="BITULER" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#dae8fc;strokeColor=#6c8ebf;" parent="1" vertex="1">
-          <mxGeometry x="1350" y="379" width="130" height="30" as="geometry" />
+          <mxGeometry x="2180" y="323" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-30" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-22" target="mgZLQg_ETMRa4hPbAOP7-27" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-22" value="MClassifier" style="swimlane;fontStyle=3;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="1" vertex="1">
-          <mxGeometry x="1064" y="180" width="110" height="40" as="geometry" />
+          <mxGeometry x="1894" y="124" width="110" height="40" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-31" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-26" target="mgZLQg_ETMRa4hPbAOP7-22" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-26" value="MHPSClassifier" style="swimlane;fontStyle=3;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="1" vertex="1">
-          <mxGeometry x="1064" y="250" width="110" height="40" as="geometry" />
+          <mxGeometry x="1894" y="194" width="110" height="40" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-27" value="AbstractClassifier" style="swimlane;fontStyle=3;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="1" vertex="1">
-          <mxGeometry x="1120" y="96" width="140" height="44" as="geometry" />
+          <mxGeometry x="1950" y="40" width="140" height="44" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-29" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-28" target="mgZLQg_ETMRa4hPbAOP7-27" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-28" value="HPSClassifier" style="swimlane;fontStyle=3;childLayout=stackLayout;horizontal=1;startSize=30;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;" parent="1" vertex="1">
-          <mxGeometry x="1204" y="180" width="110" height="40" as="geometry" />
+          <mxGeometry x="2034" y="124" width="110" height="40" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-49" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-46" target="mgZLQg_ETMRa4hPbAOP7-22" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="990" y="437" />
-              <mxPoint x="990" y="200" />
+              <mxPoint x="1820" y="381" />
+              <mxPoint x="1820" y="144" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-46" value="DT (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="844" y="422" width="130" height="30" as="geometry" />
+          <mxGeometry x="1674" y="366" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-47" value="RF&amp;nbsp; (movelets)" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#d5e8d4;strokeColor=#82b366;" parent="1" vertex="1">
-          <mxGeometry x="844" y="350" width="130" height="30" as="geometry" />
+          <mxGeometry x="1674" y="294" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-63" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-12" target="mgZLQg_ETMRa4hPbAOP7-28" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1260" y="330" />
-              <mxPoint x="1260" y="330" />
+              <mxPoint x="2090" y="274" />
+              <mxPoint x="2090" y="274" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-64" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-12" target="mgZLQg_ETMRa4hPbAOP7-26" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1220" y="270" />
+              <mxPoint x="2050" y="214" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-66" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endFill=0;" parent="1" source="mgZLQg_ETMRa4hPbAOP7-65" target="mgZLQg_ETMRa4hPbAOP7-12" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="mgZLQg_ETMRa4hPbAOP7-65" value="MSTEC" style="shape=module;align=left;spacingLeft=20;align=center;verticalAlign=top;whiteSpace=wrap;html=1;jettyWidth=16;jettyHeight=6;fillColor=#fff2cc;strokeColor=#d6b656;" parent="1" vertex="1">
-          <mxGeometry x="1171" y="414" width="130" height="30" as="geometry" />
+          <mxGeometry x="2001" y="358" width="130" height="30" as="geometry" />
         </mxCell>
         <mxCell id="BebV0c_RTAwMKaFlxQ5s-1" value="mat-model" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=110;height=30;" parent="1" vertex="1">
-          <mxGeometry x="480" y="20" width="170" height="190" as="geometry" />
+          <mxGeometry x="480" y="66" width="170" height="60" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-2" value="mat-similarity" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=140;height=31;" vertex="1" parent="1">
+          <mxGeometry x="670" y="499" width="170" height="190" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-3" value="mat-summarization" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=133;height=26;" vertex="1" parent="1">
+          <mxGeometry x="490" y="499" width="170" height="190" as="geometry" />
+        </mxCell>
+        <mxCell id="ncjso_DGpGOnADHclqbK-4" value="mat-clustering" style="shape=umlFrame;whiteSpace=wrap;html=1;pointerEvents=0;width=133;height=26;" vertex="1" parent="1">
+          <mxGeometry x="670" y="285.5" width="170" height="190" as="geometry" />
         </mxCell>
       </root>
     </mxGraphModel>
   </diagram>
 </mxfile>
```

### Comparing `mat-model-0.1b11/PKG-INFO` & `mat_model-0.1b12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b11
+Version: 0.1b12
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat-model-0.1b11/README.md` & `mat_model-0.1b12/README.md`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/Steps to Build.txt` & `mat_model-0.1b12/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/mat_model.egg-info/PKG-INFO` & `mat_model-0.1b12/mat_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b11
+Version: 0.1b12
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat-model-0.1b11/mat_model.egg-info/SOURCES.txt` & `mat_model-0.1b12/mat_model.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 MAT-Tools.drawio
 MAT-model-Tutorial.ipynb
 README.md
 Steps to Build.txt
+matmodel.drawio
 pyproject.toml
 setup.py
 mat_model.egg-info/PKG-INFO
 mat_model.egg-info/SOURCES.txt
 mat_model.egg-info/dependency_links.txt
 mat_model.egg-info/requires.txt
 mat_model.egg-info/top_level.txt
 matmodel/LICENSE
 matmodel/README.md
-matmodel/classes/Aspect.py
-matmodel/classes/Comparator.py
-matmodel/classes/Feature.py
-matmodel/classes/Movelet.py
-matmodel/classes/MultipleAspectSequence.py
-matmodel/classes/Quality.py
-matmodel/classes/Subtrajectory.py
-matmodel/classes/Trajectory.py
-matmodel/classes/__init__.py
+matmodel/base/Aspect.py
+matmodel/base/Feature.py
+matmodel/base/Movelet.py
+matmodel/base/MultipleAspectSequence.py
+matmodel/base/Subtrajectory.py
+matmodel/base/Trajectory.py
+matmodel/base/__init__.py
+matmodel/distance/Comparator.py
+matmodel/evaluation/Quality.py
```

### Comparing `mat-model-0.1b11/matmodel/LICENSE` & `mat_model-0.1b12/matmodel/LICENSE`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/matmodel/README.md` & `mat_model-0.1b12/matmodel/README.md`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/matmodel/classes/Aspect.py` & `mat_model-0.1b12/matmodel/base/Aspect.py`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/matmodel/classes/Comparator.py` & `mat_model-0.1b12/matmodel/distance/Comparator.py`

 * *Files identical despite different names*

### Comparing `mat-model-0.1b11/matmodel/classes/Feature.py` & `mat_model-0.1b12/matmodel/base/Feature.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from movelets.classes.Aspect import Aspect
+from matmodel.base.Aspect import Aspect
 
 class Quality:
     def __init__(self, value):
         self.value = value
 
 class Feature:
     def __init__(self, quality=None):
```

### Comparing `mat-model-0.1b11/matmodel/classes/Movelet.py` & `mat_model-0.1b12/matmodel/base/Movelet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from movelets.classes.Subtrajectory import Subtrajectory
-from movelets.classes.Feature import Feature
+from matmodel.base.Subtrajectory import Subtrajectory
+from matmodel.base.Feature import Feature
 # ------------------------------------------------------------------------------------------------------------
 # MOVELETS 
 # ------------------------------------------------------------------------------------------------------------
 class Movelet(Subtrajectory, Feature):
     def __init__(self, trajectory, start, size, points, attributes_index, quality):
         Subtrajectory.__init__(self, trajectory, start, size, points, attributes_index)
         Feature.__init__(self, quality=quality)
```

### Comparing `mat-model-0.1b11/matmodel/classes/MultipleAspectSequence.py` & `mat_model-0.1b12/matmodel/base/MultipleAspectSequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ------------------------------------------------------------------------------------------------------------
 # BASE for MultipleAspectSequence
 # ------------------------------------------------------------------------------------------------------------
-from movelets.classes.Aspect import instantiateAspect
+from matmodel.base.Aspect import instantiateAspect
 #from movelets.classes.Subtrajectory import Subtrajectory
 
 class MultipleAspectSequence:
     def __init__(self, seq_id, new_points=None, attributes_desc=None):
         self.tid          = seq_id
         
         self.points       = []
```

### Comparing `mat-model-0.1b11/matmodel/classes/Subtrajectory.py` & `mat_model-0.1b12/matmodel/base/Subtrajectory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ------------------------------------------------------------------------------------------------------------
 # SUBTRAJECTORIES 
 # ------------------------------------------------------------------------------------------------------------
-from movelets.classes.MultipleAspectSequence import MultipleAspectSequence
+from matmodel.base.MultipleAspectSequence import MultipleAspectSequence
 
 class Subtrajectory(MultipleAspectSequence):
     def __init__(self, trajectory, start, size, points, attributes_index):
         MultipleAspectSequence.__init__(self, trajectory.tid)
         self.sid     = 0 # TODO generate unique sid
         self.start   = start
         self.size   = size
```

### Comparing `mat-model-0.1b11/matmodel/classes/Trajectory.py` & `mat_model-0.1b12/matmodel/base/Trajectory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from movelets.classes.MultipleAspectSequence import MultipleAspectSequence
+from matmodel.base.MultipleAspectSequence import MultipleAspectSequence
 # ------------------------------------------------------------------------------------------------------------
 # TRAJECTORY 
 # ------------------------------------------------------------------------------------------------------------
 class Trajectory(MultipleAspectSequence):
     def __init__(self, tid, label, new_points, attributes_desc):
         MultipleAspectSequence.__init__(self, tid, new_points, attributes_desc)
         self.label = label
```

### Comparing `mat-model-0.1b11/pyproject.toml` & `mat_model-0.1b12/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-model"
-version = "0.1b11"
+version = "0.1b12"
 description = "MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `mat-model-0.1b11/setup.py` & `mat_model-0.1b12/setup.py`

 * *Files identical despite different names*

