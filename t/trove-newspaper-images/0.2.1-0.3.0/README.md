# Comparing `tmp/trove_newspaper_images-0.2.1.tar.gz` & `tmp/trove_newspaper_images-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove_newspaper_images-0.2.1.tar", last modified: Tue Sep 27 12:07:57 2022, max compression
+gzip compressed data, was "trove_newspaper_images-0.3.0.tar", last modified: Tue Apr 16 03:12:15 2024, max compression
```

## Comparing `trove_newspaper_images-0.2.1.tar` & `trove_newspaper_images-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-09-27 12:07:57.246923 trove_newspaper_images-0.2.1/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1069 2021-10-04 12:20:06.000000 trove_newspaper_images-0.2.1/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)      111 2021-10-03 06:43:48.000000 trove_newspaper_images-0.2.1/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     3223 2022-09-27 12:07:57.246923 trove_newspaper_images-0.2.1/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1987 2022-09-20 10:51:40.000000 trove_newspaper_images-0.2.1/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)     1108 2022-09-27 11:58:29.000000 trove_newspaper_images-0.2.1/settings.ini
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2022-09-27 12:07:57.246923 trove_newspaper_images-0.2.1/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     2541 2022-09-20 03:38:45.000000 trove_newspaper_images-0.2.1/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-09-27 12:07:57.242923 trove_newspaper_images-0.2.1/trove_newspaper_images/
--rw-rw-r--   0 tim       (1000) tim       (1000)       22 2022-09-27 12:03:18.000000 trove_newspaper_images-0.2.1/trove_newspaper_images/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1368 2022-09-27 12:03:18.000000 trove_newspaper_images-0.2.1/trove_newspaper_images/_modidx.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      449 2021-10-05 00:07:41.000000 trove_newspaper_images-0.2.1/trove_newspaper_images/_nbdev.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5797 2022-09-27 12:03:18.000000 trove_newspaper_images-0.2.1/trove_newspaper_images/articles.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-09-27 12:07:57.242923 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     3223 2022-09-27 12:07:57.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      511 2022-09-27 12:07:57.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-09-27 12:07:57.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      157 2022-09-27 12:07:57.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2021-10-04 08:19:29.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/not-zip-safe
--rw-rw-r--   0 tim       (1000) tim       (1000)       98 2022-09-27 12:07:57.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       23 2022-09-27 12:07:57.000000 trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-16 03:12:15.304102 trove_newspaper_images-0.3.0/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1069 2021-10-04 12:20:06.000000 trove_newspaper_images-0.3.0/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)      111 2021-10-03 06:43:48.000000 trove_newspaper_images-0.3.0/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2862 2024-04-16 03:12:15.304102 trove_newspaper_images-0.3.0/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2123 2024-04-16 03:11:02.000000 trove_newspaper_images-0.3.0/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1107 2024-04-16 03:10:26.000000 trove_newspaper_images-0.3.0/settings.ini
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-04-16 03:12:15.304102 trove_newspaper_images-0.3.0/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2541 2022-09-20 03:38:45.000000 trove_newspaper_images-0.3.0/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-16 03:12:15.304102 trove_newspaper_images-0.3.0/trove_newspaper_images/
+-rw-rw-r--   0 tim       (1000) tim       (1000)       22 2024-04-16 03:10:33.000000 trove_newspaper_images-0.3.0/trove_newspaper_images/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1369 2024-04-16 03:10:33.000000 trove_newspaper_images-0.3.0/trove_newspaper_images/_modidx.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      449 2021-10-05 00:07:41.000000 trove_newspaper_images-0.3.0/trove_newspaper_images/_nbdev.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6998 2024-04-16 03:10:33.000000 trove_newspaper_images-0.3.0/trove_newspaper_images/articles.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-16 03:12:15.304102 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2862 2024-04-16 03:12:15.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      511 2024-04-16 03:12:15.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-04-16 03:12:15.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      156 2024-04-16 03:12:15.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2021-10-04 08:19:29.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/not-zip-safe
+-rw-rw-r--   0 tim       (1000) tim       (1000)       98 2024-04-16 03:12:15.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       23 2024-04-16 03:12:15.000000 trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/top_level.txt
```

### Comparing `trove_newspaper_images-0.2.1/LICENSE` & `trove_newspaper_images-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trove_newspaper_images-0.2.1/PKG-INFO` & `trove_newspaper_images-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 Metadata-Version: 2.1
 Name: trove_newspaper_images
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tool to download Trove newspaper articles as images.
 Home-page: https://github.com/wragge/trove_newspaper_images
 Author: Tim Sherratt
 Author-email: tim@timsherratt.org
 License: MIT License
