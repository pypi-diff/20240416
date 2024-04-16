# Comparing `tmp/RegexFactory-1.0.0.tar.gz` & `tmp/regexfactory-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RegexFactory-1.0.0.tar", last modified: Sat Mar 12 04:13:51 2022, max compression
+gzip compressed data, was "regexfactory-1.0.1.tar", last modified: Tue Apr 16 15:40:08 2024, max compression
```

## Comparing `RegexFactory-1.0.0.tar` & `regexfactory-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-03-12 04:13:51.042615 RegexFactory-1.0.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    35149 2022-03-10 22:38:58.000000 RegexFactory-1.0.0/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3037 2022-03-12 04:13:51.042615 RegexFactory-1.0.0/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2393 2022-03-10 22:38:58.000000 RegexFactory-1.0.0/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-03-12 04:13:51.042615 RegexFactory-1.0.0/RegexFactory.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3037 2022-03-12 04:13:50.000000 RegexFactory-1.0.0/RegexFactory.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      307 2022-03-12 04:13:50.000000 RegexFactory-1.0.0/RegexFactory.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2022-03-12 04:13:50.000000 RegexFactory-1.0.0/RegexFactory.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2022-03-12 04:13:50.000000 RegexFactory-1.0.0/RegexFactory.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2022-03-08 19:39:56.000000 RegexFactory-1.0.0/RegexFactory.egg-info/zip-safe
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-03-12 04:13:51.042615 RegexFactory-1.0.0/regexfactory/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      308 2022-03-12 04:13:47.000000 RegexFactory-1.0.0/regexfactory/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2823 2022-03-12 01:04:42.000000 RegexFactory-1.0.0/regexfactory/chars.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4909 2022-03-12 04:13:08.000000 RegexFactory-1.0.0/regexfactory/pattern.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14245 2022-03-12 04:13:11.000000 RegexFactory-1.0.0/regexfactory/patterns.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      958 2022-03-12 04:13:51.042615 RegexFactory-1.0.0/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       57 2022-03-10 22:38:58.000000 RegexFactory-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:40:08.749889 regexfactory-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 15:40:03.000000 regexfactory-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-16 15:40:08.749889 regexfactory-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-16 15:40:03.000000 regexfactory-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:40:08.749889 regexfactory-1.0.1/RegexFactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-16 15:40:08.000000 regexfactory-1.0.1/RegexFactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 15:40:08.000000 regexfactory-1.0.1/RegexFactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:40:08.000000 regexfactory-1.0.1/RegexFactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 15:40:08.000000 regexfactory-1.0.1/RegexFactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 15:40:08.000000 regexfactory-1.0.1/RegexFactory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:40:08.000000 regexfactory-1.0.1/RegexFactory.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:40:08.749889 regexfactory-1.0.1/regexfactory/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-16 15:40:03.000000 regexfactory-1.0.1/regexfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-16 15:40:03.000000 regexfactory-1.0.1/regexfactory/chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-16 15:40:03.000000 regexfactory-1.0.1/regexfactory/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13891 2024-04-16 15:40:03.000000 regexfactory-1.0.1/regexfactory/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-16 15:40:08.749889 regexfactory-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-16 15:40:03.000000 regexfactory-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:40:08.749889 regexfactory-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-16 15:40:03.000000 regexfactory-1.0.1/tests/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 15:40:03.000000 regexfactory-1.0.1/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 15:40:03.000000 regexfactory-1.0.1/tests/test_or.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-16 15:40:03.000000 regexfactory-1.0.1/tests/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 15:40:03.000000 regexfactory-1.0.1/tests/test_set.py
```

### Comparing `RegexFactory-1.0.0/LICENSE` & `regexfactory-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RegexFactory-1.0.0/PKG-INFO` & `regexfactory-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: RegexFactory
-Version: 1.0.0
-Summary: UNKNOWN
+Version: 1.0.1
 Author: GrandMoff100
 Author-email: nlarsen23.student@gmail.com
 License: GPLv3
 Keywords: regex,generator,regular expression,strings
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: hypothesis; extra == "dev"
 
 # RegexFactory
 
 Dynamically construct python regex patterns.
 
 ## Examples
 
 ### Matching Initials
