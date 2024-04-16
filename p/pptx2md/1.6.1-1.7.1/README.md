# Comparing `tmp/pptx2md-1.6.1.tar.gz` & `tmp/pptx2md-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx2md-1.6.1.tar", max compression
+gzip compressed data, was "pptx2md-1.7.1.tar", max compression
```

## Comparing `pptx2md-1.6.1.tar` & `pptx2md-1.7.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     3623 2024-02-25 17:44:25.744845 pptx2md-1.6.1/pptx2md/__init__.py
--rw-r--r--   0        0        0     4833 2024-02-25 17:44:10.134848 pptx2md-1.6.1/pptx2md/__main__.py
--rw-r--r--   0        0        0      821 2024-02-25 17:25:05.825004 pptx2md-1.6.1/pptx2md/global_var.py
--rw-r--r--   0        0        0      573 2024-02-25 17:26:18.474994 pptx2md-1.6.1/pptx2md/image.py
--rw-r--r--   0        0        0     5411 2023-11-18 17:51:39.808844 pptx2md-1.6.1/pptx2md/outputter.py
--rw-r--r--   0        0        0     7818 2024-03-03 19:59:34.569375 pptx2md-1.6.1/pptx2md/parser.py
--rw-r--r--   0        0        0      819 2023-11-18 17:51:39.808844 pptx2md-1.6.1/pptx2md/tools.py
--rw-r--r--   0        0        0      575 2024-03-03 20:00:10.399365 pptx2md-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 pptx2md-1.6.1/setup.py
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 pptx2md-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3623 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/__init__.py
+-rw-r--r--   0        0        0     5114 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/__main__.py
+-rw-r--r--   0        0        0     6000 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/columns.py
+-rw-r--r--   0        0        0      103 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/custom.scss
+-rw-r--r--   0        0        0      821 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/global_var.py
+-rw-r--r--   0        0        0      550 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/image.py
+-rw-r--r--   0        0        0     7676 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/outputter.py
+-rw-r--r--   0        0        0    11947 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/parser.py
+-rw-r--r--   0        0        0      819 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/tools.py
+-rw-r--r--   0        0        0     4461 2024-04-15 13:14:55.832238 pptx2md-1.7.1/pptx2md/utils_optim.py
+-rw-r--r--   0        0        0      575 2024-04-16 14:19:25.947635 pptx2md-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 pptx2md-1.7.1/setup.py
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 pptx2md-1.7.1/PKG-INFO
```

### Comparing `pptx2md-1.6.1/pptx2md/__init__.py` & `pptx2md-1.7.1/pptx2md/__init__.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.6.1/pptx2md/__main__.py` & `pptx2md-1.7.1/pptx2md/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections 
 import collections.abc
 from pptx import Presentation
 from pptx2md.global_var import g
 import pptx2md.outputter as outputter
-from pptx2md.parser import parse
+from pptx2md.parser import parse, parse_alt
 from pptx2md.tools import fix_null_rels
 import argparse
 import os, re
 import sys
 
 
 # initialization functions
@@ -42,14 +42,15 @@
                           action="store_true")
   arg_parser.add_argument('--disable-color', help='do not add color HTML tags', action="store_true")
   arg_parser.add_argument('--disable-escaping', help='do not attempt to escape special characters', action="store_true")
   arg_parser.add_argument('--disable-notes', help='do not add presenter notes', action="store_true")
   arg_parser.add_argument('--enable-slides', help='deliniate slides `\n---\n`', action="store_true")
   arg_parser.add_argument('--wiki', help='generate output as wikitext(TiddlyWiki)', action="store_true")
   arg_parser.add_argument('--mdk', help='generate output as madoko markdown', action="store_true")
+  arg_parser.add_argument('--qmd', help='generate output as quarto markdown presentation', action="store_true")
   arg_parser.add_argument('--min-block-size',
                           help='the minimum character number of a text block to be converted',
                           type=int,
                           default=15)
   arg_parser.add_argument("--page", help="only convert the specified page", type=int, default=None)
   return arg_parser.parse_args()
 
