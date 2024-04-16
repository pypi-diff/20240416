# Comparing `tmp/polymatch-0.3.0.tar.gz` & `tmp/polymatch-0.4.0.tar.gz`

## Comparing `polymatch-0.3.0.tar` & `polymatch-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 polymatch-0.3.0/.editorconfig
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 polymatch-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 polymatch-0.3.0/codecov.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 polymatch-0.3.0/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 polymatch-0.3.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 polymatch-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 polymatch-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 polymatch-0.3.0/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polymatch-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/__init__.py
--rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/base.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/py.typed
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/matchers/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/matchers/glob.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/matchers/regex.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 polymatch-0.3.0/polymatch/matchers/standard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/base_test.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/test_glob.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/test_pickling.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/test_regex.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/test_registry.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 polymatch-0.3.0/tests/test_standard.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 polymatch-0.3.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 polymatch-0.3.0/LICENSE
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 polymatch-0.3.0/README.md
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 polymatch-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 polymatch-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 polymatch-0.4.0/.editorconfig
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 polymatch-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 polymatch-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 polymatch-0.4.0/codecov.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 polymatch-0.4.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 polymatch-0.4.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polymatch-0.4.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 polymatch-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/_version.py
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/base.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/py.typed
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/glob.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/regex.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 polymatch-0.4.0/polymatch/matchers/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/base_test.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_glob.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_pickling.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_regex.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_registry.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 polymatch-0.4.0/tests/test_standard.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 polymatch-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 polymatch-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 polymatch-0.4.0/README.md
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 polymatch-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 polymatch-0.4.0/PKG-INFO
```

### Comparing `polymatch-0.3.0/.pre-commit-config.yaml` & `polymatch-0.4.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,82 @@
-ci:
-  skip: [pylint, mypy]
 repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: c4a0b883114b00d8d76b479c820ce7950211c99b # frozen: v4.5.0
