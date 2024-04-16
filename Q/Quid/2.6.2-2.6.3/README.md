# Comparing `tmp/Quid-2.6.2.tar.gz` & `tmp/quid-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quid-2.6.2.tar", last modified: Wed Apr 10 10:38:25 2024, max compression
+gzip compressed data, was "quid-2.6.3.tar", last modified: Tue Apr 16 08:12:25 2024, max compression
```

## Comparing `Quid-2.6.2.tar` & `quid-2.6.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.428470 Quid-2.6.2/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 13:24:44.000000 Quid-2.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6817 2024-04-10 10:38:25.428470 Quid-2.6.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/Quid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6817 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 10:38:25.000000 Quid-2.6.2/Quid.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     5962 2024-04-09 13:52:32.000000 Quid-2.6.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-09 13:24:44.000000 Quid-2.6.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.420470 Quid-2.6.2/quid/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/cli/
--rw-rw-rw-   0 root         (0) root         (0)    29334 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/cli/QuidCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/core/
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/BestMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/InternalMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/InternalMatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)    18157 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/Quid.py
--rw-rw-rw-   0 root         (0) root         (0)    18592 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/QuidMatcher.py
--rw-rw-rw-   0 root         (0) root         (0)    14310 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/QuidMerger.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/Text.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/core/Token.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/helper/
--rw-rw-rw-   0 root         (0) root         (0)     1736 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/helper/Decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1891 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/helper/Loader.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/helper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/match/
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/match/Match.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/match/MatchSpan.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/match/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/passager/
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/AnalyzedWork.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/CitationSource.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/CitationSourceLink.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/Location.py
--rw-rw-rw-   0 root         (0) root         (0)    28856 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/Passager.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/SourceSegment.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetLocation.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetLocationSelection.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetMatch.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetText.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TargetTextLocationLink.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/passager/TextWithMatches.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/passager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 10:38:25.424470 Quid-2.6.2/quid/visualization/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Info.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Markup.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/MarkupSpan.py
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/TargetHtml.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/TargetTextWithContent.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Visualization.py
--rw-rw-rw-   0 root         (0) root         (0)    12916 2024-04-09 13:24:44.000000 Quid-2.6.2/quid/visualization/Visualizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 10:38:10.000000 Quid-2.6.2/quid/visualization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2024-04-10 10:38:25.428470 Quid-2.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 13:24:44.000000 quid-2.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13843 2024-04-16 08:12:25.683282 quid-2.6.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/Quid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13843 2024-04-16 08:12:25.000000 quid-2.6.3/Quid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-04-16 08:12:25.000000 quid-2.6.3/Quid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 08:12:25.000000 quid-2.6.3/Quid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-16 08:12:25.000000 quid-2.6.3/Quid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-16 08:12:25.000000 quid-2.6.3/Quid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-16 08:12:25.000000 quid-2.6.3/Quid.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    12988 2024-04-16 08:05:16.000000 quid-2.6.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-09 13:24:44.000000 quid-2.6.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/cli/
+-rw-rw-rw-   0 root         (0) root         (0)    29820 2024-04-15 07:43:48.000000 quid-2.6.3/quid/cli/QuidCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/core/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/BestMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/InternalMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/InternalMatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)    18157 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/Quid.py
+-rw-rw-rw-   0 root         (0) root         (0)    18592 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/QuidMatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    14310 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/QuidMerger.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/Text.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-09 13:24:44.000000 quid-2.6.3/quid/core/Token.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/helper/
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2024-04-09 13:24:44.000000 quid-2.6.3/quid/helper/Decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2024-04-09 13:24:44.000000 quid-2.6.3/quid/helper/Loader.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/helper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/match/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-09 13:24:44.000000 quid-2.6.3/quid/match/Match.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-04-09 13:24:44.000000 quid-2.6.3/quid/match/MatchSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/match/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/passager/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/AnalyzedWork.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/CitationSource.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/CitationSourceLink.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/Location.py
+-rw-rw-rw-   0 root         (0) root         (0)    28856 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/Passager.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/SourceSegment.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/TargetLocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/TargetLocationSelection.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/TargetMatch.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/TargetText.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/TargetTextLocationLink.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-09 13:24:44.000000 quid-2.6.3/quid/passager/TextWithMatches.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/passager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:12:25.683282 quid-2.6.3/quid/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-15 07:43:48.000000 quid-2.6.3/quid/visualization/Info.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-04-09 13:24:44.000000 quid-2.6.3/quid/visualization/Markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-09 13:24:44.000000 quid-2.6.3/quid/visualization/MarkupSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-09 13:24:44.000000 quid-2.6.3/quid/visualization/TargetHtml.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2024-04-09 13:24:44.000000 quid-2.6.3/quid/visualization/TargetTextWithContent.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-09 13:24:44.000000 quid-2.6.3/quid/visualization/Visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)    12916 2024-04-09 13:24:44.000000 quid-2.6.3/quid/visualization/Visualizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:12:11.000000 quid-2.6.3/quid/visualization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-04-16 08:12:25.687282 quid-2.6.3/setup.cfg
```

### Comparing `Quid-2.6.2/LICENSE` & `quid-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/Quid.egg-info/SOURCES.txt` & `quid-2.6.3/Quid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/cli/QuidCLI.py` & `quid-2.6.3/quid/cli/QuidCLI.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,36 +32,36 @@
 
 class OptionValueCheckAction(Action):
 
     def __call__(self, parser, namespace, values, option_string=None):
 
         if option_string == '--min-match-length':
             if int(values) < 1:
