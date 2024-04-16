# Comparing `tmp/freeze_dried_data-1.2.1.tar.gz` & `tmp/freeze_dried_data-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-1.2.1.tar", last modified: Fri Apr 12 22:49:39 2024, max compression
+gzip compressed data, was "freeze_dried_data-1.2.2.tar", last modified: Tue Apr 16 21:50:04 2024, max compression
```

## Comparing `freeze_dried_data-1.2.1.tar` & `freeze_dried_data-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:49:39.738818 freeze_dried_data-1.2.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-12 22:33:49.000000 freeze_dried_data-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-12 22:49:39.738818 freeze_dried_data-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5786 2024-04-12 22:33:49.000000 freeze_dried_data-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:49:39.738818 freeze_dried_data-1.2.1/freeze_dried_data/
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-12 22:33:49.000000 freeze_dried_data-1.2.1/freeze_dried_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10525 2024-04-12 22:33:49.000000 freeze_dried_data-1.2.1/freeze_dried_data/freeze_dried_data.py
--rw-r--r--   0 root         (0) root         (0)     7883 2024-04-12 22:33:49.000000 freeze_dried_data-1.2.1/freeze_dried_data/test_freeze_dried_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 22:49:39.738818 freeze_dried_data-1.2.1/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-12 22:49:39.000000 freeze_dried_data-1.2.1/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-12 22:49:39.000000 freeze_dried_data-1.2.1/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 22:49:39.000000 freeze_dried_data-1.2.1/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-12 22:49:39.000000 freeze_dried_data-1.2.1/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 22:49:39.738818 freeze_dried_data-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-12 22:33:49.000000 freeze_dried_data-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:04.170532 freeze_dried_data-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7523 2024-04-16 21:50:04.170532 freeze_dried_data-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6657 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:04.166532 freeze_dried_data-1.2.2/freeze_dried_data/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/freeze_dried_data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10858 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/freeze_dried_data/freeze_dried_data.py
+-rw-r--r--   0 root         (0) root         (0)     7889 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/freeze_dried_data/test_freeze_dried_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:04.166532 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7523 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      303 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 21:50:04.170532 freeze_dried_data-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/setup.py
```

### Comparing `freeze_dried_data-1.2.1/LICENSE` & `freeze_dried_data-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-1.2.1/PKG-INFO` & `freeze_dried_data-1.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,14 +19,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Freeze Dried Data
 A very simple format for machine learning datasets.
 
+FDD allows your entire dataset to be a single file. Instances are only loaded from disk when needed and can be loaded in random order.
+
 FDD treats datasets stored on disk as if they were Python dictionaries. It is designed for speed and simplicity.
 
 Keys can be any picklable objects that are valid dictionary keys, and are stored in memory until the file is closed. Values can be any picklable object and are stored on disk.
 
 FDD files can operate in either read mode or write mode. Once a file is finalized, it cannot be modified (i.e., it is "freeze-dried").
 
 Values are written to disk immediately upon insertion, while keys are written as part of the index when the FDD file is closed.
@@ -42,21 +44,21 @@
 ### Custom Properties
 - **Custom Properties**: Extend the flexibility of FDD files by allowing users to add custom attributes or metadata to the datasets. These properties are saved and loaded with the file, making it easy to store additional contextual information alongside your data.
 
 ### Compression Support
 - **Compression**: Optimize storage and speed by compressing the dataset files. FDD supports multiple compression algorithms including zlib, bz2, and gzip, which can significantly reduce the disk space used by large datasets.
 
 ### File Modes
-- **Explicit File Modes**: Control how files are accessed with `write_or_overwrite` and `read_only` modes. This ensures data integrity by preventing unwanted modifications and handling file access errors gracefully.
+- **Explicit and Implicit File Modes**: Control how files are accessed with `write_or_overwrite` and `read_only` modes. Setting `write_or_overwrite` discards existing files. The `read_only` mode opens files exclusively for reading, throwing an error if the file doesn't exist. If neither mode is specified, the library defaults to read mode for existing files and write mode for new files.
 
 ### Pythonic Interface
 - **Python Dictionary-Like Interface**: FDD files act like Python dictionaries. This makes them intuitive to use for Python developers, as they can employ familiar dictionary operations to interact with the datasets.
 
 ### Seamless Integration