+
 Say you want a regex pattern to match the initials of someones name.
 
 ```python
 import re
 from regexfactory import Amount, Range
 
 
 pattern = Amount(Range("A", "Z"), 2, 3)
 
-matches = re.findall(
-    str(pattern),
+matches = pattern.findall(
     "My initials are BDP. Valorie's are VO"
 )
 
 print(matches)
 ```
 
-```
+```bash
 ['BDP', 'VO']
 ```
 
 ### Matching Hex Strings
 
 Or how matching both uppercase and lowercase hex strings in a sentence.
 
@@ -71,58 +76,58 @@
 
 )
 
 sentence = """
 My favorite color is #000000. I also like 5fb8a0. My second favorite color is #FF21FF.
 """
 
-matches = re.findall(
-    str(pattern),
-    sentence
-)
+matches = pattern.findall(sentence)
 print(matches)
 ```
 
-```
+```bash
 ['#000000', '5fb8a0', '#FF21FF']
 ```
 
 ### Matching URLs
 
 Or what if you want to match urls in html content?
 
 ```python
 from regexfactory import *
-import re
 
 
 protocol = Amount(Range("a", "z"), 1, or_more=True)
 host = Amount(Set(WORD, DIGIT, '.'), 1, or_more=True)
-port = Optional(Group(RegexPattern(":") + Amount(DIGIT, 1, or_more=True)))
-path = Amount(Group(RegexPattern('/') + Group(Amount(NotSet('/', '#', '?', '&', WHITESPACE), 0, or_more=True))), 0, or_more=True)
+port = Optional(IfBehind(":") + Multi(DIGIT))
+path = Multi(
+    RegexPattern('/') + Multi(
+        NotSet('/', '#', '?', '&', WHITESPACE),
+        match_zero=True
+    ),
+    match_zero=True
+)
 patt = protocol + RegexPattern("://") + host + port + path
 
 
 
 sentence = "This is a cool url, https://github.com/GrandMoff100/RegexFactory/ "
 print(patt)
 
-print(re.search(str(patt), sentence))
+print(patt.search(sentence))
 ```
 
-```
-[a-z]{1,}://[\w\d.]{1,}(:\d{1,})?(/([^/#?&\s]{0,})){0,}
+```bash
+[a-z]{1,}://[\w\d.]{1,}(?:\d{1,})?(/([^/#?&\s]{0,})){0,}
 <re.Match object; span=(15, 51), match='https://github.com/GrandMoff100/RegexFactory/'>
 ```
 
 ## The Pitch
 
 This library is really good at allowing you to intuitively understand how to construct a regex expression.
 It helps you identify what exactly your regular expression is, and can help you debug it.
 This is library is also very helpful for generating regex expressions on the fly if you find uses for it.
 You can also extend this library by subclassing `RegexPattern` and add your own support for different regex flavors.
 Like generating regex expresison with Perl5 extensions.
 
 There you have it. This library is intuitive, extensible, modular, and dynamic.
 Why not use it?
-
-
```

### Comparing `RegexFactory-1.0.0/README.md` & `regexfactory-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # RegexFactory
 
 Dynamically construct python regex patterns.
 
 ## Examples
 
 ### Matching Initials
+
 Say you want a regex pattern to match the initials of someones name.
 
 ```python
 import re
 from regexfactory import Amount, Range
 
 
 pattern = Amount(Range("A", "Z"), 2, 3)
 
-matches = re.findall(
-    str(pattern),
+matches = pattern.findall(
     "My initials are BDP. Valorie's are VO"
 )
 
 print(matches)
 ```
 
-```
+```bash
 ['BDP', 'VO']
 ```
 
 ### Matching Hex Strings
 
 Or how matching both uppercase and lowercase hex strings in a sentence.
 
@@ -52,50 +52,52 @@
 
 )
 
 sentence = """
 My favorite color is #000000. I also like 5fb8a0. My second favorite color is #FF21FF.
 """
 
-matches = re.findall(
-    str(pattern),
-    sentence
-)
+matches = pattern.findall(sentence)
 print(matches)
 ```
 
-```
+```bash
 ['#000000', '5fb8a0', '#FF21FF']
 ```
 
 ### Matching URLs
 
 Or what if you want to match urls in html content?
 
 ```python
 from regexfactory import *
