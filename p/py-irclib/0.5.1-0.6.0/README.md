# Comparing `tmp/py_irclib-0.5.1.tar.gz` & `tmp/py_irclib-0.6.0.tar.gz`

## Comparing `py_irclib-0.5.1.tar` & `py_irclib-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.editorconfig
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 py_irclib-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 py_irclib-0.5.1/codecov.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.vscode/extensions.json
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.vscode/settings.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/__init__.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/errors.py
--rw-r--r--   0        0        0    17230 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/py.typed
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/util/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/util/commands.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/util/compare.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/util/frozendict.py
--rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/util/numerics.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 py_irclib-0.5.1/irclib/util/string.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/commands_test.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/frozendict_test.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/numerics_test.py
--rw-r--r--   0        0        0    27838 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/parser_test.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/string_test.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/test_construct.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 py_irclib-0.5.1/tests/test_masks.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 py_irclib-0.5.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 py_irclib-0.5.1/LICENSE
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 py_irclib-0.5.1/README.md
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 py_irclib-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 py_irclib-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.editorconfig
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 py_irclib-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 py_irclib-0.6.0/codecov.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/_version.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/errors.py
+-rw-r--r--   0        0        0    17235 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/py.typed
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/util/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/util/commands.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/util/compare.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/util/frozendict.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/util/numerics.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 py_irclib-0.6.0/irclib/util/string.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/commands_test.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/frozendict_test.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/numerics_test.py
+-rw-r--r--   0        0        0    28369 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/parser_test.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/string_test.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/test_construct.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 py_irclib-0.6.0/tests/test_masks.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 py_irclib-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 py_irclib-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 py_irclib-0.6.0/README.md
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 py_irclib-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 py_irclib-0.6.0/PKG-INFO
```

### Comparing `py_irclib-0.5.1/.pre-commit-config.yaml` & `py_irclib-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/.devcontainer/devcontainer.json` & `py_irclib-0.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/irclib/parser.py` & `py_irclib-0.6.0/irclib/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,18 +126,18 @@
     def __str__(self) -> str:
         if self.value:
             return CAP_VALUE_SEP.join((self.name, self.value))
 
         return self.name
 
     @classmethod
-    def parse(cls, text: str) -> "Cap":
+    def parse(cls, text: str) -> Self:
         """Parse a CAP entity from a string"""
         name, _, value = text.partition(CAP_VALUE_SEP)
-        return Cap(name, value or None)
+        return cls(name, value or None)
 
 
 class CapList(Parseable, List[Cap]):
     """Represents a list of CAP entities"""
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, str):
@@ -157,29 +157,29 @@
 
         return NotImplemented
 
     def __str__(self) -> str:
         return CAP_SEP.join(map(str, self))
 
     @classmethod
-    def parse(cls, text: str) -> "CapList":
+    def parse(cls, text: str) -> Self:
         """Parse a list of CAPs from a string"""
         if text.startswith(":"):
             text = text[1:]  # Remove leading colon
 
         # We want to strip any leading or trailing whitespace
         # Some networks (ie: freenode) send a trailing space in a CAP ACK
         stripped = text.strip()
 
         caps: Iterable[Cap]
         caps = (
             [] if not text else (Cap.parse(s) for s in stripped.split(CAP_SEP))
         )
 
-        return CapList(caps)
+        return cls(caps)
 
 
 class MessageTag(Parseable):
     """
     Basic class to wrap a message tag
     """
 
@@ -255,26 +255,26 @@
 
         if isinstance(other, MessageTag):
             return not (self.name == other.name and self.value == other.value)
 
         return NotImplemented
 
     @classmethod
-    def parse(cls, text: str) -> "MessageTag":
+    def parse(cls, text: str) -> Self:
         """
         Parse a tag from a string
 
         :param text: The basic tag string
         :return: The MessageTag object
         """
         name, sep, value = text.partition(TAG_VALUE_SEP)
         if value:
             value = MessageTag.unescape(value)
 
