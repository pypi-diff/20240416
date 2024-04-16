# Comparing `tmp/termax-0.0.1.tar.gz` & `tmp/termax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termax-0.0.1.tar", last modified: Wed Mar  6 03:11:39 2024, max compression
+gzip compressed data, was "termax-0.1.1.tar", last modified: Tue Apr 16 03:36:13 2024, max compression
```

## Comparing `termax-0.0.1.tar` & `termax-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:39.471351 termax-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-06 03:11:30.000000 termax-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-06 03:11:39.471351 termax-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-06 03:11:30.000000 termax-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:39.467350 termax-0.0.1/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:30.000000 termax-0.0.1/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-06 03:11:39.471351 termax-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-06 03:11:30.000000 termax-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:39.467350 termax-0.0.1/termax/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-06 03:11:30.000000 termax-0.0.1/termax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-06 03:11:30.000000 termax-0.0.1/termax/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-06 03:11:30.000000 termax-0.0.1/termax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:39.471351 termax-0.0.1/termax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-06 03:11:39.000000 termax-0.0.1/termax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-06 03:11:39.000000 termax-0.0.1/termax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 03:11:39.000000 termax-0.0.1/termax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 03:11:39.000000 termax-0.0.1/termax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-06 03:11:39.000000 termax-0.0.1/termax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-06 03:11:39.000000 termax-0.0.1/termax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:39.471351 termax-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 03:11:30.000000 termax-0.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-16 03:36:04.000000 termax-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 03:36:13.055791 termax-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-16 03:36:04.000000 termax-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.047791 termax-0.1.1/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 03:36:13.055791 termax-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-16 03:36:04.000000 termax-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.047791 termax-0.1.1/termax/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 03:36:04.000000 termax-0.1.1/termax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_qianfan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/_qianwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-16 03:36:04.000000 termax-0.1.1/termax/agent/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/termax/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-04-16 03:36:04.000000 termax-0.1.1/termax/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-16 03:36:04.000000 termax-0.1.1/termax/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/function/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/function/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-16 03:36:04.000000 termax-0.1.1/termax/function/openai/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/plugin/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/fish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/shell/zsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-16 03:36:04.000000 termax-0.1.1/termax/plugin/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.051791 termax-0.1.1/termax/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/termax/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/termax/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-16 03:36:04.000000 termax-0.1.1/termax/prompt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/termax/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-16 03:36:04.000000 termax-0.1.1/termax/utils/qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 03:36:04.000000 termax-0.1.1/termax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/termax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 03:36:13.000000 termax-0.1.1/termax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:13.055791 termax-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:36:04.000000 termax-0.1.1/tests/__init__.py
```

### Comparing `termax-0.0.1/LICENSE` & `termax-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `termax-0.0.1/setup.py` & `termax-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     author_email='huangyz0918@gmail.com',
     url='https://github.com/huangyz0918/termax',
     download_url='https://github.com/huangyz0918/termax/archive/refs/heads/main.zip',
     keywords=['LLM', 'deep learning', 'MLOps', 'shell', 'neural networks', 'command line', 'terminal', 'autocomplete'],
     packages=find_packages(),
     entry_points={
         "console_scripts": [
-            "termax=termax.cli:cli",
-            "t=termax.cli:cli",
+            "termax=termax.cli.cli:cli",
+            "t=termax.cli.cli:cli",
         ]
     },
     include_package_data=True,
     install_requires=requirements,
     setup_requires=['setuptools>=38.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