-Description: trove-newspaper-images
-        ================
-        
-        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-        
-        ## Background and alternatives
-        
-        There’s no reliable way of downloading an image of a Trove newspaper
-        article from the web interface. The image download option produces an
-        HTML page with embedded images, and the article is often sliced into
-        pieces to fit the page.
-        
-        This package includes tools to download articles as complete JPEG
-        images. If an article is printed across multiple newspaper pages,
-        multiple images will be downloaded – one for each page. It’s intended
-        for integration into other tools and processing workflows, or for people
-        who like working on the command line.
-        
-        If you just want to quickly download an article as an image without
-        installing anything, you can [use this web
-        app](https://glam-workbench.net/trove-newspapers/#save-a-trove-newspaper-article-as-an-image)
-        in the GLAM Workbench. To download images of all articles returned by a
-        search in Trove, you can also use the [Trove Newspaper and Gazette
-        Harvester](https://glam-workbench.net/trove-harvester/).
-        
-        See the
-        [documentation](https://wragge.github.io/trove_newspaper_images/) for
-        more information.
-        
-        ## Install
-        
-        `pip install trove-newspaper-images`
-        
-        ## Download articles as images
-        
-        ### Use as a library
-        
-        ``` python
-        from trove_newspaper_images.articles import download_images
-        
-        images = download_images('107024751')
-        images
-        ```
-        
-            ['nla.news-article107024751-11565831.jpg']
-        
-        ### Use from the command line
-        
-        Just call `trove_newspaper_images.download` from the command line with
-        an article identifier. You can use the `--output_dir` parameter to
-        specify a directory for the downloaded images. For example:
-        
-        ``` shell
-        trove_newspaper_images.download 107024751 --output_dir images
-        ```
-        
-        ------------------------------------------------------------------------
-        
-        Created by [Tim Sherratt](https://timsherratt.org)
-        ([@wragge](https://twitter.com/wragge)) for the [GLAM
-        Workbench](https://glam-workbench.net/).
-        
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# trove-newspaper-images
+
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+## Background and alternatives
+
+There’s no reliable way of downloading an image of a Trove newspaper
+article from the web interface. The image download option produces an
+HTML page with embedded images, and the article is often sliced into
+pieces to fit the page.
+
+This package includes tools to download articles as complete JPEG
+images. If an article is printed across multiple newspaper pages,
+multiple images will be downloaded – one for each page. It’s intended
+for integration into other tools and processing workflows, or for people
+who like working on the command line.
+
+If you just want to quickly download an article as an image without
+installing anything, you can [use this web
+app](https://glam-workbench.net/trove-newspapers/#save-a-trove-newspaper-article-as-an-image)
+in the GLAM Workbench. To download images of all articles returned by a
+search in Trove, you can also use the [Trove Newspaper and Gazette
+Harvester](https://glam-workbench.net/trove-harvester/).
+
+See the
+[documentation](https://wragge.github.io/trove_newspaper_images/) for
+more information.
+
+## Install
+
+`pip install trove-newspaper-images`
+
+## Download articles as images
+
+### Use as a library
+
+``` python
+from trove_newspaper_images.articles import download_images
+
+images = download_images('107024751')
+images
+```
+
+    ['nla.news-article107024751-11565831.jpg']
+
+### Use from the command line
+
+Just call `trove_newspaper_images.download` from the command line with
+an article identifier. You can use the `--output_dir` parameter to
+specify a directory for the downloaded images. For example:
+
+``` shell
+trove_newspaper_images.download 107024751 --output_dir images
+```
+
+Add the `--masked` parameter to try and remove content from neighbouring
+articles.
+
+``` shell
+trove_newspaper_images.download 107024751 --masked
+```
+
+------------------------------------------------------------------------
+
+Created by [Tim Sherratt](https://timsherratt.org)
+([@wragge](https://twitter.com/wragge)) for the [GLAM
+Workbench](https://glam-workbench.net/).
```

### Comparing `trove_newspaper_images-0.2.1/README.md` & `trove_newspaper_images-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-trove-newspaper-images
-================
+# trove-newspaper-images
+
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Background and alternatives
 
 There’s no reliable way of downloading an image of a Trove newspaper
 article from the web interface. The image download option produces an
@@ -50,12 +50,19 @@
 an article identifier. You can use the `--output_dir` parameter to
 specify a directory for the downloaded images. For example:
 
 ``` shell
 trove_newspaper_images.download 107024751 --output_dir images
 ```
 
+Add the `--masked` parameter to try and remove content from neighbouring
+articles.
+
+``` shell
+trove_newspaper_images.download 107024751 --masked
+```
+
 ------------------------------------------------------------------------
 
 Created by [Tim Sherratt](https://timsherratt.org)
 ([@wragge](https://twitter.com/wragge)) for the [GLAM
 Workbench](https://glam-workbench.net/).
```

### Comparing `trove_newspaper_images-0.2.1/settings.ini` & `trove_newspaper_images-0.3.0/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = trove_newspaper_images
 lib_name = %(repo)s
-version = 0.2.1
+version = 0.3.0
 min_python = 3.8
 license = mit
 
 ### nbdev ###
 doc_path = _docs
 lib_path = trove_newspaper_images
 nbs_path = .
 recursive = False
 tst_flags = notest
-put_version_in_init = False
+put_version_in_init = True
 
 ### Docs ###
 branch = master
 custom_sidebar = False
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
```

### Comparing `trove_newspaper_images-0.2.1/setup.py` & `trove_newspaper_images-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `trove_newspaper_images-0.2.1/trove_newspaper_images/_modidx.py` & `trove_newspaper_images-0.3.0/trove_newspaper_images/_modidx.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
   'syms': { 'trove_newspaper_images.articles': { 'trove_newspaper_images.articles.download_images': ( 'articles.html#download_images',
                                                                                                       'trove_newspaper_images/articles.py'),
                                                  'trove_newspaper_images.articles.get_article_boxes': ( 'articles.html#get_article_boxes',
                                                                                                         'trove_newspaper_images/articles.py'),
                                                  'trove_newspaper_images.articles.get_box': ( 'articles.html#get_box',
                                                                                               'trove_newspaper_images/articles.py'),
                                                  'trove_newspaper_images.articles.main': ( 'articles.html#main',
-                                                                                           'trove_newspaper_images/articles.py')}}}
+                                                                                           'trove_newspaper_images/articles.py')}}}
```

### Comparing `trove_newspaper_images-0.2.1/trove_newspaper_images/articles.py` & `trove_newspaper_images-0.3.0/trove_newspaper_images/articles.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,29 +25,38 @@
     # Set a top value larger than the image height
     top = 10000
     bottom = 0
     # Get the page identifier
     page_id = zones[0]["data-page-id"]
 
     # Loop through zones to find the outer boundaries of the article
+    z_boxes = []
     for zone in zones:
-        if int(zone["data-y"]) < top:
-            top = int(zone["data-y"])
-        if int(zone["data-x"]) < left:
-            left = int(zone["data-x"])
-        if (int(zone["data-x"]) + int(zone["data-w"])) > right:
-            right = int(zone["data-x"]) + int(zone["data-w"])
-        if (int(zone["data-y"]) + int(zone["data-h"])) > bottom:
-            bottom = int(zone["data-y"]) + int(zone["data-h"])
+        z_left = int(zone["data-x"])
+        z_top = int(zone["data-y"])
+        z_right = int(zone["data-x"]) + int(zone["data-w"])
+        z_bottom = int(zone["data-y"]) + int(zone["data-h"])
+        z_boxes.append(
+            {"left": z_left, "top": z_top, "right": z_right, "bottom": z_bottom}
+        )
+        if z_top < top:
+            top = z_top
+        if z_left < left:
+            left = z_left
+        if z_right > right:
+            right = z_right
+        if z_bottom > bottom:
+            bottom = z_bottom
     return {
         "page_id": page_id,
         "left": left,
         "top": top,
         "right": right,
         "bottom": bottom,
+        "zones": z_boxes,
     }
 
 
 def get_article_boxes(article_id):
     """
     Get a list of boundary boxes for an article, each box representing the position of an article on a page.
 
@@ -98,35 +107,36 @@
                 current_page = zone["data-page-id"]
 
         # Get the article boundary box for this page and add it to the list of boxes
         boxes.append(get_box(zones))
     return boxes
 
 
-def download_images(article_id, output_dir="", size=None):
+def download_images(article_id, output_dir="", size=None, masked=False):
     """
     Extract an image of a newspaper article from the page image(s), download and save it, and return the image filename(s).
 
     Parameters:
 
     * article_id -- identifier for a Trove newspaper article
     * output_dir -- a directory to save images in (will be created if it doesn't exist)
     * size -- maximum dimensions of image
+    * masked -- `True` or `False`, remove content that isn't part of the article
 
     Returns:
 
     * a list of image file names
     """
     images = []
     if output_dir:
         output_path = Path(output_dir)
         output_path.mkdir(exist_ok=True, parents=True)
     else:
         output_path = ""
-    
+
     # Get position of article on the page(s)
     boxes = get_article_boxes(article_id)
     for box in boxes:
         cropped_file = Path(
             output_path, f'nla.news-article{article_id}-{box["page_id"]}.jpg'
         )
         if not cropped_file.exists():
@@ -138,33 +148,59 @@
 
             # Open download as an image for editing
             img = Image.open(BytesIO(response.content))
 
             # Use coordinates of the bounding box to crop article
             points = (box["left"], box["top"], box["right"], box["bottom"])
 
-            # Crop image to article box
-            cropped = img.crop(points)
+            if masked:
+
+                # Create a new empty image the same size as the original
+                new_img = Image.new("RGB", img.size, "#fdfdfd")
+
+                # Process each zone separately
+                for zone in box["zones"]:
+                    
+                    # Get zone coords
+                    z_points = (
+                        zone["left"],
+                        zone["top"],
+                        zone["right"],
+                        zone["bottom"],
+                    )
+
+                    # Crop the zone from the original image
+                    zone_crop = img.crop(z_points)
+
+                    # Paste the zone into the new image
+                    new_img.paste(zone_crop, z_points)
+
+                # Crop the new image to the article box
+                cropped = new_img.crop(points)
+
+            else:
+
+                # Crop image to article box
+                cropped = img.crop(points)
 
             # Resize if necessary
             if size:
                 cropped.thumbnail((size, size), Image.LANCZOS)
 
             # Save cropped image
-            
-
             cropped.save(cropped_file)
         images.append(cropped_file.name)
     # print(f'Downloaded: {images}')
     return images
 
 
 def main():
     """
     CLI configuration
     """
     parser = argparse.ArgumentParser(prog="trove_newspaper_images.download")
     parser.add_argument("article_id", help="article identifier")
     parser.add_argument("--output_dir", help="directory to save images")
     parser.add_argument("--size", help="maximum image dimensions")
+    parser.add_argument('--masked', action="store_true", help="mask image")
     args = parser.parse_args()
-    download_images(args.article_id, args.output_dir, args.size)
+    download_images(args.article_id, args.output_dir, args.size, args.masked)
```

### Comparing `trove_newspaper_images-0.2.1/trove_newspaper_images.egg-info/PKG-INFO` & `trove_newspaper_images-0.3.0/trove_newspaper_images.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 Metadata-Version: 2.1
 Name: trove-newspaper-images
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tool to download Trove newspaper articles as images.
 Home-page: https://github.com/wragge/trove_newspaper_images
 Author: Tim Sherratt
 Author-email: tim@timsherratt.org
 License: MIT License
-Description: trove-newspaper-images
-        ================
-        
-        <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
-        
-        ## Background and alternatives
-        
-        There’s no reliable way of downloading an image of a Trove newspaper
-        article from the web interface. The image download option produces an
-        HTML page with embedded images, and the article is often sliced into
-        pieces to fit the page.
-        
-        This package includes tools to download articles as complete JPEG
-        images. If an article is printed across multiple newspaper pages,
-        multiple images will be downloaded – one for each page. It’s intended
-        for integration into other tools and processing workflows, or for people
-        who like working on the command line.
-        
-        If you just want to quickly download an article as an image without
-        installing anything, you can [use this web
-        app](https://glam-workbench.net/trove-newspapers/#save-a-trove-newspaper-article-as-an-image)
-        in the GLAM Workbench. To download images of all articles returned by a
-        search in Trove, you can also use the [Trove Newspaper and Gazette
-        Harvester](https://glam-workbench.net/trove-harvester/).
-        
-        See the
-        [documentation](https://wragge.github.io/trove_newspaper_images/) for
-        more information.
-        
-        ## Install
-        
-        `pip install trove-newspaper-images`
-        
-        ## Download articles as images
-        
-        ### Use as a library
-        
-        ``` python
-        from trove_newspaper_images.articles import download_images
-        
-        images = download_images('107024751')
-        images
-        ```
-        
-            ['nla.news-article107024751-11565831.jpg']
-        
-        ### Use from the command line
-        
-        Just call `trove_newspaper_images.download` from the command line with
-        an article identifier. You can use the `--output_dir` parameter to
-        specify a directory for the downloaded images. For example:
-        
-        ``` shell
-        trove_newspaper_images.download 107024751 --output_dir images
-        ```
-        
-        ------------------------------------------------------------------------
-        
-        Created by [Tim Sherratt](https://timsherratt.org)
-        ([@wragge](https://twitter.com/wragge)) for the [GLAM
-        Workbench](https://glam-workbench.net/).
-        
 Keywords: nbdev jupyter notebook python
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# trove-newspaper-images
+
+
+<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+## Background and alternatives
+
+There’s no reliable way of downloading an image of a Trove newspaper
+article from the web interface. The image download option produces an
+HTML page with embedded images, and the article is often sliced into
+pieces to fit the page.
+
+This package includes tools to download articles as complete JPEG
+images. If an article is printed across multiple newspaper pages,
+multiple images will be downloaded – one for each page. It’s intended
+for integration into other tools and processing workflows, or for people
+who like working on the command line.
+
+If you just want to quickly download an article as an image without
+installing anything, you can [use this web
+app](https://glam-workbench.net/trove-newspapers/#save-a-trove-newspaper-article-as-an-image)
+in the GLAM Workbench. To download images of all articles returned by a
+search in Trove, you can also use the [Trove Newspaper and Gazette
+Harvester](https://glam-workbench.net/trove-harvester/).
+
+See the
+[documentation](https://wragge.github.io/trove_newspaper_images/) for
+more information.
+
+## Install
+
+`pip install trove-newspaper-images`
+
+## Download articles as images
+
+### Use as a library
+
+``` python
+from trove_newspaper_images.articles import download_images
+
+images = download_images('107024751')
+images
+```
+
+    ['nla.news-article107024751-11565831.jpg']
+
+### Use from the command line
+
+Just call `trove_newspaper_images.download` from the command line with
+an article identifier. You can use the `--output_dir` parameter to
+specify a directory for the downloaded images. For example:
+
+``` shell
+trove_newspaper_images.download 107024751 --output_dir images
+```
+
+Add the `--masked` parameter to try and remove content from neighbouring
+articles.
+
+``` shell
+trove_newspaper_images.download 107024751 --masked
+```
+
+------------------------------------------------------------------------
+
+Created by [Tim Sherratt](https://timsherratt.org)
+([@wragge](https://twitter.com/wragge)) for the [GLAM
+Workbench](https://glam-workbench.net/).
```