-- **Seamless Integration with Data Loaders**: FDD is designed to work effortlessly with data loaders in machine learning frameworks like PyTorch. This allows for easy use of FDD files in multi-process data loading, which is essential for efficient training of models on large datasets.
+- **Seamless Integration with Data Loaders**: FDD is designed to work effortlessly with data loaders in machine learning frameworks like PyTorch. This allows for easy use of FDD files in multi-process data loading, which is essential for efficient training of models on large datasets. 
 
 ### Context Management
 - **Context Management Support**: FDD supports Python’s context management (using `with` statements), which ensures that files are properly closed after operations are completed, preventing data corruption and resource leaks.
 
 ## Examples
 
 ### Example 1: Creating an FDD File
@@ -145,25 +147,41 @@
 
 ### Example 6: Using in a PyTorch DataLoader with Workers
 ```python
 import torch
 from torch.utils.data import Dataset, DataLoader
 from freeze_dried_data import FDD
 
+with FDD('new dataset.fdd', write_or_overwrite=True) as dataset:
+    dataset.train_keys = ['key1', 'key2', 'key3']
+    dataset.val_keys = ['key4', 'key5']
+    dataset['key1'] = 'train_data1'
+    dataset['key2'] = 'train_data2'
+    dataset['key3'] = 'train_data3'
+    dataset['key4'] = 'val_data1'
+    dataset['key5'] = 'val_data2'
+
 class FDDDataset(Dataset):
-    def __init__(self, filename):
+    def __init__(self, filename, split='train'):
         self.fdd = FDD(filename, read_only=True)
-        self.keys = list(self.fdd.index.keys())
+        if split == 'train':
+            self.keys = self.fdd.train_keys
+        else:
+            self.keys = self.fdd.val_keys
     
     def __len__(self):
-        return len(self.fdd)
+        return len(self.keys)
     
     def __getitem__(self, idx):
         key = self.keys[idx]
         return key, self.fdd[key]
 
-dataset = FDDDataset('new dataset.fdd')
+dataset = FDDDataset('new dataset.fdd', split='train')
 dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=4)
 
 for key, value in dataloader:
     print(f'Batch: {key} - {value}')
+
+# Example output:
+# Batch: ('key3', 'key2') - ('train_data3', 'train_data2')
+# Batch: ('key1',) - ('train_data1',)
 ```
```

### Comparing `freeze_dried_data-1.2.1/README.md` & `freeze_dried_data-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Freeze Dried Data
 A very simple format for machine learning datasets.
 
+FDD allows your entire dataset to be a single file. Instances are only loaded from disk when needed and can be loaded in random order.
+
 FDD treats datasets stored on disk as if they were Python dictionaries. It is designed for speed and simplicity.
 
 Keys can be any picklable objects that are valid dictionary keys, and are stored in memory until the file is closed. Values can be any picklable object and are stored on disk.
 
 FDD files can operate in either read mode or write mode. Once a file is finalized, it cannot be modified (i.e., it is "freeze-dried").
 
 Values are written to disk immediately upon insertion, while keys are written as part of the index when the FDD file is closed.
@@ -20,21 +22,21 @@
 ### Custom Properties
 - **Custom Properties**: Extend the flexibility of FDD files by allowing users to add custom attributes or metadata to the datasets. These properties are saved and loaded with the file, making it easy to store additional contextual information alongside your data.
 
 ### Compression Support
 - **Compression**: Optimize storage and speed by compressing the dataset files. FDD supports multiple compression algorithms including zlib, bz2, and gzip, which can significantly reduce the disk space used by large datasets.
 
 ### File Modes
-- **Explicit File Modes**: Control how files are accessed with `write_or_overwrite` and `read_only` modes. This ensures data integrity by preventing unwanted modifications and handling file access errors gracefully.
+- **Explicit and Implicit File Modes**: Control how files are accessed with `write_or_overwrite` and `read_only` modes. Setting `write_or_overwrite` discards existing files. The `read_only` mode opens files exclusively for reading, throwing an error if the file doesn't exist. If neither mode is specified, the library defaults to read mode for existing files and write mode for new files.
 
 ### Pythonic Interface
 - **Python Dictionary-Like Interface**: FDD files act like Python dictionaries. This makes them intuitive to use for Python developers, as they can employ familiar dictionary operations to interact with the datasets.
 
 ### Seamless Integration
