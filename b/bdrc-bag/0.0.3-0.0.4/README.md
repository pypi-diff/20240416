# Comparing `tmp/bdrc_bag-0.0.3-py3-none-any.whl.zip` & `tmp/bdrc_bag-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 20996 bytes, number of entries: 9
--rw-r--r--  2.0 unx       34 b- defN 24-Mar-07 20:55 bdrc_bag/__init__.py
--rw-r--r--  2.0 unx     6197 b- defN 24-Mar-08 23:46 bdrc_bag/bag_main.py
--rw-r--r--  2.0 unx    12290 b- defN 24-Mar-08 21:12 bdrc_bag/bag_ops.py
--rw-r--r--  2.0 unx    35149 b- defN 24-Mar-08 23:47 bdrc_bag-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1777 b- defN 24-Mar-08 23:47 bdrc_bag-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-08 23:47 bdrc_bag-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Mar-08 23:47 bdrc_bag-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-08 23:47 bdrc_bag-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      716 b- defN 24-Mar-08 23:47 bdrc_bag-0.0.3.dist-info/RECORD
-9 files, 56316 bytes uncompressed, 19762 bytes compressed:  64.9%
+Zip file size: 21127 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       34 b- defN 24-Mar-11 16:19 bdrc_bag/__init__.py
+-rw-r--r--  2.0 unx     6197 b- defN 24-Mar-11 16:19 bdrc_bag/bag_main.py
+-rw-r--r--  2.0 unx    12486 b- defN 24-Apr-15 22:02 bdrc_bag/bag_ops.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-Apr-16 16:45 bdrc_bag-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1948 b- defN 24-Apr-16 16:45 bdrc_bag-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 16:45 bdrc_bag-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-16 16:45 bdrc_bag-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-16 16:45 bdrc_bag-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      716 b- defN 24-Apr-16 16:45 bdrc_bag-0.0.4.dist-info/RECORD
+9 files, 56683 bytes uncompressed, 19893 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: bdrc_bag/bag_main.py
 Comment: 
 
 Filename: bdrc_bag/bag_ops.py
 Comment: 
 
-Filename: bdrc_bag-0.0.3.dist-info/LICENSE
+Filename: bdrc_bag-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: bdrc_bag-0.0.3.dist-info/METADATA
+Filename: bdrc_bag-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: bdrc_bag-0.0.3.dist-info/WHEEL
+Filename: bdrc_bag-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: bdrc_bag-0.0.3.dist-info/entry_points.txt
+Filename: bdrc_bag-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: bdrc_bag-0.0.3.dist-info/top_level.txt
+Filename: bdrc_bag-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: bdrc_bag-0.0.3.dist-info/RECORD
+Filename: bdrc_bag-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bdrc_bag/bag_ops.py