-                parser.error("Minimum value for {0} is 1".format(option_string))
+                parser.error('Minimum value for {0} is 1'.format(option_string))
         elif option_string == '--look-back-limit':
             if int(values) < 0:
-                parser.error("{0} must be positive".format(option_string))
+                parser.error('{0} must be positive'.format(option_string))
         elif option_string == '--look-ahead-limit':
             if int(values) < 0:
-                parser.error("{0} must be positive".format(option_string))
+                parser.error('{0} must be positive'.format(option_string))
         elif option_string == '--max-merge-distance':
             if int(values) < 0:
-                parser.error("{0} must be positive".format(option_string))
+                parser.error('{0} must be positive'.format(option_string))
         elif option_string == '--max-merge-ellipsis-distance':
             if int(values) < 0:
-                parser.error("{0} must be positive".format(option_string))
+                parser.error('{0} must be positive'.format(option_string))
         elif option_string == '--max-num-processes':
             if int(values) <= 0:
-                parser.error("{0} must be greater 0".format(option_string))
+                parser.error('{0} must be greater 0'.format(option_string))
         elif option_string == 'min_levenshtein_distance':
             if float(values) < 0 or float(values) > 1:
-                parser.error("{0} must be between 0 and 1".format(option_string))
+                parser.error('{0} must be between 0 and 1'.format(option_string))
         elif option_string == 'split_length':
             if int(values) <= 0:
-                parser.error("{0} must be greater 0".format(option_string))
+                parser.error('{0} must be greater 0'.format(option_string))
 
         setattr(namespace, self.dest, values)
 
 
 def __json_decoder_target_text(json_input):
     if 'filename' in json_input:
         return TargetText(json_input['my_id'], json_input['filename'], json_input['target_locations'])
@@ -150,15 +150,15 @@
 def __run_compare(source_file_path, target_path, export_text, output_type, csv_sep, min_match_length, look_ahead_limit,
                   look_back_limit, max_merge_distance, max_merge_ellipsis_distance, output_folder_path,
                   num_of_processes, keep_ambiguous_matches, min_levenshtein_similarity,
                   min_levenshtein_similarity_short, max_length_short_token, split_long_texts, split_length):
     with open(source_file_path, 'r', encoding='utf-8') as source_file:
         source_file_content = source_file.read()
 
