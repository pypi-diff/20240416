# Comparing `tmp/ezregex-1.9.1.tar.gz` & `tmp/ezregex-1.9.2.tar.gz`

## Comparing `ezregex-1.9.1.tar` & `ezregex-1.9.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.1/.coveragerc
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.1/MANIFEST.in
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ezregex-1.9.1/requirements.txt
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 ezregex-1.9.1/setup.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 ezregex-1.9.1/todo.txt
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.1/tox.ini
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.1/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0    18421 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/EZRegex.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/_dialects.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/_docs.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/api.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/api.pyi
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/generate.py
--rw-r--r--   0        0        0    24594 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/invert.py
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/invert_old.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/base/__init__.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/base/elements.py
--rw-r--r--   0        0        0    13333 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/base/interface.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/javascript/psuedonymns.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/__init__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/elements.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/perl/psuedonymns.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/__init__.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/elements.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/elements.pyi
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.1/ezregex/python/psuedonymns.py
--rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/_groups.py
--rw-r--r--   0        0        0    29505 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/_regexs.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/test_generate.py
--rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/testing_color_algorithm.ipynb
--rw-r--r--   0        0        0    15151 2020-02-02 00:00:00.000000 ezregex-1.9.1/tests/tests.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.1/LICENSE
--rw-r--r--   0        0        0    49171 2020-02-02 00:00:00.000000 ezregex-1.9.1/README.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ezregex-1.9.1/pyproject.toml
--rw-r--r--   0        0        0    49406 2020-02-02 00:00:00.000000 ezregex-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ezregex-1.9.2/.coveragerc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ezregex-1.9.2/MANIFEST.in
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 ezregex-1.9.2/requirements.txt
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 ezregex-1.9.2/setup.py
+-rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 ezregex-1.9.2/todo.txt
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 ezregex-1.9.2/tox.ini
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ezregex-1.9.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 ezregex-1.9.2/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0    18421 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/EZRegex.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/_dialects.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/_docs.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/api.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/api.pyi
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/generate.py
+-rw-r--r--   0        0        0    24561 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/invert.py
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/invert_old.py
+-rw-r--r--   0        0        0  6825598 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/assets/words.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/base/__init__.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/base/elements.py
+-rw-r--r--   0        0        0    13333 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/base/interface.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/javascript/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/javascript/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/javascript/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/javascript/psuedonymns.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/perl/__init__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/perl/elements.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/perl/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/perl/psuedonymns.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/python/__init__.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/python/elements.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/python/elements.pyi
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 ezregex-1.9.2/ezregex/python/psuedonymns.py
+-rw-r--r--   0        0        0    13484 2020-02-02 00:00:00.000000 ezregex-1.9.2/tests/_groups.py
+-rw-r--r--   0        0        0    29505 2020-02-02 00:00:00.000000 ezregex-1.9.2/tests/_regexs.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ezregex-1.9.2/tests/test_generate.py
+-rw-r--r--   0        0        0    37422 2020-02-02 00:00:00.000000 ezregex-1.9.2/tests/testing_color_algorithm.ipynb
+-rw-r--r--   0        0        0    15156 2020-02-02 00:00:00.000000 ezregex-1.9.2/tests/tests.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ezregex-1.9.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ezregex-1.9.2/LICENSE
+-rw-r--r--   0        0        0    49171 2020-02-02 00:00:00.000000 ezregex-1.9.2/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ezregex-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0    49379 2020-02-02 00:00:00.000000 ezregex-1.9.2/PKG-INFO
```

### Comparing `ezregex-1.9.1/setup.py` & `ezregex-1.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             break
     else:
         version = '0.0.1'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
