# Comparing `tmp/pagegen-3.9.1-py3-none-any.whl.zip` & `tmp/pagegen-3.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 56644 bytes, number of entries: 57
+Zip file size: 56665 bytes, number of entries: 57
 -rw-rw-r--  2.0 unx       17 b- defN 22-May-18 10:14 pagegen/__init__.py
 -rw-rw-r--  2.0 unx     2464 b- defN 24-Jan-09 12:03 pagegen/auto_build_serve.py
 -rw-rw-r--  2.0 unx      787 b- defN 24-Jan-09 12:03 pagegen/constants.py
 -rw-rw-r--  2.0 unx     3293 b- defN 22-May-18 10:14 pagegen/markdown_inline_graphviz.py
 -rw-rw-r--  2.0 unx     8004 b- defN 24-Jan-09 12:03 pagegen/page.py
 -rw-rw-r--  2.0 unx      651 b- defN 22-May-18 10:14 pagegen/pagegen-reload-on-regenerate.js
--rw-rw-r--  2.0 unx     7666 b- defN 24-Jan-09 12:25 pagegen/pagegen.py
+-rw-rw-r--  2.0 unx     7693 b- defN 24-Jan-09 12:44 pagegen/pagegen.py
 -rw-rw-r--  2.0 unx     5552 b- defN 24-Jan-09 12:03 pagegen/searchindex.py
 -rw-rw-r--  2.0 unx     3469 b- defN 24-Jan-09 12:03 pagegen/shortcodes.py
 -rw-rw-r--  2.0 unx     4904 b- defN 24-Jan-09 12:03 pagegen/shortcodes_built_in.py
 -rw-rw-r--  2.0 unx    34818 b- defN 24-Jan-09 12:03 pagegen/site.py
 -rw-rw-r--  2.0 unx     4234 b- defN 24-Jan-09 12:03 pagegen/utility.py
 -rw-rw-r--  2.0 unx     1743 b- defN 24-Jan-09 12:03 pagegen/utility_no_deps.py
 -rw-rw-r--  2.0 unx     5440 b- defN 24-Jan-09 12:03 pagegen/virtualpage.py
@@ -46,14 +46,14 @@
 -rw-rw-r--  2.0 unx      171 b- defN 22-May-18 10:14 pagegen/skel/themes/pgsite/templates/blog_home_page.mako
 -rw-rw-r--  2.0 unx      165 b- defN 22-May-18 10:14 pagegen/skel/themes/pgsite/templates/directories.mako
 -rw-rw-r--  2.0 unx      886 b- defN 22-May-18 10:14 pagegen/skel/themes/pgsite/templates/list_posts.mako
 -rw-rw-r--  2.0 unx      275 b- defN 22-May-18 10:14 pagegen/skel/themes/pgsite/templates/pages.mako
 -rw-rw-r--  2.0 unx     2032 b- defN 22-May-24 14:05 pagegen/skel/themes/pgsite/templates/search.mako
 -rw-rw-r--  2.0 unx      190 b- defN 22-May-24 08:14 pagegen/skel/themes/pgsite/templates/tag.mako
 -rw-rw-r--  2.0 unx      206 b- defN 22-May-24 08:14 pagegen/skel/themes/pgsite/templates/tags.mako
--rw-rw-r--  2.0 unx      665 b- defN 24-Jan-09 12:27 pagegen-3.9.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      984 b- defN 24-Jan-09 12:27 pagegen-3.9.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-09 12:27 pagegen-3.9.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 24-Jan-09 12:27 pagegen-3.9.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 24-Jan-09 12:27 pagegen-3.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5279 b- defN 24-Jan-09 12:27 pagegen-3.9.1.dist-info/RECORD
-57 files, 127911 bytes uncompressed, 48014 bytes compressed:  62.5%
+-rw-rw-r--  2.0 unx      665 b- defN 24-Jan-09 12:52 pagegen-3.9.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      984 b- defN 24-Jan-09 12:52 pagegen-3.9.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Jan-09 12:52 pagegen-3.9.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 24-Jan-09 12:52 pagegen-3.9.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 24-Jan-09 12:52 pagegen-3.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5279 b- defN 24-Jan-09 12:52 pagegen-3.9.2.dist-info/RECORD
+57 files, 127938 bytes uncompressed, 48035 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -147,26 +147,26 @@
 
 Filename: pagegen/skel/themes/pgsite/templates/tag.mako
 Comment: 
 
 Filename: pagegen/skel/themes/pgsite/templates/tags.mako
 Comment: 
 