-    hooks:
-      - id: trailing-whitespace
-        args: ["--markdown-linebreak-ext=md,markdown"]
-      - id: end-of-file-fixer
-      - id: check-yaml
-      - id: check-added-large-files
-      - id: check-ast
-      - id: check-byte-order-marker
-      - id: check-merge-conflict
-      - id: debug-statements
-      - id: detect-private-key
-      - id: check-builtin-literals
-      - id: check-case-conflict
-      - id: check-docstring-first
-      - id: check-executables-have-shebangs
-      - id: check-json
-        exclude: '^\.(vscode|devcontainer)/'
-      - id: pretty-format-json
-        args:
-          - --indent
-          - "4"
-          - --autofix
-          - --no-sort-keys
-        exclude: '^\.(vscode|devcontainer)/'
-      - id: check-toml
-      - id: fix-encoding-pragma
-        args:
-          - --remove
-  - repo: https://github.com/psf/black
-    rev: 552baf822992936134cbd31a38f69c8cfe7c0f05 # frozen: 24.3.0
-    hooks:
-      - id: black
-  - repo: https://github.com/pycqa/isort
-    rev: c235f5e450b4b84e58d114ed4c589cbf454175a3 # frozen: 5.13.2
-    hooks:
-      - id: isort
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: 3a6eb0fadf60b3cccfd80bad9dbb6fae7e47b316 # frozen: v1.10.0
-    hooks:
-      - id: python-no-eval
-      - id: python-no-log-warn
-
-  - repo: https://github.com/ikamensh/flynt/
-    rev: "651c822fdcf45fffcf9743dc755085f32acb65e3" # frozen: 1.0.1
-    hooks:
-      - id: flynt
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: 12af25eb252deaaecb6b259df40d01f42e716dc3 # frozen: v3.15.2
-    hooks:
-      - id: pyupgrade
-        args:
-          - "--py38-plus"
-
-  - repo: https://github.com/MarcoGorelli/auto-walrus
-    rev: e95a3f5b9cd6a6808b803aef0c68a24c35b5891c # frozen: v0.2.2
-    hooks:
-      - id: auto-walrus
-
-  - repo: local
-    hooks:
-      - id: mypy
-        name: mypy
-        entry: hatch run python3 -m mypy
-        language: system
-        types: [python]
-        exclude: tests/.*
+- hooks:
+  - args:
+    - --markdown-linebreak-ext=md,markdown
+    id: trailing-whitespace
+  - id: end-of-file-fixer
+  - id: check-yaml
+  - id: check-added-large-files
+  - id: check-ast
+  - id: fix-byte-order-marker
+  - id: check-merge-conflict
+  - id: debug-statements
+  - id: detect-private-key
+  - id: check-builtin-literals
+  - id: check-case-conflict
+  - id: check-docstring-first
+  - id: check-executables-have-shebangs
+  - id: check-shebang-scripts-are-executable
+  - id: check-symlinks
+  - args:
+    - --fix=lf
+    id: mixed-line-ending
+  - exclude: ^\.(vscode|devcontainer)/
+    id: check-json
+  - args:
+    - --indent
+    - '4'
+    - --autofix
+    - --no-sort-keys
+    exclude: ^\.(vscode|devcontainer)/
+    id: pretty-format-json
+  - id: check-toml
+  repo: https://github.com/pre-commit/pre-commit-hooks
+  rev: 2c9f875913ee60ca25ce70243dc24d5b6415598c
+- hooks:
+  - id: black
+  repo: https://github.com/psf/black
+  rev: 8fe627072f15ff2e3d380887b92f7868efaf6d05
+- hooks:
+  - id: isort
+  repo: https://github.com/pycqa/isort
+  rev: c235f5e450b4b84e58d114ed4c589cbf454175a3
+- hooks:
+  - id: python-no-eval
+  - id: python-no-log-warn
+  repo: https://github.com/pre-commit/pygrep-hooks
+  rev: 3a6eb0fadf60b3cccfd80bad9dbb6fae7e47b316
+- hooks:
+  - id: flynt
+  repo: https://github.com/ikamensh/flynt
+  rev: 651c822fdcf45fffcf9743dc755085f32acb65e3
+- hooks:
+  - args:
+    - --py38-plus
+    id: pyupgrade
+  repo: https://github.com/asottile/pyupgrade
+  rev: 12af25eb252deaaecb6b259df40d01f42e716dc3
+- hooks:
+  - additional_dependencies:
+    - tomli ; python_version < '3.11'
+    id: auto-walrus
+  repo: https://github.com/MarcoGorelli/auto-walrus
+  rev: 7855759486496a3248e9ff37dce7c6d57d39bfce
+- hooks:
+  - additional_dependencies:
+    - tomli ; python_version < '3.11'
+    id: codespell
+  repo: https://github.com/codespell-project/codespell
+  rev: 6e41aba91fb32e9feb741a6258eefeb9c6e4a482
+- hooks:
+  - id: commitizen
+  repo: https://github.com/commitizen-tools/commitizen
+  rev: 7c0bc1591103b1f089aab9810fc2a201ccb0552b
+- hooks:
+  - entry: hatch run python3 -m mypy
+    exclude: tests/.*
+    id: mypy
+    language: system
+    name: mypy
+    types:
+    - python
+  repo: local
```

### Comparing `polymatch-0.3.0/.devcontainer/devcontainer.json` & `polymatch-0.4.0/.devcontainer/devcontainer.json`

 * *Files 9% similar despite different names*

```diff
@@ -32,25 +32,27 @@
                 "ms-python.python",
                 "ms-python.vscode-pylance",
                 "EditorConfig.EditorConfig",
                 "GitHub.vscode-pull-request-github",
                 "github.vscode-github-actions",
                 "redhat.vscode-yaml",
                 "ms-python.black-formatter",
-                "ms-python.isort"
+                "ms-python.isort",
+                "ms-azuretools.vscode-docker",
+                "ms-python.mypy-type-checker"
             ],
             "settings": {
                 "python.defaultInterpreterPath": "~/.virtualenvs/polymatch/bin/python",
                 "python.testing.pytestArgs": ["--no-cov"],
                 "terminal.integrated.profiles.linux": {
                     "zsh": {
                         "path": "/usr/bin/zsh"
                     }
                 },
                 "terminal.integrated.defaultProfile.linux": "zsh",
                 "[python]": {
-                    "editor.defaultFormatter": "ms-python.python"
+                    "editor.defaultFormatter": "ms-python.black-formatter"
                 }
             }
         }
     }
 }