-- **Seamless Integration with Data Loaders**: FDD is designed to work effortlessly with data loaders in machine learning frameworks like PyTorch. This allows for easy use of FDD files in multi-process data loading, which is essential for efficient training of models on large datasets.
+- **Seamless Integration with Data Loaders**: FDD is designed to work effortlessly with data loaders in machine learning frameworks like PyTorch. This allows for easy use of FDD files in multi-process data loading, which is essential for efficient training of models on large datasets. 
 
 ### Context Management
 - **Context Management Support**: FDD supports Python’s context management (using `with` statements), which ensures that files are properly closed after operations are completed, preventing data corruption and resource leaks.
 
 ## Examples
 
 ### Example 1: Creating an FDD File
@@ -123,25 +125,41 @@
 
 ### Example 6: Using in a PyTorch DataLoader with Workers
 ```python
 import torch
 from torch.utils.data import Dataset, DataLoader
 from freeze_dried_data import FDD
 
+with FDD('new dataset.fdd', write_or_overwrite=True) as dataset:
+    dataset.train_keys = ['key1', 'key2', 'key3']
+    dataset.val_keys = ['key4', 'key5']
+    dataset['key1'] = 'train_data1'
+    dataset['key2'] = 'train_data2'
+    dataset['key3'] = 'train_data3'
+    dataset['key4'] = 'val_data1'
+    dataset['key5'] = 'val_data2'
+
 class FDDDataset(Dataset):
-    def __init__(self, filename):
+    def __init__(self, filename, split='train'):
         self.fdd = FDD(filename, read_only=True)
-        self.keys = list(self.fdd.index.keys())
+        if split == 'train':
+            self.keys = self.fdd.train_keys
+        else:
+            self.keys = self.fdd.val_keys
     
     def __len__(self):
-        return len(self.fdd)
+        return len(self.keys)
     
     def __getitem__(self, idx):
         key = self.keys[idx]
         return key, self.fdd[key]
 
-dataset = FDDDataset('new dataset.fdd')
+dataset = FDDDataset('new dataset.fdd', split='train')
 dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=4)
 
 for key, value in dataloader:
     print(f'Batch: {key} - {value}')
+
+# Example output:
+# Batch: ('key3', 'key2') - ('train_data3', 'train_data2')
+# Batch: ('key1',) - ('train_data1',)
 ```
```

### Comparing `freeze_dried_data-1.2.1/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-1.2.2/freeze_dried_data/freeze_dried_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,17 +224,27 @@
         self.file = open(self.filename, 'rb+')
 
     def keys(self) -> Iterator[Any]:
         """ Return an iterator over the keys in the file. """
         return self.index.keys()
 
     def items(self) -> Iterator[Tuple[Any, Any]]:
-        """ Yield (key, value) pairs. """
-        for k in self.keys():
-            yield k, self[k]
+        """ Yield (key, value) pairs, with length awareness for tqdm compatibility. """
+        class ItemsWithLength:
+            def __init__(self, parent):
+                self.parent = parent
+
+            def __iter__(self):
+                for k in self.parent.keys():
+                    yield k, self.parent[k]
+
+            def __len__(self):
+                return len(self.parent.index)
+
+        return ItemsWithLength(self)
 
     def __contains__(self, item: Any) -> bool:
         """ Check if a key exists in the index. """
         return item in self.index
 
     def __len__(self) -> int:
         """ Return the number of items in the file. """
```

### Comparing `freeze_dried_data-1.2.1/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-1.2.2/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,18 @@
             fdd['key3'] = 'value3'
 
             self.assertEqual(len(fdd), 3)
 
         with FDD(self.test_file, read_only=True) as fdd:
             self.assertEqual(fdd.property_one, 'changed')
             self.assertEqual(fdd.property_two, 123)
+            dct = {}
             for k,v in fdd.items():
-                self.assertTrue(k in ['key1', 'key2', 'key3'])
-                self.assertTrue(v in ['value1', 'value2', 'value3'])
+                dct[k] = v
+            self.assertEqual(dct, {'key1': 'value1', 'key2': 'value2', 'key3': 'value3'})
     
     def test_delete_custom_attributes(self):
         with FDD(self.test_file, write_or_overwrite=True) as fdd:
             fdd.some_property = 'value'
             self.assertEqual(fdd.some_property, 'value')
 
             # Now delete the property
```

### Comparing `freeze_dried_data-1.2.1/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-1.2.2/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-dried-data
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,14 +19,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Freeze Dried Data
 A very simple format for machine learning datasets.
 