-Filename: pagegen-3.9.1.dist-info/LICENSE.txt
+Filename: pagegen-3.9.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pagegen-3.9.1.dist-info/METADATA
+Filename: pagegen-3.9.2.dist-info/METADATA
 Comment: 
 
-Filename: pagegen-3.9.1.dist-info/WHEEL
+Filename: pagegen-3.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: pagegen-3.9.1.dist-info/entry_points.txt
+Filename: pagegen-3.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pagegen-3.9.1.dist-info/top_level.txt
+Filename: pagegen-3.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pagegen-3.9.1.dist-info/RECORD
+Filename: pagegen-3.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pagegen/pagegen.py

```diff
@@ -1,13 +1,12 @@
-from getopt import getopt, GetoptError
-from os import getcwd, listdir, chdir, X_OK, access, get_terminal_size, makedirs, getenv
-from pagegen.constants import SITECONF, HOME, CONFROOT, TARGETDIR, HOOKDIR, CONTENTDIR, ASSETDIR, THEMEDIR, SHORTCODECUSTOM, DIRDEFAULTFILE
-from sys import exit, argv
 from pagegen.utility_no_deps import report_error, report_notice, get_site_conf_path, exec_script
 from os.path import expanduser, basename, join, isfile, isdir, dirname, exists, abspath
+from sys import exit, argv
+from os import getcwd, listdir, chdir, X_OK, access, get_terminal_size, makedirs, getenv
+from pagegen.constants import SITECONF, HOME, CONFROOT, TARGETDIR, HOOKDIR, CONTENTDIR, ASSETDIR, THEMEDIR, SHORTCODECUSTOM, DIRDEFAULTFILE
 from subprocess import run, PIPE
 from glob import glob
 
 
 def usage(exit_after=True):
 	print('Usage: pagegen [-i|--init] [-g|--generate <environment>] [-s|--serve <environment>] [-v|--version] [-h|--help] <item>')
 
@@ -237,14 +236,17 @@
 		if len(argv) == 1:
 			file_mode(False, site_config)
 		elif not argv[1].startswith('-'):
 			file_mode(argv[1], site_config)
 
 	environment=None
 
+	# Lazy load what we can
+	from getopt import getopt, GetoptError
+
 	try:
 		opts, args=getopt(argv[1:],"ig:vs:h", ["init", "generate=", "version", "serve=", "help"])
 	except GetoptError as e:
 		usage(exit_after=False)
 		report_error(1, "Invalid arguments: %s" % e)
 
 	mode=False
```

## Comparing `pagegen-3.9.1.dist-info/LICENSE.txt` & `pagegen-3.9.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pagegen-3.9.1.dist-info/METADATA` & `pagegen-3.9.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pagegen
-Version: 3.9.1
+Version: 3.9.2
 Summary: Static site generator
 Home-page: http://pagegen.phnd.net
 Author: Oliver Fields
 Author-email: pagegen@phnd.net
 License: UNKNOWN
 Project-URL: Issues, https://github.com/oliverfields/pagegen/issues
 Project-URL: Repository, https://github.com/oliverfields/pagegen
```

## Comparing `pagegen-3.9.1.dist-info/RECORD` & `pagegen-3.9.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pagegen/__init__.py,sha256=N3wBLCd-MiURsLToOhDMAH5WRtDyP3XAA4cqHOKov5s,17
 pagegen/auto_build_serve.py,sha256=X4NZnqVXkh6DRQQt5eqxtp5S0xvEqDPTwx11c0chyiM,2464
 pagegen/constants.py,sha256=aGQ4UtMlaQLkRzMySXQ5xD-krh2s7peyCzi15pY7YUo,787
 pagegen/markdown_inline_graphviz.py,sha256=Ky5iTCBq7wpAlpxpdQAZ5vveS4CisRY6RjVzb7Q9pOs,3293
 pagegen/page.py,sha256=_H4lryMDzEzgRG-jgHHsM6Y82vE3m7Z6HRh3jZRfyk8,8004
 pagegen/pagegen-reload-on-regenerate.js,sha256=rb1qwH6W8Ji93YwdJJbGTrDLCCc1tLvjNW5Ad1nZTPU,651