-        return MessageTag(name, value, has_value=bool(sep))
+        return cls(name, value, has_value=bool(sep))
 
 
 class TagList(Parseable, Dict[str, MessageTag]):
     """Object representing the list of message tags on a line"""
 
     def __init__(self, tags: Iterable[MessageTag] = ()) -> None:
         super().__init__((tag.name, tag) for tag in tags)
@@ -312,29 +312,27 @@
         obj = self._cmp_type_map(other)
         if obj is NotImplemented:
             return NotImplemented
 
         return dict(self) != dict(obj)
 
     @classmethod
-    def parse(cls, text: str) -> "TagList":
+    def parse(cls, text: str) -> Self:
         """
         Parse the list of tags from a string
 
         :param text: The string to parse
         :return: The parsed object
         """
-        return TagList(
-            map(MessageTag.parse, filter(None, text.split(TAGS_SEP)))
-        )
+        return cls(map(MessageTag.parse, filter(None, text.split(TAGS_SEP))))
 
-    @staticmethod
-    def from_dict(tags: Dict[str, str]) -> "TagList":
+    @classmethod
+    def from_dict(cls, tags: Dict[str, str]) -> Self:
         """Create a TagList from a dict of tags"""
-        return TagList(MessageTag(k, v) for k, v in tags.items())
+        return cls(MessageTag(k, v) for k, v in tags.items())
 
 
 class Prefix(Parseable):
     """
     Object representing the prefix of a line
     """
 
@@ -410,32 +408,32 @@
 
         if isinstance(other, Prefix):
             return self._data != other._data
 
         return NotImplemented
 
     @classmethod
-    def parse(cls, text: str) -> "Prefix":
+    def parse(cls, text: str) -> Self:
         """
         Parse the prefix from a string
 
         :param text: String to parse
         :return: Parsed Object
         """
         if not text:
-            return Prefix()
+            return cls()
 
         match = PREFIX_RE.match(text)
         if not match:  # pragma: no cover
             # This should never trip, we are pretty lenient with prefixes
             msg = "Invalid IRC prefix format"
             raise ParseError(msg)
 
         nick, user, host = match.groups()
-        return Prefix(nick, user, host)
+        return cls(nick, user, host)
 
 
 class ParamList(Parseable, List[str]):
     """
     An object representing the parameter list from a line
     """
 
@@ -477,32 +475,32 @@
             return self != self.parse(other)
 
         if isinstance(other, list):
             return list(self) != list(other)
 
         return NotImplemented
 
-    @staticmethod
-    def from_list(data: Sequence[str]) -> "ParamList":
+    @classmethod
+    def from_list(cls, data: Sequence[str]) -> Self:
         """Create a ParamList from a Sequence of strings."""
         if not data:
-            return ParamList()
+            return cls()
 
         args = list(data[:-1])
         if data[-1].startswith(TRAIL_SENTINEL) or not data[-1]:
             has_trail = True
             args.append(data[-1])
         else:
             has_trail = False
             args.append(data[-1])
 
-        return ParamList(*args, has_trail=has_trail)
+        return cls(*args, has_trail=has_trail)
 
     @classmethod
-    def parse(cls, text: str) -> "ParamList":
+    def parse(cls, text: str) -> Self:
         """
         Parse a list of parameters
 
         :param text: The list of parameters
         :return: The parsed object
         """
         args = []
@@ -513,15 +511,15 @@
                 has_trail = True
                 break
 
             arg, _, text = text.partition(PARAM_SEP)
             if arg:
                 args.append(arg)
 
-        return ParamList(*args, has_trail=has_trail)
+        return cls(*args, has_trail=has_trail)
 
 
 def _parse_tags(
     tags: Union[TagList, Dict[str, str], str, None, List[str]],
 ) -> MsgTagList:
     if isinstance(tags, TagList):
         return tags
@@ -635,17 +633,20 @@
 
         if isinstance(other, Message):
             return self.as_tuple() != other.as_tuple()
 
         return NotImplemented
 
     @classmethod
