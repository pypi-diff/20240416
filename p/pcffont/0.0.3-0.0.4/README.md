# Comparing `tmp/pcffont-0.0.3.tar.gz` & `tmp/pcffont-0.0.4.tar.gz`

## Comparing `pcffont-0.0.3.tar` & `pcffont-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.3/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/artwiz/anorexia.pcf
--rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/artwiz/kates.pcf
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/dweep/dweep.pcf
--rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/profont-x11/ProFont_r400-29.pcf
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/raize/raize-normal-19.pcf
--rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/sgi/rock36.pcf
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/trisk/trisk.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.3/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.3/examples/__init__.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pcffont-0.0.3/examples/create.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 pcffont-0.0.3/examples/load.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/error.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/font.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/format.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/header.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/metric.py
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.3/src/pcffont/internal/util.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_dump.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_example.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_load_save.py
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 pcffont-0.0.3/tests/test_reload.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.3/LICENSE
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 pcffont-0.0.3/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 pcffont-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/artwiz/anorexia.pcf
+-rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/artwiz/kates.pcf
+-rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/dweep/dweep.pcf
+-rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/profont-x11/ProFont_r400-29.pcf
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/raize/raize-normal-19.pcf
+-rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/sgi/rock36.pcf
+-rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/trisk/trisk.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.4/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.4/examples/__init__.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 pcffont-0.0.4/examples/create.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pcffont-0.0.4/examples/load.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/error.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/font.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/format.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/header.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/metric.py
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    11654 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.4/src/pcffont/internal/util.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_dump.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_example.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_load_save.py
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 pcffont-0.0.4/tests/test_reload.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 pcffont-0.0.4/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 pcffont-0.0.4/PKG-INFO
```

### Comparing `pcffont-0.0.3/.github/workflows/publish.yml` & `pcffont-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/.github/workflows/test.yml` & `pcffont-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/artwiz/anorexia.pcf` & `pcffont-0.0.4/assets/artwiz/anorexia.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/artwiz/kates.pcf` & `pcffont-0.0.4/assets/artwiz/kates.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/dweep/dweep.pcf` & `pcffont-0.0.4/assets/dweep/dweep.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/profont-x11/ProFont_r400-29.pcf` & `pcffont-0.0.4/assets/profont-x11/ProFont_r400-29.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/raize/raize-normal-19.pcf` & `pcffont-0.0.4/assets/raize/raize-normal-19.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/sgi/rock36.pcf` & `pcffont-0.0.4/assets/sgi/rock36.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/trisk/trisk.pcf` & `pcffont-0.0.4/assets/trisk/trisk.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/unifont/OFL.txt` & `pcffont-0.0.4/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.4/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/examples/create.py` & `pcffont-0.0.4/examples/create.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/examples/load.py` & `pcffont-0.0.4/examples/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
         glyph_name = font.glyph_names[glyph_index]
         metric = font.metrics[glyph_index]
         bitmap = font.bitmaps[glyph_index]
         print(f'char: {chr(code_point)} ({code_point:04X})')
         print(f'glyph_name: {glyph_name}')
         print(f'advance_width: {metric.character_width}')
-        print(f'offset: ({-metric.left_side_bearing}, {-metric.descent})')
+        print(f'offset: ({metric.left_side_bearing}, {-metric.descent})')
         for bitmap_row in bitmap:
             text = ''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')
             print(f'{text}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
```

### Comparing `pcffont-0.0.3/src/pcffont/error.py` & `pcffont-0.0.4/src/pcffont/error.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/font.py` & `pcffont-0.0.4/src/pcffont/font.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/format.py` & `pcffont-0.0.4/src/pcffont/format.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/header.py` & `pcffont-0.0.4/src/pcffont/header.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/metric.py` & `pcffont-0.0.4/src/pcffont/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,22 @@
         self.left_side_bearing = left_side_bearing
         self.right_side_bearing = right_side_bearing
         self.character_width = character_width
         self.ascent = ascent
         self.descent = descent
         self.attributes = attributes
 
+    @property
+    def glyph_width(self) -> int:
+        return self.right_side_bearing - self.left_side_bearing
+
+    @property
+    def glyph_height(self) -> int:
+        return self.ascent + self.descent
+
     def dump(self, buffer: Buffer, is_ms_byte: bool, is_compressed: bool):
         if is_compressed:
             buffer.write_int8(self.left_side_bearing + 0x80)
             buffer.write_int8(self.right_side_bearing + 0x80)
             buffer.write_int8(self.character_width + 0x80)
             buffer.write_int8(self.ascent + 0x80)
             buffer.write_int8(self.descent + 0x80)
```

### Comparing `pcffont-0.0.3/src/pcffont/t_accelerators.py` & `pcffont-0.0.4/src/pcffont/t_accelerators.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/t_bitmaps.py` & `pcffont-0.0.4/src/pcffont/t_bitmaps.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/t_encodings.py` & `pcffont-0.0.4/src/pcffont/t_encodings.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/t_glyph_names.py` & `pcffont-0.0.4/src/pcffont/t_glyph_names.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/t_metrics.py` & `pcffont-0.0.4/src/pcffont/t_metrics.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/t_properties.py` & `pcffont-0.0.4/src/pcffont/t_properties.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/t_scalable_widths.py` & `pcffont-0.0.4/src/pcffont/t_scalable_widths.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/table.py` & `pcffont-0.0.4/src/pcffont/table.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/internal/buffer.py` & `pcffont-0.0.4/src/pcffont/internal/buffer.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/src/pcffont/internal/util.py` & `pcffont-0.0.4/src/pcffont/internal/util.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/tests/test_dump.py` & `pcffont-0.0.4/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/tests/test_load_save.py` & `pcffont-0.0.4/tests/test_load_save.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/tests/test_reload.py` & `pcffont-0.0.4/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/.gitignore` & `pcffont-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/LICENSE` & `pcffont-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.3/README.md` & `pcffont-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
         glyph_name = font.glyph_names[glyph_index]
         metric = font.metrics[glyph_index]
         bitmap = font.bitmaps[glyph_index]
         print(f'char: {chr(code_point)} ({code_point:04X})')
         print(f'glyph_name: {glyph_name}')
         print(f'advance_width: {metric.character_width}')
-        print(f'offset: ({-metric.left_side_bearing}, {-metric.descent})')
+        print(f'offset: ({metric.left_side_bearing}, {-metric.descent})')
         for bitmap_row in bitmap:
             text = ''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')
             print(f'{text}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
```

### Comparing `pcffont-0.0.3/pyproject.toml` & `pcffont-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.3"
+version = "0.0.4"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pcffont-0.0.3/PKG-INFO` & `pcffont-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pcffont
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for manipulating Portable Compiled Format (PCF) Fonts.
 Project-URL: homepage, https://github.com/TakWolf/pcffont
 Project-URL: source, https://github.com/TakWolf/pcffont
 Project-URL: issues, https://github.com/TakWolf/pcffont/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
@@ -56,15 +56,15 @@
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
         glyph_name = font.glyph_names[glyph_index]
         metric = font.metrics[glyph_index]
         bitmap = font.bitmaps[glyph_index]
         print(f'char: {chr(code_point)} ({code_point:04X})')
         print(f'glyph_name: {glyph_name}')
         print(f'advance_width: {metric.character_width}')
-        print(f'offset: ({-metric.left_side_bearing}, {-metric.descent})')
+        print(f'offset: ({metric.left_side_bearing}, {-metric.descent})')
         for bitmap_row in bitmap:
             text = ''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')
             print(f'{text}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
```

