# Comparing `tmp/thulearn2018-2.4.3.tar.gz` & `tmp/thulearn2018-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thulearn2018-2.4.3.tar", last modified: Sun Apr  7 11:24:18 2024, max compression
+gzip compressed data, was "thulearn2018-2.4.4.tar", last modified: Tue Apr 16 09:02:15 2024, max compression
```

## Comparing `thulearn2018-2.4.3.tar` & `thulearn2018-2.4.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/
--rw-r--r--   0 hyr       (1000) hyr       (1000)       75 2023-09-13 09:31:57.000000 thulearn2018-2.4.3/.gitignore
--rw-r--r--   0 hyr       (1000) hyr       (1000)     1074 2023-09-13 09:31:57.000000 thulearn2018-2.4.3/LICENSE
--rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/PKG-INFO
--rw-r-----   0 hyr       (1000) hyr       (1000)     5277 2024-04-07 05:13:15.000000 thulearn2018-2.4.3/README.md
--rw-r-----   0 hyr       (1000) hyr       (1000)       38 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/setup.cfg
--rw-r-----   0 hyr       (1000) hyr       (1000)     2540 2024-04-07 11:21:35.000000 thulearn2018-2.4.3/setup.py
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/thulearn2018/
--rw-r--r--   0 hyr       (1000) hyr       (1000)       22 2023-09-13 09:31:57.000000 thulearn2018-2.4.3/thulearn2018/__init__.py
--rw-r-----   0 hyr       (1000) hyr       (1000)    10580 2024-04-07 11:23:07.000000 thulearn2018-2.4.3/thulearn2018/browser.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     5708 2024-04-07 05:13:21.000000 thulearn2018-2.4.3/thulearn2018/filemanager.py
--rw-r-----   0 hyr       (1000) hyr       (1000)      415 2024-04-07 05:12:59.000000 thulearn2018-2.4.3/thulearn2018/jsonhelper.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3596 2024-04-07 05:13:14.000000 thulearn2018-2.4.3/thulearn2018/learn.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3207 2024-04-07 05:13:14.000000 thulearn2018-2.4.3/thulearn2018/settings.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     3941 2024-04-07 05:13:20.000000 thulearn2018-2.4.3/thulearn2018/soup.py
--rw-r-----   0 hyr       (1000) hyr       (1000)     1263 2024-04-07 10:52:59.000000 thulearn2018-2.4.3/thulearn2018/utils.py
-drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-07 11:24:18.585221 thulearn2018-2.4.3/thulearn2018.egg-info/
--rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/PKG-INFO
--rw-r--r--   0 hyr       (1000) hyr       (1000)      449 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/SOURCES.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)        1 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/dependency_links.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       50 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/entry_points.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       79 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/requires.txt
--rw-r--r--   0 hyr       (1000) hyr       (1000)       13 2024-04-07 11:24:18.000000 thulearn2018-2.4.3/thulearn2018.egg-info/top_level.txt
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-16 09:02:15.517825 thulearn2018-2.4.4/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       75 2023-09-13 09:31:57.000000 thulearn2018-2.4.4/.gitignore
+-rw-r--r--   0 hyr       (1000) hyr       (1000)     1074 2024-04-16 08:17:55.000000 thulearn2018-2.4.4/LICENSE
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-16 09:02:15.517825 thulearn2018-2.4.4/PKG-INFO
+-rw-r-----   0 hyr       (1000) hyr       (1000)     5277 2024-04-07 05:13:15.000000 thulearn2018-2.4.4/README.md
+-rw-r-----   0 hyr       (1000) hyr       (1000)       38 2024-04-16 09:02:15.517825 thulearn2018-2.4.4/setup.cfg
+-rw-r-----   0 hyr       (1000) hyr       (1000)     2540 2024-04-16 09:02:10.000000 thulearn2018-2.4.4/setup.py
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-16 09:02:15.513825 thulearn2018-2.4.4/thulearn2018/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       22 2023-09-13 09:31:57.000000 thulearn2018-2.4.4/thulearn2018/__init__.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)    10638 2024-04-16 08:16:25.000000 thulearn2018-2.4.4/thulearn2018/browser.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     5708 2024-04-07 05:13:21.000000 thulearn2018-2.4.4/thulearn2018/filemanager.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)      415 2024-04-07 05:12:59.000000 thulearn2018-2.4.4/thulearn2018/jsonhelper.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3779 2024-04-16 08:16:36.000000 thulearn2018-2.4.4/thulearn2018/learn.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3207 2024-04-07 05:13:14.000000 thulearn2018-2.4.4/thulearn2018/settings.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     3941 2024-04-07 05:13:20.000000 thulearn2018-2.4.4/thulearn2018/soup.py
+-rw-r-----   0 hyr       (1000) hyr       (1000)     1263 2024-04-07 10:52:59.000000 thulearn2018-2.4.4/thulearn2018/utils.py
+drwxr-x---   0 hyr       (1000) hyr       (1000)        0 2024-04-16 09:02:15.513825 thulearn2018-2.4.4/thulearn2018.egg-info/
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      716 2024-04-16 09:02:15.000000 thulearn2018-2.4.4/thulearn2018.egg-info/PKG-INFO
+-rw-r--r--   0 hyr       (1000) hyr       (1000)      449 2024-04-16 09:02:15.000000 thulearn2018-2.4.4/thulearn2018.egg-info/SOURCES.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)        1 2024-04-16 09:02:15.000000 thulearn2018-2.4.4/thulearn2018.egg-info/dependency_links.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       50 2024-04-16 09:02:15.000000 thulearn2018-2.4.4/thulearn2018.egg-info/entry_points.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       79 2024-04-16 09:02:15.000000 thulearn2018-2.4.4/thulearn2018.egg-info/requires.txt
+-rw-r--r--   0 hyr       (1000) hyr       (1000)       13 2024-04-16 09:02:15.000000 thulearn2018-2.4.4/thulearn2018.egg-info/top_level.txt
```

### Comparing `thulearn2018-2.4.3/LICENSE` & `thulearn2018-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.3/PKG-INFO` & `thulearn2018-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thulearn2018
-Version: 2.4.3
+Version: 2.4.4
 Summary: Tools for Web Learning of Tsinghua University
 Home-page: https://github.com/euxcet/thulearn2018
 Author: Chengchi Zhou, Yingtian Liu, Yurui Hong
 Author-email: zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,yuruihong02@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thulearn2018-2.4.3/README.md` & `thulearn2018-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.3/setup.py` & `thulearn2018-2.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="thulearn2018",