-    def parse(cls, text: Union[str, bytes]) -> "Message":
+    def parse(cls, text: Union[str, bytes]) -> Self:
         """Parse an IRC message in to objects"""
-        if isinstance(text, bytes):
+        if isinstance(text, memoryview):
+            text = text.tobytes().decode(errors="ignore")
+
+        if isinstance(text, (bytes, bytearray)):
             text = text.decode(errors="ignore")
 
         tags = ""
         prefix = ""
         if text.startswith(TAGS_SENTINEL):
             tags, _, text = text.partition(PARAM_SEP)
 
@@ -655,8 +656,8 @@
         command, _, params = text.partition(PARAM_SEP)
         # Differentiate empty tags '@ CMD' from no tags 'CMD'
         tags_obj = TagList.parse(tags[1:]) if tags else None
         # Differentiate empty prefix ': CMD' from no prefix 'CMD'
         prefix_obj = Prefix.parse(prefix[1:]) if prefix else None
         command = command.upper()
         param_obj = ParamList.parse(params)
-        return Message(tags_obj, prefix_obj, command, param_obj)
+        return cls(tags_obj, prefix_obj, command, param_obj)
```

### Comparing `py_irclib-0.5.1/irclib/util/commands.py` & `py_irclib-0.6.0/irclib/util/commands.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/irclib/util/frozendict.py` & `py_irclib-0.6.0/irclib/util/frozendict.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/irclib/util/numerics.py` & `py_irclib-0.6.0/irclib/util/numerics.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/irclib/util/string.py` & `py_irclib-0.6.0/irclib/util/string.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/tests/commands_test.py` & `py_irclib-0.6.0/tests/commands_test.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/tests/frozendict_test.py` & `py_irclib-0.6.0/tests/frozendict_test.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/tests/parser_test.py` & `py_irclib-0.6.0/tests/parser_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -703,14 +703,26 @@
 
     def test_parse_bytes(self) -> None:
         """Test parsing bytes"""
         line = Message.parse(b"COMMAND some params :and stuff")
         assert line.command == "COMMAND"
         assert line.parameters == ["some", "params", "and stuff"]
 
