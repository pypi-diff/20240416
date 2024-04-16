# Comparing `tmp/docscheck-0.1.0.tar.gz` & `tmp/docscheck-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docscheck-0.1.0.tar", max compression
+gzip compressed data, was "docscheck-0.1.1.tar", max compression
```

## Comparing `docscheck-0.1.0.tar` & `docscheck-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      563 2024-03-31 14:42:08.136026 docscheck-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      408 2024-03-26 17:38:10.788491 docscheck-0.1.0/README.md
--rw-r--r--   0        0        0        2 2024-03-26 17:38:09.965221 docscheck-0.1.0/src/docsCheck/__init__.py
--rw-r--r--   0        0        0     2290 2024-03-31 15:09:27.575620 docscheck-0.1.0/src/docsCheck/__main__.py
--rw-r--r--   0        0        0     1325 2024-03-26 17:38:09.595180 docscheck-0.1.0/src/docsCheck/Aspose.WordsforPythonvia.NET.lic
--rw-r--r--   0        0        0    44052 2024-03-31 14:47:14.701488 docscheck-0.1.0/src/docsCheck/checker.py
--rw-r--r--   0        0        0     1125 2024-03-31 14:55:45.161370 docscheck-0.1.0/src/docsCheck/runners.py
--rw-r--r--   0        0        0     2069 2024-03-31 13:36:41.358028 docscheck-0.1.0/src/docsCheck/utils.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 docscheck-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      563 2024-04-16 12:21:55.334043 docscheck-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      741 2024-04-16 12:02:21.417237 docscheck-0.1.1/README.md
+-rw-r--r--   0        0        0        2 2024-03-26 17:38:09.965221 docscheck-0.1.1/src/docsCheck/__init__.py
+-rw-r--r--   0        0        0     2396 2024-04-01 13:39:15.565517 docscheck-0.1.1/src/docsCheck/__main__.py
+-rw-r--r--   0        0        0     1347 2024-04-14 15:04:16.696462 docscheck-0.1.1/src/docsCheck/Aspose.WordsforPythonvia.NET.lic
+-rw-r--r--   0        0        0    45039 2024-04-16 12:20:27.212349 docscheck-0.1.1/src/docsCheck/checker.py
+-rw-r--r--   0        0        0     1125 2024-03-31 14:55:45.161370 docscheck-0.1.1/src/docsCheck/runners.py
+-rw-r--r--   0        0        0     2069 2024-03-31 13:36:41.358028 docscheck-0.1.1/src/docsCheck/utils.py
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 docscheck-0.1.1/PKG-INFO
```

### Comparing `docscheck-0.1.0/pyproject.toml` & `docscheck-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docsCheck"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Dmitry Proskurin <proskurin.dima16@gmail.com>"]
 readme = "README.md"
 packages = [{include = "docsCheck", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `docscheck-0.1.0/src/docsCheck/__main__.py` & `docscheck-0.1.1/src/docsCheck/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 doc_type - один из доступных типов документов (опционально)
 
 Доступные типы документов:
 ОБЩЕЕ - Только общая проверка (по умолчанию),
 ТЗ - Техническое задание,
 РО - Руководство оператора,
 ПЗ - Пояснительная записка
+ПИМИ - Программа и методика испытаний
+ТП - Текст программы
 
 Помощь:
 docsCheck --help
 
 """
```

### Comparing `docscheck-0.1.0/src/docsCheck/checker.py` & `docscheck-0.1.1/src/docsCheck/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
                 "Внизу листа утверждения или титульного листа не содержится указание года издания (утверждения)."
             )
 
         return verdict
 
     @staticmethod
     def _check_registration_and_storing(registration_table: aw.tables.Table) -> Verdict:
-        verdict = Verdict(standard="ГОСТ.601-78")
+        verdict = Verdict(standard="ГОСТ 19.601-78")
         if registration_table.rows.count != 5:
             verdict.add_message("В таблице регистрации и хранения должно быть 5 колонок.")
             return verdict
 
         left_length = registration_table.absolute_horizontal_distance
         for cell in registration_table.rows[0].as_row().cells:
             left_length += cell.as_cell().cell_format.width
@@ -342,15 +342,15 @@
                 f'Используется некорректный шрифт, используйте "{right_font}" 12 или 14',
                 position=f"Страница {page_number}"
             )
         layout_collector.document = None
         return verdict
 
     def check_line_spacing(self):