```diff
@@ -232,64 +232,66 @@
 # --test_bag-size BAG_SIZE
 # --test_bag-group-identifier BAG_GROUP_IDENTIFIER
 # --test_bag-count BAG_COUNT
 # --internal-sender-identifier INTERNAL_SENDER_IDENTIFIER
 # --internal-sender-description INTERNAL_SENDER_DESCRIPTION
 # --bagit-profile-identifier BAGIT_PROFILE_IDENTIFIER
 
-def bag(bag_src: str, bag_dest: str, preserve_source: bool, in_daemon: bool):
+def bag(bag_src: str, bag_dest: str, preserve_source: bool, in_daemon: bool, do_append: bool = False,
+        append_dest: str = None):
     """
     Creates a test_bag from the source
     :param bag_src: Path to work to test_bag. Can be a pre-existing test_bag
     :param bag_dest: directory to contain resulting zip archive of test_bag
     :param preserve_source: True if you want to preserve the source, false if you
     want to override it.
     :return:
     """
 
-    n_processes:int  = 1 if in_daemon else 6
+    n_processes: int = 1 if in_daemon else 6
     # name of destination, under bag_dest
     dest_base_name = Path(bag_src).name
 
     # Easiest way to always remove the tmp dir
     with tempfile.TemporaryDirectory() as bag_temp_dir:
         # Test if we're zipping an already existing test_bag
         try:
             dest_bag = bagit.Bag(bag_src)
         except bagit.BagError:
             # Existing source is not a bag. Make new one.
             if preserve_source:
                 # should result in bag_temp_dir/dest_base_name
                 save_dir: Path = Path(bag_temp_dir, dest_base_name)
-                bag_src: str = shutil.copytree(bag_src, save_dir )
-                logging.debug(f"Preserving source in {bag_src}")
+                bag_src: str = shutil.copytree(bag_src, save_dir)
+                logging.info(f"Preserving source in {bag_src}")
             dest_bag = bagit.make_bag(bag_src, processes=n_processes, checksums=['sha512'])
 
         bag_errors: [] = []
         # If the given folder is not a test_bag, make one from it
         if not validate_bag(dest_bag, bag_errors, n_processes):
             log_bag_errors(bag_errors)
             sys.exit(1)
 
         dest_bag.info['BDRC-RID'] = dest_base_name  # Assume it's the RID
         dest_bag.save(manifests=True, processes=n_processes)
 
         # Create a zip that contains top level folders named WXXXX.test_bag
-        archive_root: Path = Path(dest_base_name + BAG_SRC_SUFFIX)
 
-        output_archive_path: Path = Path(bag_dest, archive_root.name + ".zip")
-        logging.debug(f"Creating {output_archive_path}")
+        archive_root: Path = Path(dest_base_name + BAG_SRC_SUFFIX )
+        output_archive_path: Path = Path(bag_dest, archive_root.name + ".zip") if not do_append else Path(append_dest)
+        archive_mode = 'w' if not do_append else 'a'
+        logging.info(f"{'Creating' if not do_append else 'Appending'} {output_archive_path}")
         # if os.path.exists(output_archive_path):
         #     os.remove(output_archive_path)
 
         # We don't bother with compression - it takes
         # too long, and the image files don't compress a lot
         try:
-            with zipfile.ZipFile(output_archive_path, 'w') as zf:
-                zf.write(bag_src, arcname=archive_root )
+            with zipfile.ZipFile(output_archive_path,  archive_mode) as zf:
+                zf.write(bag_src, arcname=archive_root)
                 for root, dirs, files in os.walk(bag_src):
                     # Write the dirs first
                     for zip_dir in dirs:
                         dn: Path = Path(root, zip_dir)
                         adn: Path = Path(archive_root, dn.relative_to(bag_src))
                         zf.write(dn, arcname=adn)
                     for file in files:
```

## Comparing `bdrc_bag-0.0.3.dist-info/LICENSE` & `bdrc_bag-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bdrc_bag-0.0.3.dist-info/METADATA` & `bdrc_bag-0.0.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: bdrc-bag
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create and extract BDRC bags
+Author: jimk
 Author-email: Jim Katz <jim@tbrc.org>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bdrc-util
 Requires-Dist: bagit
 
 # Packaging BDRC Bag applications
 BDRC has been packaging its internal utilities as `pip` modules,
@@ -31,8 +32,9 @@
 - wget https://bootstrap.pypa.io/get-pip.py
 - sudo python3 get-pip.py
 - Script will let you know where 'pip' is now installed.  Make sure to add to your PATH.
 
 # Changelog
 | version | commit                                                                                               | description                             |
 |---------|------------------------------------------------------------------------------------------------------|-----------------------------------------|
+| 0.0.04  | [d9d656df](https://github.com/buda-base/archive-ops/commit/d9d656df90e5db0fd8cacff81e002b6a56609111) | Incrementally add a bag to its zip      | 
 | 0.0.03  | [ec875566](https://github.com/buda-base/archive-ops/commit/ec875566a0c389da6af4c5583ba8182f45a47c59) | Support single process to run in docker |
```