-    if isfile(target_path) and target_path.endswith(".txt"):
+    if isfile(target_path) and target_path.endswith('.txt'):
         with open(target_path, 'r', encoding='utf-8') as target_file:
             target_file_content = target_file.read()
 
         filename = splitext(basename(target_path))[0]
 
         __process_file(source_file_content, target_file_content, export_text, output_type, csv_sep, min_match_length,
                        look_ahead_limit, look_back_limit, max_merge_distance, max_merge_ellipsis_distance,
@@ -178,15 +178,15 @@
         logging.info(f'\n--- Runtime prepare source: {end_time - start_time: .2f} seconds ---')
 
         pool = multiprocessing.Pool(num_of_processes)
 
         for file_or_folder in listdir(target_path):
             full_path = join(target_path, file_or_folder)
 
-            if isfile(full_path) and full_path.endswith(".txt"):
+            if isfile(full_path) and full_path.endswith('.txt'):
                 with open(full_path, 'r', encoding='utf-8') as target_file:
                     target_file_content = target_file.read()
 
                 filename = splitext(basename(full_path))[0]
                 pool.apply_async(__process_file, args=(source_file_content, target_file_content, export_text,
                                                        output_type, csv_sep, min_match_length, look_ahead_limit,
                                                        look_back_limit, max_merge_distance,
@@ -367,134 +367,140 @@
 
     with open(join(output_folder_path, 'target_texts.json'), 'w', encoding='utf-8') as target_texts_output_file:
         content = json.dumps(target_texts, default=__json_encoder_visualization)
         target_texts_output_file.write(content)
 
 
 def main(argv=None):
-    compare_description = "Quid compare allows the user to find quotations in two texts, a source text and a target " \
-                          "text. If known, the source text should be the one that is quoted by the target text. " \
-                          "This allows the algorithm to handle things like ellipsis in quotations."
+    compare_description = 'Quid compare allows the user to find quotations in two texts, a source text and a target ' \
+                          'text. If known, the source text should be the one that is quoted by the target text. ' \
+                          'This allows the algorithm to handle things like ellipsis in quotations.'
 
-    argument_parser = ArgumentParser(prog='quid', description="Quid is a tool to find quotations in texts and to"
-                                                              " visualize the matching segments.")
+    argument_parser = ArgumentParser(prog='quid', description='Quid is a tool to find quotations in texts and to'
+                                                              ' visualize the matching segments.')
 
-    argument_parser.add_argument("--log-level", dest="log_level", choices=['DEBUG', 'INFO', 'WARNING', 'ERROR',
+    argument_parser.add_argument('--log-level', dest='log_level', choices=['DEBUG', 'INFO', 'WARNING', 'ERROR',
                                                                            'CRITICAL'],
-                                 help="Set the logging level", default="WARNING")
+                                 help='Set the logging level (default: %(default)s)', default='WARNING')
 
     subparsers = argument_parser.add_subparsers(dest='command')
     subparsers.required = True
 
     parser_compare = subparsers.add_parser('compare', help=compare_description, description=compare_description)
 
-    parser_compare.add_argument("source_file_path", nargs=1, metavar="source-file-path",
-                                help="Path to the source text file")
-    parser_compare.add_argument("target_path", nargs=1, metavar="target-path",
-                                help="Path to the target text file or folder")
-    parser_compare.add_argument('--text', dest="export_text", default=True, action=BooleanOptionalAction,
-                                help="Include matched text in the returned data structure")
-    parser_compare.add_argument('--output-type', choices=['json', 'text', 'csv'], dest="output_type", default="json",
-                                help="The output type")
-    parser_compare.add_argument('--csv-sep', dest='csv_sep', type=str, help="output separator for csv (default: '\\t')",
-                                default='\t')
-    parser_compare.add_argument('--output-folder-path', dest="output_folder_path",
-                                help="The output folder path. If this option is set the output will be saved to a file"
-                                     " created in the specified folder")
-    parser_compare.add_argument('--min-match-length', dest="min_match_length", action=OptionValueCheckAction,
-                                default=5, type=int, help="The minimum number of tokens a match needs to have"
-                                                          " (>= 1, default: 5)")
-    parser_compare.add_argument('--look-back-limit', dest="look_back_limit", action=OptionValueCheckAction,
-                                default=10, type=int, help="The maximum number of tokens to skip when extending a match"
-                                                           " backwards (>= 0, default: 10)")
-    parser_compare.add_argument('--look-ahead-limit', dest="look_ahead_limit", action=OptionValueCheckAction,
-                                default=3, type=int, help="The maximum number of tokens to skip when extending a match"
-                                                          " forwards (>= 0, default: 3)")
-    parser_compare.add_argument('--max-merge-distance', dest="max_merge_distance", action=OptionValueCheckAction,
-                                default=2, type=int, help="The maximum distance in tokens between two matches"
-                                                          " considered for merging (>= 0, default: 2)")
-    parser_compare.add_argument('--max-merge-ellipsis-distance', dest="max_merge_ellipsis_distance",
+    parser_compare.add_argument('source_file_path', nargs=1, metavar='source-file-path',
+                                help='Path to the source text file')
+    parser_compare.add_argument('target_path', nargs=1, metavar='target-path',
+                                help='Path to the target text file or folder')
+    parser_compare.add_argument('--text', dest='export_text', default=True, action=BooleanOptionalAction,
+                                help='Include matched text in the returned data structure')
+    parser_compare.add_argument('--output-type', choices=['json', 'text', 'csv'], dest='output_type',
+                                default='json', help='The output type (default: %(default)s)')
+    parser_compare.add_argument('--csv-sep', dest='csv_sep', type=str,
+                                help='output separator for csv (default: %(default)s)', default='\t')
+    parser_compare.add_argument('--output-folder-path', dest='output_folder_path',
+                                help='The output folder path. If this option is set the output will be saved to a file'
+                                     ' created in the specified folder')
+    parser_compare.add_argument('--min-match-length', dest='min_match_length', action=OptionValueCheckAction,
+                                default=5, type=int, help='The minimum number of tokens a match needs to have'
+                                                          ' (>= 1, default: %(default)d)')
+    parser_compare.add_argument('--look-back-limit', dest='look_back_limit', action=OptionValueCheckAction,
+                                default=10, type=int, help='The maximum number of tokens to skip when extending a match'
+                                                           ' backwards (>= 0, default: %(default)d)')
+    parser_compare.add_argument('--look-ahead-limit', dest='look_ahead_limit', action=OptionValueCheckAction,
+                                default=3, type=int, help='The maximum number of tokens to skip when extending a match'
+                                                          ' forwards (>= 0, (default: %(default)d)')
+    parser_compare.add_argument('--max-merge-distance', dest='max_merge_distance', action=OptionValueCheckAction,
+                                default=2, type=int, help='The maximum distance in tokens between two matches'
+                                                          ' considered for merging (>= 0, default: %(default)d)')
+    parser_compare.add_argument('--max-merge-ellipsis-distance', dest='max_merge_ellipsis_distance',
                                 action=OptionValueCheckAction, default=10, type=int,
-                                help="The maximum distance in tokens between two matches considered for merging where"
-                                     " the target text contains an ellipsis between the matches (>= 0, default: 10)")
-    parser_compare.add_argument('--create-dated-subfolder', dest="create_dated_subfolder", default=False,
+                                help='The maximum distance in tokens between two matches considered for merging where'
+                                     ' the target text contains an ellipsis between the matches (>= 0,'
+                                     ' default: %(default)d)')
+    parser_compare.add_argument('--create-dated-subfolder', dest='create_dated_subfolder', default=False,
                                 action=BooleanOptionalAction,
-                                help="Create a subfolder named with the current date to store the results")
-    parser_compare.add_argument('--max-num-processes', dest="max_num_processes", action=OptionValueCheckAction,
-                                default=1, type=int, help="Maximum number of processes to use for parallel processing")
-    parser_compare.add_argument('--keep-ambiguous-matches', dest="keep_ambiguous_matches", default=False,
-                                action=BooleanOptionalAction, help="For a match with multiple matched segments in the"
-                                                                   " source text, multiple matches will be returned.")
-    parser_compare.add_argument('--min-levenshtein-similarity', dest="min_levenshtein_similarity",
+                                help='Create a subfolder named with the current date to store the results')
+    parser_compare.add_argument('--max-num-processes', dest='max_num_processes', action=OptionValueCheckAction,
+                                default=1, type=int, help='Maximum number of processes to use for parallel processing'
+                                                          ' (default: %(default)d)')
+    parser_compare.add_argument('--keep-ambiguous-matches', dest='keep_ambiguous_matches', default=False,
+                                action=BooleanOptionalAction, help='For a match with multiple matched segments in the'
+                                                                   ' source text, multiple matches will be returned.')
+    parser_compare.add_argument('--min-levenshtein-similarity', dest='min_levenshtein_similarity',
                                 action=OptionValueCheckAction, default=0.85, type=float,
-                                help="The threshold for the minimal levenshtein similarity between tokens and the"
-                                     " initial n-grams to be accepted as a match (between 0 and 1, default: 0.85)")
-    parser_compare.add_argument('--min-levenshtein-similarity-short', dest="min_levenshtein_similarity_short",
+                                help='The threshold for the minimal levenshtein similarity between tokens and the'
+                                     ' initial n-grams to be accepted as a match (between 0 and 1,'
+                                     ' default: %(default).2f)')
+    parser_compare.add_argument('--min-levenshtein-similarity-short', dest='min_levenshtein_similarity_short',
                                 action=OptionValueCheckAction, default=0.85, type=float,
-                                help="The threshold for the minimal levenshtein similarity between short tokens"
-                                     " (as set by --max-length-short-token) and the initial n-grams to be accepted as a"
-                                     " match (between 0 and 1, default: 0.85)")
-    parser_compare.add_argument('--max-length-short-token', dest="max_length_short_token",
+                                help='The threshold for the minimal levenshtein similarity between short tokens'
+                                     ' (as set by --max-length-short-token) and the initial n-grams to be accepted as a'
+                                     ' match (between 0 and 1, default: %(default).2f)')
+    parser_compare.add_argument('--max-length-short-token', dest='max_length_short_token',
                                 action=OptionValueCheckAction, default=10, type=int,
-                                help="The maximum length in characters of a token to be considered short"
-                                     " (>= 0, default: 10)")
-    parser_compare.add_argument('--split-long-texts', dest="split_long_texts", default=False,
-                                action=BooleanOptionalAction, help="Split texts longer than split-length words for"
-                                                                   " faster processing")
-    parser_compare.add_argument('--split-length', dest="split_length", action=OptionValueCheckAction,
-                                default=30000, type=int, help="If split-long-texts is set to True, texts longer (in"
-                                                              " number of words) than this threshold will be split for"
-                                                              " faster processing.")
+                                help='The maximum length in characters of a token to be considered short'
+                                     ' (>= 0, default: %(default)d)')
+    parser_compare.add_argument('--split-long-texts', dest='split_long_texts', default=False,
+                                action=BooleanOptionalAction, help='Split texts longer than split-length words for'
+                                                                   ' faster processing')
+    parser_compare.add_argument('--split-length', dest='split_length', action=OptionValueCheckAction,
+                                default=30000, type=int, help='If split-long-texts is set to True, texts longer (in'
+                                                              ' number of words) than this threshold will be split for'
+                                                              ' faster processing (default: %(default)d)')
 
     passage_description = 'Quid passage allows the user to extract key passages from the found matches.'
 
     parser_passage = subparsers.add_parser('passage', help=passage_description, description=passage_description)
 
-    parser_passage.add_argument("source_file_path", nargs=1, metavar="source-file-path",
-                                help="Path to the source text file")
-    parser_passage.add_argument("target_folder_path", nargs=1, metavar="target-folder-path",
-                                help="Path to the target texts folder path")
-    parser_passage.add_argument("matches_folder_path", nargs=1, metavar="matches-folder-path",
-                                help="Path to the folder with the match files, i.e. the results from quid compare")
-    parser_passage.add_argument("output_folder_path", nargs=1, metavar="output-folder-path",
-                                help="Path to the output folder")
+    parser_passage.add_argument('source_file_path', nargs=1, metavar='source-file-path',
+                                help='Path to the source text file')
+    parser_passage.add_argument('target_folder_path', nargs=1, metavar='target-folder-path',
+                                help='Path to the target texts folder path')
+    parser_passage.add_argument('matches_folder_path', nargs=1, metavar='matches-folder-path',
+                                help='Path to the folder with the match files, i.e. the results from quid compare')
+    parser_passage.add_argument('output_folder_path', nargs=1, metavar='output-folder-path',
+                                help='Path to the output folder')
 
     parser_visualize = subparsers.add_parser('visualize',
-                                             help="Quid visualize allows the user to create the files needed"
-                                                  " for a website that visualizes the quid algorithm results.",
-                                             description="Quid visualize allows the user to create the files needed"
-                                                         " for a website that visualizes the quid algorithm results.")
-
-    parser_visualize.add_argument("source_file_path", nargs=1, metavar="source-file-path",
-                                  help="Path to the source text file")
-    parser_visualize.add_argument("target_folder_path", nargs=1, metavar="target-folder-path",
-                                  help="Path to the target texts folder path")
-    parser_visualize.add_argument("passages_folder_path", nargs=1, metavar="passages-folder-path",
-                                  help="Path to the folder with the key passages files, i.e. the resulting files from"
-                                       " quid passage")
-    parser_visualize.add_argument("output_folder_path", nargs=1, metavar="output-folder-path",
-                                  help="Path to the output folder")
-    parser_visualize.add_argument("--markup-file-path", dest="markup_file_path", help="Path to the markup file")
-    parser_visualize.add_argument("--title", dest="title", help="Title of the work", default="NN")
-    parser_visualize.add_argument("--author", dest="author", help="Author of the work", default="NN")
-    parser_visualize.add_argument("--year", dest="year", help="Year of the work", default="0", type=int)
-    parser_visualize.add_argument('--censor', dest="censor", default=False, action=BooleanOptionalAction,
-                                  help="Censor scholarly works to prevent copyright violations")
+                                             help='Quid visualize allows the user to create the files needed'
+                                                  ' for a website that visualizes the quid algorithm results.',
+                                             description='Quid visualize allows the user to create the files needed'
+                                                         ' for a website that visualizes the quid algorithm results.')
+
+    parser_visualize.add_argument('source_file_path', nargs=1, metavar='source-file-path',
+                                  help='Path to the source text file')
+    parser_visualize.add_argument('target_folder_path', nargs=1, metavar='target-folder-path',
+                                  help='Path to the target texts folder path')
+    parser_visualize.add_argument('passages_folder_path', nargs=1, metavar='passages-folder-path',
+                                  help='Path to the folder with the key passages files, i.e. the resulting files from'
+                                       ' quid passage')
+    parser_visualize.add_argument('output_folder_path', nargs=1, metavar='output-folder-path',
+                                  help='Path to the output folder')
+    parser_visualize.add_argument('--markup-file-path', dest='markup_file_path', help='Path to the markup file')
+    parser_visualize.add_argument('--title', dest='title', help='Title of the work (default: %(default)s)',
+                                  default='NN')
+    parser_visualize.add_argument('--author', dest='author', help='Author of the work (default: %(default)s)',
+                                  default='NN')
+    parser_visualize.add_argument('--year', dest='year', help='Year of the work (default: %(default)d)',
+                                  default=1900, type=int)
+    parser_visualize.add_argument('--censor', dest='censor', default=False, action=BooleanOptionalAction,
+                                  help='Censor scholarly works to prevent copyright violations')
 
     args = argument_parser.parse_args(argv)
 
     log_level = args.log_level
     logging.getLogger().setLevel(logging.getLevelName(log_level))
 
     if args.command == 'compare':
         source_path = args.source_file_path[0]
         target_path = args.target_path[0]
         export_text = args.export_text
         output_type = args.output_type
-        csv_sep = bytes(args.csv_sep, "utf-8").decode("unicode_escape")
+        csv_sep = bytes(args.csv_sep, 'utf-8').decode('unicode_escape')
         output_folder_path = args.output_folder_path
         min_match_length = args.min_match_length
         look_ahead_limit = args.look_ahead_limit
         look_back_limit = args.look_back_limit
         max_merge_distance = args.max_merge_distance
         max_merge_ellipsis_distance = args.max_merge_ellipsis_distance
         create_dated_subfolder = args.create_dated_subfolder
@@ -508,15 +514,15 @@
 
         if output_folder_path:
             if not exists(output_folder_path):
                 raise FileNotFoundError(f'{output_folder_path} does not exist!')
 
             if create_dated_subfolder:
                 now = datetime.now()
-                date_time_string = now.strftime("%Y_%m_%d_%H_%M_%S")
+                date_time_string = now.strftime('%Y_%m_%d_%H_%M_%S')
                 output_folder_path = join(args.output_folder_path, date_time_string)
                 Path(output_folder_path).mkdir(parents=True, exist_ok=True)
 
         start_time = time.perf_counter()
 
         __run_compare(source_path, target_path, export_text, output_type, csv_sep, min_match_length, look_ahead_limit,
                       look_back_limit, max_merge_distance, max_merge_ellipsis_distance, output_folder_path,
```

### Comparing `Quid-2.6.2/quid/core/Quid.py` & `quid-2.6.3/quid/core/Quid.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/core/QuidMatcher.py` & `quid-2.6.3/quid/core/QuidMatcher.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/core/QuidMerger.py` & `quid-2.6.3/quid/core/QuidMerger.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/helper/Decoder.py` & `quid-2.6.3/quid/helper/Decoder.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/helper/Loader.py` & `quid-2.6.3/quid/helper/Loader.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/passager/AnalyzedWork.py` & `quid-2.6.3/quid/passager/AnalyzedWork.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/passager/CitationSource.py` & `quid-2.6.3/quid/passager/CitationSource.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/passager/Passager.py` & `quid-2.6.3/quid/passager/Passager.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/passager/SourceSegment.py` & `quid-2.6.3/quid/passager/SourceSegment.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/passager/TargetText.py` & `quid-2.6.3/quid/passager/TargetText.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/quid/visualization/Visualizer.py` & `quid-2.6.3/quid/visualization/Visualizer.py`

 * *Files identical despite different names*

### Comparing `Quid-2.6.2/setup.cfg` & `quid-2.6.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Quid
-version = 2.6.2
+version = 2.6.3
 author = Frederik Arnold
 author_email = frederik.arnold@hu-berlin.de
 description = Quid is a tool for quotation detection in texts and can deal with common properties of quotations, for example, ellipses or inaccurate quotations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = quotation detection, quotation identification, literal citation extraction, key passages, natural language processing, nlp, text reuse
 url = https://hu.berlin/quid
```