+    def test_parse_bytearray(self) -> None:
+        """Test parsing bytearray"""
+        line = Message.parse(bytearray(b"COMMAND some params :and stuff"))
+        assert line.command == "COMMAND"
+        assert line.parameters == ["some", "params", "and stuff"]
+
+    def test_parse_memoryview(self) -> None:
+        """Test parsing memoryview"""
+        line = Message.parse(memoryview(b"COMMAND some params :and stuff"))
+        assert line.command == "COMMAND"
+        assert line.parameters == ["some", "params", "and stuff"]
+
     @pytest.mark.parametrize(
         ("obj", "text"),
         [
             (Message(None, None, None), ""),
             (Message(None, None, None, None), ""),
             (Message(None, None, None, []), ""),
             (Message(None, None, "COMMAND"), "COMMAND"),
```

### Comparing `py_irclib-0.5.1/tests/string_test.py` & `py_irclib-0.6.0/tests/string_test.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/tests/test_construct.py` & `py_irclib-0.6.0/tests/test_construct.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/tests/test_masks.py` & `py_irclib-0.6.0/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/.gitignore` & `py_irclib-0.6.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,45 @@
 # Created by .ignore support plugin (hsz.mobi)
+### VirtualEnv template
+# Virtualenv
+# http://iamzed.com/2009/05/07/a-primer-on-virtualenv/
+.Python
+[Bb]in
+[Ii]nclude
+[Ll]ib
+[Ll]ib64
+[Ll]ocal
+[Ss]cripts
+pyvenv.cfg
+.venv
+pip-selfcheck.json
+### Linux template
+*~
+
+# temporary files which can be created if a process still has a handle open of a deleted file
+.fuse_hidden*
+
+# KDE directory preferences
+.directory
+
+# Linux trash folder which might appear on any partition or disk
+.Trash-*
+
+# .nfs files are created when an open file is removed but is still being accessed
+.nfs*
 ### Python template
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
-.Python
 env/
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
@@ -22,15 +48,14 @@
 parts/
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
 *.egg
-MANIFEST
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
@@ -42,15 +67,15 @@
 htmlcov/
 .tox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
-*.cover
+*,cover
 .hypothesis/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
@@ -82,43 +107,22 @@
 # SageMath parsed files
 *.sage.py
 
 # dotenv
 .env
 
 # virtualenv
-.venv
 venv/
 ENV/
-env.bak/
-venv.bak/
 
 # Spyder project settings
 .spyderproject
-.spyproject
 
 # Rope project settings
 .ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-### VirtualEnv template
-# Virtualenv
-# http://iamzed.com/2009/05/07/a-primer-on-virtualenv/
-[Bb]in
-[Ii]nclude
-[Ll]ib
-[Ll]ib64
-[Ll]ocal
-[Ss]cripts
-pyvenv.cfg
-pip-selfcheck.json
 ### JetBrains template
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio and Webstorm
 # Reference: https://intellij-support.jetbrains.com/hc/en-us/articles/206544839
 
 # User-specific stuff:
 .idea/**/workspace.xml
 .idea/**/tasks.xml
@@ -133,68 +137,49 @@
 .idea/**/dynamic.xml
 .idea/**/uiDesigner.xml
 
 # Gradle:
 .idea/**/gradle.xml
 .idea/**/libraries
 
-# CMake
-cmake-build-debug/
-
 # Mongo Explorer plugin:
 .idea/**/mongoSettings.xml
 
 ## File-based project format:
 *.iws
 
 ## Plugin-specific files:
 
 # IntelliJ
-out/
+/out/
 
 # mpeltonen/sbt-idea plugin
 .idea_modules/
 
 # JIRA plugin
 atlassian-ide-plugin.xml
 
-# Cursive Clojure plugin
-.idea/replstate.xml
-
 # Crashlytics plugin (for Android Studio and IntelliJ)
 com_crashlytics_export_strings.xml
 crashlytics.properties
 crashlytics-build.properties
 fabric.properties
-### Linux template
-*~
-
-# temporary files which can be created if a process still has a handle open of a deleted file
-.fuse_hidden*
-
-# KDE directory preferences
-.directory
-
-# Linux trash folder which might appear on any partition or disk
-.Trash-*
-
-# .nfs files are created when an open file is removed but is still being accessed
-.nfs*
 ### Vim template
-# Swap
+# swap
 [._]*.s[a-v][a-z]
 [._]*.sw[a-p]
 [._]s[a-v][a-z]
 [._]sw[a-p]
-
-# Session
+# session
 Session.vim
-
-# Temporary
+# temporary
 .netrwhist
-# Auto-generated tag files
+# auto-generated tag files
 tags
 
+*/_version.py
+
+.mypy_cache/
 .pytest_cache/
 .ruff_cache/
-
+coverage.*
 .coverage.*
```

### Comparing `py_irclib-0.5.1/LICENSE` & `py_irclib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/README.md` & `py_irclib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `py_irclib-0.5.1/pyproject.toml` & `py_irclib-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/.github"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["irclib"]
 
+[tool.hatch.build.hooks.vcs]
+version-file = "irclib/_version.py"
+
 [tool.hatch.env]
 requires = ["hatch-containers"]
 
 [tool.hatch.envs.default]
 dependencies = [
     "coverage[toml]>=6.5",
     "pytest>=6.0",
@@ -94,15 +97,18 @@
 
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
@@ -151,22 +157,22 @@
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
 testpaths = ["irclib", "tests"]
 filterwarnings = ["error"]
```

### Comparing `py_irclib-0.5.1/PKG-INFO` & `py_irclib-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-irclib
-Version: 0.5.1
+Version: 0.6.0
 Summary: A simple library for working with the IRC protocol
 Project-URL: Homepage, https://github.com/TotallyNotRobots/py-irclib
 Author-email: linuxdaemon <linuxdaemon.irc@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: irc,irc-parser
 Classifier: Development Status :: 3 - Alpha
```

