# Comparing `tmp/labgym-2.4.3.tar.gz` & `tmp/labgym-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labgym-2.4.3.tar", last modified: Thu Apr 11 06:01:11 2024, max compression
+gzip compressed data, was "labgym-2.4.4.tar", last modified: Tue Apr 16 02:19:47 2024, max compression
```

## Comparing `labgym-2.4.3.tar` & `labgym-2.4.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    31919 2024-04-11 06:01:06.448275 labgym-2.4.3/LICENSE.txt
--rw-r--r--   0        0        0      417 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/COPYRIGHT.txt
--rw-r--r--   0        0        0      131 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/NOTICE.txt
--rw-r--r--   0        0        0      882 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/__main__.py
--rw-r--r--   0        0        0    87666 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/analyzebehaviors.py
--rw-r--r--   0        0        0   173802 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/analyzebehaviorsdetector.py
--rw-r--r--   0        0        0    68079 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/categorizers.py
--rw-r--r--   0        0        0    12995 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/detector.py
--rw-r--r--   0        0        0      859 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/detectors/__init__.py
--rw-r--r--   0        0        0      889 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/__init__.py
--rw-r--r--   0        0        0      904 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/__init__.py
--rw-r--r--   0        0        0     2115 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/analysis_module.py
--rw-r--r--   0        0        0    67941 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/analyze_behaviors.py
--rw-r--r--   0        0        0     7276 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/behavior_plot.py
--rw-r--r--   0        0        0     9322 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/analysis/mine_results.py
--rw-r--r--   0        0        0     4833 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/main_window.py
--rw-r--r--   0        0        0    22593 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/preprocessing.py
--rw-r--r--   0        0        0      904 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/__init__.py
--rw-r--r--   0        0        0    51881 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/behavior_examples.py
--rw-r--r--   0        0        0    33348 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/categorizers.py
--rw-r--r--   0        0        0    22307 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/detectors.py
--rw-r--r--   0        0        0     5203 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/training/training_module.py
--rw-r--r--   0        0        0     4473 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/gui/utils.py
--rw-r--r--   0        0        0     8091 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/minedata.py
--rw-r--r--   0        0        0      859 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/models/__init__.py
--rw-r--r--   0        0        0    49154 2024-04-11 06:01:06.452275 labgym-2.4.3/LabGym/tools.py
--rw-r--r--   0        0        0      131 2024-04-11 06:01:06.452275 labgym-2.4.3/NOTICE.txt
--rw-r--r--   0        0        0    13320 2024-04-11 06:01:06.452275 labgym-2.4.3/README.md
--rw-r--r--   0        0        0     2164 2024-04-11 06:01:11.084287 labgym-2.4.3/pyproject.toml
--rw-r--r--   0        0        0      859 2024-04-11 06:01:06.460275 labgym-2.4.3/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-11 06:01:06.460275 labgym-2.4.3/tests/test_main.py
--rw-r--r--   0        0        0     1093 2024-04-11 06:01:06.460275 labgym-2.4.3/tests/test_tools.py
--rw-r--r--   0        0        0    14864 1970-01-01 00:00:00.000000 labgym-2.4.3/PKG-INFO
+-rw-r--r--   0        0        0    31919 2024-04-16 02:19:42.956648 labgym-2.4.4/LICENSE.txt
+-rw-r--r--   0        0        0      417 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/COPYRIGHT.txt
+-rw-r--r--   0        0        0      131 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/NOTICE.txt
+-rw-r--r--   0        0        0      882 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/__main__.py
+-rw-r--r--   0        0        0    87666 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/analyzebehaviors.py
+-rw-r--r--   0        0        0   173802 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/analyzebehaviorsdetector.py
+-rw-r--r--   0        0        0    68079 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/categorizers.py
+-rw-r--r--   0        0        0    13019 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/detector.py
+-rw-r--r--   0        0        0      859 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/detectors/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/__init__.py
+-rw-r--r--   0        0        0     2115 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/analysis_module.py
+-rw-r--r--   0        0        0    67907 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/analyze_behaviors.py
+-rw-r--r--   0        0        0     7276 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/behavior_plot.py
+-rw-r--r--   0        0        0     9322 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/analysis/mine_results.py
+-rw-r--r--   0        0        0     4833 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/main_window.py
+-rw-r--r--   0        0        0    22593 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/preprocessing.py
+-rw-r--r--   0        0        0      904 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/__init__.py
+-rw-r--r--   0        0        0    51881 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/behavior_examples.py
+-rw-r--r--   0        0        0    33348 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/categorizers.py
+-rw-r--r--   0        0        0    22300 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/detectors.py
+-rw-r--r--   0        0        0     5203 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/training/training_module.py
+-rw-r--r--   0        0        0     4473 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/gui/utils.py
+-rw-r--r--   0        0        0     8091 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/minedata.py
+-rw-r--r--   0        0        0      859 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/models/__init__.py
+-rw-r--r--   0        0        0    49154 2024-04-16 02:19:42.960648 labgym-2.4.4/LabGym/tools.py
+-rw-r--r--   0        0        0      131 2024-04-16 02:19:42.960648 labgym-2.4.4/NOTICE.txt
+-rw-r--r--   0        0        0    13320 2024-04-16 02:19:42.960648 labgym-2.4.4/README.md
+-rw-r--r--   0        0        0     2172 2024-04-16 02:19:47.984604 labgym-2.4.4/pyproject.toml
+-rw-r--r--   0        0        0      859 2024-04-16 02:19:42.968648 labgym-2.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-16 02:19:42.968648 labgym-2.4.4/tests/test_main.py
+-rw-r--r--   0        0        0     1093 2024-04-16 02:19:42.968648 labgym-2.4.4/tests/test_tools.py
+-rw-r--r--   0        0        0    14874 1970-01-01 00:00:00.000000 labgym-2.4.4/PKG-INFO
```

### Comparing `labgym-2.4.3/LICENSE.txt` & `labgym-2.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/__init__.py` & `labgym-2.4.4/LabGym/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 210 Washtenaw Avenue, Room 5403
 Ann Arbor, MI 48109-2216
 USA
 
 Email: bingye@umich.edu
 """
 
-__version__ = "2.4.3"
+__version__ = "2.4.4"
```

### Comparing `labgym-2.4.3/LabGym/__main__.py` & `labgym-2.4.4/LabGym/__main__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/analyzebehaviors.py` & `labgym-2.4.4/LabGym/analyzebehaviors.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/analyzebehaviorsdetector.py` & `labgym-2.4.4/LabGym/analyzebehaviorsdetector.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/categorizers.py` & `labgym-2.4.4/LabGym/categorizers.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/detector.py` & `labgym-2.4.4/LabGym/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,17 +289,17 @@
 
     def delete(self) -> None:
         """Permanently delete this detector."""
         shutil.rmtree(str(self.path))
 
 
 def get_detector_names() -> list[str]:
-    """Return the names of all saved detectors."""
+    """Return the names of all saved detectors in sorted order."""
     ignore = ["__pycache__", "__init__", "__init.py__"]
-    return [path.name for path in DETECTOR_FOLDER.glob("*") if path.is_dir() and path.name not in ignore]
+    return sorted([path.name for path in DETECTOR_FOLDER.glob("*") if path.is_dir() and path.name not in ignore])
 
 
 def get_annotation_class_names(annotation_path: str) -> list[str]:
     """Return a list of class names associated with the annotation file.
 
     Args:
         annotation_path: The absolute path to the COCO annotation file.