-import re
 
 
 protocol = Amount(Range("a", "z"), 1, or_more=True)
 host = Amount(Set(WORD, DIGIT, '.'), 1, or_more=True)
-port = Optional(Group(RegexPattern(":") + Amount(DIGIT, 1, or_more=True)))
-path = Amount(Group(RegexPattern('/') + Group(Amount(NotSet('/', '#', '?', '&', WHITESPACE), 0, or_more=True))), 0, or_more=True)
+port = Optional(IfBehind(":") + Multi(DIGIT))
+path = Multi(
+    RegexPattern('/') + Multi(
+        NotSet('/', '#', '?', '&', WHITESPACE),
+        match_zero=True
+    ),
+    match_zero=True
+)
 patt = protocol + RegexPattern("://") + host + port + path
 
 
 
 sentence = "This is a cool url, https://github.com/GrandMoff100/RegexFactory/ "
 print(patt)
 
-print(re.search(str(patt), sentence))
+print(patt.search(sentence))
 ```
 
-```
-[a-z]{1,}://[\w\d.]{1,}(:\d{1,})?(/([^/#?&\s]{0,})){0,}
+```bash
+[a-z]{1,}://[\w\d.]{1,}(?:\d{1,})?(/([^/#?&\s]{0,})){0,}
 <re.Match object; span=(15, 51), match='https://github.com/GrandMoff100/RegexFactory/'>
 ```
 
 ## The Pitch
 
 This library is really good at allowing you to intuitively understand how to construct a regex expression.
 It helps you identify what exactly your regular expression is, and can help you debug it.
```

### Comparing `RegexFactory-1.0.0/RegexFactory.egg-info/PKG-INFO` & `regexfactory-1.0.1/RegexFactory.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 Metadata-Version: 2.1
 Name: RegexFactory
-Version: 1.0.0
-Summary: UNKNOWN
+Version: 1.0.1
 Author: GrandMoff100
 Author-email: nlarsen23.student@gmail.com
 License: GPLv3
 Keywords: regex,generator,regular expression,strings
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: hypothesis; extra == "dev"
 
 # RegexFactory
 
 Dynamically construct python regex patterns.
 
 ## Examples
 
 ### Matching Initials
+
 Say you want a regex pattern to match the initials of someones name.
 
 ```python
 import re
 from regexfactory import Amount, Range
 
 
 pattern = Amount(Range("A", "Z"), 2, 3)
 
-matches = re.findall(
-    str(pattern),
+matches = pattern.findall(
     "My initials are BDP. Valorie's are VO"
 )
 
 print(matches)
 ```
 
-```
+```bash
 ['BDP', 'VO']
 ```
 
 ### Matching Hex Strings
 
 Or how matching both uppercase and lowercase hex strings in a sentence.
 
@@ -71,58 +76,58 @@
 
 )
 
 sentence = """
 My favorite color is #000000. I also like 5fb8a0. My second favorite color is #FF21FF.
 """
 
-matches = re.findall(
-    str(pattern),
-    sentence
-)
+matches = pattern.findall(sentence)
 print(matches)
 ```
 
-```
+```bash
 ['#000000', '5fb8a0', '#FF21FF']
 ```
 
 ### Matching URLs
 
 Or what if you want to match urls in html content?
 
 ```python
 from regexfactory import *
-import re
 
 
 protocol = Amount(Range("a", "z"), 1, or_more=True)
 host = Amount(Set(WORD, DIGIT, '.'), 1, or_more=True)
-port = Optional(Group(RegexPattern(":") + Amount(DIGIT, 1, or_more=True)))
-path = Amount(Group(RegexPattern('/') + Group(Amount(NotSet('/', '#', '?', '&', WHITESPACE), 0, or_more=True))), 0, or_more=True)
+port = Optional(IfBehind(":") + Multi(DIGIT))
+path = Multi(
+    RegexPattern('/') + Multi(
+        NotSet('/', '#', '?', '&', WHITESPACE),
+        match_zero=True
+    ),
+    match_zero=True
+)
 patt = protocol + RegexPattern("://") + host + port + path
 
 
 
 sentence = "This is a cool url, https://github.com/GrandMoff100/RegexFactory/ "
 print(patt)
 