@@ -63,14 +64,16 @@
   if args.title:
     g.use_custom_title
     prepare_titles(args.title)
     g.use_custom_title = True
 
   if args.wiki:
     out_path = 'out.tid'
+  elif args.qmd:
+    out_path = 'out.qmd'
   else:
     out_path = 'out.md'
 
   if args.output:
     out_path = args.output
 
   g.out_path = os.path.abspath(out_path)
@@ -139,14 +142,20 @@
     else:
       print('unknown error, please report this bug at https://github.com/ssine/pptx2md/issues')
       sys.exit(1)
   if args.wiki:
     out = outputter.wiki_outputter(out_path)
   elif args.mdk:
     out = outputter.madoko_outputter(out_path)
+  elif args.qmd:
+    out = outputter.quarto_outputter(out_path)
   else:
     out = outputter.md_outputter(out_path)
-  parse(prs, out)
+  
+  if args.qmd:
+    parse_alt(prs, out)
+  else:
+    parse(prs, out)
 
 
 if __name__ == '__main__':
   main()
```

### Comparing `pptx2md-1.6.1/pptx2md/global_var.py` & `pptx2md-1.7.1/pptx2md/global_var.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.6.1/pptx2md/outputter.py` & `pptx2md-1.7.1/pptx2md/outputter.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 class outputter(object):
 
   def __init__(self, file_path):
     os.makedirs(os.path.dirname(os.path.abspath(file_path)), exist_ok=True)
     self.ofile = open(file_path, 'w', encoding='utf8')
 
+  def put_header(self):
+    pass
+
   def put_title(self, text, level):
     pass
 
   def put_list(self, text, level):
     pass
 
   def put_para(self, text):
@@ -192,7 +195,80 @@
   def esc_repl(self, match):
     return '\\' + match.group(0)
 
   def get_escaped(self, text):
     text = re.sub(self.esc_re1, self.esc_repl, text)
     text = re.sub(self.esc_re2, self.esc_repl, text)
     return text
+
+
+class quarto_outputter(outputter):
+  # write outputs to quarto markdown - reveal js
+  def __init__(self, file_path):
+    super().__init__(file_path)
+    self.esc_re1 = re.compile(r'([\\\*`!_\{\}\[\]\(\)#\+-\.])')
+    self.esc_re2 = re.compile(r'(<[^>]+>)')
+
+  def put_header(self):
+    self.ofile.write('''---
+title: "Presentation Title"
+author: "Author"
+format: 
+  revealjs:
+    slide-number: c/t
+    width: 1600
+    height: 900
+    logo: img/logo.png
+    footer: "Organization"
+    incremental: true
+    theme: [simple, custom.scss]
+---
+''')
+    
+  def put_title(self, text, level):
+    text = text.strip()
+    if not fuzz.ratio(text, g.last_title.get(level, ''), score_cutoff=92):
+      self.ofile.write('#' * level + ' ' + text + '\n\n')
+      g.last_title[level] = text
+    else:
+      # Allow for repeated slide titles - One or more - Add (cont.) to the title
+      self.ofile.write('#' * level + ' ' + text + ' (cont.)' + '\n\n')
+      g.last_title[level] = text
+
+  def put_list(self, text, level):
+    self.ofile.write('  ' * level + '* ' + text.strip() + '\n')
+
+  def put_para(self, text):
+    self.ofile.write(text + '\n\n')
+
+  def put_image(self, path, max_width=None):
+    if max_width is None:
+      self.ofile.write(f'![]({urllib.parse.quote(path)})\n\n')
+    else:
+      self.ofile.write(f'<img src="{path}" style="max-width:{max_width}px;" />\n\n')
+
+  def put_table(self, table):
+    gen_table_row = lambda row: '| ' + ' | '.join([c.replace('\n', '<br />') for c in row]) + ' |'
+    self.ofile.write(gen_table_row(table[0]) + '\n')
+    self.ofile.write(gen_table_row([':-:' for _ in table[0]]) + '\n')
+    self.ofile.write('\n'.join([gen_table_row(row) for row in table[1:]]) + '\n\n')
+
+  def get_accent(self, text):
+    return ' _' + text + '_ '
+
+  def get_strong(self, text):
+    return ' __' + text + '__ '
+
+  def get_colored(self, text, rgb):
+    return ' <span style="color:#%s">%s</span> ' % (str(rgb), text)
+
+  def get_hyperlink(self, text, url):
+    return '[' + text + '](' + url + ')'
+
+  def esc_repl(self, match):
+    return '\\' + match.group(0)
+
+  def get_escaped(self, text):
+    text = re.sub(self.esc_re1, self.esc_repl, text)
+    text = re.sub(self.esc_re2, self.esc_repl, text)
+    return text
+
```

### Comparing `pptx2md-1.6.1/pptx2md/parser.py` & `pptx2md-1.7.1/pptx2md/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 from __future__ import print_function
 
 import collections
 import collections.abc
 import pptx
 from pptx.enum.shapes import PP_PLACEHOLDER, MSO_SHAPE_TYPE
 from pptx.enum.dml import MSO_COLOR_TYPE, MSO_THEME_COLOR
