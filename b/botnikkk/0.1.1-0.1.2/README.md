# Comparing `tmp/botnikkk-0.1.1.tar.gz` & `tmp/botnikkk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.1.1.tar", last modified: Wed Apr 10 17:56:38 2024, max compression
+gzip compressed data, was "botnikkk-0.1.2.tar", last modified: Tue Apr 16 11:14:46 2024, max compression
```

## Comparing `botnikkk-0.1.1.tar` & `botnikkk-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 17:56:38.585167 botnikkk-0.1.1/
--rw-rw-rw-   0        0        0     1094 2024-04-10 17:07:38.000000 botnikkk-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4104 2024-04-10 17:56:38.579549 botnikkk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3386 2024-04-10 17:56:32.000000 botnikkk-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 17:56:38.568243 botnikkk-0.1.1/botnikkk/
--rw-rw-rw-   0        0        0      212 2024-04-10 17:07:38.000000 botnikkk-0.1.1/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     3208 2024-04-10 17:35:18.000000 botnikkk-0.1.1/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-10 17:56:38.578230 botnikkk-0.1.1/botnikkk.egg-info/
--rw-rw-rw-   0        0        0     4104 2024-04-10 17:56:38.000000 botnikkk-0.1.1/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-04-10 17:56:38.000000 botnikkk-0.1.1/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 17:56:38.000000 botnikkk-0.1.1/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-10 17:56:38.000000 botnikkk-0.1.1/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-10 17:56:38.000000 botnikkk-0.1.1/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 17:56:38.585167 botnikkk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1000 2024-04-10 17:54:21.000000 botnikkk-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:14:46.551473 botnikkk-0.1.2/
+-rw-rw-rw-   0        0        0     3103 2024-04-16 11:14:46.542996 botnikkk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2024-04-10 16:40:35.000000 botnikkk-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 11:14:46.537901 botnikkk-0.1.2/botnikkk/
+-rw-rw-rw-   0        0        0      212 2024-04-10 15:13:48.000000 botnikkk-0.1.2/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     3208 2024-04-16 11:14:17.000000 botnikkk-0.1.2/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:14:46.542996 botnikkk-0.1.2/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0     3103 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 11:14:46.000000 botnikkk-0.1.2/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:14:46.551473 botnikkk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-04-16 11:08:59.000000 botnikkk-0.1.2/setup.py
```

### Comparing `botnikkk-0.1.1/botnikkk/formatting.py` & `botnikkk-0.1.2/botnikkk/formatting.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         gap = 128
 
         left_align = (int(screen_width/2) - int(gap/2))
         left_gap = (int(gap/2) - int(len(string)/2))
         right_gap = gap - left_gap - len(string)
     
     return {"left_align" : left_align, "left_gap" : left_gap, "right_gap" : right_gap, "default_gap" : gap }
-    
 
 def centre(title='',symbol=" ",left_alignment=None, str_end="\n") :
     #aligns the title in centre with symbols around it
     alignments = get_alignments(title)
     left_align = alignments["left_align"]*" "
     left_gap = alignments["left_gap"]
     right_gap = alignments["right_gap"]
@@ -34,15 +33,15 @@
     else :
         print_string = f"{left_align}|{left_gap*symbol}{title}{right_gap*symbol}|"
 
     print(print_string,end=str_end)
 
 def format_input(ques='') : 
     alignments = get_alignments(ques)
-    left_align = alignments["left_align"]
+    left_align = alignments["left_align"]*" "
     left_gap = alignments["left_gap"]*" "
     right_gap = alignments["right_gap"]*" "
 
     string = f"{left_align}|{left_gap}{ques}{right_gap}|\n{left_align}| -"
     output = input(string)
     return output
 
@@ -89,7 +88,8 @@
         gap = str(symbol)*(64-int((len(title)/2)))
         gap2 = str(symbol)*(128- len(title) - len(gap))
         centre(title, str_end="\r")
         await asyncio.sleep(1) 
 
 async def redirect(redirect='UNKNOWN'):
     await redirect_function(redirect)
+
```

### Comparing `botnikkk-0.1.1/setup.py` & `botnikkk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'a personal package'
 
 # Setting up
 setup(
     name="botnikkk",
     version=VERSION,
     author="BotNikkk",
```