-REQUIRES = ['rich', 'random_word']
+REQUIRES = []
 
 kwargs = {
     'name': 'ezregex',
     'version': version,
     'description': '',
     'long_description': readme,
     'author': 'Copeland Carter',
```

### Comparing `ezregex-1.9.1/todo.txt` & `ezregex-1.9.2/todo.txt`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/.github/FUNDING.yml` & `ezregex-1.9.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/.github/workflows/unit-tests.yml` & `ezregex-1.9.2/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/EZRegex.py` & `ezregex-1.9.2/ezregex/EZRegex.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/_dialects.py` & `ezregex-1.9.2/ezregex/_dialects.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/_docs.py` & `ezregex-1.9.2/ezregex/_docs.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/api.py` & `ezregex-1.9.2/ezregex/api.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/api.pyi` & `ezregex-1.9.2/ezregex/api.pyi`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/generate.py` & `ezregex-1.9.2/ezregex/generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/invert.py` & `ezregex-1.9.2/ezregex/invert.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 import string
 import traceback
 from random import choice, choices, randint
 from re import search
 from sys import version_info
 from typing import Literal, Union
 
-from random_word.services.local import Local
-
 from ezregex import *
 
 if version_info.minor <= 10:
     from re import sre_parse as sre  # type: ignore
 else:
     from re import _parser as sre  # type: ignore
 
 # So I can debug this function directly
 if __name__ != '__main__':
     from .invert_old import invertRegex
 
-with open(Local().source) as f:
+with open('ezregex/assets/words.json') as f:
     words = json.load(f).keys()
 
 # Don't use string.whitespace, because we don't want to use weird difficult to print characters.
 # We want the replacement to be readable.
 _whitespace   = ' '
 _everything   = string.digits + string.ascii_letters + string.punctuation + _whitespace + '_'
```

### Comparing `ezregex-1.9.1/ezregex/invert_old.py` & `ezregex-1.9.2/ezregex/invert_old.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/base/elements.py` & `ezregex-1.9.2/ezregex/base/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/base/interface.py` & `ezregex-1.9.2/ezregex/base/interface.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/javascript/elements.py` & `ezregex-1.9.2/ezregex/javascript/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/javascript/psuedonymns.py` & `ezregex-1.9.2/ezregex/javascript/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/perl/elements.py` & `ezregex-1.9.2/ezregex/perl/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/perl/psuedonymns.py` & `ezregex-1.9.2/ezregex/perl/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/python/elements.py` & `ezregex-1.9.2/ezregex/python/elements.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/ezregex/python/psuedonymns.py` & `ezregex-1.9.2/ezregex/python/psuedonymns.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/tests/_groups.py` & `ezregex-1.9.2/tests/_groups.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/tests/_regexs.py` & `ezregex-1.9.2/tests/_regexs.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/tests/test_generate.py` & `ezregex-1.9.2/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/tests/testing_color_algorithm.ipynb` & `ezregex-1.9.2/tests/testing_color_algorithm.ipynb`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/tests/tests.py` & `ezregex-1.9.2/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,21 +248,21 @@
 
     print('All Tests Passed!')
 
 # From 1-100, 1 is easy, 100 is hard
 difficulty = 1
 runTests(
     # These should remain on, for the GitHub automated tests
-    singletons=True,
-    _invert=False,
-    replacement=True,
-    operators=True,
-    _generate=True,
+    singletons=False,
+    _invert=True,
+    replacement=False,
+    operators=False,
+    _generate=False,
     # These display for you to check that they look correct
     testMethod=False,
-    _api=False,
+    # _api=False,
     # Settings
     strictness=difficulty,
     invert_tries=101-difficulty,
     dontIncludePassed=True,
     invertBackend='re_parser',
 )
```

### Comparing `ezregex-1.9.1/.gitignore` & `ezregex-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/LICENSE` & `ezregex-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/README.md` & `ezregex-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ezregex-1.9.1/pyproject.toml` & `ezregex-1.9.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 python_version = ['3.10', '3.11', '3.12', 'pypy', 'pypy3']
 
 [tool.hatch.commands]
 prerelease = 'hatch build'
 
 [project]
 name = 'ezregex'
-version = '1.9.1'
+version = '1.9.2'
 description = 'A readable and intuitive way to generate Regular Expressions'
-dependencies = ['random_word']
+dependencies = []
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `ezregex-1.9.1/PKG-INFO` & `ezregex-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ezregex
-Version: 1.9.1
+Version: 1.9.2
 Summary: A readable and intuitive way to generate Regular Expressions
 License-File: LICENSE
 Requires-Python: >=3.10
-Requires-Dist: random-word
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://ezregex.org/favicon.png"><br>
     <p></p>
 
 <a href="https://github.com/smartycope/ezregex/actions/workflows/unit-tests.yml">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-Metadata-Version: 2.1 Name: ezregex Version: 1.9.1 Summary: A readable and
+Metadata-Version: 2.3 Name: ezregex Version: 1.9.2 Summary: A readable and
 intuitive way to generate Regular Expressions License-File: LICENSE Requires-
-Python: >=3.10 Requires-Dist: random-word Description-Content-Type: text/
-markdown
+Python: >=3.10 Description-Content-Type: text/markdown
                        [https://ezregex.org/favicon.png]
    _[_U_n_i_t_ _T_e_s_t_s_]_[_P_y_P_I_ _L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
 _s_m_a_r_t_y_c_o_p_e_/_e_z_r_e_g_e_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_i_m_p_l_e_m_e_n_t_a_t_i_o_n_/_e_z_r_e_g_e_x_]_[_h_t_t_p_s_:_/
                      _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_f_o_r_m_a_t_/_e_z_r_e_g_e_x_]
 # EZRegex A readable and intuitive way to make Regular Expressions without
 having to know any of the syntax Try my new frontend for this library at
 [ezregex.org](https://ezregex.org/)! TLDR: This is to regular expressions what
```