+from pptx.util import Length
+
+import numpy as np
+
 from PIL import Image
 import os
 from rapidfuzz import process as fuze_process
 from operator import attrgetter
 
 from tqdm import tqdm
 from pptx2md.global_var import g
 from pptx2md import global_var
 
+import pptx2md.outputter as outputter
+
+from pptx2md.columns import is_two_column_text, assign_shapes
+
+from pptx2md.utils_optim import normal_pdf, fit_column_model
+
+
 picture_count = 0
 
 global out
 
 
 # pptx type defination rules
 def is_title(shape):
@@ -125,16 +136,23 @@
       text = get_formatted_text(para)
       out.put_para(text)
   return []
 
 
 def process_notes(text, _):
   global out
-  out.put_para('---')
-  out.put_para(text)
+  if(isinstance(out, outputter.quarto_outputter)):
+    
+    out.put_para("::: {.notes}")
+    out.put_para(text)
+    out.put_para(":::")
+  else:
+    out.put_para('---')
+    out.put_para(text)
+
   return []
 
 
 def process_picture(shape, slide_idx):
   notes = []
   if g.disable_image:
     return notes
@@ -174,42 +192,70 @@
   except Exception as e:
     notes.append(
         f'Cannot convert image {output_path} in slide {slide_idx} to png, this probably won\'t be displayed correctly.'
     )
     out.put_image(img_outputter_path, g.max_img_width)
   return notes
 
-
 def process_table(shape, _):
   global out
   table = [[cell.text for cell in row.cells] for row in shape.table.rows]
   if len(table) > 0:
     out.put_table(table)
   return []
 
-
 def ungroup_shapes(shapes):
   res = []
   for shape in shapes:
     try:
       if shape.shape_type == MSO_SHAPE_TYPE.GROUP:
         res.extend(ungroup_shapes(shape.shapes))
       else:
         res.append(shape)
     except Exception as e:
       print(f'failed to load shape {shape}, skipped. error: {e}')
   return res
 
+def process_shapes(current_shapes, slide_id):
+      local_notes = []
+      for shape in current_shapes:
+        if is_title(shape):
+          local_notes += process_title(shape, slide_id + 1)
+        elif is_text_block(shape):
+          local_notes += process_text_block(shape, slide_id + 1)
+        elif shape.shape_type == MSO_SHAPE_TYPE.PICTURE:
+          try:
+            local_notes += process_picture(shape, slide_id + 1)
+          except AttributeError as e:
+            print(f'Failed to process picture, skipped: {e}')
+        elif shape.shape_type == MSO_SHAPE_TYPE.TABLE:
+          local_notes += process_table(shape, slide_id + 1)
+        else:
+          try:
+            ph = shape.placeholder_format
+            if ph.type == PP_PLACEHOLDER.OBJECT and hasattr(shape, "image") and getattr(shape, "image"):
+              local_notes += process_picture(shape, slide_id + 1)
+          except:
+            pass
+
+      return(local_notes)
 
 # main
 def parse(prs, outputer):
   global out
   out = outputer
   notes = []