-pagegen/pagegen.py,sha256=a75SfVymzhKw6O6SqjeZ3elxUTKEo2JynjP7w_DE7Rc,7666
+pagegen/pagegen.py,sha256=X36cutWJ3tC-bvTmYIgGs84vlpYTeJonmUoOFanObj4,7693
 pagegen/searchindex.py,sha256=EuZ-hrmRz9ama2p25JpxJDpVpkwegKWPUpQDYaTYnio,5552
 pagegen/shortcodes.py,sha256=2KZxglQR3QJyi1xK1Lt1DDFHyXiab-eyItH3bwE5IFc,3469
 pagegen/shortcodes_built_in.py,sha256=zdBphd4OYJucSVAUcuODVNpg_W7m1oxSCybx4U85dhU,4904
 pagegen/site.py,sha256=ZwFWLtxiKLcGYamGin9hA6lvRCTWS-mEyljNJ9pMUK4,34818
 pagegen/utility.py,sha256=DK8F7NO_ULKBLUksHt-2cWm6H3p7BtqtvomkqRbiNmg,4234
 pagegen/utility_no_deps.py,sha256=ymlOk9YlTEGjabXiZGqvKFxwyotj7LS66pdCa-VADLo,1743
 pagegen/virtualpage.py,sha256=dEGz86NbXvHVGIv7wEGKrFPO6bTgx9CJ6sPnl_Rp8OA,5440
@@ -45,13 +45,13 @@
 pagegen/skel/themes/pgsite/templates/blog_home_page.mako,sha256=LyflmN77wCjULnlARLV0XH904buTlW-Rd0g_zc_1K5U,171
 pagegen/skel/themes/pgsite/templates/directories.mako,sha256=XzHvmNHJ5XKGdbhdXvBguD7COZ9DRs7guqHZOgyWpHA,165
 pagegen/skel/themes/pgsite/templates/list_posts.mako,sha256=nIx4FOOde7S0E-ASPqtiBERtxJtSH6fjG0PxsxWGY4U,886
 pagegen/skel/themes/pgsite/templates/pages.mako,sha256=uSVUQAsYv1AwezdKYT8Kn_xVAdPieJRjsN47rpMegoE,275
 pagegen/skel/themes/pgsite/templates/search.mako,sha256=W2f5usWRAhLf7DHB2Ns8r2ZtLcfo3LQ-vDBRq9zhpY4,2032
 pagegen/skel/themes/pgsite/templates/tag.mako,sha256=ElAPZFJEwx0v4haSE9ZyjTaw7NWbtgdzeKJTfwrNHyg,190
 pagegen/skel/themes/pgsite/templates/tags.mako,sha256=zLp9iJ_IPMPUlbY-PnQ_c4956O5z3IrhZNlR1CZqiuo,206
-pagegen-3.9.1.dist-info/LICENSE.txt,sha256=U4C2f0otQc1yN3yAR7pm7KNl7KYXcj_PJ0GDINMaoDk,665
-pagegen-3.9.1.dist-info/METADATA,sha256=u1RSwD5DF0Xdx5h9pNf_NdEOrMzdkkhTDJBHa5bL1FE,984
-pagegen-3.9.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pagegen-3.9.1.dist-info/entry_points.txt,sha256=oV6mATw-hYD4ZVNsjydKqPifIUlqQl5jEU4N44kFSJg,50
-pagegen-3.9.1.dist-info/top_level.txt,sha256=e7onoAoSuW9MCU7UhkOfbK3_qf5Bor4hNzS7rwFKaOo,8
-pagegen-3.9.1.dist-info/RECORD,,
+pagegen-3.9.2.dist-info/LICENSE.txt,sha256=U4C2f0otQc1yN3yAR7pm7KNl7KYXcj_PJ0GDINMaoDk,665
+pagegen-3.9.2.dist-info/METADATA,sha256=aiIr8LQpTgfm83JvoDctvYg_-Tsc48Rg6lPi8ugAdGU,984
+pagegen-3.9.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pagegen-3.9.2.dist-info/entry_points.txt,sha256=oV6mATw-hYD4ZVNsjydKqPifIUlqQl5jEU4N44kFSJg,50
+pagegen-3.9.2.dist-info/top_level.txt,sha256=e7onoAoSuW9MCU7UhkOfbK3_qf5Bor4hNzS7rwFKaOo,8
+pagegen-3.9.2.dist-info/RECORD,,
```

