# Comparing `tmp/dutree-1.7.tar.gz` & `tmp/dutree-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dutree-1.7.tar", last modified: Tue Apr  9 09:33:57 2024, max compression
+gzip compressed data, was "dutree-1.8.tar", last modified: Tue Apr 16 14:41:41 2024, max compression
```

## Comparing `dutree-1.7.tar` & `dutree-1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2024-04-09 09:33:57.000000 dutree-1.7/
--rw-rw-r--   0 walter    (1000) walter    (1000)     2748 2024-04-09 09:30:53.000000 dutree-1.7/README.rst
--rw-rw-r--   0 walter    (1000) walter    (1000)     4199 2024-04-09 09:33:57.000000 dutree-1.7/PKG-INFO
--rw-rw-r--   0 walter    (1000) walter    (1000)     2101 2024-04-09 09:30:53.000000 dutree-1.7/setup.py
-drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2024-04-09 09:33:57.000000 dutree-1.7/dutree/
--rw-rw-r--   0 walter    (1000) walter    (1000)    11664 2024-04-09 09:01:09.000000 dutree-1.7/dutree/test_dutree.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     1439 2019-01-31 14:33:58.000000 dutree-1.7/dutree/__init__.py
--rwxrwxr-x   0 walter    (1000) walter    (1000)    21287 2024-04-09 09:30:53.000000 dutree-1.7/dutree/dutree.py
--rw-rw-r--   0 walter    (1000) walter    (1000)     7530 2024-04-09 09:30:53.000000 dutree-1.7/dutree/bogofs.py
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2024-04-16 14:41:41.736314 dutree-1.8/
+-rw-rw-r--   0 walter    (1000) walter    (1000)     4426 2024-04-16 14:41:41.736314 dutree-1.8/PKG-INFO
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2919 2024-04-16 14:41:29.460249 dutree-1.8/README.rst
+drwxrwxr-x   0 walter    (1000) walter    (1000)        0 2024-04-16 14:41:41.736314 dutree-1.8/dutree/
+-rw-rw-r--   0 walter    (1000) walter    (1000)     1439 2019-01-31 14:33:58.896460 dutree-1.8/dutree/__init__.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     7530 2024-04-09 09:30:53.352228 dutree-1.8/dutree/bogofs.py
+-rwxrwxr-x   0 walter    (1000) walter    (1000)    30656 2024-04-16 14:41:29.460249 dutree-1.8/dutree/dutree.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)    11664 2024-04-09 09:01:09.665405 dutree-1.8/dutree/test_dutree.py
+-rw-rw-r--   0 walter    (1000) walter    (1000)     2101 2024-04-16 14:41:29.460249 dutree-1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dutree-1.7/README.rst` & `dutree-1.8/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,21 @@
     python2 dutree/test_dutree.py
     python3 dutree/test_dutree.py
 
 
 History
 -------
 
+* v1.8
+
+  - **Add experimental feature to do scanning from a file instead of the
+    filesystem.**
+    See commit bbebcf98 for details.
+    Original code by Seppe Lucas.
+
 * v1.7
 
   - **Skip /proc and /sys filesystems by default.**
   - **Use --xdev to stay on the same filesystem.**
   - **Uses --count-blocks by default; use --apparent-size to negate.**
 
 * v1.6
```

### Comparing `dutree-1.7/PKG-INFO` & `dutree-1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dutree
-Version: 1.7
+Version: 1.8
 Summary: Disk usage summary, showing large dirs/files
 Home-page: https://github.com/ossobv/dutree
 Author: Walter Doekes, OSSO B.V.
 Author-email: wjdoekes+dutree@osso.nl
 License: GPLv3+
 Description: dutree :: Disk usage summary
         ============================
@@ -73,14 +73,21 @@
             python2 dutree/test_dutree.py
             python3 dutree/test_dutree.py
         
         
         History
         -------
         
+        * v1.8
+        
+          - **Add experimental feature to do scanning from a file instead of the
+            filesystem.**
+            See commit bbebcf98 for details.
+            Original code by Seppe Lucas.
+        
         * v1.7
         
           - **Skip /proc and /sys filesystems by default.**
           - **Use --xdev to stay on the same filesystem.**
           - **Uses --count-blocks by default; use --apparent-size to negate.**
         
         * v1.6