+FDD allows your entire dataset to be a single file. Instances are only loaded from disk when needed and can be loaded in random order.
+
 FDD treats datasets stored on disk as if they were Python dictionaries. It is designed for speed and simplicity.
 
 Keys can be any picklable objects that are valid dictionary keys, and are stored in memory until the file is closed. Values can be any picklable object and are stored on disk.
 
 FDD files can operate in either read mode or write mode. Once a file is finalized, it cannot be modified (i.e., it is "freeze-dried").
 
 Values are written to disk immediately upon insertion, while keys are written as part of the index when the FDD file is closed.
@@ -42,21 +44,21 @@
 ### Custom Properties
 - **Custom Properties**: Extend the flexibility of FDD files by allowing users to add custom attributes or metadata to the datasets. These properties are saved and loaded with the file, making it easy to store additional contextual information alongside your data.
 
 ### Compression Support
 - **Compression**: Optimize storage and speed by compressing the dataset files. FDD supports multiple compression algorithms including zlib, bz2, and gzip, which can significantly reduce the disk space used by large datasets.
 
 ### File Modes
-- **Explicit File Modes**: Control how files are accessed with `write_or_overwrite` and `read_only` modes. This ensures data integrity by preventing unwanted modifications and handling file access errors gracefully.
+- **Explicit and Implicit File Modes**: Control how files are accessed with `write_or_overwrite` and `read_only` modes. Setting `write_or_overwrite` discards existing files. The `read_only` mode opens files exclusively for reading, throwing an error if the file doesn't exist. If neither mode is specified, the library defaults to read mode for existing files and write mode for new files.
 
 ### Pythonic Interface
 - **Python Dictionary-Like Interface**: FDD files act like Python dictionaries. This makes them intuitive to use for Python developers, as they can employ familiar dictionary operations to interact with the datasets.
 
 ### Seamless Integration
-- **Seamless Integration with Data Loaders**: FDD is designed to work effortlessly with data loaders in machine learning frameworks like PyTorch. This allows for easy use of FDD files in multi-process data loading, which is essential for efficient training of models on large datasets.
+- **Seamless Integration with Data Loaders**: FDD is designed to work effortlessly with data loaders in machine learning frameworks like PyTorch. This allows for easy use of FDD files in multi-process data loading, which is essential for efficient training of models on large datasets. 
 
 ### Context Management
 - **Context Management Support**: FDD supports Python’s context management (using `with` statements), which ensures that files are properly closed after operations are completed, preventing data corruption and resource leaks.
 
 ## Examples
 
 ### Example 1: Creating an FDD File
@@ -145,25 +147,41 @@
 
 ### Example 6: Using in a PyTorch DataLoader with Workers
 ```python
 import torch
 from torch.utils.data import Dataset, DataLoader
 from freeze_dried_data import FDD
 
+with FDD('new dataset.fdd', write_or_overwrite=True) as dataset:
+    dataset.train_keys = ['key1', 'key2', 'key3']
+    dataset.val_keys = ['key4', 'key5']
+    dataset['key1'] = 'train_data1'
+    dataset['key2'] = 'train_data2'
+    dataset['key3'] = 'train_data3'
+    dataset['key4'] = 'val_data1'
+    dataset['key5'] = 'val_data2'
+
 class FDDDataset(Dataset):
-    def __init__(self, filename):
+    def __init__(self, filename, split='train'):
         self.fdd = FDD(filename, read_only=True)
-        self.keys = list(self.fdd.index.keys())
+        if split == 'train':
+            self.keys = self.fdd.train_keys
+        else:
+            self.keys = self.fdd.val_keys
     
     def __len__(self):
-        return len(self.fdd)
+        return len(self.keys)
     
     def __getitem__(self, idx):
         key = self.keys[idx]
         return key, self.fdd[key]
 
-dataset = FDDDataset('new dataset.fdd')
+dataset = FDDDataset('new dataset.fdd', split='train')
 dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=4)
 
 for key, value in dataloader:
     print(f'Batch: {key} - {value}')
+
+# Example output:
+# Batch: ('key3', 'key2') - ('train_data3', 'train_data2')
+# Batch: ('key1',) - ('train_data1',)
 ```
```

### Comparing `freeze_dried_data-1.2.1/setup.py` & `freeze_dried_data-1.2.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='1.2.1',
+    version='1.2.2',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