-print(re.search(str(patt), sentence))
+print(patt.search(sentence))
 ```
 
-```
-[a-z]{1,}://[\w\d.]{1,}(:\d{1,})?(/([^/#?&\s]{0,})){0,}
+```bash
+[a-z]{1,}://[\w\d.]{1,}(?:\d{1,})?(/([^/#?&\s]{0,})){0,}
 <re.Match object; span=(15, 51), match='https://github.com/GrandMoff100/RegexFactory/'>
 ```
 
 ## The Pitch
 
 This library is really good at allowing you to intuitively understand how to construct a regex expression.
 It helps you identify what exactly your regular expression is, and can help you debug it.
 This is library is also very helpful for generating regex expressions on the fly if you find uses for it.
 You can also extend this library by subclassing `RegexPattern` and add your own support for different regex flavors.
 Like generating regex expresison with Perl5 extensions.
 
 There you have it. This library is intuitive, extensible, modular, and dynamic.
 Why not use it?
-
-
```

### Comparing `RegexFactory-1.0.0/regexfactory/chars.py` & `regexfactory-1.0.1/regexfactory/chars.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 *******************
 
 Common regex special characters, such as :code:`\d`, :code:`.`, ...
 More information about special characters in python regex available
 `here <https://docs.python.org/3/library/re.html#regular-expression-syntax>`__
 """
 
-from .patterns import RegexPattern
+from .pattern import RegexPattern
 
 #: (Dot.) In the default mode, this matches any character except a newline. If the :data:`re.DOTALL` flag has been specified, this matches any character including a newline.
 ANY = RegexPattern(r".")
 
 #: (Caret.) Matches the start of the string, and in  :data:`re.MULTILINE` mode also matches immediately after each newline.
-ANCHOR_START = RegexPattern(r"^")
+ANCHOR_START = RegexPattern(r"^", _precedence=2)
 
 #: Matches the end of the string or just before the newline at the end of the string, and in :data:`re.MULTILINE` mode also matches before a newline. foo matches both :code:`foo` and :code:`foobar`, while the regular expression :code:`foo$` matches only :code:`foo`. More interestingly, searching for :code:`foo.$` in :code:`foo1\nfoo2\n` matches :code:`foo2` normally, but :code:`foo1` in  :data:`re.MULTILINE` mode; searching for a single $ in :code:`foo\n` will find two (empty) matches: one just before the newline, and one at the end of the string.
-ANCHOR_END = RegexPattern(r"$")
+ANCHOR_END = RegexPattern(r"$", _precedence=2)
 
 #: Matches Unicode whitespace characters (which includes :code:`[ \t\n\r\f\v]`, and also many other characters, for example the non-breaking spaces mandated by typography rules in many languages). If the :data:`re.ASCII` flag is used, only :code:`[ \t\n\r\f\v]` is matched.
 WHITESPACE = RegexPattern(r"\s")
 
 #: Matches any character which is not a whitespace character. This is the opposite of \s. If the :data:`re.ASCII` flag is used this becomes the equivalent of :code:`[^ \t\n\r\f\v]`.
 NOTWHITESPACE = RegexPattern(r"\S")
```

### Comparing `RegexFactory-1.0.0/regexfactory/pattern.py` & `regexfactory-1.0.1/regexfactory/pattern.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Base Pattern Module
 *******************
 
 Module for the :class:`RegexPattern` class.
 """
 
+# pylint: disable=cyclic-import
+
+
 import re
-from typing import Any, Generator, List, Optional, Tuple, Union
+from typing import Any, Iterator, List, Optional, Tuple, Union
 
 #:
 ValidPatternType = Union[re.Pattern, str, "RegexPattern"]
 
 #: Special characters that need to be escaped to be used without their special meanings.
 ESCAPED_CHARACTERS = "()[]{}?*+-|^$\\.&~#"
 
@@ -31,46 +34,93 @@
 class RegexPattern:
     """
     The main object that represents Regular Expression Pattern strings for this library.
     """
 
     regex: str
 
