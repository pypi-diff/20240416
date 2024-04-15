# Comparing `tmp/sqlmodel_filters-0.0.4.tar.gz` & `tmp/sqlmodel_filters-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_filters-0.0.4.tar", max compression
+gzip compressed data, was "sqlmodel_filters-0.0.5.tar", max compression
```

## Comparing `sqlmodel_filters-0.0.4.tar` & `sqlmodel_filters-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/LICENSE
--rw-r--r--   0        0        0     7420 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/README.md
--rw-r--r--   0        0        0     1022 2024-04-13 23:39:49.324200 sqlmodel_filters-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/__init__.py
--rw-r--r--   0        0        0     4550 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/builder.py
--rw-r--r--   0        0        0     5689 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/components.py
--rw-r--r--   0        0        0      165 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/exceptions.py
--rw-r--r--   0        0        0      637 2024-04-13 23:39:35.636172 sqlmodel_filters-0.0.4/sqlmodel_filters/utils.py
--rw-r--r--   0        0        0     8005 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7693 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/README.md
+-rw-r--r--   0        0        0     1022 2024-04-15 23:23:13.105450 sqlmodel_filters-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/__init__.py
+-rw-r--r--   0        0        0     5029 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/builder.py
+-rw-r--r--   0        0        0     5689 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/components.py
+-rw-r--r--   0        0        0      165 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/exceptions.py
+-rw-r--r--   0        0        0      637 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/utils.py
+-rw-r--r--   0        0        0     8278 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.5/PKG-INFO
```

### Comparing `sqlmodel_filters-0.0.4/LICENSE` & `sqlmodel_filters-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.4/README.md` & `sqlmodel_filters-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,23 @@
 
 ### `AND`, `OR`, `NOT` and `GROUP` (Grouping)
 
 | Query                                    | SQL (Where Clause)                                                                |
 | ---------------------------------------- | --------------------------------------------------------------------------------- |
 | `name:Rusty AND age:48`                  | `WHERE hero.name LIKE '%Rusty%' AND hero.age = 48`                                |
 | `name:Rusty OR age:47`                   | `WHERE hero.name LIKE '%Rusty%' OR hero.age = 47`                                 |
-| `name:Rusty NOT age:47`                  | `WHERE hero.name LIKE '%Rusty%' AND hero.age != 47`                               |
+| `NOT name:Rusty`                         | `WHERE hero.name NOT LIKE '%Rusty%'`                                              |
 | `(name:Spider OR age:48) AND name:Rusty` | `WHERE (hero.name LIKE '%Spider%' OR hero.age = 48) AND hero.name LIKE '%Rusty%'` |
 
+Note that the default conjunction is `OR`.
+
+| Query               | SQL (Where Clause)                                |
+| ------------------- | ------------------------------------------------- |
+| `name:Rusty age:48` | `WHERE hero.name LIKE '%Rusty%' OR hero.age = 48` |
+
 ### Relationship
 
 Set `relationships` (key-to-model mapping) to do filtering on relationship(s).
 
 ```py
 >>> parsed = parse('name:Spider AND team.name:"Preventers" AND team.headquarter.name:Sharp')
 >>> builder = SelectBuilder(Hero, relationships={"team": Team, "headquarter": Headquarter})
```

### Comparing `sqlmodel_filters-0.0.4/pyproject.toml` & `sqlmodel_filters-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlmodel-filters"
-version = "0.0.4"
+version = "0.0.5"
 description = "A Lucene query like fliltering for SQLModel"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sqlmodel_filters-0.0.4/sqlmodel_filters/builder.py` & `sqlmodel_filters-0.0.5/sqlmodel_filters/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     def get_expressions(self, node: Item):
         match node:
             case SearchField():
                 yield from self._handel_search_field(node)
             case Not():
                 search_field = node.children[0]
-                for condition in self._handel_search_field(search_field):
-                    yield not_(condition)
+                expressions = self.get_expressions(search_field)
+                yield not_(*expressions)
             case Group():
                 yield from self._handle_group(node)
             case AndOperation():
                 yield from self._handle_and_operation(node)
             case OrOperation():
                 yield from self._handle_or_operation(node)
             case unknown:
@@ -55,38 +55,50 @@
         yield from super().generic_visit(node, context)
 
     def _handle_group(self, node: Group):
         # NOTE: group can be processed as And operation
         yield from self._handle_and_operation(node)  # type: ignore
 
     def _handle_and_operation(self, node: AndOperation):
-        expressions: list[Any] = []
+        expressions: list[_ColumnExpressionArgument] = []
         for child in node.children:
             expressions.extend(list(self.get_expressions(child)))
 
         if len(expressions) > 0:
             yield and_(*expressions)
 
     def visit_and_operation(self, node: AndOperation, context: dict):
         self.expressions.extend(list(self._handle_and_operation(node)))
         yield from super().generic_visit(node, context)
 
     def _handle_or_operation(self, node: OrOperation):
-        expressions: list[Any] = []
+        expressions: list[_ColumnExpressionArgument] = []
         for child in node.children:
             expressions.extend(list(self.get_expressions(child)))
 
         if len(expressions) > 0:
             first, *others = expressions
             yield or_(first, *others)
 
     def visit_or_operation(self, node: OrOperation, context: dict):
         self.expressions.extend(list(self._handle_or_operation(node)))
         yield from super().generic_visit(node, context)
 
+    def _handle_not(self, node: Not):
+        expressions: list[_ColumnExpressionArgument] = []
+        for child in node.children:
+            expressions.extend(list(self.get_expressions(child)))
+
+        if len(expressions) > 0:
+            yield not_(*expressions)
+
+    def visit_not(self, node: Not, context: dict):
+        self.expressions.extend(list(self._handle_not(node)))
+        yield from super().generic_visit(node, context)
+
     def visit_unknown_operation(self, node: UnknownOperation, context: dict):
         for child in node.children:
             self.expressions.extend(list(self.get_expressions(child)))
 
         yield from super().generic_visit(node, context)
 
     def __call__(self, tree: Item):
@@ -114,8 +126,8 @@
             entities = self.model
 
         s = select(*entities) if isinstance(entities, (tuple, list)) else select(entities)
 
         for join in self.relationships.values():
             s = s.join(join)
 
-        return s.where(*self.expressions)
+        return s.where(or_(*self.expressions))
```

### Comparing `sqlmodel_filters-0.0.4/sqlmodel_filters/components.py` & `sqlmodel_filters-0.0.5/sqlmodel_filters/components.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.4/sqlmodel_filters/utils.py` & `sqlmodel_filters-0.0.5/sqlmodel_filters/utils.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.4/PKG-INFO` & `sqlmodel_filters-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-filters
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Lucene query like fliltering for SQLModel
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -180,17 +180,23 @@
 
 ### `AND`, `OR`, `NOT` and `GROUP` (Grouping)
 
 | Query                                    | SQL (Where Clause)                                                                |
 | ---------------------------------------- | --------------------------------------------------------------------------------- |
 | `name:Rusty AND age:48`                  | `WHERE hero.name LIKE '%Rusty%' AND hero.age = 48`                                |
 | `name:Rusty OR age:47`                   | `WHERE hero.name LIKE '%Rusty%' OR hero.age = 47`                                 |
-| `name:Rusty NOT age:47`                  | `WHERE hero.name LIKE '%Rusty%' AND hero.age != 47`                               |
+| `NOT name:Rusty`                         | `WHERE hero.name NOT LIKE '%Rusty%'`                                              |
 | `(name:Spider OR age:48) AND name:Rusty` | `WHERE (hero.name LIKE '%Spider%' OR hero.age = 48) AND hero.name LIKE '%Rusty%'` |
 
+Note that the default conjunction is `OR`.
+
+| Query               | SQL (Where Clause)                                |
+| ------------------- | ------------------------------------------------- |
+| `name:Rusty age:48` | `WHERE hero.name LIKE '%Rusty%' OR hero.age = 48` |
+
 ### Relationship
 
 Set `relationships` (key-to-model mapping) to do filtering on relationship(s).
 
 ```py
 >>> parsed = parse('name:Spider AND team.name:"Preventers" AND team.headquarter.name:Sharp')
 >>> builder = SelectBuilder(Hero, relationships={"team": Team, "headquarter": Headquarter})
```

