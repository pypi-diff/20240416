# Comparing `tmp/langbank-0.1.3.tar.gz` & `tmp/langbank-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langbank-0.1.3.tar", last modified: Mon Apr 15 10:41:53 2024, max compression
+gzip compressed data, was "langbank-0.1.4.tar", last modified: Mon Apr 15 14:22:09 2024, max compression
```

## Comparing `langbank-0.1.3.tar` & `langbank-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.141145 langbank-0.1.3/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 10:41:53.140886 langbank-0.1.3/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      622 2024-04-15 10:40:40.000000 langbank-0.1.3/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-15 10:41:53.141183 langbank-0.1.3/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-15 10:41:37.000000 langbank-0.1.3/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.139183 langbank-0.1.3/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.139875 langbank-0.1.3/src/langbank/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1.3/src/langbank/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     4429 2024-04-15 10:15:02.000000 langbank-0.1.3/src/langbank/main.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.140705 langbank-0.1.3/src/langbank.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      208 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 14:22:09.053862 langbank-0.1.4/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 14:22:09.053580 langbank-0.1.4/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      622 2024-04-15 10:40:40.000000 langbank-0.1.4/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-15 14:22:09.053902 langbank-0.1.4/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-15 14:22:02.000000 langbank-0.1.4/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 14:22:09.051853 langbank-0.1.4/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 14:22:09.052565 langbank-0.1.4/src/langbank/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1.4/src/langbank/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     4426 2024-04-15 14:21:04.000000 langbank-0.1.4/src/langbank/main.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 14:22:09.053385 langbank-0.1.4/src/langbank.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 14:22:09.000000 langbank-0.1.4/src/langbank.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      208 2024-04-15 14:22:09.000000 langbank-0.1.4/src/langbank.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-15 14:22:09.000000 langbank-0.1.4/src/langbank.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-15 14:22:09.000000 langbank-0.1.4/src/langbank.egg-info/top_level.txt
```

### Comparing `langbank-0.1.3/PKG-INFO` & `langbank-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langbank
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple word bank for language learning
 Home-page: https://github.com/tebby24/langbank
 Author: Teddy Gonyea
 Author-email: enterted@gmail.com
 Keywords: language learning
 Description-Content-Type: text/markdown
```

### Comparing `langbank-0.1.3/README.md` & `langbank-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langbank-0.1.3/src/langbank/main.py` & `langbank-0.1.4/src/langbank/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,17 @@
             tags: a list of string tags
         """
         if tags is None:
             tags = []
 
         dt = datetime.now()
         entry = {"word": word, "datetime": dt.strftime(DATETIME_FORMAT), "tags": tags}
-        with open(self.file_path, "a") as f:
-            f.write(json.dumps(entry) + "\n")
+        bank = self.get_bank()
+        bank.append(entry)
+        self.write_bank(bank)
 
     def get_words_from_past_n_days(self, n=0):
         """
         Get a list of all the words added in the past n days, where n=0 will return the words added today
         """
         bank = self.get_bank()
         today = datetime.now().date()
```

### Comparing `langbank-0.1.3/src/langbank.egg-info/PKG-INFO` & `langbank-0.1.4/src/langbank.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langbank
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple word bank for language learning
 Home-page: https://github.com/tebby24/langbank
 Author: Teddy Gonyea
 Author-email: enterted@gmail.com
 Keywords: language learning
 Description-Content-Type: text/markdown
```