-    version="2.4.3",
+    version="2.4.4",
     author="Chengchi Zhou, Yingtian Liu, Yurui Hong",
     author_email="zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,"
                  "yuruihong02@outlook.com",
     description="Tools for Web Learning of Tsinghua University",
     long_description="Tools for Web Learning of Tsinghua University",
     long_description_content_type="text/markdown",
     url="https://github.com/euxcet/thulearn2018",
```

### Comparing `thulearn2018-2.4.3/thulearn2018/browser.py` & `thulearn2018-2.4.4/thulearn2018/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,18 +222,19 @@
         response = self.jh.loads(self.post(settings.upload_api, form=form,
                                  headers=settings.upload_headers))
         if response["result"] == "success":
             print("done")
         else:
             print(f"Error: assignment may have expired. Details:\n{response}")
 
-    def get_ddl(self, lessons):
+    def get_ddl(self, lessons, download_submission=False):
         ddls = []
         for lesson in lessons:
-            ddls += self.download_homework(lesson[0], lesson[4], False)
+            ddls += self.download_homework(
+                lesson[0], lesson[4], download_submission)
         # delete expired homework by comparing ddl[2] with current time
         ddls = [ddl for ddl in ddls if not utils.expired(ddl[2])]
         ddls.sort(key=lambda x: x[2])
         return [[ddl[0], ddl[1], ddl[2], utils.time_delta(ddl[2]), ddl[3]]
                 for ddl in ddls]
```

### Comparing `thulearn2018-2.4.3/thulearn2018/filemanager.py` & `thulearn2018-2.4.4/thulearn2018/filemanager.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.3/thulearn2018/learn.py` & `thulearn2018-2.4.4/thulearn2018/learn.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,27 +74,29 @@
 
 @click.command(help='Show homework deadlines.')
 @click.option('-e', '--exclude', default='', help='excluded courses(override)')
 @click.option('-i', '--include', default='', help='included courses')
 @click.option('-s', '--semester', default='',
               help='Semester to show ddl, e.g. 2023-2024-1')
 @click.option('-o', '--path', default='', help='Path to save homework files')
-def ddl(exclude, include, semester, path):
+@click.option('--download-submission', is_flag=True, default=False,
+              help='Download submissions, used when not locally stored')
+def ddl(exclude, include, semester, path, download_submission):
     def align(string, length=0):
         len_en = len(string)
         len_utf8 = len(string.encode('utf-8'))
         lent = len_en + (len_utf8 - len_en) // 2
         return string + ' ' * (length - lent)
     learn.login()
     learn.set_semester(semester)
     if (path != ''):
         learn.path = path
     ddls = learn.get_ddl(learn.init_lessons(
         exclude=exclude.split(',') if exclude else [],
-        include=include.split(',') if include else []))
+        include=include.split(',') if include else []), download_submission)
     print('Total %d ddl(s)' % (len(ddls)))
     for ddl in ddls:
         print(align(ddl[0][0:8], 25), align(
             ddl[1][0:20], 30) + align(ddl[3][0:20], 30), ddl[4])
 
 
 @click.group()
```

### Comparing `thulearn2018-2.4.3/thulearn2018/settings.py` & `thulearn2018-2.4.4/thulearn2018/settings.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.3/thulearn2018/soup.py` & `thulearn2018-2.4.4/thulearn2018/soup.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.3/thulearn2018/utils.py` & `thulearn2018-2.4.4/thulearn2018/utils.py`

 * *Files identical despite different names*

### Comparing `thulearn2018-2.4.3/thulearn2018.egg-info/PKG-INFO` & `thulearn2018-2.4.4/thulearn2018.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thulearn2018
-Version: 2.4.3
+Version: 2.4.4
 Summary: Tools for Web Learning of Tsinghua University
 Home-page: https://github.com/euxcet/thulearn2018
 Author: Chengchi Zhou, Yingtian Liu, Yurui Hong
 Author-email: zcc16@mails.tsinghua.edu.cn, liu-yt16@mails.tsinghua.edu.cn,yuruihong02@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