-    def __init__(self, pattern: ValidPatternType, /) -> None:
+    #: The precedence of the pattern. Higher precedence patterns are evaluated first.
+    # Precedence order here (https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap09.html#tag_09_04_08)
+    precedence: int
+
+    def __init__(self, pattern: ValidPatternType, /, _precedence: int = 1) -> None:
         self.regex = self.get_regex(pattern)
+        self.precedence = (
+            _precedence if not isinstance(pattern, RegexPattern) else pattern.precedence
+        )
 
     def __repr__(self) -> str:
         raw_regex = f"{self.regex!r}".replace("\\\\", "\\")
         return f"<RegexPattern {raw_regex}>"
 
     def __str__(self) -> str:
         return self.regex
 
     def __add__(self, other: ValidPatternType) -> "RegexPattern":
         """Adds two :class:`ValidPatternType`'s together, into a :class:`RegexPattern`"""
+        from .patterns import Group  # pylint: disable=import-outside-toplevel
+
+        try:
+            other_pattern = (
+                RegexPattern(other) if not isinstance(other, RegexPattern) else other
+            )
+        except TypeError:
+            return NotImplemented
+
+        if self.precedence > other_pattern.precedence:
+            return RegexPattern(
+                self.regex + self.get_regex(Group(other_pattern, capturing=False))
+            )
+        if self.precedence < other_pattern.precedence:
+            return RegexPattern(
+                self.get_regex(Group(self, capturing=False)) + other_pattern.regex
+            )
+        return RegexPattern(self.regex + other_pattern.regex)
+
+    def __radd__(self, other: ValidPatternType) -> "RegexPattern":
+        """Adds two :class:`ValidPatternType`'s together, into a :class:`RegexPattern`"""
+        from .patterns import Group  # pylint: disable=import-outside-toplevel
+
         try:
-            other = self.get_regex(other)
+            other_pattern = (
+                RegexPattern(other) if not isinstance(other, RegexPattern) else other
+            )
         except TypeError:
             return NotImplemented
 
-        return RegexPattern(self.regex + other)
+        if self.precedence > other_pattern.precedence:
+            return RegexPattern(
+                self.get_regex(Group(other_pattern, capturing=False)) + self.regex
+            )
+        if self.precedence < other_pattern.precedence:
+            return RegexPattern(
+                other_pattern.regex + self.get_regex(Group(self, capturing=False))
+            )
+        return RegexPattern(other_pattern.regex + self.regex)
 
     def __mul__(self, coefficient: int) -> "RegexPattern":
         """Treats :class:`RegexPattern` as a string and multiplies it by an integer."""
         return RegexPattern(self.regex * coefficient)
 
     def __eq__(self, other: Any) -> bool:
         """
         Returns whether or not two :class:`ValidPatternType`'s have the same regex.
         Otherwise return false.
         """
         if isinstance(other, (str, re.Pattern, RegexPattern)):
-            return self.regex == self.get_regex(other)
+            return (
+                self.regex == RegexPattern(other).regex
+                and self.precedence == RegexPattern(other).precedence
+            )
         return super().__eq__(other)
 
+    def __hash__(self) -> int:
+        """Hashes the regex string."""
+        return hash(self.regex)
+
     @staticmethod
     def get_regex(obj: ValidPatternType, /) -> str:
         """
         Extracts the regex content from :class:`RegexPattern` or :class:`re.Pattern` objects
         else return the input :class:`str`.
         """
         if isinstance(obj, RegexPattern):
