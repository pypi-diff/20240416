# Comparing `tmp/pyTwistyScrambler-1.6.tar.gz` & `tmp/pytwistyscrambler-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Wes\dev\pyTwistyScrambler\dist\tmpv8rh1_6m\pyTwistyScrambler-1.6.tar", last modified: Mon Apr  5 16:51:12 2021, max compression
+gzip compressed data, was "C:\Users\Wes\dev\pyTwistyScrambler\dist\.tmp-g2js0nzv\pytwistyscrambler-1.7.tar", last modified: Tue Apr 16 20:52:29 2024, max compression
```

## Comparing `pyTwistyScrambler-1.6.tar` & `pytwistyscrambler-1.7.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2021-04-05 16:51:12.462054 pyTwistyScrambler-1.6/
--rw-rw-rw-   0        0        0       43 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    10223 2021-04-05 16:51:12.462054 pyTwistyScrambler-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     8363 2021-04-04 15:59:52.000000 pyTwistyScrambler-1.6/README.md
-drwxrwxrwx   0        0        0        0 2021-04-05 16:51:12.424065 pyTwistyScrambler-1.6/pyTwistyScrambler/
--rw-rw-rw-   0        0        0     2698 2021-01-11 03:37:38.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/__init__.py
--rw-rw-rw-   0        0        0      910 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/bigCubesScrambler.py
--rw-rw-rw-   0        0        0      830 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/clockScrambler.py
--rw-rw-rw-   0        0        0     1891 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/cuboidsScrambler.py
--rw-rw-rw-   0        0        0     2745 2021-01-11 03:38:34.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/ftoScrambler.py
-drwxrwxrwx   0        0        0        0 2021-04-05 16:51:12.461053 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/
--rw-rw-rw-   0        0        0      785 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/1x3x3.js
--rw-rw-rw-   0        0        0     2373 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/2x2x2.js
--rw-rw-rw-   0        0        0     2607 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/2x2x3.js
--rw-rw-rw-   0        0        0     5854 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/cross.js
--rw-rw-rw-   0        0        0    59583 2021-04-04 15:50:43.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/fto.js
--rw-rw-rw-   0        0        0     6826 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/mathlib.js
--rw-rw-rw-   0        0        0    11890 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/megascramble.js
--rw-rw-rw-   0        0        0     2726 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/pyraminx.js
--rw-rw-rw-   0        0        0     9600 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble.js
--rw-rw-rw-   0        0        0    40380 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble_333_edit.js
--rw-rw-rw-   0        0        0    73355 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble_444.js
--rw-rw-rw-   0        0        0    18682 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble_sq1.js
--rw-rw-rw-   0        0        0     3785 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/skewb.js
--rw-rw-rw-   0        0        0    14312 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/utilscramble.js
--rw-rw-rw-   0        0        0      923 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/megaminxScrambler.py
--rw-rw-rw-   0        0        0      435 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/pyraminxScrambler.py
--rw-rw-rw-   0        0        0     3101 2021-04-04 15:55:09.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/rexScrambler.py
--rw-rw-rw-   0        0        0      635 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler222.py
--rw-rw-rw-   0        0        0     4145 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler333.py
--rw-rw-rw-   0        0        0     1141 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler444.py
--rw-rw-rw-   0        0        0      950 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler555.py
--rw-rw-rw-   0        0        0      789 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler666.py
--rw-rw-rw-   0        0        0      793 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler777.py
--rw-rw-rw-   0        0        0      440 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/skewbScrambler.py
--rw-rw-rw-   0        0        0      773 2021-01-11 02:41:59.000000 pyTwistyScrambler-1.6/pyTwistyScrambler/squareOneScrambler.py
-drwxrwxrwx   0        0        0        0 2021-04-05 16:51:12.444058 pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/
--rw-rw-rw-   0        0        0    10223 2021-04-05 16:51:12.000000 pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1424 2021-04-05 16:51:12.000000 pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-05 16:51:12.000000 pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2021-04-05 16:51:12.000000 pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2021-04-05 16:51:12.000000 pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2021-04-04 16:18:52.000000 pyTwistyScrambler-1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2021-04-05 16:51:12.462054 pyTwistyScrambler-1.6/setup.cfg
--rw-rw-rw-   0        0        0      798 2021-04-05 16:50:33.000000 pyTwistyScrambler-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:52:29.402874 pytwistyscrambler-1.7/
+-rw-rw-rw-   0        0        0     1093 2021-04-04 16:41:29.000000 pytwistyscrambler-1.7/LICENSE
+-rw-rw-rw-   0        0        0       43 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8877 2024-04-16 20:52:29.400877 pytwistyscrambler-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8363 2021-04-04 15:59:52.000000 pytwistyscrambler-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 20:52:29.344879 pytwistyscrambler-1.7/pyTwistyScrambler/
+-rw-rw-rw-   0        0        0     2698 2021-01-11 03:37:38.000000 pytwistyscrambler-1.7/pyTwistyScrambler/__init__.py
+-rw-rw-rw-   0        0        0      910 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/bigCubesScrambler.py
+-rw-rw-rw-   0        0        0      830 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/clockScrambler.py
+-rw-rw-rw-   0        0        0     1891 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/cuboidsScrambler.py
+-rw-rw-rw-   0        0        0     2745 2021-01-11 03:38:34.000000 pytwistyscrambler-1.7/pyTwistyScrambler/ftoScrambler.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:52:29.394880 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/
+-rw-rw-rw-   0        0        0      785 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/1x3x3.js
+-rw-rw-rw-   0        0        0     2373 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/2x2x2.js
+-rw-rw-rw-   0        0        0     2607 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/2x2x3.js
+-rw-rw-rw-   0        0        0     5854 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/cross.js
+-rw-rw-rw-   0        0        0    59583 2021-04-04 15:50:43.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/fto.js
+-rw-rw-rw-   0        0        0     6826 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/mathlib.js
+-rw-rw-rw-   0        0        0    11890 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/megascramble.js
+-rw-rw-rw-   0        0        0     2726 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/pyraminx.js
+-rw-rw-rw-   0        0        0     9600 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble.js
+-rw-rw-rw-   0        0        0    40380 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble_333_edit.js
+-rw-rw-rw-   0        0        0    73355 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble_444.js
+-rw-rw-rw-   0        0        0    18682 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble_sq1.js
+-rw-rw-rw-   0        0        0     3785 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/skewb.js
+-rw-rw-rw-   0        0        0    14020 2024-04-16 20:12:57.000000 pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/utilscramble.js
+-rw-rw-rw-   0        0        0      923 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/megaminxScrambler.py
+-rw-rw-rw-   0        0        0      301 2024-04-16 20:14:26.000000 pytwistyscrambler-1.7/pyTwistyScrambler/miscScrambler.py
+-rw-rw-rw-   0        0        0      435 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/pyraminxScrambler.py
+-rw-rw-rw-   0        0        0     3101 2021-04-04 15:55:09.000000 pytwistyscrambler-1.7/pyTwistyScrambler/rexScrambler.py
+-rw-rw-rw-   0        0        0      635 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/scrambler222.py
+-rw-rw-rw-   0        0        0     4145 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/scrambler333.py
+-rw-rw-rw-   0        0        0     1141 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/scrambler444.py
+-rw-rw-rw-   0        0        0      950 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/scrambler555.py
+-rw-rw-rw-   0        0        0      789 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/scrambler666.py
+-rw-rw-rw-   0        0        0      793 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/scrambler777.py
+-rw-rw-rw-   0        0        0      440 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/skewbScrambler.py
+-rw-rw-rw-   0        0        0      773 2021-01-11 02:41:59.000000 pytwistyscrambler-1.7/pyTwistyScrambler/squareOneScrambler.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:52:29.398875 pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/
+-rw-rw-rw-   0        0        0     8877 2024-04-16 20:52:29.000000 pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1467 2024-04-16 20:52:29.000000 pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 20:52:29.000000 pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-16 20:52:29.000000 pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 20:52:29.000000 pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2021-04-04 16:18:52.000000 pytwistyscrambler-1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 20:52:29.402874 pytwistyscrambler-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      798 2024-04-16 20:15:57.000000 pytwistyscrambler-1.7/setup.py
```

### Comparing `pyTwistyScrambler-1.6/README.md` & `pytwistyscrambler-1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/__init__.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/bigCubesScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/bigCubesScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/clockScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/clockScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/cuboidsScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/cuboidsScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/ftoScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/ftoScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/1x3x3.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/1x3x3.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/2x2x2.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/2x2x2.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/2x2x3.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/2x2x3.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/cross.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/cross.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/fto.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/fto.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/mathlib.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/mathlib.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/megascramble.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/megascramble.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/pyraminx.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/pyraminx.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble_333_edit.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble_333_edit.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble_444.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble_444.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/scramble_sq1.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/scramble_sq1.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/skewb.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/skewb.js`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/js_resources/utilscramble.js` & `pytwistyscrambler-1.7/pyTwistyScrambler/js_resources/utilscramble.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,499 +1,506 @@
-"use strict";
-
-var util_scramble = (function(rn, rndEl, mega) {
-    var cubesuff = ["", "2", "'"];
-    var minxsuff = ["", "2", "'", "2'"];
-    var seq = [];
-    var p = [];
-
-    function helicubescramble(type, len) {
-        var faces = ["UF", "UR", "UB", "UL", "FR", "BR", "BL", "FL", "DF", "DR", "DB", "DL"];
-        // adjacency table
-        var adj = [0x09a, 0x035, 0x06a, 0x0c5, 0x303, 0x606, 0xc0c, 0x909, 0xa90, 0x530, 0xa60, 0x5c0];
-        var used = 0;
-        var face;
-        var ret = [];
-        for (var j = 0; j < len; j++) {
-            do {
-                face = rn(12);
-            } while (((used >> face) & 1) != 0);
-            ret.push(faces[face]);
-            used &= ~adj[face];
-            used |= 1 << face;
-        }
-        return ret.join(" ");
-    }
-    //scramble.reg('heli', helicubescramble);
-
-    function yj4x4(type, len) {
-        // the idea is to keep the fixed center on U and do Rw or Lw, Fw or Bw, to not disturb it
-        var turns = [
-            ["U", "D"],
-            ["R", "L", "r"],
-            ["F", "B", "f"]
-        ];
-        var donemoves = [];
-        var lastaxis;
-        var fpos = 0; // 0 = Ufr, 1 = Ufl, 2 = Ubl, 3 = Ubr
-        var j, k;
-        var s = "";
-        lastaxis = -1;
-        for (j = 0; j < len; j++) {
-            var done = 0;
-            do {
-                var first = rn(turns.length);
-                var second = rn(turns[first].length);
-                if (first != lastaxis || donemoves[second] == 0) {
-                    if (first == lastaxis) {
-                        donemoves[second] = 1;
-                        var rs = rn(cubesuff.length);
-                        if (first == 0 && second == 0) {
-                            fpos = (fpos + 4 + rs) % 4;
-                        }
-                        if (first == 1 && second == 2) { // r or l
-                            if (fpos == 0 || fpos == 3) s += "l" + cubesuff[rs] + " ";
-                            else s += "r" + cubesuff[rs] + " ";
-                        } else if (first == 2 && second == 2) { // f or b
-                            if (fpos == 0 || fpos == 1) s += "b" + cubesuff[rs] + " ";
-                            else s += "f" + cubesuff[rs] + " ";
-                        } else {
-                            s += turns[first][second] + cubesuff[rs] + " ";
-                        }
-                    } else {
-                        for (k = 0; k < turns[first].length; k++) {
-                            donemoves[k] = 0;
-                        }
-                        lastaxis = first;
-                        donemoves[second] = 1;
-                        var rs = rn(cubesuff.length);
-                        if (first == 0 && second == 0) {
-                            fpos = (fpos + 4 + rs) % 4;
-                        }
-                        if (first == 1 && second == 2) { // r or l
-                            if (fpos == 0 || fpos == 3) s += "l" + cubesuff[rs] + " ";
-                            else s += "r" + cubesuff[rs] + " ";
-                        } else if (first == 2 && second == 2) { // f or b
-                            if (fpos == 0 || fpos == 1) s += "b" + cubesuff[rs] + " ";
-                            else s += "f" + cubesuff[rs] + " ";
-                        } else {
-                            s += turns[first][second] + cubesuff[rs] + " ";
-                        }
-                    }
-                    done = 1;
-                }
-            } while (done == 0);
-        }
-        return s;
-    }
-
-    //scramble.reg('444yj', yj4x4);
-
-    function bicube(type, len) {
-        function canMove(face) {
-            var u = [],
-                i, j, done, z = 0;
-            for (i = 0; i < 9; i++) {
-                done = 0;
-                for (j = 0; j < u.length; j++) {
-                    if (u[j] == start[d[face][i]]) done = 1;
-                }
-                if (done == 0) {
-                    u[u.length] = start[d[face][i]];
-                    if (start[d[face][i]] == 0) z = 1;
-                }
-            }
-            return (u.length == 5 && z == 1);
-        }
-
-        function doMove(face, amount) {
-            for (var i = 0; i < amount; i++) {
-                var t = start[d[face][0]];
-                start[d[face][0]] = start[d[face][6]];
-                start[d[face][6]] = start[d[face][4]];
-                start[d[face][4]] = start[d[face][2]];
-                start[d[face][2]] = t;
-                t = start[d[face][7]];
-                start[d[face][7]] = start[d[face][5]];
-                start[d[face][5]] = start[d[face][3]];
-                start[d[face][3]] = start[d[face][1]];
-                start[d[face][1]] = t;
-            }
-        }
-
-        var d = [
-            [0, 1, 2, 5, 8, 7, 6, 3, 4],
-            [6, 7, 8, 13, 20, 19, 18, 11, 12],
-            [0, 3, 6, 11, 18, 17, 16, 9, 10],
-            [8, 5, 2, 15, 22, 21, 20, 13, 14]
-        ];
-        var start = [1, 1, 2, 3, 3, 2, 4, 4, 0, 5, 6, 7, 8, 9, 10, 10, 5, 6, 7, 8, 9, 11, 11],
-            move = "UFLR",
-            s = "",
-            arr = [],
-            poss, done, i, j, x, y;
-        while (arr.length < len) {
-            poss = [1, 1, 1, 1];
-            for (j = 0; j < 4; j++) {
-                if (poss[j] == 1 && !canMove(j))
-                    poss[j] = 0;
-            }
-            done = 0;
-            while (done == 0) {
-                x = rn(4);
-                if (poss[x] == 1) {
-                    y = rn(3) + 1;
-                    doMove(x, y);
-                    done = 1;
-                }
-            }
-            arr[arr.length] = [x, y];
-            if (arr.length >= 2) {
-                if (arr[arr.length - 1][0] == arr[arr.length - 2][0]) {
-                    arr[arr.length - 2][1] = (arr[arr.length - 2][1] + arr[arr.length - 1][1]) % 4;
-                    arr = arr.slice(0, arr.length - 1);
-                }
-            }
-            if (arr.length >= 1) {
-                if (arr[arr.length - 1][1] == 0) {
-                    arr = arr.slice(0, arr.length - 1);
-                }
-            }
-        }
-        for (i = 0; i < len; i++) {
-            s += move[arr[i][0]] + cubesuff[arr[i][1] - 1] + " ";
-        }
-        return s;
-    }
-
-    //scramble.reg('bic', bicube);
-
-
-
-    // Clock functions.
-    function c(s) {
-        var array = [s + "=0", s + "+1", s + "+2", s + "+3", s + "+4", s + "+5", s + "+6", s + "-5", s + "-4", s + "-3", s + "-2", s + "-1"];
-        return " " + rndEl(array) + " ";
-    }
-
-    function c2() {
-        return rndEl(["U", "d"]) + rndEl(["U", "d"]);
-    }
-
-    function c3() {
-        return "     "
-    }
-
-    function do15puzzle(mirrored, len) {
-        var moves = (mirrored ? ["U", "L", "R", "D"] : ["D", "R", "L", "U"]);
-        var effect = [
-            [0, -1],
-            [1, 0],
-            [-1, 0],
-            [0, 1]
-        ];
-        var x = 0,
-            y = 3,
-            k, done, r, lastr = 5;
-        ret = "";
-        for (k = 0; k < len; k++) {
-            done = false;
-            while (!done) {
-                r = rn(4);
-                if (x + effect[r][0] >= 0 && x + effect[r][0] <= 3 && y + effect[r][1] >= 0 && y + effect[r][1] <= 3 && r + lastr != 3) {
-                    done = true;
-                    x += effect[r][0];
-                    y += effect[r][1];
-                    ret += moves[r] + " ";
-                    lastr = r;
-                }
-            }
-        }
-        return ret;
-    }
-
-    function pochscramble(x, y) {
-        var ret = "";
-        var i, j;
-        for (i = 0; i < y; i++) {
-            ret += "  ";
-            for (j = 0; j < x; j++) {
-                ret += (j % 2 == 0 ? "R" : "D") + rndEl(["++", "--"]) + " ";
-            }
-            ret += "U" + (ret.endsWith("-- ") ? "'\n" : " \n");
-        }
-        return ret;
-    }
-
-    function carrotscramble(x, y) {
-        var ret = "";
-        var i, j;
-        for (i = 0; i < y; i++) {
-            ret += " ";
-            for (j = 0; j < x / 2; j++) {
-                ret += rndEl(["+", "-"]) + rndEl(["+", "-"]) + " ";
-            }
-            ret += "U" + rndEl(["'\n", " \n"]);
-        }
-        return ret;
-    }
-
-    function gigascramble(len) {
-        var ret = "";
-        var i, j;
-        for (i = 0; i < Math.ceil(len / 10); i++) {
-            ret += "  ";
-            for (j = 0; j < 10; j++) {
-                ret += (j % 2 == 0 ? ("Rr".charAt(rn(2))) : ("Dd".charAt(rn(2)))) + rndEl(["+ ", "++", "- ", "--"]) + " ";
-            }
-            ret += "y" + rndEl(minxsuff) + "\n";
-        }
-        return ret;
-    }
-
-    function sq1_scramble(type, len) {
-        seq = [];
-        var i, k;
-        sq1_getseq(1, type, len);
-        var s = "";
-        for (i = 0; i < seq[0].length; i++) {
-            k = seq[0][i];
-            if (k[0] == 7) {
-                s += "/";
-            } else {
-                s += " (" + k[0] + "," + k[1] + ") ";
-            }
-        }
-        return s;
-    }
-
-    function ssq1t_scramble(len) {
-        seq = [];
-        var i;
-        sq1_getseq(2, 0, len);
-        var s = seq[0],
-            t = seq[1],
-            u = "";
-        if (s[0][0] == 7) s = [
-            [0, 0]
-        ].concat(s);
-        if (t[0][0] == 7) t = [
-            [0, 0]
-        ].concat(t);
-        for (i = 0; i < len; i++) {
-            u += "(" + s[2 * i][0] + "," + t[2 * i][0] + "," + t[2 * i][1] + "," + s[2 * i][1] + ") / ";
-        }
-        return u;
-    }
-
-    function sq1_getseq(num, type, len) {
-        for (var n = 0; n < num; n++) {
-            p = [1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0];
-            seq[n] = [];
-            var cnt = 0;
-            while (cnt < len) {
-                var x = rn(12) - 5;
-                var y = (type == 2) ? 0 : rn(12) - 5;
-                var size = (x == 0 ? 0 : 1) + (y == 0 ? 0 : 1);
-                if ((cnt + size <= len || type != 1) && (size > 0 || cnt == 0)) {
-                    if (sq1_domove(x, y)) {
-                        if (type == 1) cnt += size;
-                        if (size > 0) seq[n][seq[n].length] = [x, y];
-                        if (cnt < len || type != 1) {
-                            cnt++;
-                            seq[n][seq[n].length] = [7, 0];
-                            sq1_domove(7, 0);
-                        }
-                    }
-                }
-            }
-        }
-    }
-
-    function sq1_domove(x, y) {
-        var i, px, py;
-        if (x == 7) {
-            for (i = 0; i < 6; i++) {
-                mathlib.circle(p, i + 6, i + 12);
-            }
-            return true;
-        } else {
-            if (p[(17 - x) % 12] || p[(11 - x) % 12] || p[12 + (17 - y) % 12] || p[12 + (11 - y) % 12]) {
-                return false;
-            } else {
-                // do the move itself
-                px = p.slice(0, 12);
-                py = p.slice(12, 24);
-                for (i = 0; i < 12; i++) {
-                    p[i] = px[(12 + i - x) % 12];
-                    p[i + 12] = py[(12 + i - y) % 12];
-                }
-                return true;
-            }
-        }
-    }
-
-    function oldminxscramble(len) {
-        var faces = ["F", "B", "U", "D", "L", "DBR", "DL", "BR", "DR", "BL", "R", "DBL"];
-        // adjacency table
-        var adj = [0x554, 0xaa8, 0x691, 0x962, 0xa45, 0x58a, 0x919, 0x626, 0x469, 0x896, 0x1a5, 0x25a];
-        var used = 0;
-        var face;
-        var ret = "";
-        for (var j = 0; j < len; j++) {
-            do {
-                face = rn(12);
-            } while (((used >> face) & 1) != 0);
-            ret += faces[face] + rndEl(minxsuff) + " ";
-            used &= ~adj[face];
-            used |= 1 << face;
-        }
-        return ret;
-    }
-
-    function utilscramble(type, len) {
-        var ret = "";
-        switch (type) {
-            case "15p": // 15 puzzle
-                return do15puzzle(false, len);
-            case "15pm": // 15 puzzle, mirrored
-                return do15puzzle(true, len);
-            case "clkwca": // Clock (WCA Notation)
-                var clkapp = ["0+", "1+", "2+", "3+", "4+", "5+", "6+", "1-", "2-", "3-", "4-", "5-"];
-                var ret = "UR? DR? DL? UL? U? R? D? L? ALL? y2 U? R? D? L? ALL?????";
-                for (var i = 0; i < 14; i++) {
-                    ret = ret.replace('?', rndEl(clkapp));
-                }
-                return ret.replace('?', rndEl(["", " UR"])).replace('?', rndEl(["", " DR"])).replace('?', rndEl(["", " DL"])).replace('?', rndEl(["", " UL"]));
-            case "clk": // Clock (Jaap order)
-                return "UU" + c("u") + "dU" + c("u") + "dd" + c("u") + "Ud" + c("u") + "dU" + c("u") + "Ud" + c("u") + "UU" + c("u") + "UU" + c("u") + "UU" + c("u") + "dd" + c3() + c2() + "\ndd" + c("d") + "dU" + c("d") + "UU" + c("d") + "Ud" + c("d") + "UU" + c3() + "UU" + c3() + "Ud" + c3() + "dU" + c3() + "UU" + c3() + "dd" + c("d") + c2();
-            case "clkc": // Clock (concise)
-                ret = "";
-                for (var i = 0; i < 4; i++) ret += "(" + (rn(12) - 5) + ", " + (rn(12) - 5) + ") / ";
-                for (var i = 0; i < 6; i++) ret += "(" + (rn(12) - 5) + ") / ";
-                for (var i = 0; i < 4; i++) ret += rndEl(["d", "U"]);
-                return ret;
-            case "clke": // Clock (efficient order)
-                return "UU" + c("u") + "dU" + c("u") + "dU" + c("u") + "UU" + c("u") + "UU" + c("u") + "UU" + c("u") + "Ud" + c("u") + "Ud" + c("u") + "dd" + c("u") + "dd" + c3() + c2() + "\nUU" + c3() + "UU" + c3() + "dU" + c("d") + "dU" + c3() + "dd" + c("d") + "Ud" + c3() + "Ud" + c("d") + "UU" + c3() + "UU" + c("d") + "dd" + c("d") + c2();
-            case "giga": // Gigaminx
-                return gigascramble(len);
-            case "mgmo": // Megaminx (old style)
-                return oldminxscramble(len);
-                break;
-            case "mgmp": // Megaminx (Pochmann)
-                return pochscramble(10, Math.ceil(len / 10));
-            case "mgmc": // Megaminx (Carrot)
-                return carrotscramble(10, Math.ceil(len / 10));
-            case "pyrm": // Pyraminx (random moves)
-                ret = mega([
-                    ["U"],
-                    ["L"],
-                    ["R"],
-                    ["B"]
-                ], ["!", "'"]);
-                var cnt = 0;
-                var rnd = [];
-                for (var i = 0; i < 4; i++) {
-                    rnd[i] = rn(3);
-                    if (rnd[i] > 0) cnt++;
-                }
-                ret = ret.substr(0, ret.length - 3 * cnt);
-                ret = ["", "b ", "b' "][rnd[0]] + ["", "l ", "l' "][rnd[1]] + ["", "u ", "u' "][rnd[2]] + ["", "r ", "r' "][rnd[3]] + ret;
-                return ret.replace(/!/g, "");
-            case "prcp": // Pyraminx Crystal (Pochmann)
-                return pochscramble(10, Math.ceil(len / 10));
-            case "r3": // multiple 3x3x3 relay
-                for (var i = 0; i < len; i++) {
-                    ret += (i == 0 ? "" : "\n") + (i + 1) + ") ${333}";
-                }
-                return scramble.formatScramble(ret);
-            case "sq1h": // Square-1 (turn metric)
-                return sq1_scramble(1);
-            case "sq1t": // Square-1 (twist metric)
-                return sq1_scramble(0);
-            case "sq2": // Square-2
-                var i = 0;
-                while (i < len) {
-                    var rndu = rn(12) - 5;
-                    var rndd = rn(12) - 5;
-                    if (rndu != 0 || rndd != 0) {
-                        i++;
-                        ret += "(" + rndu + "," + rndd + ") / ";
-                    }
-                }
-                return ret;
-            case "ssq1t": // Super Square-1 (twist metric)
-                return ssq1t_scramble(len);
-            case "bsq": // Bandaged Square-1 </,(1,0)>
-                return sq1_scramble(2, len);
-            case "-1": // -1x-1x-1 (micro style)
-                for (var i = 0; i < len; i++) {
-                    ret += String.fromCharCode(32 + rn(224));
-                }
-                ret += "Error: subscript out of range";
-                return ret;
-            case "333noob": // 3x3x3 for noobs
-                ret = mega(SCRAMBLE_NOOBST, SCRAMBLE_NOOBSS.split('|')).replace(/t/, "T");
-                return ret.substr(0, ret.length - 2) + ".";
-            case "lol": // LOL
-                ret = mega([
-                    ["L"],
-                    ["O"]
-                ]);
-                return ret.replace(/ /g, "");
-        }
-        console.log('Error');
-    }
-
-    function getMegaminxWCAScramble(n) {
-        return utilscramble("mgmp", n);
-    }
-
-    function getMegaminxCarrotScramble(n) {
-        return utilscramble("mgmc", n);
-    }
-
-    function getMegaminxOldStyleScramble(n) {
-        return utilscramble("mgmo", n);
-    }
-
-    function getClockWCAScramble() {
-        return utilscramble("clkwca", 0);
-    }
-
-    function getClockJaapScramble() {
-        return utilscramble("clk", 0);
-    }
-
-    function getClockConciseScramble() {
-        return utilscramble("clkc", 0);
-    }
-
-    function getClockEfficientPinOrderScramble() {
-        return utilscramble("clke", 0);
-    }
-
-    function getSquareOneTurnMetricScramble(n) {
-        return sq1_scramble(1, n);
-    }
-
-    function getSquareOneTwistMetricScramble(n) {
-        return sq1_scramble(0, n);
-    }
-
-    return {
-        getMegaminxWCAScramble: getMegaminxWCAScramble,
-        getMegaminxCarrotScramble: getMegaminxCarrotScramble,
-        getMegaminxOldStyleScramble: getMegaminxOldStyleScramble,
-        getSquareOneTurnMetricScramble: getSquareOneTurnMetricScramble,
-        getSquareOneTwistMetricScramble: getSquareOneTwistMetricScramble,
-
-        getClockWCAScramble: getClockWCAScramble,
-        getClockJaapScramble: getClockJaapScramble,
-        getClockConciseScramble: getClockConciseScramble,
-        getClockEfficientPinOrderScramble: getClockEfficientPinOrderScramble,
-    }
-
-
-    //scramble.reg(['15p', '15pm', 'clkwca', 'clk', 'clkc', 'clke', 'giga', 'mgmo', 'mgmp', 'mgmc', 'pyrm', 'prcp', 'r3', 'sq1h', 'sq1t', 'sq2', 'ssq1t', 'bsq', '-1', '333noob', 'lol'], utilscramble);
-
+"use strict";
+
+var util_scramble = (function(rn, rndEl, mega) {
+    var cubesuff = ["", "2", "'"];
+    var minxsuff = ["", "2", "'", "2'"];
+    var seq = [];
+    var p = [];
+
+    function helicubescramble(type, len) {
+        var faces = ["UF", "UR", "UB", "UL", "FR", "BR", "BL", "FL", "DF", "DR", "DB", "DL"];
+        // adjacency table
+        var adj = [0x09a, 0x035, 0x06a, 0x0c5, 0x303, 0x606, 0xc0c, 0x909, 0xa90, 0x530, 0xa60, 0x5c0];
+        var used = 0;
+        var face;
+        var ret = [];
+        for (var j = 0; j < len; j++) {
+            do {
+                face = rn(12);
+            } while (((used >> face) & 1) != 0);
+            ret.push(faces[face]);
+            used &= ~adj[face];
+            used |= 1 << face;
+        }
+        return ret.join(" ");
+    }
+    //scramble.reg('heli', helicubescramble);
+
+    function yj4x4(type, len) {
+        // the idea is to keep the fixed center on U and do Rw or Lw, Fw or Bw, to not disturb it
+        var turns = [
+            ["U", "D"],
+            ["R", "L", "r"],
+            ["F", "B", "f"]
+        ];
+        var donemoves = [];
+        var lastaxis;
+        var fpos = 0; // 0 = Ufr, 1 = Ufl, 2 = Ubl, 3 = Ubr
+        var j, k;
+        var s = "";
+        lastaxis = -1;
+        for (j = 0; j < len; j++) {
+            var done = 0;
+            do {
+                var first = rn(turns.length);
+                var second = rn(turns[first].length);
+                if (first != lastaxis || donemoves[second] == 0) {
+                    if (first == lastaxis) {
+                        donemoves[second] = 1;
+                        var rs = rn(cubesuff.length);
+                        if (first == 0 && second == 0) {
+                            fpos = (fpos + 4 + rs) % 4;
+                        }
+                        if (first == 1 && second == 2) { // r or l
+                            if (fpos == 0 || fpos == 3) s += "l" + cubesuff[rs] + " ";
+                            else s += "r" + cubesuff[rs] + " ";
+                        } else if (first == 2 && second == 2) { // f or b
+                            if (fpos == 0 || fpos == 1) s += "b" + cubesuff[rs] + " ";
+                            else s += "f" + cubesuff[rs] + " ";
+                        } else {
+                            s += turns[first][second] + cubesuff[rs] + " ";
+                        }
+                    } else {
+                        for (k = 0; k < turns[first].length; k++) {
+                            donemoves[k] = 0;
+                        }
+                        lastaxis = first;
+                        donemoves[second] = 1;
+                        var rs = rn(cubesuff.length);
+                        if (first == 0 && second == 0) {
+                            fpos = (fpos + 4 + rs) % 4;
+                        }
+                        if (first == 1 && second == 2) { // r or l
+                            if (fpos == 0 || fpos == 3) s += "l" + cubesuff[rs] + " ";
+                            else s += "r" + cubesuff[rs] + " ";
+                        } else if (first == 2 && second == 2) { // f or b
+                            if (fpos == 0 || fpos == 1) s += "b" + cubesuff[rs] + " ";
+                            else s += "f" + cubesuff[rs] + " ";
+                        } else {
+                            s += turns[first][second] + cubesuff[rs] + " ";
+                        }
+                    }
+                    done = 1;
+                }
+            } while (done == 0);
+        }
+        return s;
+    }
+
+    //scramble.reg('444yj', yj4x4);
+
+    function bicube(type, len) {
+        function canMove(face) {
+            var u = [],
+                i, j, done, z = 0;
+            for (i = 0; i < 9; i++) {
+                done = 0;
+                for (j = 0; j < u.length; j++) {
+                    if (u[j] == start[d[face][i]]) done = 1;
+                }
+                if (done == 0) {
+                    u[u.length] = start[d[face][i]];
+                    if (start[d[face][i]] == 0) z = 1;
+                }
+            }
+            return (u.length == 5 && z == 1);
+        }
+
+        function doMove(face, amount) {
+            for (var i = 0; i < amount; i++) {
+                var t = start[d[face][0]];
+                start[d[face][0]] = start[d[face][6]];
+                start[d[face][6]] = start[d[face][4]];
+                start[d[face][4]] = start[d[face][2]];
+                start[d[face][2]] = t;
+                t = start[d[face][7]];
+                start[d[face][7]] = start[d[face][5]];
+                start[d[face][5]] = start[d[face][3]];
+                start[d[face][3]] = start[d[face][1]];
+                start[d[face][1]] = t;
+            }
+        }
+
+        var d = [
+            [0, 1, 2, 5, 8, 7, 6, 3, 4],
+            [6, 7, 8, 13, 20, 19, 18, 11, 12],
+            [0, 3, 6, 11, 18, 17, 16, 9, 10],
+            [8, 5, 2, 15, 22, 21, 20, 13, 14]
+        ];
+        var start = [1, 1, 2, 3, 3, 2, 4, 4, 0, 5, 6, 7, 8, 9, 10, 10, 5, 6, 7, 8, 9, 11, 11],
+            move = "UFLR",
+            s = "",
+            arr = [],
+            poss, done, i, j, x, y;
+        while (arr.length < len) {
+            poss = [1, 1, 1, 1];
+            for (j = 0; j < 4; j++) {
+                if (poss[j] == 1 && !canMove(j))
+                    poss[j] = 0;
+            }
+            done = 0;
+            while (done == 0) {
+                x = rn(4);
+                if (poss[x] == 1) {
+                    y = rn(3) + 1;
+                    doMove(x, y);
+                    done = 1;
+                }
+            }
+            arr[arr.length] = [x, y];
+            if (arr.length >= 2) {
+                if (arr[arr.length - 1][0] == arr[arr.length - 2][0]) {
+                    arr[arr.length - 2][1] = (arr[arr.length - 2][1] + arr[arr.length - 1][1]) % 4;
+                    arr = arr.slice(0, arr.length - 1);
+                }
+            }
+            if (arr.length >= 1) {
+                if (arr[arr.length - 1][1] == 0) {
+                    arr = arr.slice(0, arr.length - 1);
+                }
+            }
+        }
+        for (i = 0; i < len; i++) {
+            s += move[arr[i][0]] + cubesuff[arr[i][1] - 1] + " ";
+        }
+        return s;
+    }
+
+    //scramble.reg('bic', bicube);
+
+
+
+    // Clock functions.
+    function c(s) {
+        var array = [s + "=0", s + "+1", s + "+2", s + "+3", s + "+4", s + "+5", s + "+6", s + "-5", s + "-4", s + "-3", s + "-2", s + "-1"];
+        return " " + rndEl(array) + " ";
+    }
+
+    function c2() {
+        return rndEl(["U", "d"]) + rndEl(["U", "d"]);
+    }
+
+    function c3() {
+        return "     "
+    }
+
+    function do15puzzle(mirrored, len) {
+        var moves = (mirrored ? ["U", "L", "R", "D"] : ["D", "R", "L", "U"]);
+        var effect = [
+            [0, -1],
+            [1, 0],
+            [-1, 0],
+            [0, 1]
+        ];
+        var x = 0,
+            y = 3,
+            k, done, r, lastr = 5;
+        ret = "";
+        for (k = 0; k < len; k++) {
+            done = false;
+            while (!done) {
+                r = rn(4);
+                if (x + effect[r][0] >= 0 && x + effect[r][0] <= 3 && y + effect[r][1] >= 0 && y + effect[r][1] <= 3 && r + lastr != 3) {
+                    done = true;
+                    x += effect[r][0];
+                    y += effect[r][1];
+                    ret += moves[r] + " ";
+                    lastr = r;
+                }
+            }
+        }
+        return ret;
+    }
+
+    function pochscramble(x, y) {
+        var ret = "";
+        var i, j;
+        for (i = 0; i < y; i++) {
+            ret += "  ";
+            for (j = 0; j < x; j++) {
+                ret += (j % 2 == 0 ? "R" : "D") + rndEl(["++", "--"]) + " ";
+            }
+            ret += "U" + (ret.endsWith("-- ") ? "'\n" : " \n");
+        }
+        return ret;
+    }
+
+    function carrotscramble(x, y) {
+        var ret = "";
+        var i, j;
+        for (i = 0; i < y; i++) {
+            ret += " ";
+            for (j = 0; j < x / 2; j++) {
+                ret += rndEl(["+", "-"]) + rndEl(["+", "-"]) + " ";
+            }
+            ret += "U" + rndEl(["'\n", " \n"]);
+        }
+        return ret;
+    }
+
+    function gigascramble(len) {
+        var ret = "";
+        var i, j;
+        for (i = 0; i < Math.ceil(len / 10); i++) {
+            ret += "  ";
+            for (j = 0; j < 10; j++) {
+                ret += (j % 2 == 0 ? ("Rr".charAt(rn(2))) : ("Dd".charAt(rn(2)))) + rndEl(["+ ", "++", "- ", "--"]) + " ";
+            }
+            ret += "y" + rndEl(minxsuff) + "\n";
+        }
+        return ret;
+    }
+
+    function sq1_scramble(type, len) {
+        seq = [];
+        var i, k;
+        sq1_getseq(1, type, len);
+        var s = "";
+        for (i = 0; i < seq[0].length; i++) {
+            k = seq[0][i];
+            if (k[0] == 7) {
+                s += "/";
+            } else {
+                s += " (" + k[0] + "," + k[1] + ") ";
+            }
+        }
+        return s;
+    }
+
+    function ssq1t_scramble(len) {
+        seq = [];
+        var i;
+        sq1_getseq(2, 0, len);
+        var s = seq[0],
+            t = seq[1],
+            u = "";
+        if (s[0][0] == 7) s = [
+            [0, 0]
+        ].concat(s);
+        if (t[0][0] == 7) t = [
+            [0, 0]
+        ].concat(t);
+        for (i = 0; i < len; i++) {
+            u += "(" + s[2 * i][0] + "," + t[2 * i][0] + "," + t[2 * i][1] + "," + s[2 * i][1] + ") / ";
+        }
+        return u;
+    }
+
+    function sq1_getseq(num, type, len) {
+        for (var n = 0; n < num; n++) {
+            p = [1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0, 0, 1, 0];
+            seq[n] = [];
+            var cnt = 0;
+            while (cnt < len) {
+                var x = rn(12) - 5;
+                var y = (type == 2) ? 0 : rn(12) - 5;
+                var size = (x == 0 ? 0 : 1) + (y == 0 ? 0 : 1);
+                if ((cnt + size <= len || type != 1) && (size > 0 || cnt == 0)) {
+                    if (sq1_domove(x, y)) {
+                        if (type == 1) cnt += size;
+                        if (size > 0) seq[n][seq[n].length] = [x, y];
+                        if (cnt < len || type != 1) {
+                            cnt++;
+                            seq[n][seq[n].length] = [7, 0];
+                            sq1_domove(7, 0);
+                        }
+                    }
+                }
+            }
+        }
+    }
+
+    function sq1_domove(x, y) {
+        var i, px, py;
+        if (x == 7) {
+            for (i = 0; i < 6; i++) {
+                mathlib.circle(p, i + 6, i + 12);
+            }
+            return true;
+        } else {
+            if (p[(17 - x) % 12] || p[(11 - x) % 12] || p[12 + (17 - y) % 12] || p[12 + (11 - y) % 12]) {
+                return false;
+            } else {
+                // do the move itself
+                px = p.slice(0, 12);
+                py = p.slice(12, 24);
+                for (i = 0; i < 12; i++) {
+                    p[i] = px[(12 + i - x) % 12];
+                    p[i + 12] = py[(12 + i - y) % 12];
+                }
+                return true;
+            }
+        }
+    }
+
+    function oldminxscramble(len) {
+        var faces = ["F", "B", "U", "D", "L", "DBR", "DL", "BR", "DR", "BL", "R", "DBL"];
+        // adjacency table
+        var adj = [0x554, 0xaa8, 0x691, 0x962, 0xa45, 0x58a, 0x919, 0x626, 0x469, 0x896, 0x1a5, 0x25a];
+        var used = 0;
+        var face;
+        var ret = "";
+        for (var j = 0; j < len; j++) {
+            do {
+                face = rn(12);
+            } while (((used >> face) & 1) != 0);
+            ret += faces[face] + rndEl(minxsuff) + " ";
+            used &= ~adj[face];
+            used |= 1 << face;
+        }
+        return ret;
+    }
+
+    function utilscramble(type, len) {
+        var ret = "";
+        switch (type) {
+            case "bicube": // BiCube / Meffert's Bandaged Cube
+                return bicube(null, 30);
+            case "15p": // 15 puzzle
+                return do15puzzle(false, len);
+            case "15pm": // 15 puzzle, mirrored
+                return do15puzzle(true, len);
+            case "clkwca": // Clock (WCA Notation)
+                var clkapp = ["0+", "1+", "2+", "3+", "4+", "5+", "6+", "1-", "2-", "3-", "4-", "5-"];
+                var ret = "UR? DR? DL? UL? U? R? D? L? ALL? y2 U? R? D? L? ALL?????";
+                for (var i = 0; i < 14; i++) {
+                    ret = ret.replace('?', rndEl(clkapp));
+                }
+                return ret.replace('?', rndEl(["", " UR"])).replace('?', rndEl(["", " DR"])).replace('?', rndEl(["", " DL"])).replace('?', rndEl(["", " UL"]));
+            case "clk": // Clock (Jaap order)
+                return "UU" + c("u") + "dU" + c("u") + "dd" + c("u") + "Ud" + c("u") + "dU" + c("u") + "Ud" + c("u") + "UU" + c("u") + "UU" + c("u") + "UU" + c("u") + "dd" + c3() + c2() + "\ndd" + c("d") + "dU" + c("d") + "UU" + c("d") + "Ud" + c("d") + "UU" + c3() + "UU" + c3() + "Ud" + c3() + "dU" + c3() + "UU" + c3() + "dd" + c("d") + c2();
+            case "clkc": // Clock (concise)
+                ret = "";
+                for (var i = 0; i < 4; i++) ret += "(" + (rn(12) - 5) + ", " + (rn(12) - 5) + ") / ";
+                for (var i = 0; i < 6; i++) ret += "(" + (rn(12) - 5) + ") / ";
+                for (var i = 0; i < 4; i++) ret += rndEl(["d", "U"]);
+                return ret;
+            case "clke": // Clock (efficient order)
+                return "UU" + c("u") + "dU" + c("u") + "dU" + c("u") + "UU" + c("u") + "UU" + c("u") + "UU" + c("u") + "Ud" + c("u") + "Ud" + c("u") + "dd" + c("u") + "dd" + c3() + c2() + "\nUU" + c3() + "UU" + c3() + "dU" + c("d") + "dU" + c3() + "dd" + c("d") + "Ud" + c3() + "Ud" + c("d") + "UU" + c3() + "UU" + c("d") + "dd" + c("d") + c2();
+            case "giga": // Gigaminx
+                return gigascramble(len);
+            case "mgmo": // Megaminx (old style)
+                return oldminxscramble(len);
+                break;
+            case "mgmp": // Megaminx (Pochmann)
+                return pochscramble(10, Math.ceil(len / 10));
+            case "mgmc": // Megaminx (Carrot)
+                return carrotscramble(10, Math.ceil(len / 10));
+            case "pyrm": // Pyraminx (random moves)
+                ret = mega([
+                    ["U"],
+                    ["L"],
+                    ["R"],
+                    ["B"]
+                ], ["!", "'"]);
+                var cnt = 0;
+                var rnd = [];
+                for (var i = 0; i < 4; i++) {
+                    rnd[i] = rn(3);
+                    if (rnd[i] > 0) cnt++;
+                }
+                ret = ret.substr(0, ret.length - 3 * cnt);
+                ret = ["", "b ", "b' "][rnd[0]] + ["", "l ", "l' "][rnd[1]] + ["", "u ", "u' "][rnd[2]] + ["", "r ", "r' "][rnd[3]] + ret;
+                return ret.replace(/!/g, "");
+            case "prcp": // Pyraminx Crystal (Pochmann)
+                return pochscramble(10, Math.ceil(len / 10));
+            case "r3": // multiple 3x3x3 relay
+                for (var i = 0; i < len; i++) {
+                    ret += (i == 0 ? "" : "\n") + (i + 1) + ") ${333}";
+                }
+                return scramble.formatScramble(ret);
+            case "sq1h": // Square-1 (turn metric)
+                return sq1_scramble(1);
+            case "sq1t": // Square-1 (twist metric)
+                return sq1_scramble(0);
+            case "sq2": // Square-2
+                var i = 0;
+                while (i < len) {
+                    var rndu = rn(12) - 5;
+                    var rndd = rn(12) - 5;
+                    if (rndu != 0 || rndd != 0) {
+                        i++;
+                        ret += "(" + rndu + "," + rndd + ") / ";
+                    }
+                }
+                return ret;
+            case "ssq1t": // Super Square-1 (twist metric)
+                return ssq1t_scramble(len);
+            case "bsq": // Bandaged Square-1 </,(1,0)>
+                return sq1_scramble(2, len);
+            case "-1": // -1x-1x-1 (micro style)
+                for (var i = 0; i < len; i++) {
+                    ret += String.fromCharCode(32 + rn(224));
+                }
+                ret += "Error: subscript out of range";
+                return ret;
+            case "333noob": // 3x3x3 for noobs
+                ret = mega(SCRAMBLE_NOOBST, SCRAMBLE_NOOBSS.split('|')).replace(/t/, "T");
+                return ret.substr(0, ret.length - 2) + ".";
+            case "lol": // LOL
+                ret = mega([
+                    ["L"],
+                    ["O"]
+                ]);
+                return ret.replace(/ /g, "");
+        }
+        console.log('Error');
+    }
+
+    function getBicubeScramble() {
+        return utilscramble('bicube', 30);
+    }
+
+    function getMegaminxWCAScramble(n) {
+        return utilscramble("mgmp", n);
+    }
+
+    function getMegaminxCarrotScramble(n) {
+        return utilscramble("mgmc", n);
+    }
+
+    function getMegaminxOldStyleScramble(n) {
+        return utilscramble("mgmo", n);
+    }
+
+    function getClockWCAScramble() {
+        return utilscramble("clkwca", 0);
+    }
+
+    function getClockJaapScramble() {
+        return utilscramble("clk", 0);
+    }
+
+    function getClockConciseScramble() {
+        return utilscramble("clkc", 0);
+    }
+
+    function getClockEfficientPinOrderScramble() {
+        return utilscramble("clke", 0);
+    }
+
+    function getSquareOneTurnMetricScramble(n) {
+        return sq1_scramble(1, n);
+    }
+
+    function getSquareOneTwistMetricScramble(n) {
+        return sq1_scramble(0, n);
+    }
+
+    return {
+        getBicubeScramble: getBicubeScramble,
+        getMegaminxWCAScramble: getMegaminxWCAScramble,
+        getMegaminxCarrotScramble: getMegaminxCarrotScramble,
+        getMegaminxOldStyleScramble: getMegaminxOldStyleScramble,
+        getSquareOneTurnMetricScramble: getSquareOneTurnMetricScramble,
+        getSquareOneTwistMetricScramble: getSquareOneTwistMetricScramble,
+
+        getClockWCAScramble: getClockWCAScramble,
+        getClockJaapScramble: getClockJaapScramble,
+        getClockConciseScramble: getClockConciseScramble,
+        getClockEfficientPinOrderScramble: getClockEfficientPinOrderScramble,
+    }
+
+
+    //scramble.reg(['15p', '15pm', 'clkwca', 'clk', 'clkc', 'clke', 'giga', 'mgmo', 'mgmp', 'mgmc', 'pyrm', 'prcp', 'r3', 'sq1h', 'sq1t', 'sq2', 'ssq1t', 'bsq', '-1', '333noob', 'lol'], utilscramble);
+
 })(mathlib.rn, mathlib.rndEl, scramble.mega);
```

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/megaminxScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/megaminxScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/rexScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/rexScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler222.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/scrambler222.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler333.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/scrambler333.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler444.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/scrambler444.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler555.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/scrambler555.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler666.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/scrambler666.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/scrambler777.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/scrambler777.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler/squareOneScrambler.py` & `pytwistyscrambler-1.7/pyTwistyScrambler/squareOneScrambler.py`

 * *Files identical despite different names*

### Comparing `pyTwistyScrambler-1.6/pyTwistyScrambler.egg-info/SOURCES.txt` & `pytwistyscrambler-1.7/pyTwistyScrambler.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pyTwistyScrambler/__init__.py
 pyTwistyScrambler/bigCubesScrambler.py
 pyTwistyScrambler/clockScrambler.py
 pyTwistyScrambler/cuboidsScrambler.py
 pyTwistyScrambler/ftoScrambler.py
 pyTwistyScrambler/megaminxScrambler.py
+pyTwistyScrambler/miscScrambler.py
 pyTwistyScrambler/pyraminxScrambler.py
 pyTwistyScrambler/rexScrambler.py
 pyTwistyScrambler/scrambler222.py
 pyTwistyScrambler/scrambler333.py
 pyTwistyScrambler/scrambler444.py
 pyTwistyScrambler/scrambler555.py
 pyTwistyScrambler/scrambler666.py
```

### Comparing `pyTwistyScrambler-1.6/setup.py` & `pytwistyscrambler-1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyTwistyScrambler",
-    version="1.6",
+    version="1.7",
     author="euphwes",
     author_email="euphwes@gmail.com",
     packages=setuptools.find_packages(),
     include_package_data=True,
     description="A Python utility package for generating scrambles for twisty puzzles",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/euphwes/pyTwistyScrambler",
     project_urls={
         "Bug Tracker": "https://github.com/euphwes/pyTwistyScrambler/issues",
     },
     install_requires=[
-        'appdirs',
-        'packaging',
-        'PyExecJS',
-        'pyparsing',
-        'six',
+        "appdirs",
+        "packaging",
+        "PyExecJS",
+        "pyparsing",
+        "six",
     ],
 )
```