```

### Comparing `labgym-2.4.3/LabGym/detectors/__init__.py` & `labgym-2.4.4/LabGym/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/__init__.py` & `labgym-2.4.4/LabGym/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/analysis/__init__.py` & `labgym-2.4.4/LabGym/gui/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/analysis/analysis_module.py` & `labgym-2.4.4/LabGym/gui/analysis/analysis_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/analysis/analyze_behaviors.py` & `labgym-2.4.4/LabGym/gui/analysis/analyze_behaviors.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
             self.text_outputfolder.SetLabel("Results will be in: " + self.result_path + ".")
         dialog.Destroy()
 
     def select_method(self, event):
         if self.behavior_mode <= 1:
             methods = [
                 "Use trained Detectors (versatile but slow)",
-                "Subtract background (fast but requires static background & stable illumination)", 
+                "Subtract background (fast but requires static background & stable illumination)",
             ]
         else:
             methods = ["Use trained Detectors (versatile but slow)"]
 
         dialog = wx.SingleChoiceDialog(
             self,
             message="How to detect the animals?",
@@ -608,15 +608,14 @@
                 dialog1.Destroy()
 
             else:
                 self.use_detector = True
                 self.animal_number = {}
 
                 detectors = get_detector_names()
-                detectors.sort()
                 if "Choose a new directory of the Detector" not in detectors:
                     detectors.append("Choose a new directory of the Detector")
 
                 dialog1 = wx.SingleChoiceDialog(
                     self,
                     message="Select a Detector for animal detection",
                     caption="Select a Detector",
```

### Comparing `labgym-2.4.3/LabGym/gui/analysis/behavior_plot.py` & `labgym-2.4.4/LabGym/gui/analysis/behavior_plot.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/analysis/mine_results.py` & `labgym-2.4.4/LabGym/gui/analysis/mine_results.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/main_window.py` & `labgym-2.4.4/LabGym/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/preprocessing.py` & `labgym-2.4.4/LabGym/gui/preprocessing.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/training/__init__.py` & `labgym-2.4.4/LabGym/gui/training/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/training/behavior_examples.py` & `labgym-2.4.4/LabGym/gui/training/behavior_examples.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/training/categorizers.py` & `labgym-2.4.4/LabGym/gui/training/categorizers.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/training/detectors.py` & `labgym-2.4.4/LabGym/gui/training/detectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,15 +542,15 @@
 
     def delete_detector(self, event):
         """Delete a Detector."""
         dialog = wx.SingleChoiceDialog(
             self,
             message="Select a Detector to delete",
             caption="Delete a Detector",
-            choices=get_detector_names().sort(),
+            choices=get_detector_names(),
         )
         if dialog.ShowModal() != wx.ID_OK:
             dialog.Destroy()
             return
 
         detector = Detector(name=dialog.GetStringSelection())
         confirm = wx.MessageDialog(
```

### Comparing `labgym-2.4.3/LabGym/gui/training/training_module.py` & `labgym-2.4.4/LabGym/gui/training/training_module.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/gui/utils.py` & `labgym-2.4.4/LabGym/gui/utils.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/minedata.py` & `labgym-2.4.4/LabGym/minedata.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/models/__init__.py` & `labgym-2.4.4/LabGym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/LabGym/tools.py` & `labgym-2.4.4/LabGym/tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/README.md` & `labgym-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/pyproject.toml` & `labgym-2.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     { name = "Yujia Hu", email = "henryhu@umich.edu" },
     { name = "Rohan Satapathy", email = "rohansat@umich.edu" },
     { name = "M. Victor Struman", email = "strmark@umich.edu" },
     { name = "Kelly Goss", email = "khgoss@umich.edu" },
     { name = "Isabelle Baker", email = "ibaker@umich.edu" },
 ]
 dependencies = [
-    "tensorflow>=2.10.1; platform_system != 'Windows'",
+    "tensorflow>=2.10.1,<2.16.0; platform_system != 'Windows'",
     "tensorflow<2.11; platform_system == 'Windows'",
     "matplotlib",
     "opencv-python",
     "opencv-contrib-python",
     "openpyxl",
     "xlsxwriter",
     "pandas",
@@ -45,15 +45,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = []
-version = "2.4.3"
+version = "2.4.4"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.urls]
 Homepage = "http://github.com/umyelab/LabGym"
 Documentation = "https://labgym.readthedocs.io/en/latest/"
```

### Comparing `labgym-2.4.3/tests/__init__.py` & `labgym-2.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/tests/test_main.py` & `labgym-2.4.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/tests/test_tools.py` & `labgym-2.4.4/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `labgym-2.4.3/PKG-INFO` & `labgym-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: LabGym
-Version: 2.4.3
+Version: 2.4.4
 Summary: Quantify user-defined behaviors.
-Keywords: behavior analysis behavioral analysis user defined behaviors
-Author-Email: Yujia Hu <henryhu@umich.edu>, Rohan Satapathy <rohansat@umich.edu>, M. Victor Struman <strmark@umich.edu>, Kelly Goss <khgoss@umich.edu>, Isabelle Baker <ibaker@umich.edu>
+Keywords: behavior analysis,behavioral analysis,user defined behaviors
+Author-Email: Yujia Hu <henryhu@umich.edu>, Rohan Satapathy <rohansat@umich.edu>, "M. Victor Struman" <strmark@umich.edu>, Kelly Goss <khgoss@umich.edu>, Isabelle Baker <ibaker@umich.edu>
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Project-URL: Homepage, http://github.com/umyelab/LabGym
 Project-URL: Documentation, https://labgym.readthedocs.io/en/latest/
 Project-URL: Issues, http://github.com/umyelab/LabGym/issues
 Requires-Python: <3.11,>=3.9
-Requires-Dist: tensorflow>=2.10.1; platform_system != "Windows"
+Requires-Dist: tensorflow<2.16.0,>=2.10.1; platform_system != "Windows"
 Requires-Dist: tensorflow<2.11; platform_system == "Windows"
 Requires-Dist: matplotlib
 Requires-Dist: opencv-python
 Requires-Dist: opencv-contrib-python
 Requires-Dist: openpyxl
 Requires-Dist: xlsxwriter
 Requires-Dist: pandas
```