@@ -121,26 +171,26 @@
 
     def finditer(
         self,
         content: str,
         /,
         *,
         flags: int = 0,
-    ) -> Generator[re.Match, None, None]:
+    ) -> Iterator[re.Match]:
         """See :meth:`re.Pattern.finditer`."""
         return self.compile(flags=flags).finditer(content)
 
     def split(
         self,
         content: str,
         /,
         maxsplit: int = 0,
         *,
         flags: int = 0,
-    ) -> Tuple[str, ...]:
+    ) -> List[Any]:
         """See :meth:`re.Pattern.split`."""
         return self.compile(flags=flags).split(content, maxsplit=maxsplit)
 
     def sub(
         self,
         replacement: str,
         content: str,
```

### Comparing `RegexFactory-1.0.0/regexfactory/patterns.py` & `regexfactory-1.0.1/regexfactory/patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 
 class Or(RegexPattern):
     """
     For matching multiple patterns.
     This pattern `or` that pattern `or` that other pattern.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import Or
 
         patt = Or("Bob", "Alice", "Sally")
 
         print(patt.match("Alice"))
         print(patt.match("Bob"))
@@ -56,16 +55,15 @@
     to translate characters their Unicode numbers and back again.
     For example, :code:`chr(97)` returns the string :code:`'a'`,
     while :code:`chr(8364)` returns the string :code:`'€'`
     Thus, matching characters between :code:`'a'` and :code:`'z'`
     is really checking whether a characters unicode number
     is between :code:`ord('a')` and :code:`ord('z')`
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import Range, Or
 
         patt = Or("Bob", Range("a", "z"))
 
         print(patt.findall("my job is working for Bob"))
 
@@ -89,16 +87,15 @@
     functions the same as :code:`Or("a", ".", "z")`
     The difference being that :class:`Or` accepts :class:`RegexPattern` 's
     and :class:`Set` accepts characters only.
     Special characters do **NOT** lose their special meaings inside an :class:`Or` though.
     The other big difference is performance,
     :class:`Or` is a lot slower than :class:`Set`.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         import time
         from regexfactory import Or, Set
 
         start_set = time.time()
         print(patt := Set(*"a.z").compile())
         print("Set took", time.time() - start_set, "seconds to compile")
@@ -124,16 +121,15 @@
 
 
 class NotSet(RegexPattern):
     """
     For matching a character that is **NOT** in a list of characters.
     Keep in mind special characters lose their special meanings inside :class:`NotSet`'s as well.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import NotSet, Set
 
         not_abc = NotSet(*"abc")
 
         is_abc = Set(*"abc")
 
@@ -161,16 +157,15 @@
     You can also pass a :code:`greedy=False` keyword-argument  to :class:`Amount`,
     (default is True)
     which tells the regex compiler match as few characters as possible rather than
     the default behavior which is to match as many characters as possible.
 
     Best explained with an example.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import Amount, Set
 
         # We are using the same Pattern with different amounts.
 
         content = "acbccbaabbccaaca"
 
@@ -218,15 +213,15 @@
         pattern: ValidPatternType,
         match_zero: bool = False,
         greedy: bool = True,
     ):
         suffix = "*" if match_zero else "+"
         if greedy is False:
             suffix += "?"
-        regex = self.get_regex(pattern)
+        regex = self.get_regex(Group(pattern, capturing=False))
         super().__init__(regex + suffix)
 
 
 class Optional(RegexPattern):
     """
     Matches the passed :class:`ValidPatternType` between zero and one times.
     Functions the same as :code:`Amount(pattern, 0, 1)`.
@@ -245,16 +240,15 @@
         super().__init__(f"(?{prefix}{regex})")
 
 
 class NamedGroup(Extension):
     """
     Lets you sepparate your regex into named groups that you can extract from :meth:`re.Match.groupdict`.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import NamedGroup, WORD, Multi
 
         stuff = "George Washington"
 
         patt = NamedGroup("first_name", Multi(WORD)) + " " + NamedGroup("last_name", Multi(WORD))
 
@@ -268,16 +262,15 @@
         super().__init__(f"P<{self.name}>", pattern)
 
 
 class NamedReference(Extension):
     """
     Lets you reference :class:`NamedGroup`'s that you've already created, by name, or by passing the :class:`NamedGroup` itself.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import NamedReference, NamedGroup, DIGIT, RegexPattern
 
         timestamp = NamedGroup("time_at", f"{DIGIT * 2}:{DIGIT * 2}am")
 
         patt = RegexPattern(f"Created at {timestamp}, and then updated at {NamedReference(timestamp)}")
         patt2 = RegexPattern(f"Created at {timestamp}, and then updated at {NamedReference('time_at')}")
@@ -293,16 +286,15 @@
         super().__init__("P=", name)
 
 
 class NumberedReference(RegexPattern):
     """
     Lets you reference the literal match to :class:`Group`'s that you've already created, by its group index.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import NumberedReference, Group, DIGIT, RegexPattern
 
         timestamp = Group(f"{DIGIT * 2}:{DIGIT * 2}am")
 
         patt = RegexPattern(f"{timestamp},{NumberedReference(1)},{NumberedReference(1)}")
         print(patt.match("09:59am,09:59am,09:59am"))
