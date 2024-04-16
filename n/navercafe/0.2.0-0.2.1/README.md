# Comparing `tmp/navercafe-0.2.0.tar.gz` & `tmp/navercafe-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navercafe-0.2.0.tar", max compression
+gzip compressed data, was "navercafe-0.2.1.tar", max compression
```

## Comparing `navercafe-0.2.0.tar` & `navercafe-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       88 2022-12-27 07:46:58.583092 navercafe-0.2.0/navercafe/__init__.py
--rw-r--r--   0        0        0     4468 2022-12-27 07:43:48.992741 navercafe-0.2.0/navercafe/main.py
--rw-r--r--   0        0        0      373 2022-12-27 07:52:14.728505 navercafe-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      565 2022-12-27 07:38:37.181645 navercafe-0.2.0/README.md
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 navercafe-0.2.0/setup.py
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 navercafe-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      532 2024-04-16 12:15:33.126234 navercafe-0.2.1/README.md
+-rw-r--r--   0        0        0       83 2024-04-16 12:31:38.200159 navercafe-0.2.1/navercafe/__init__.py
+-rw-r--r--   0        0        0     4267 2024-04-16 12:10:29.469965 navercafe-0.2.1/navercafe/main.py
+-rw-r--r--   0        0        0      380 2024-04-16 12:31:47.333535 navercafe-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 navercafe-0.2.1/PKG-INFO
```

### Comparing `navercafe-0.2.0/PKG-INFO` & `navercafe-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: navercafe
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Yong Choi
-Author-email: sk8er.choi@gmail.com
+Author-email: ychoi_kr@naver.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: selenium (>=4.7.2,<5.0.0)
-Requires-Dist: webdriver-manager (>=3.8.5,<4.0.0)
+Requires-Dist: webdriver-manager (>=4.0.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## Setup
 
 ```
 $ pip install navercafe
 ```
@@ -31,15 +33,15 @@
 cafe = NaverCafe(cafe_name, club_id)
 
 # 2. (optional) enter user id and pw
 # This is semi-automatic (needs manual authentication)
 cafe.enter_id_pw('your_id', 'your_pw')
 
 # 3. get article board
-board_id = 34
+board_id = 28
 df1 = cafe.articleboard(board_id)
 print(len(df1))
 print(df1.head())
 
 # 4. get comments
 article_id = 139
 df2 = cafe.comments(article_id)
```