+
+  print("Starting conversion")
+
+  # Adding inclusion of header for the first slide
+  out.put_header()
+
   for idx, slide in enumerate(tqdm(prs.slides, desc='Converting slides')):
+  # for idx, slide in enumerate(prs.slides):
     if g.page is not None and idx + 1 != g.page:
         continue
     shapes = []
     try:
       shapes = sorted(ungroup_shapes(slide.shapes), key=attrgetter('top', 'left'))
     except:
       print('Bad shapes encountered in this slide. Please check or move them and try again.')
@@ -217,38 +263,129 @@
       try:
         for sp in slide.shapes:
           print(sp.shape_type)
           print(sp.top, sp.left, sp.width, sp.height)
       except:
         print('failed to print all bad shapes.')
 
-    for shape in shapes:
-      if is_title(shape):
-        notes += process_title(shape, idx + 1)
-      elif is_text_block(shape):
-        notes += process_text_block(shape, idx + 1)
-      elif shape.shape_type == MSO_SHAPE_TYPE.PICTURE:
-        try:
-          notes += process_picture(shape, idx + 1)
-        except AttributeError as e:
-          print(f'Failed to process picture, skipped: {e}')
-      elif shape.shape_type == MSO_SHAPE_TYPE.TABLE:
-        notes += process_table(shape, idx + 1)
-      else:
-        try:
-          ph = shape.placeholder_format
-          if ph.type == PP_PLACEHOLDER.OBJECT and hasattr(shape, "image") and getattr(shape, "image"):
-            notes += process_picture(shape, idx + 1)
-        except:
-          pass
+    process_shapes(shapes, idx + 1)
+
     if not g.disable_notes and slide.has_notes_slide:
       text = slide.notes_slide.notes_text_frame.text
       if text:
         notes += process_notes(text, idx + 1)
     if idx < len(prs.slides)-1 and g.enable_slides:
         out.put_para("\n---\n")
   out.close()
 
   if len(notes) > 0:
     print('Process finished with notice:')
     for note in notes:
       print(note)
