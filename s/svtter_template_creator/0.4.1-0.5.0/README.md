# Comparing `tmp/svtter_template_creator-0.4.1.tar.gz` & `tmp/svtter_template_creator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svtter_template_creator-0.4.1.tar", max compression
+gzip compressed data, was "svtter_template_creator-0.5.0.tar", max compression
```

## Comparing `svtter_template_creator-0.4.1.tar` & `svtter_template_creator-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0        3 2023-09-19 03:01:44.268024 svtter_template_creator-0.4.1/LICENSE
--rw-r--r--   0        0        0      635 2023-09-19 04:25:07.605771 svtter_template_creator-0.4.1/README.md
--rw-r--r--   0        0        0      890 2023-09-19 04:51:26.854137 svtter_template_creator-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-09-19 04:49:05.712473 svtter_template_creator-0.4.1/src/svtter_template_creator/__init__.py
--rw-r--r--   0        0        0     1114 2023-09-19 04:46:31.868300 svtter_template_creator-0.4.1/src/svtter_template_creator/__main__.py
--rw-r--r--   0        0        0      476 2023-09-19 03:01:44.269024 svtter_template_creator-0.4.1/src/svtter_template_creator/tc.py
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 svtter_template_creator-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 08:26:32.251785 svtter_template_creator-0.5.0/LICENSE
+-rw-r--r--   0        0        0      579 2024-04-16 08:46:58.609471 svtter_template_creator-0.5.0/README.md
+-rw-r--r--   0        0        0     1015 2024-04-16 08:41:08.095185 svtter_template_creator-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:32:06.941521 svtter_template_creator-0.5.0/src/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 08:46:16.612727 svtter_template_creator-0.5.0/src/svtter_template_creator/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-16 08:42:48.311329 svtter_template_creator-0.5.0/src/svtter_template_creator/__main__.py
+-rw-r--r--   0        0        0     1042 2024-04-16 08:45:06.742666 svtter_template_creator-0.5.0/src/svtter_template_creator/lib.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:20:55.369974 svtter_template_creator-0.5.0/src/svtter_template_creator/tests/__init__.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 svtter_template_creator-0.5.0/PKG-INFO
```

### Comparing `svtter_template_creator-0.4.1/pyproject.toml` & `svtter_template_creator-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 [tool.poetry]
 # poetry version == 1.6
 name = "svtter_template_creator"
-version = "0.4.1"
+version = "0.5.0"
 readme = "README.md"
 description = ""
 authors = [ "svtter <svtter@163.com>",]
 keywords = ["template", "django"]
 include = ["src/*",]
 
 
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
+# [[tool.poetry.source]]
+# name = "tsinghua"
+# url = "https://pypi.tuna.tsinghua.edu.cn/simple"
+# priority = "default"
+
 [[tool.poetry.source]]
-name = "tsinghua"
-url = "https://pypi.tuna.tsinghua.edu.cn/simple"
+name = "aliyun"
+url = "http://mirrors.aliyun.com/pypi/simple/"
 priority = "default"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "supplemental"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.10"
 click = "^8.1.3"
 cookiecutter = "^2.1.1"
 toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-xdist = "^3.0.2"
 pre-commit = "^2.20.0"
 
 [tool.poetry.scripts]
 tt = "svtter_template_creator.__main__:cli"
 
-[tool.pytest.ini_options]
-DJANGO_SETTINGS_MODULE = "conf.settings"
-python_files = "tests.py test_*.py *_tests.py"
-addopts = "-n3"
+# [tool.pytest.ini_options]
+# DJANGO_SETTINGS_MODULE = "conf.settings"
+# python_files = "tests.py test_*.py *_tests.py"
+# addopts = "-n3"
```

### Comparing `svtter_template_creator-0.4.1/src/svtter_template_creator/__main__.py` & `svtter_template_creator-0.5.0/src/svtter_template_creator/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,31 @@
+import toml
 import click
+from pathlib import Path
 
-from svtter_template_creator import __version__, tc
+from svtter_template_creator import __version__, lib
 
 
 @click.group()
 def cli():
     pass
 
 
 @click.command()
 @click.option(
     "--name",
     prompt="template name",
     help="The template need to create",
-    type=click.Choice(
-        [
-            "django",
-            "package",
-            "compose",
-        ]
-    ),
+    type=click.Choice(lib.get_choice()),
 )
 def create(name):
     """
     create template via name
     """
-    tc.create(name)
+    lib.create(name)
 
 
 @click.command()
 def version():
     """show version information"""
     click.echo(f"ttc version is: {__version__}")
 
@@ -37,18 +33,14 @@
 @click.command(help="write version to __init__.py and pyproject.toml")
 @click.option("--version", help="The new verison!", required=True)
 def write(version):
     filepath = "src/ttc/__init__.py"
     with open(filepath, "w") as f:
         f.write(f'__version__ = "{version}"')
 
-    from pathlib import Path
-
-    import toml
-
     p = Path("./pyproject.toml")
     res = toml.load(p)
     res["tool"]["poetry"]["version"] = version
     # write back
     with open(p, "w") as f:
         toml.dump(res, f)
```