-        verdict = Verdict(position="Весь документ")
+        verdict = Verdict(position="Весь документ", standard="ГОСТ 19.103-78")
 
         layout_collector = aw.layout.LayoutCollector(self.doc)
         page_set = set()
         for para in self.doc.get_child_nodes(aw.NodeType.PARAGRAPH, True):
             paragraph = para.as_paragraph()
             if paragraph.paragraph_format.style.name.startswith("Heading"):
                 continue
@@ -363,15 +363,15 @@
                         page_number = layout_collector.get_start_page_index(para)
                         if 2 < page_number < self.doc.page_count:
                             page_set.add(page_number)
 
         for page_number in page_set:
             verdict.add_message(
                 "Используется некорректный межстрочный интервал",
-                position=f"Страница {page_number}"
+                position=f"Страница {page_number}",
             )
 
         return verdict
 
     def check_headers(self) -> Verdict:
         sections_count = self.doc.sections.count
         (main_verdict, has_correct_id_by_section, has_page_number_by_section, miss_header_by_section,
@@ -526,15 +526,15 @@
     name_to_page = None
     name_to_real_name = None
     name_to_bookmark = None
     has_no_number = None
     numbers_to_names = None
 
     def main_check(self) -> Verdict:
-        main_verdict = Verdict(position="Весь документ.", standard="ГОСТ 19.103-78")
+        main_verdict = Verdict(position="Весь документ", standard="ГОСТ 19.103-78")
 
         main_verdict += self.check_page_margins()
         main_verdict += self.check_certification_page()
         main_verdict += self.check_title_page()
         main_verdict += self.check_fonts()
 
         main_verdict += self.check_footers()
@@ -828,15 +828,15 @@
             self.numbers_to_names = numbers_to_names
 
         return verdict
 
 
 class TechTaskChecker(BaseChecker):
     doc_type: str = "ТЗ"
-    doc_type_id: str = "01-1"
+    doc_type_id: str = "05"
     chapters: List[str] = [
         "аннотация", "введение", "содержание",
         "лист регистрации изменений", "назначение разработки",
         "требования к программе",
         "требования к программной документации",
         "технико-экономические показатели",
         "стадии и этапы разработки",
@@ -870,20 +870,48 @@
         "технические характеристики",
         "ожидаемые технико-экономические показатели",
         "источники, использованные при разработке"
     ]
     doc_standard: str = "ГОСТ 19.404-79"
 
 
+class TestProgramAndMethods(BaseChecker):
+    doc_type: str = "51"
+    doc_type_id: str = "01-1"
+    chapters: List[str] = [
+        "содержание",
+        "лист регистрации изменений",
+        "объект испытаний",
+        "цель испытаний",
+        "требования к программной документации",
+        "состав и порядок испытаний",
+        "методы испытаний"
+    ]
+    doc_standard: str = "ГОСТ 19.301-79"
+
+
+class ProgramText(BaseChecker):
+    doc_type: str = "12"
+    doc_type_id: str = "01-1"
+    chapters: List[str] = [
+        "лист регистрации изменений",
+    ]
+    doc_standard: str = "ГОСТ 19.401-78"
+
+
 allowed_checkers = {
     "ОБЩЕЕ": BaseChecker,
     "ТЗ": TechTaskChecker,
     "РО": OperatorManualChecker,
     "ПЗ": ExplanatoryNoteChecker,
+    "ПИМИ": TestProgramAndMethods,
+    "ТП": ProgramText
 }
 
 full_allowed_checkers_name = {
     "ОБЩЕЕ": "Только общая проверка",
     "ТЗ": "Техническое задание",
     "РО": "Руководство оператора",
-    "ПЗ": "Пояснительная записка"
+    "ПЗ": "Пояснительная записка",
+    "ПИМИ": "Программа и методика испытаний",
+    "ТП": "Текст программы"
 }
```

### Comparing `docscheck-0.1.0/src/docsCheck/runners.py` & `docscheck-0.1.1/src/docsCheck/runners.py`

 * *Files identical despite different names*

### Comparing `docscheck-0.1.0/src/docsCheck/utils.py` & `docscheck-0.1.1/src/docsCheck/utils.py`

 * *Files identical despite different names*