+
+
+# Alternative parse function for qmd files
+def parse_alt(prs, outputer):
+  global out
+  out = outputer
+  notes = []
+
+  slide_width = pptx.util.Length(prs.slide_width)
+  slide_width_mm = slide_width.mm
+
+  t_vector = np.arange(1, slide_width_mm)
+
+  print("Starting convertion to qmd file")
+
+  # Adding inclusion of header for the first slide
+  out.put_header()
+
+  for idx, slide in enumerate(tqdm(prs.slides, desc='Converting slides')):
+  # for idx, slide in enumerate(prs.slides):
+    if g.page is not None and idx + 1 != g.page:
+        continue
+    shapes = []
+    try:
+      shapes = sorted(ungroup_shapes(slide.shapes), key=attrgetter('top', 'left'))
+    except:
+      print('Bad shapes encountered in this slide. Please check or move them and try again.')
+      print('shapes:')
+      try:
+        for sp in slide.shapes:
+          print(sp.shape_type)
+          print(sp.top, sp.left, sp.width, sp.height)
+      except:
+        print('failed to print all bad shapes.')
+
+    pdf_modelo = is_two_column_text(slide)
+    
+    if(pdf_modelo):
+      # Model to infer number of columns
+
+      salida = map(lambda mu, sigma: normal_pdf(t_vector, mu, sigma), pdf_modelo[0], pdf_modelo[1])
+      sum_of_gaussian = np.mean(list(salida), axis=0)
+      parameters = fit_column_model(t_vector, sum_of_gaussian)
+
+      num_cols = int(len(parameters)/2)
+
+      dict_shapes = assign_shapes(slide, parameters, num_cols, slide_width_mm=slide_width_mm)
+      print("Cantidad de elementos")
+      print("pre: %d"%len(dict_shapes["shapes_pre"]))
+      print("l: %d"%len(dict_shapes["shapes_l"]))
+      print("c: %d"%len(dict_shapes["shapes_c"]))
+      print("r: %d"%len(dict_shapes["shapes_r"]))
+            
+      notes.extend(process_shapes(dict_shapes["shapes_pre"], idx))
+      if num_cols == 1:
+        pass
+      
+      elif num_cols == 2:
+        out.put_para(':::: {.columns}')
+
+        out.put_para('::: {.column width="50%"}')
+        notes.extend(process_shapes(dict_shapes["shapes_l"], idx))
+        out.put_para(':::')
+        out.put_para('::: {.column width="50%"}')
+        notes.extend(process_shapes(dict_shapes["shapes_r"], idx))
+        out.put_para(':::')
+        out.put_para('::::')
+
+
+      elif num_cols == 3:
+        out.put_para(':::: {.columns}')
+        
+        if(dict_shapes["shapes_l"]):
+          out.put_para('::: {.column width="33%"}')
+          notes.extend(process_shapes(dict_shapes["shapes_l"], idx))
+          out.put_para(':::')
+
+        if(dict_shapes["shapes_c"]):
+          out.put_para('::: {.column width="33%"}')
+          notes.extend(process_shapes(dict_shapes["shapes_c"], idx))
+          out.put_para(':::')
+        
+        if(dict_shapes["shapes_r"]):
+          out.put_para('::: {.column width="33%"}')
+          notes.extend(process_shapes(dict_shapes["shapes_r"], idx))
+          out.put_para(':::')
+        
+        out.put_para('::::')
+
+      else:
+        raise(ValueError, "Number of columns not allowed")
+
+    else:
+      notes.extend(process_shapes(shapes, idx))
+
+
+    if not g.disable_notes and slide.has_notes_slide:
+      text = slide.notes_slide.notes_text_frame.text
+      if text:
+        notes += process_notes(text, idx + 1)
+    if idx < len(prs.slides)-1 and g.enable_slides:
+        out.put_para("\n---\n")
+  out.close()
+
+  if len(notes) > 0:
+    print('Process finished with notice:')
+    for note in notes:
+      print(note)
```

### Comparing `pptx2md-1.6.1/pptx2md/tools.py` & `pptx2md-1.7.1/pptx2md/tools.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.6.1/pyproject.toml` & `pptx2md-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pptx2md"
-version = "1.6.1"
+version = "1.7.1"
 description = "This package converts pptx to markdown"
 repository = "https://github.com/ssine/pptx2md"
 authors = ["Liu Siyao <liu.siyao@qq.com>"]
 license = "MIT Licence"
 
 [tool.poetry.scripts]
 pptx2md = "pptx2md.__main__:main"
```

### Comparing `pptx2md-1.6.1/setup.py` & `pptx2md-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=6.0.0', 'python-pptx>=0.6.18', 'rapidfuzz>=0.10.0', 'tqdm>=4']
 
 entry_points = \
 {'console_scripts': ['pptx2md = pptx2md.__main__:main']}
 
 setup_kwargs = {
     'name': 'pptx2md',
-    'version': '1.6.1',
+    'version': '1.7.1',
     'description': 'This package converts pptx to markdown',
     'long_description': 'None',
     'author': 'Liu Siyao',
     'author_email': 'liu.siyao@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ssine/pptx2md',
```

### Comparing `pptx2md-1.6.1/PKG-INFO` & `pptx2md-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx2md
-Version: 1.6.1
+Version: 1.7.1
 Summary: This package converts pptx to markdown
 Home-page: https://github.com/ssine/pptx2md
 License: MIT Licence
 Author: Liu Siyao
 Author-email: liu.siyao@qq.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
```

