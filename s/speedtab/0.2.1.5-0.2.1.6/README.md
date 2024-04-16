# Comparing `tmp/speedtab-0.2.1.5.tar.gz` & `tmp/speedtab-0.2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.2.1.5.tar", max compression
+gzip compressed data, was "speedtab-0.2.1.6.tar", max compression
```

## Comparing `speedtab-0.2.1.5.tar` & `speedtab-0.2.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2024-04-08 13:19:07.106531 speedtab-0.2.1.5/pyproject.toml
--rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.5/speedtab/__init__.py
--rw-r--r--   0        0        0    86960 2024-04-08 13:19:45.082116 speedtab-0.2.1.5/speedtab/client.py
--rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.5/speedtab/enums.py
--rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.5/speedtab/formats.py
--rw-r--r--   0        0        0      783 2024-04-08 13:19:53.278076 speedtab-0.2.1.5/setup.py
--rw-r--r--   0        0        0      808 2024-04-08 13:19:53.279066 speedtab-0.2.1.5/PKG-INFO
+-rw-r--r--   0        0        0      567 2024-04-16 07:50:48.088234 speedtab-0.2.1.6/pyproject.toml
+-rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.6/speedtab/__init__.py
+-rw-r--r--   0        0        0    86804 2024-04-16 07:50:34.216380 speedtab-0.2.1.6/speedtab/client.py
+-rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.6/speedtab/enums.py
+-rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.6/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2024-04-16 07:50:57.741227 speedtab-0.2.1.6/setup.py
+-rw-r--r--   0        0        0      808 2024-04-16 07:50:57.741227 speedtab-0.2.1.6/PKG-INFO
```

### Comparing `speedtab-0.2.1.5/pyproject.toml` & `speedtab-0.2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.2.1.5"
+version = "0.2.1.6"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.2.1.5/speedtab/client.py` & `speedtab-0.2.1.6/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -793,27 +793,25 @@
                             'widthPixels': 800 * x_scale,
                             'heightPixels': 400 * y_scale,
                         }
                     }}}}, self.work_zone))
         return self
 
     def auto_size(self, axis: Union[str, int] = 1):
-        # TODO: Works strange, how axis works? Param approximate True/False: T -> approx func, F -> default
-        # TODO: catch the bug (see warning).
         """Autosizes rows (axis=0) or columns (axis=1) in a selected range or sheet.
 
         WARNING! This method may work incorrectly. The source of the error in its behavior is yet to be established.
         In case it does not autosize, please, resort to a .set_size() method to set a specific size of the cells.
         Otherwise, use .reset_size() to restore default sizes.
 
         :param axis: An axis to autosize, defaults to 1 (column).
         :return: A SpreadSheet object.
         """
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
-        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+        self._task_queue.append(Task('chart', self._increment_task(), self.sheet_id, {
             'autoResizeDimensions': {
                 'dimensions': {
                     'sheetId': self.sheet_id,
                     'dimension': axis,
                     'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get(
                         'startColumnIndex'),
                     'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get(
```

### Comparing `speedtab-0.2.1.5/speedtab/enums.py` & `speedtab-0.2.1.6/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.5/speedtab/formats.py` & `speedtab-0.2.1.6/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.5/setup.py` & `speedtab-0.2.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.2.1.5',
+    'version': '0.2.1.6',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.2.1.5/PKG-INFO` & `speedtab-0.2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.2.1.5
+Version: 0.2.1.6
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