```

### Comparing `dutree-1.7/setup.py` & `dutree-1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from os.path import dirname, join
 
 
 if __name__ == '__main__':
     long_descriptions = []
     with open(join(dirname(__file__), 'README.rst')) as file:
         long_descriptions.append(file.read())
-    version = '1.7'
+    version = '1.8'
 
     setup(
         name='dutree',
         version=version,
         data_files=[('share/doc/dutree', ['README.rst'])],
         entry_points={'console_scripts': ['dutree = dutree.dutree:main']},
         packages=['dutree'],
```

### Comparing `dutree-1.7/dutree/test_dutree.py` & `dutree-1.8/dutree/test_dutree.py`

 * *Files identical despite different names*

### Comparing `dutree-1.7/dutree/__init__.py` & `dutree-1.8/dutree/__init__.py`

 * *Files identical despite different names*

### Comparing `dutree-1.7/dutree/dutree.py` & `dutree-1.8/dutree/dutree.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,19 +49,21 @@
 #                    takes up a tiny bit of space
 #       -----
 #      80.6 G  TOTAL (86558511658)
 #
 # **NOTE**: The directories do not count the size of themselves, only of
 # their contents. This explains any discrepancies with ``du -sb`` output.
 #
+from __future__ import print_function
+
 import argparse
 import sys
 import warnings
 
-from os import listdir, lstat, path
+from os import environ, listdir, lstat, path
 from stat import S_ISDIR, S_ISREG
 
 
 class OsWarning(UserWarning):
     pass
 
 
@@ -298,20 +300,23 @@
         return '  {:12d}  {}'.format(self.app_size(), name)
 
 
 class DuScan:
     "Disk Usage Tree scanner"
 
     def __init__(self, pathname):
+        if not path.isdir(pathname):
+            # ENOTDIR
+            raise OSError(20, 'Not a directory: {!r}'.format(pathname))
+
         self._dev_allow = []
         self._dev_deny = []
         self._dev = lstat(pathname).st_dev
-        self._path = self._normpath(pathname)
+        self._path = pathname.rstrip('/')  # no trailing slashes
         self._tree = None
-        self._check_path()
 
     def skip_other_filesystems(self):
         self._dev_allow = [self._dev]
 
     def skip_proc_sys_filesystems(self):
         """
         Skip /proc and /sys. There's nothing of interest for us there
@@ -326,28 +331,14 @@
                 warnings.warn(
                     '{} not found, so device is not skipped'.format(devname),
                     OsWarning)
             finally:
                 if device != self._dev:
                     self._dev_deny.append(device)
 
-    def _normpath(self, pathname):
-        "Return path normalized for duscan usage: no trailing slash."
-        if pathname == '/':
-            pathname = ''
-        elif pathname.endswith('/'):
-            pathname = pathname[:-1]
-        assert not pathname.endswith('/'), pathname
-        return pathname
-
-    def _check_path(self):
-        "Immediately check if we can access path. Otherwise bail."
-        if not path.isdir(self._path or '/'):
-            raise OSError('Path {!r} is not a directory'.format(self._path))
-
     def scan(self, use_apparent_size=True):
         assert self._tree is None
         self._tree = DuNode.new_dir(self._path)
         self._app_subtotal = self._use_subtotal = 0
         app_leftover_bytes, use_leftover_bytes, new_fraction, keep_node = (
             self._scan(self._path, self._tree, use_apparent_size))
         assert keep_node and not app_leftover_bytes, (
@@ -358,19 +349,24 @@
         self._tree.prune_if_smaller_than(
             new_fraction, use_apparent_size)
         self._tree.merge_upwards_if_smaller_than(
             new_fraction, use_apparent_size)
         return self._tree
 
     def _scan(self, pathname, parent_node, a_or_u):
-        fraction = (  # initialize fraction
+        fraction = (    # initialize fraction
             (self._use_subtotal, self._app_subtotal)[a_or_u] // 20)
-        children = []                        # large separate child nodes
+        children = []   # large separate child nodes
 
         try:
+            # The code has been tried using os.scandir(). It improved nothing:
+            # - If it's a file, we have to lstat always;
+            # - if it's a directory, we could skip the lstat, but we
+            #   have to os.scandir() it, and that does a newfstatat()
+            #   anyway.
             files = listdir(pathname or '/')
         except OSError as e:
             # PermissionError: [Errno 13] Permission denied:
             #   '/sys/fs/fuse/connections/85'
             warnings.warn(str(e), OsWarning)
             app_mixed_total = 0
             use_mixed_total = 0
@@ -478,14 +474,267 @@
             # Recalculate fraction based on updated subtotal.
             fraction = (
                 (self._use_subtotal, self._app_subtotal)[a_or_u] // 20)
 
         return app_mixed_total, use_mixed_total, fraction
 
 
+class PlanbSwiftSyncListFiles:
+    """
+    Path object generator used by the PlanB SwiftSync Disk Usage Tree scanner
+
+    Scans a single text file that has the following format:
+
+        media/0023f5ac/1080.jpg|2022-02-24T09:58:28.598120|113948
+        media/0023f5ac/2668.jpg|2021-06-08T07:03:33.043100|241190
+        media/0023f5ac/3224.jpg|2021-06-08T07:03:35.341960|66773
+        ...
+
+    Or optionally with container/bucket prefix:
+
+        bucket1|media/0023f5ac/1080.jpg|2022-02-24T09:58:28.598120|113948
+        bucket1|media/0023f5ac/2668.jpg|2021-06-08T07:03:33.043100|241190
+        bucket1|media/0023f5ac/3224.jpg|2021-06-08T07:03:35.341960|66773
+        ...
+
+    Allows the files to be listed by:
+
+        planbswiftsynclistfiles.listdir(pathobj)
+
+    Where pathobj is a previously returned object from get_root() or listdir().
+
+    A path object looks like this:
+
+        (pathname, filesize_if_dir_else_None, path_without_slash_length)
+
+    I would have preferred a nice object, but all the indirection in
+    Python takes valuable CPU user time. This tuple layout seemed to be
+    fastest.
+
+    Users have to know:
+
+        - If tuple[1] is None, the path is a directory.
+        - If tuple[1] is not None, it is an integer size. The path is a file.
+        - The path name (file or directory) is tuple[0][0:tuple[2]].
+
+    The manual slicing hopes to avoid many duplicate Python objects in memory:
+
+        - Instead of "A/", "A/B/", "A/B/C.txt",
+        - we have "A/B/C.txt" three times with lengths: 1, 3, 9.
+
+    The mentioned file format is used by PlanB SwiftSync
+    https://github.com/ossobv/planb/blob/main/contrib/planb-swiftsync.py
+    """
+    def __init__(self, filename, root_name=''):
+        self._root_with_slash = root_name + '/'
+        self._fp = open(filename, 'rb')
+        self._fpit = iter(self._fp)
+
+        # We must store the currently available file here, because
+        # multiple invocations of PlanbSwiftSyncListFiles.listdir() can
+        # use it.
+        self._fileobj = None
+
+    def close(self):
+        """
+        Close this when done
+        """
+        self._fp.close()
+        self._fp = None
+
+    def get_root(self):
+        """
+        Construct the root path object that we'll use to start the scan
+
+        Every path object returned by PlanbSwiftSyncListFiles is a::
+
+            (pathname, filesize_if_dir_else_None, path_without_slash_length)
+
+        We would like this to be a nice object instead, but that is
+        significantly slower.
+        """
+        return (
+            self._root_with_slash, None, len(self._root_with_slash) - 1)
+
+    def get(self):
+        """
+        Get a path object from the filelist
+
+        The path object looks like::
+
+            (filename, filesize, filename_length)
+
+        That is a subset of the path object. The filelist only contains
+        files, so we'll only return the leaf objects here.
+
+        At EOF, get() raises a StopIteration.
+        """
+        if self._fileobj is not None:
+            return self._fileobj
+
+        # Can raise StopIteration
+        line = next(self._fpit).decode('utf-8')
+
+        filename, date, filesize = line.rsplit('|', 2)
+        filename = (
+            self._root_with_slash +
+            filename.replace('|', '/').rstrip('/'))
+        filesize = int(filesize)
+
+        # Again, the tuple:
+        # (pathname, size_if_dir_else_None, path_without_slash_length)
+        # Instead of substrings, we pass "string slices" around by
+        # manually passing the length of the path name.
+        self._fileobj = (filename, filesize, len(filename))
+
+        return self._fileobj
+
+    def use(self):
+        self._fileobj = None
+
+    def listdir(self, dirobj):
+        dirname, dirsize, dirlength = dirobj
+        # assert dirsize is None, (dirname, dirsize, dirlength)
+
+        while True:
+            # For path object A/B/C/D and dirobj A/B, we have the
+            # following cases:
+            # - A/B/C/D -> a child listdir() will pick this up;
+            # - A/B/C/ -> we pick this up
+            # - A/B/C.txt -> we pick this up
+            # - A/C -> a parent listdir() picks this up.
+            try:
+                # This pathobj can change between runs, even though we
+                # do not self.use() it. Why? Because child listdir()s
+                # will also use it, and if _they_ are at the file level,
+                # they will mark it as used.
+                pathobj = self.get()
+            except StopIteration:
+                # EOF
+                break
+
+            if not pathobj[0].startswith(dirname[0:(dirlength + 1)]):
+                # New file is higher in the directory tree. Parent
+                # listdir() will continue.
+                break
+
+            slashidx = pathobj[0].find('/', dirlength + 1)
+            if slashidx > -1:
+                # New file is in this directory tree.
+                yield (pathobj[0], None, slashidx)
+
+            else:
+                # New file is in this directory tree, and it is a file.
+                # assert pathobj[1] is not None, pathobj
+                yield pathobj
+
+                # We're done with the file (and no one has needed to
+                # listdir() anything yet, because this was a leaf), mark
+                # it as used.
+                self.use()
+
+
+class PlanbSwiftSyncDuScan:
+    """
+    PlanB SwiftSync (file) Disk Usage Tree scanner
+
+    See PlanbSwiftSyncListFiles docs for the file format it scans.
+    """
+    def __init__(self, pathname, root_name=''):  # 'ROOT'
+        self._listfiles = PlanbSwiftSyncListFiles(pathname, root_name)
+        self._path = self._listfiles.get_root()
+        self._tree = None
+
+    def scan(self, use_apparent_size=None):
+        assert self._tree is None
+        self._tree = DuNode.new_dir(self._path[0][0:self._path[2]])
+        self._app_subtotal = 0
+        app_leftover_bytes, new_fraction, keep_node = (
+            self._scan(self._path, self._tree))
+        assert keep_node and not app_leftover_bytes, (
+            keep_node, app_leftover_bytes)
+
+        # Close our file.
+        self._listfiles.close()
+
+        # Do another prune run, since the fraction size has grown during the
+        # scan. Then merge nodes that couldn't get merged sooner.
+        self._tree.prune_if_smaller_than(new_fraction, True)
+        self._tree.merge_upwards_if_smaller_than(new_fraction, True)
+        return self._tree
+
+    def _scan(self, pathobj, parent_node):
+        fraction = self._app_subtotal // 20
+        children = []   # large separate child nodes
+
+        try:
+            files = self._listfiles.listdir(pathobj)
+        except OSError as e:
+            # PermissionError: [Errno 13] Permission denied:
+            #   '/sys/fs/fuse/connections/85'
+            warnings.warn(str(e), OsWarning)
+            app_mixed_total = 0
+        else:
+            app_mixed_total, fraction = (
+                self._scan_inner(files, children, fraction))
+
+        # Do we have children or a total that's large enough: keep this
+        # node.
+        if children or app_mixed_total >= fraction:
+            parent_node.add_branches(*children)
+            if children:
+                filename, filesize, length = pathobj
+                pathname = filename[0:length]
+                child_node = DuNode.new_leftovers(
+                    pathname, app_mixed_total, app_mixed_total)
+                parent_node.add_branches(child_node)
+            else:
+                parent_node._set_size(app_mixed_total, app_mixed_total)
+            app_mixed_total = 0
+            keep_node = True
+        else:
+            keep_node = False
+
+        # Leftovers, the new fraction and whether to keep the child.
+        return app_mixed_total, fraction, keep_node
+
+    def _scan_inner(self, files, children, fraction):
+        app_mixed_total = 0  # "rest of the dir", add to this node
+
+        for pathobj in files:
+            pathname, pathsize, pathlength = pathobj
+
+            if pathsize is not None:
+                if pathsize >= fraction:
+                    child_node = DuNode.new_file(pathname, pathsize, pathsize)
+                    children.append(child_node)
+                    self._app_subtotal += child_node.app_size()
+                else:
+                    # The file is too small and it doesn't get its own
+                    # node. Count it on this node.
+                    app_mixed_total += pathsize
+                    self._app_subtotal += pathsize
+
+            else:
+                child_node = DuNode.new_dir(pathname[0:pathlength])
+
+                app_leftover_bytes, fraction, keep_node = (
+                    self._scan(pathobj, child_node))
+                if keep_node:
+                    # assert not app_leftover_bytes, app_leftover_bytes
+                    children.append(child_node)
+                else:
+                    app_mixed_total += app_leftover_bytes
+
+            # Recalculate fraction based on updated subtotal.
+            fraction = self._app_subtotal // 20
+
+        return app_mixed_total, fraction
+
+
 def human(value):
     "If val>=1000 return val/1024+KiB, etc."
     if value >= 1073741824000:
         return '{:.1f} T'.format(value / 1099511627776.0)
     if value >= 1048576000:
         return '{:.1f} G'.format(value / 1073741824.0)
     if value >= 1024000:
@@ -516,33 +765,47 @@
     args = parser.parse_args()
 
     if args.count_blocks:
         warnings.warn(
             '--count-blocks is default now, use --apparent-size to negate',
             OsWarning)
 
-    run(pathname=args.path, use_apparent_size=args.apparent_size,
-        xdev=args.xdev, skip_proc_sys=(not args.no_skip_proc_sys))
+    try:
+        run(pathname=args.path, use_apparent_size=args.apparent_size,
+            xdev=args.xdev, skip_proc_sys=(not args.no_skip_proc_sys))
+    except OSError as e:
+        print('dutree: error: {}'.format(e), file=sys.stderr)
+        exit(1)
 
 
 def run(pathname, use_apparent_size, xdev, skip_proc_sys):
     if use_apparent_size:
         def getsize(node):
             return node.app_size()
     else:
         def getsize(node):
             return node.use_size()
 
     verbose = True and not use_apparent_size
-    scanner = DuScan(pathname)
-    if xdev:
-        scanner.skip_other_filesystems()
-    elif skip_proc_sys:
-        scanner.skip_proc_sys_filesystems()
+
+    try:
+        scanner = DuScan(pathname)
+        if xdev:
+            scanner.skip_other_filesystems()
+        elif skip_proc_sys:
+            scanner.skip_proc_sys_filesystems()
+    except OSError as e:
+        if e.args[0] == 20 and environ.get('DUTREE_EXPERIMENTAL'):  # ENOTDIR
+            scanner = PlanbSwiftSyncDuScan(
+                pathname, '{{{}}}'.format(pathname))
+        else:
+            raise
+
     tree = scanner.scan(use_apparent_size=use_apparent_size)
+
     for leaf in tree.get_leaves():
         sys.stdout.write(' {0:>7s}  {1}{2}\n'.format(
             human(getsize(leaf)), leaf.name(),
             (' (app={})'.format(human(leaf.app_size())) if verbose else '')))
     sys.stdout.write('   -----\n')
     size = getsize(tree)
     sys.stdout.write(' {0:>7s}  TOTAL ({1}{2})\n'.format(
```

### Comparing `dutree-1.7/dutree/bogofs.py` & `dutree-1.8/dutree/bogofs.py`

 * *Files identical despite different names*