```

### Comparing `polymatch-0.3.0/polymatch/__init__.py` & `polymatch-0.4.0/polymatch/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/polymatch/base.py` & `polymatch-0.4.0/polymatch/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from abc import ABCMeta, abstractmethod
 from enum import Enum
-from typing import AnyStr, Callable, Generic, Optional, Tuple, Type, TypeVar
+from typing import (
+    AnyStr,
+    Callable,
+    Generic,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    cast,
+)
 
 import polymatch
 from polymatch.error import (
     PatternCompileError,
     PatternNotCompiledError,
     PatternTextTypeMismatchError,
 )
@@ -23,15 +32,17 @@
 TUPLE_V2 = Tuple[
     str, AnyStr, CaseAction, bool, Optional[AnyPattern], Type[AnyStr], object
 ]
 
 CompileFunc = Callable[[AnyStr], AnyPattern]
 MatchFunc = Callable[[AnyPattern, AnyStr], bool]
 
-FuncTuple = Tuple[CompileFunc[AnyStr, AnyPattern], MatchFunc[AnyPattern, AnyStr]]
+FuncTuple = Tuple[
+    CompileFunc[AnyStr, AnyPattern], MatchFunc[AnyPattern, AnyStr]
+]
 
 
 class PolymorphicMatcher(Generic[AnyStr, AnyPattern], metaclass=ABCMeta):
     _empty = object()
 
     def __init__(
         self,
@@ -139,19 +150,24 @@
 
     def _get_case_functions(
         self,
     ) -> Tuple[CompileFunc[AnyStr, AnyPattern], MatchFunc[AnyPattern, AnyStr]]:
         suffix = self.case_action.value[1]
 
         if suffix:
-            suffix = "_" + suffix
+            suffix = f"_{suffix}"
 
-        return getattr(self, "compile_pattern" + suffix), getattr(
-            self, "match_text" + suffix
+        comp_func = cast(
+            CompileFunc[AnyStr, AnyPattern],
+            getattr(self, f"compile_pattern{suffix}"),
+        )
+        match_func = cast(
+            MatchFunc[AnyPattern, AnyStr], getattr(self, f"match_text{suffix}")
         )
+        return comp_func, match_func
 
     @classmethod
     @abstractmethod
     def get_type(cls) -> str:
         raise NotImplementedError
 
     @property
@@ -173,15 +189,17 @@
                 self.get_type(),
                 self.case_action.value[1],
                 self.pattern,
             )
 
         return (
             "{}{}:{}:".format(
-                "~" if self.inverted else "", self.get_type(), self.case_action.value[1]
+                "~" if self.inverted else "",
+                self.get_type(),
+                self.case_action.value[1],
             )
         ).encode() + self.pattern
 
     def __str__(self) -> str:
         res = self.to_string()
         if isinstance(res, str):
             return res
```

### Comparing `polymatch-0.3.0/polymatch/error.py` & `polymatch-0.4.0/polymatch/error.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/polymatch/registry.py` & `polymatch-0.4.0/polymatch/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,17 +44,21 @@
         invert, name, opts, pattern = _opt_split(text, b":", b"", b"~")
         return invert, name.decode(), opts.decode(), pattern
 
     msg = f"Unable to parse pattern string of type {type(text).__name__!r}"
     raise TypeError(msg)
 
 
+_Matcher = PolymorphicMatcher[Any, Any]
+_MatcherCls = Type[_Matcher]
+
+
 class PatternMatcherRegistry:
     def __init__(self) -> None:
-        self._matchers: Dict[str, Type[PolymorphicMatcher[Any, Any]]] = OrderedDict()
+        self._matchers: Dict[str, _MatcherCls] = OrderedDict()
 
     def register(self, cls: Type[Any]) -> None:
         if not issubclass(cls, PolymorphicMatcher):
             msg = "Pattern matcher must be of type {!r} not {!r}".format(
                 PolymorphicMatcher.__name__, cls.__name__
             )
             raise TypeError(msg)
@@ -64,32 +68,34 @@
             raise DuplicateMatcherRegistrationError(name)
 
         self._matchers[name] = cls
 
     def remove(self, name: str) -> None:
         del self._matchers[name]
 
-    def __getitem__(self, item: str) -> Type[PolymorphicMatcher[Any, Any]]:
+    def __getitem__(self, item: str) -> _MatcherCls:
         return self.get_matcher(item)
 
-    def get_matcher(self, name: str) -> Type[PolymorphicMatcher[Any, Any]]:
+    def get_matcher(self, name: str) -> _MatcherCls:
         try:
             return self._matchers[name]
         except LookupError as e:
             raise NoSuchMatcherError(name) from e
 
-    def get_default_matcher(self) -> Type[PolymorphicMatcher[Any, Any]]:
+    def get_default_matcher(self) -> _MatcherCls:
         if self._matchers:
             return next(iter(self._matchers.values()))
 
         raise NoMatchersAvailableError
 
-    def pattern_from_string(self, text: AnyStr) -> PolymorphicMatcher[Any, Any]:
+    def pattern_from_string(self, text: AnyStr) -> _Matcher:
         invert, name, opts, pattern = _parse_pattern_string(text)
-        match_cls = self.get_default_matcher() if not name else self.get_matcher(name)
+        match_cls = (
+            self.get_default_matcher() if not name else self.get_matcher(name)
+        )
 
         case_action: Optional[CaseAction] = None
         for action in CaseAction:
             if action.value[1] == opts:
                 case_action = action
                 break
```

### Comparing `polymatch-0.3.0/polymatch/matchers/glob.py` & `polymatch-0.4.0/polymatch/matchers/glob.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/polymatch/matchers/regex.py` & `polymatch-0.4.0/polymatch/matchers/regex.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,33 +7,47 @@
 
 class RegexMatcher(PolymorphicMatcher[AnyStr, "regex.Pattern[AnyStr]"]):
     def compile_pattern(
         self, raw_pattern: AnyStr, *, flags: int = 0
     ) -> "regex.Pattern[AnyStr]":
         return regex.compile(raw_pattern, flags)
 
-    def compile_pattern_cs(self, raw_pattern: AnyStr) -> "regex.Pattern[AnyStr]":
+    def compile_pattern_cs(
+        self, raw_pattern: AnyStr
+    ) -> "regex.Pattern[AnyStr]":
         return self.compile_pattern(raw_pattern)
 
-    def compile_pattern_ci(self, raw_pattern: AnyStr) -> "regex.Pattern[AnyStr]":
+    def compile_pattern_ci(
+        self, raw_pattern: AnyStr
+    ) -> "regex.Pattern[AnyStr]":
         return self.compile_pattern(raw_pattern, flags=regex.IGNORECASE)
 
-    def compile_pattern_cf(self, raw_pattern: AnyStr) -> "regex.Pattern[AnyStr]":
+    def compile_pattern_cf(
+        self, raw_pattern: AnyStr
+    ) -> "regex.Pattern[AnyStr]":
         return self.compile_pattern(
             raw_pattern, flags=regex.FULLCASE | regex.IGNORECASE
         )
 
-    def match_text(self, pattern: "regex.Pattern[AnyStr]", text: AnyStr) -> bool:
-        return bool(pattern.match(text))
-
-    def match_text_cf(self, pattern: "regex.Pattern[AnyStr]", text: AnyStr) -> bool:
+    def match_text(
+        self, pattern: "regex.Pattern[AnyStr]", text: AnyStr
+    ) -> bool:
+        return pattern.match(text) is not None
+
+    def match_text_cf(
+        self, pattern: "regex.Pattern[AnyStr]", text: AnyStr
+    ) -> bool:
         return self.match_text(pattern, text)
 
-    def match_text_ci(self, pattern: "regex.Pattern[AnyStr]", text: AnyStr) -> bool:
+    def match_text_ci(
+        self, pattern: "regex.Pattern[AnyStr]", text: AnyStr
+    ) -> bool:
         return self.match_text(pattern, text)
 
-    def match_text_cs(self, pattern: "regex.Pattern[AnyStr]", text: AnyStr) -> bool:
+    def match_text_cs(
+        self, pattern: "regex.Pattern[AnyStr]", text: AnyStr
+    ) -> bool:
         return self.match_text(pattern, text)
 
     @classmethod
     def get_type(cls) -> str:
         return "regex"
```

### Comparing `polymatch-0.3.0/polymatch/matchers/standard.py` & `polymatch-0.4.0/polymatch/matchers/standard.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/tests/base_test.py` & `polymatch-0.4.0/tests/base_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pytest
 
 from polymatch import pattern_registry
 from polymatch.base import CaseAction
-from polymatch.error import PatternNotCompiledError, PatternTextTypeMismatchError
+from polymatch.error import (
+    PatternNotCompiledError,
+    PatternTextTypeMismatchError,
+)
 from polymatch.matchers.standard import ExactMatcher
 
 
 def test_case_action_validate() -> None:
     with pytest.raises(
         TypeError, match="Case-folding is not supported with bytes patterns"
     ):
```

### Comparing `polymatch-0.3.0/tests/test_glob.py` & `polymatch-0.4.0/tests/test_glob.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/tests/test_pickling.py` & `polymatch-0.4.0/tests/test_pickling.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,30 +33,32 @@
 
     assert compiled_pattern.is_compiled()
 
     uncompiled_pattern = pattern_registry.pattern_from_string(pattern)
 
     assert not uncompiled_pattern.is_compiled()
 
-    pat1, pat2 = cycle_pickle((compiled_pattern, uncompiled_pattern), pickle_proto)
+    pat1, pat2 = cycle_pickle(
+        (compiled_pattern, uncompiled_pattern), pickle_proto
+    )
 
     assert pat1.is_compiled() is compiled_pattern.is_compiled()
 
     assert pat2.is_compiled() is uncompiled_pattern.is_compiled()
 
 
 @pytest.mark.parametrize(
     ("pattern", "pickle_proto"),
     itertools.product(patterns, range(pickle.HIGHEST_PROTOCOL + 1)),
 )
 def test_properties(pattern: str, pickle_proto: int) -> None:
     pat = pattern_registry.pattern_from_string(pattern)
     pat.compile()
 
-    inv_pat = pattern_registry.pattern_from_string("~" + pattern)
+    inv_pat = pattern_registry.pattern_from_string(f"~{pattern}")
     inv_pat.compile()
 
     assert not pat.inverted
     assert inv_pat.inverted
 
     new_pat = cycle_pickle(pat, pickle_proto)
     new_inv_pat = cycle_pickle(inv_pat, pickle_proto)
```

### Comparing `polymatch-0.3.0/tests/test_regex.py` & `polymatch-0.4.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/tests/test_registry.py` & `polymatch-0.4.0/tests/test_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     assert not matcher.match("Foo")
     assert isinstance(matcher, ExactMatcher)
     assert not matcher.inverted
     assert matcher.case_action == CaseAction.NONE
 
 
 def test_parse_error_bad_type() -> None:
-    with pytest.raises(TypeError, match="Unable to parse pattern string of type 'int'"):
+    with pytest.raises(
+        TypeError, match="Unable to parse pattern string of type 'int'"
+    ):
         pattern_registry.pattern_from_string(27)  # type: ignore[type-var]
 
 
 def test_parse_error_no_matcher() -> None:
     with pytest.raises(LookupError, match="av"):
         pattern_registry.pattern_from_string("av:cs:foo")
```

### Comparing `polymatch-0.3.0/tests/test_standard.py` & `polymatch-0.4.0/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/LICENSE` & `polymatch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatch-0.3.0/pyproject.toml` & `polymatch-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "polymatch"
 dynamic = ["version"]
 description = "A polymorphic pattern matching library for Python"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
-authors = [{ name = "linuxdaemon", email = "linuxdaemon@snoonet.org" }]
+authors = [{ name = "linuxdaemon", email = "linuxdaemon.irc@gmail.com" }]
 keywords = ["library", "pattern-matching", "utility", "regex"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -23,15 +23,24 @@
 ]
 dependencies = ["typing-extensions", "regex"]
 
 [project.urls]
 Homepage = "https://github.com/TotallyNotRobots/polymatch"
 
 [tool.hatch.version]
-path = "polymatch/__init__.py"
+source = "vcs"
+
+[tool.hatch.build.targets.sdist]
+exclude = ["/.github"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["polymatch"]
+
+[tool.hatch.build.hooks.vcs]
+version-file = "polymatch/_version.py"
 
 [tool.hatch.env]
 requires = ["hatch-containers"]
 
 [tool.hatch.envs.default]
 dependencies = [
     "coverage[toml]>=6.5",
@@ -48,55 +57,58 @@
     "- coverage combine",
     "coverage xml",
     "coverage report --show-missing",
 ]
 cov = ["- coverage erase", "test-cov", "cov-report"]
 cov-all = ["- coverage erase", "hatch run testall:test-cov", "cov-report"]
 
-setup-pre-commit = "python3 -m pre_commit install --install-hooks"
+setup-pre-commit = "python3 -m pre_commit install --install-hooks -t commit-msg -t pre-push -t pre-commit"
 setup-dev = ["setup-pre-commit"]
 
 pre-commit = "python3 -m pre_commit run {args:--all}"
 
 [tool.hatch.envs.testall]
 type = "container"
 dependencies = ["coverage[toml]>=6.5", "pytest>=6.0"]
 
 [[tool.hatch.envs.testall.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.isort]
 profile = "black"
-line_length = 88
+line_length = 80
 include_trailing_comma = true
 use_parentheses = true
 known_first_party = ["polymatch"]
 float_to_top = true
 
 [tool.black]
-line-length = 88
+line-length = 80
 target-version = ["py38"]
 include = '\.pyi?$'
 
 [tool.ruff]
-line-length = 88
+line-length = 80
 target-version = 'py38'
 
 [tool.ruff.format]
 docstring-code-format = true
 line-ending = "lf"
 skip-magic-trailing-comma = true
 
 [tool.ruff.lint]
 ignore-init-module-imports = false
 extend-safe-fixes = [
     "EM101",
     "EM102",
     "EM103",
+    "FLY002",
     "TCH001",
+    "TCH002",
+    "TRY400",
     "SIM117",
     "SIM108",
     "ANN201",
 ]
 ignore = [
     "D",
     "TRY003", # TODO(aspen): Switch to custom exceptions
@@ -113,68 +125,80 @@
 "tests/*.py" = [
     "PLR2004", # Allow "magic values" in tests -aspen
     "S101",    # Allow asserts in tests
     "S301",    # Allow pickle in tests
     "SIM201",  # We need to test weird comparison operators
     "SIM202",  # We need to test weird comparison operstors
     "SIM300",  # We need to test both forward and reverse comparisons
-    "FBT001",  # Boolean paramters are fine for test cases
+    "FBT001",  # Boolean parameters are fine for test cases
 ]
 
 [tool.ruff.lint.pycodestyle]
 max-line-length = 100
 
 [tool.ruff.lint.isort]
 split-on-trailing-comma = false
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
+[tool.flynt]
+aggressive = true
+transform-joins = true
+transform-concats = true
+
 [tool.mypy]
 namespace_packages = true
 python_version = "3.8"
 warn_unused_configs = true
 strict = true
 strict_optional = true
-ignore_missing_imports = true
 check_untyped_defs = true
 show_error_codes = true
 warn_unused_ignores = true
 no_implicit_reexport = true
 warn_redundant_casts = true
 strict_equality = true
 disallow_any_generics = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_untyped_decorators = true
 extra_checks = true
 warn_unreachable = true
 warn_return_any = true
 warn_no_return = true
+incremental = false
 enable_error_code = [
     "redundant-self",
     "redundant-expr",
     "possibly-undefined",
     "truthy-bool",
     "truthy-iterable",
     "ignore-without-code",
-    "unused-awaitable",
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--doctest-modules"
 testpaths = ["polymatch", "tests"]
 filterwarnings = ["error"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
-    'if __name__ == .__main__.:',
-    'if TYPE_CHECKING:',
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
 ]
 
 [tool.coverage.run]
 branch = true
 relative_files = true
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+tag_format = "v$version"
+version_scheme = "semver"
+version_provider = "scm"
+update_changelog_on_bump = true
+major_version_zero = true
```