@@ -314,16 +306,15 @@
         super().__init__(f"\\{group_number}")
 
 
 class Comment(Extension):
     """
     Lets you include comment strings that are ignored by regex compilers to document your regex's.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import Comment, DIGIT, WORD, Or
 
         patt = Or(DIGIT, WORD)
         patt_with_comment = patt + Comment("I love comments in regex!")
 
         print("Pattern without comment:", patt)
@@ -340,16 +331,15 @@
 class IfAhead(Extension):
     """
     A mini if-statement in regex.
     It does not consume any string content.
     Makes the whole pattern match only if followed by the given pattern
     at this position in the whole pattern.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import IfAhead, escape, WORD, Multi, Or
 
         name = Multi(WORD) + IfAhead(
             Or(
                 escape(" Jr."),
                 escape(" Sr."),
@@ -367,40 +357,38 @@
 class IfNotAhead(Extension):
     """
     A mini if-statement in regex.
     It does not consume any string content.
     Makes the whole pattern match only if **NOT** followed by the given pattern
     at this position in the whole pattern.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import IfNotAhead, RegexPattern
 
         patt = RegexPattern("Foo") + IfNotAhead("bar")
 
         print(patt.match("Foo"))
         print(patt.match("Foobar"))
         print(patt.match("Fooba"))
-        
+
     """
 
     def __init__(self, pattern: ValidPatternType):
         super().__init__("!", pattern)
 
 
 class IfBehind(Extension):
     """
     A mini if-statement in regex.
     It does not consume any string content.
     Makes the whole pattern match only if preceded by the given pattern
     at this position in the whole pattern.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import IfBehind, DIGIT, Multi, Optional
 
         rank = IfBehind("Rank: ") + Multi(DIGIT)
 
         print(rank.findall("Rank: 27, Score: 30, Power: 123"))
 
@@ -413,16 +401,15 @@
 class IfNotBehind(Extension):
     """
     A mini if-statement in regex.
     It does not consume any string content.
     Makes the whole pattern match only if **NOT** preceded by the given pattern
     at this position in the whole pattern.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import IfNotBehind, WORD, Multi, DIGIT
 
         patt = IfNotBehind(WORD) + Multi(DIGIT)
 
         print(patt.match("b64"))
         print(patt.match("64"))
@@ -436,16 +423,15 @@
 class Group(Extension):
     """
     For separating your Patterns into fields for extraction.
     Basically you use Group to reference regex inside of it later with :class:`NumberedReference`.
     Passing :code:`capturing=False` unifies the regex inside the group into a single token
     but does not capture the group. Seen below.
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
         from regexfactory import Group, WORD, Multi
 
         name = Group(Multi(WORD)) + " " + Group(Multi(WORD), capturing=False)
 
         print(name.match("Nate Larsen").groups())
 
@@ -462,21 +448,20 @@
 
 
 class IfGroup(Extension):
     """
     Matches with :code:`yes_pattern` if the given group name or group index succeeds in matching and exists,
     otherwise matches with :code:`no_pattern`
 
-    .. execute_code::
-        :hide_headers:
+    .. exec_code::
 
-        from regexfactory import IfGroup, NamedGroup, Optional
+        from regexfactory import IfGroup, NamedGroup, Optional, escape
 
         patt = (
-            Optional(NamedGroup("title", "Mr\. ")) +
+            Optional(NamedGroup("title", escape("Mr. "))) +
             IfGroup("title", "Dillon", NamedGroup("first_name", "Bob")) +
             Optional(IfGroup("first_name", " Dillon", ""))
         )
         # If NamedGroup "title" matches then use the last name pattern
         # else use the first name pattern
 
         print(patt.match("Mr. Dillon"))
@@ -488,8 +473,8 @@
 
     def __init__(
         self,
         name_or_id: t.Union[str, int],
         yes_pattern: ValidPatternType,
         no_pattern: ValidPatternType,
     ):
-        super().__init__(Group(str(name_or_id)), Or(yes_pattern, no_pattern))
+        super().__init__(str(Group(str(name_or_id))), Or(yes_pattern, no_pattern))
```

