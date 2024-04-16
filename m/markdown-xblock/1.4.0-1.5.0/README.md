# Comparing `tmp/markdown-xblock-1.4.0.tar.gz` & `tmp/markdown-xblock-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown-xblock-1.4.0.tar", last modified: Thu Dec 21 12:43:39 2023, max compression
+gzip compressed data, was "markdown-xblock-1.5.0.tar", last modified: Tue Apr 16 05:56:42 2024, max compression
```

## Comparing `markdown-xblock-1.4.0.tar` & `markdown-xblock-1.5.0.tar`

### file list

```diff
@@ -1,144 +1,145 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      256 2023-12-21 12:39:48.000000 markdown-xblock-1.4.0/.bumpversion.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.569043 markdown-xblock-1.4.0/.githooks/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       29 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/.githooks/pre-commit
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       19 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/.githooks/pre-push
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.557046 markdown-xblock-1.4.0/.github/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.569043 markdown-xblock-1.4.0/.github/workflows/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/.github/workflows/tox.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      630 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/.gitlab-ci.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2277 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/HACKING.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35136 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6372 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4691 2023-12-21 12:39:48.000000 markdown-xblock-1.4.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/manage.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.573042 markdown-xblock-1.4.0/markdown_xblock/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12046 2023-12-20 11:41:56.000000 markdown-xblock-1.4.0/markdown_xblock/html.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.561045 markdown-xblock-1.4.0/markdown_xblock/public/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.561045 markdown-xblock-1.4.0/markdown_xblock/public/plugins/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.577042 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1106 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/LICENSE
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.561045 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.561045 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.577042 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      502 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/dialog.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4872 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/dialog.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.577042 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      116 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/fullscreen.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1494 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/fullscreen.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/edit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5268 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/edit/matchbrackets.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6740 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/search.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7720 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/searchcursor.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/selection/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2442 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/selection/active-line.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8166 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   332949 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.561045 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/css/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31664 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/css/css.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/htmlmixed/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5008 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/htmlmixed/htmlmixed.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.581041 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/javascript/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26092 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/javascript/javascript.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/markdown/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32795 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/markdown/markdown.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/xml/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12375 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/xml/xml.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/langs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      216 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/langs/en.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1081 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/plugin.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8161 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/source.html
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/css/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2400 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/css/prism.css
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/js/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23415 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/js/prism.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19335 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/plugin.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/image/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16029 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/image/plugin.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/link/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8919 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/link/plugin.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/lists/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14256 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/lists/plugin.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.585040 markdown-xblock-1.4.0/markdown_xblock/public/plugins/textcolor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4924 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/plugins/textcolor/plugin.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.589039 markdown-xblock-1.4.0/markdown_xblock/public/skin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      971 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/content.inline.min.css
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1857 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/content.min.css
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.589039 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8344 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.eot
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    25886 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.svg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8160 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.ttf
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8336 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.woff
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8268 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.eot
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    26077 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.svg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8104 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.ttf
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8400 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.woff
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       67 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/readme.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.589039 markdown-xblock-1.4.0/markdown_xblock/public/skin/img/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       53 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/img/anchor.gif
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     2569 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/img/loader.gif
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      152 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/img/object.gif
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/img/trans.gif
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       46 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/img/wline.gif
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    27691 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/skin.ie7.min.css
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1567 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/skin.json
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    27802 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/public/skin/skin.min.css
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.565044 markdown-xblock-1.4.0/markdown_xblock/static/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.589039 markdown-xblock-1.4.0/markdown_xblock/static/css/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      284 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/css/html.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5053 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/css/pygments.css
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.593038 markdown-xblock-1.4.0/markdown_xblock/static/html/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      120 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/html/lms.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/html/studio.html
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.593038 markdown-xblock-1.4.0/markdown_xblock/static/js/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8529 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/js/html.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.597037 markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.565044 markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/themes/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.597037 markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/themes/modern/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   131421 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/themes/modern/theme.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   911420 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/tinymce.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   351170 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/tinymce.min.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.597037 markdown-xblock-1.4.0/markdown_xblock/translations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      295 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/translations/README.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      161 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/markdown_xblock/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.577042 markdown-xblock-1.4.0/markdown_xblock.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6372 2023-12-21 12:43:39.000000 markdown-xblock-1.4.0/markdown_xblock.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4422 2023-12-21 12:43:39.000000 markdown-xblock-1.4.0/markdown_xblock.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-21 12:43:39.000000 markdown-xblock-1.4.0/markdown_xblock.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-12-21 12:43:39.000000 markdown-xblock-1.4.0/markdown_xblock.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-12-21 12:43:39.000000 markdown-xblock-1.4.0/markdown_xblock.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2023-12-21 12:43:39.000000 markdown-xblock-1.4.0/markdown_xblock.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.565044 markdown-xblock-1.4.0/releasenotes/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/releasenotes/notes/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/add-default-css-for-tables-3a53e02e8a350253.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/add_public_view-d24763b7941dc2b0.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      149 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/custom-css-classes-7984a9c95147d39c.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/export-md-to-file-ab1528b4c28cb2f0.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      169 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/fix-course-export-b35c78a22be0c6b5.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      197 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/missing-codemirror-files-d64ccb15d0faf640.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      190 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/pypi-release-3e4d5ceb7b6e252a.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      193 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/refactor-ci-36abda8c15250d06.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      240 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/refactor-export-import-49bbf0e8a364f139.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      291 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/remove_py35-0b265861449b1753.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      304 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/safe_mode_replace_escape-40fdb78ec8aa5eff.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/releasenotes/notes/show_in_read_only_mode-3af39459d5d56b33.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2023-12-21 12:11:54.000000 markdown-xblock-1.4.0/requirements/base.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       36 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/requirements/dev.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/requirements/reno.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      204 2023-12-21 12:11:54.000000 markdown-xblock-1.4.0/requirements/test.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       25 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1533 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11687 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/tests/test_basics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/tox.ini
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-21 12:43:39.601036 markdown-xblock-1.4.0/var/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2023-12-19 15:26:09.000000 markdown-xblock-1.4.0/var/.placeholder
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:42.016537 markdown-xblock-1.5.0/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      256 2024-04-16 05:55:10.000000 markdown-xblock-1.5.0/.bumpversion.cfg
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.936797 markdown-xblock-1.5.0/.githooks/
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       29 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/.githooks/pre-commit
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       19 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/.githooks/pre-push
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.922975 markdown-xblock-1.5.0/.github/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.937308 markdown-xblock-1.5.0/.github/workflows/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1777 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/.github/workflows/tox.yml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      630 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/.gitignore
+-rw-r--r--   0 maaritamm   (501) staff       (20)      474 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/.gitlab-ci.yml
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2277 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/HACKING.md
+-rw-r--r--   0 maaritamm   (501) staff       (20)    35136 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/LICENSE
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5271 2024-04-16 05:56:42.015977 markdown-xblock-1.5.0/PKG-INFO
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4691 2024-04-16 05:55:10.000000 markdown-xblock-1.5.0/README.md
+-rw-r--r--   0 maaritamm   (501) staff       (20)      293 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/manage.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.939004 markdown-xblock-1.5.0/markdown_xblock/
+-rw-r--r--   0 maaritamm   (501) staff       (20)       77 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/__init__.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    12060 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/markdown_xblock/html.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.927643 markdown-xblock-1.5.0/markdown_xblock/public/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.927468 markdown-xblock-1.5.0/markdown_xblock/public/plugins/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.943087 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1106 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/LICENSE
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.925296 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.924840 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.944491 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      502 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/dialog.css
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4872 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/dialog.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.945756 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      116 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/fullscreen.css
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1494 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/fullscreen.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.946465 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/edit/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5268 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/edit/matchbrackets.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.947953 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     6740 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/search.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)     7720 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/searchcursor.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.948778 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/selection/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2442 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/selection/active-line.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.950157 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     8166 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.css
+-rw-r--r--   0 maaritamm   (501) staff       (20)   332949 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.926122 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.952966 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/css/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    31664 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/css/css.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.954139 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/htmlmixed/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5008 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/htmlmixed/htmlmixed.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.954867 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/javascript/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    26092 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/javascript/javascript.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.955945 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/markdown/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    32795 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/markdown/markdown.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.956937 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/xml/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    12375 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/xml/xml.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.957659 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/langs/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      216 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/langs/en.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1081 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/plugin.min.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)     8161 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/source.html
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.958386 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.959601 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/css/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     2400 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/css/prism.css
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.960404 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/js/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    23415 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/js/prism.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)    19335 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/plugin.min.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.961431 markdown-xblock-1.5.0/markdown_xblock/public/plugins/image/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    16029 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/image/plugin.min.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.962152 markdown-xblock-1.5.0/markdown_xblock/public/plugins/link/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     8919 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/link/plugin.min.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.962892 markdown-xblock-1.5.0/markdown_xblock/public/plugins/lists/
+-rw-r--r--   0 maaritamm   (501) staff       (20)    14256 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/lists/plugin.min.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.963689 markdown-xblock-1.5.0/markdown_xblock/public/plugins/textcolor/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4924 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/plugins/textcolor/plugin.min.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.968586 markdown-xblock-1.5.0/markdown_xblock/public/skin/
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)      971 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/content.inline.min.css
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     1857 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/content.min.css
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.976834 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     8344 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.eot
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)    25886 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.svg
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     8160 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.ttf
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     8336 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.woff
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     8268 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.eot
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)    26077 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.svg
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     8104 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.ttf
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     8400 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.woff
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       67 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/readme.md
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.981027 markdown-xblock-1.5.0/markdown_xblock/public/skin/img/
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       53 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/img/anchor.gif
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     2569 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/img/loader.gif
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)      152 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/img/object.gif
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       43 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/img/trans.gif
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)       46 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/img/wline.gif
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)    27691 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/skin.ie7.min.css
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)     1567 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/skin.json
+-rwxr-xr-x   0 maaritamm   (501) staff       (20)    27802 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/public/skin/skin.min.css
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.928757 markdown-xblock-1.5.0/markdown_xblock/static/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.982417 markdown-xblock-1.5.0/markdown_xblock/static/css/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      284 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/css/html.css
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5053 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/css/pygments.css
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.983915 markdown-xblock-1.5.0/markdown_xblock/static/html/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      120 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/html/lms.html
+-rw-r--r--   0 maaritamm   (501) staff       (20)      999 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/html/studio.html
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.984647 markdown-xblock-1.5.0/markdown_xblock/static/js/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     8529 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/js/html.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.991033 markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.929320 markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/themes/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.994691 markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/themes/modern/
+-rw-r--r--   0 maaritamm   (501) staff       (20)   131421 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/themes/modern/theme.min.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)   911420 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/tinymce.js
+-rw-r--r--   0 maaritamm   (501) staff       (20)   351170 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/tinymce.min.js
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.997865 markdown-xblock-1.5.0/markdown_xblock/translations/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      295 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/translations/README.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)      161 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/markdown_xblock/utils.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.941371 markdown-xblock-1.5.0/markdown_xblock.egg-info/
+-rw-r--r--   0 maaritamm   (501) staff       (20)     5271 2024-04-16 05:56:41.000000 markdown-xblock-1.5.0/markdown_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 maaritamm   (501) staff       (20)     4483 2024-04-16 05:56:41.000000 markdown-xblock-1.5.0/markdown_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)        1 2024-04-16 05:56:41.000000 markdown-xblock-1.5.0/markdown_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       54 2024-04-16 05:56:41.000000 markdown-xblock-1.5.0/markdown_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       45 2024-04-16 05:56:41.000000 markdown-xblock-1.5.0/markdown_xblock.egg-info/requires.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       16 2024-04-16 05:56:41.000000 markdown-xblock-1.5.0/markdown_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:41.929793 markdown-xblock-1.5.0/releasenotes/
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:42.009503 markdown-xblock-1.5.0/releasenotes/notes/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      131 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/add-default-css-for-tables-3a53e02e8a350253.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       76 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/add_public_view-d24763b7941dc2b0.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      149 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/custom-css-classes-7984a9c95147d39c.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      147 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/export-md-to-file-ab1528b4c28cb2f0.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      169 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/fix-course-export-b35c78a22be0c6b5.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      197 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/missing-codemirror-files-d64ccb15d0faf640.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      190 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/pypi-release-3e4d5ceb7b6e252a.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)       52 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/releasenotes/notes/python-3.12-support-dac839f8d01ac6b9.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      193 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/refactor-ci-36abda8c15250d06.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      240 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/refactor-export-import-49bbf0e8a364f139.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      291 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/remove_py35-0b265861449b1753.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      304 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/safe_mode_replace_escape-40fdb78ec8aa5eff.yaml
+-rw-r--r--   0 maaritamm   (501) staff       (20)      293 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/releasenotes/notes/show_in_read_only_mode-3af39459d5d56b33.yaml
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:42.012700 markdown-xblock-1.5.0/requirements/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      144 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/requirements/base.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       36 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/requirements/dev.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)        5 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/requirements/reno.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)      210 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/requirements/test.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       25 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/requirements.txt
+-rw-r--r--   0 maaritamm   (501) staff       (20)       38 2024-04-16 05:56:42.016751 markdown-xblock-1.5.0/setup.cfg
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1538 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/setup.py
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:42.014202 markdown-xblock-1.5.0/tests/
+-rw-r--r--   0 maaritamm   (501) staff       (20)       20 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/tests/__init__.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)    12276 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/tests/test_basics.py
+-rw-r--r--   0 maaritamm   (501) staff       (20)     1048 2024-04-15 11:25:28.000000 markdown-xblock-1.5.0/tox.ini
+drwxr-xr-x   0 maaritamm   (501) staff       (20)        0 2024-04-16 05:56:42.014939 markdown-xblock-1.5.0/var/
+-rw-r--r--   0 maaritamm   (501) staff       (20)      108 2024-04-09 11:26:17.000000 markdown-xblock-1.5.0/var/.placeholder
```

### Comparing `markdown-xblock-1.4.0/.github/workflows/tox.yml` & `markdown-xblock-1.5.0/.github/workflows/tox.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,36 @@
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
-          - 3.8
+          - '3.8'
+          - '3.10'
+        pip-version:
+          - 22.0.4
+          - 23.2.1
+        include:
+          - python-version: '3.12'
+            pip-version: '23.2.1'
 
     steps:
     - name: Check out code
       uses: actions/checkout@v1
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
-        pip install "tox<4" tox-gh-actions tox-pip-version 'setuptools_scm<6'
-    - name: Test with tox
+        pip install "tox<4" tox-gh-actions tox-pip-version 'setuptools_scm'
+    - name: Test with tox (pip ${{ matrix.pip-version }})
       env:
-        TOX_PIP_VERSION: '20.2.4'
+        TOX_PIP_VERSION: ${{ matrix.pip-version }}
       run: tox
     - name: Upload coverage data
       uses: actions/upload-artifact@v2
       with:
         name: coverage-${{ matrix.python-version }}
         path: .coverage*
         retention-days: 1
```

### Comparing `markdown-xblock-1.4.0/.gitignore` & `markdown-xblock-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/HACKING.md` & `markdown-xblock-1.5.0/HACKING.md`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/LICENSE` & `markdown-xblock-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/README.md` & `markdown-xblock-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 This XBlock allows course authors to create and edit course content in Markdown
 and displays it as HTML.
 
 ## Installation with [Tutor](https://docs.tutor.edly.io)
 You may install the markdown-xblock to your Tutor environment by adding it to the `OPENEDX_EXTRA_PIP_REQUIREMENTS` list in `config.yml`:
 ```
 OPENEDX_EXTRA_PIP_REQUIREMENTS:
-- markdown-xblock==1.4.0
+- markdown-xblock==1.5.0
 ```
 
 Or, if you prefer to install directly from Git:
 ```
 OPENEDX_EXTRA_PIP_REQUIREMENTS:
-- git+https://github.com/citynetwork/markdown-xblock.git@v1.4.0
+- git+https://github.com/citynetwork/markdown-xblock.git@v1.5.0
 ```
 For additional information, please refer to the official [documentation](https://docs.tutor.edly.io/configuration.html#open-edx-customisation).
 
 The minimum supported Python version is 3.8.
 
 To enable this block, add `"markdown"` to the course's advanced module list. 
 The option `Markdown` will appear in the advanced components.
```

### Comparing `markdown-xblock-1.4.0/markdown_xblock/html.py` & `markdown-xblock-1.5.0/markdown_xblock/html.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """This XBlock help creating a secure and easy-to-use HTML blocks in edx-platform."""
 
 import logging
 import os
 
 import markdown2
 from path import Path as path
-import pkg_resources
 from django.conf import settings as django_settings
 from xblock.core import XBlock
 from xblock.fields import List, Scope, String
 from xblock.fragment import Fragment
 from xblockutils.resources import ResourceLoader
 from xblockutils.settings import XBlockWithSettingsMixin
 from xblockutils.studio_editable import StudioEditableXBlockMixin, loader
@@ -68,33 +67,27 @@
         default=u'',
         scope=Scope.content
     )
     editor = 'markdown'
     editable_fields = ('display_name', 'classes')
     show_in_read_only_mode = True
 
-    @staticmethod
-    def resource_string(path):
-        """Handy helper for getting resources from our kit."""
-        data = pkg_resources.resource_string(__name__, path)
-        return data.decode('utf8')
-
     @XBlock.supports('multi_device')
     def student_view(self, context=None):  # pylint: disable=unused-argument
         """
         Return a fragment that contains the html for the student view.
         """
         frag = Fragment()
         frag.content = xblock_loader.render_django_template('static/html/lms.html', {'self': self})
 
-        frag.add_css(self.resource_string('public/plugins/codesample/css/prism.css'))
-        frag.add_javascript(self.resource_string('public/plugins/codesample/js/prism.js'))
+        frag.add_css_url(self.runtime.local_resource_url(self, 'public/plugins/codesample/css/prism.css'))
+        frag.add_javascript_url(self.runtime.local_resource_url(self, 'public/plugins/codesample/js/prism.js'))
 
-        frag.add_css(self.resource_string('static/css/pygments.css'))
-        frag.add_css(self.resource_string('static/css/html.css'))
+        frag.add_css_url(self.runtime.local_resource_url(self, 'static/css/pygments.css'))
+        frag.add_css_url(self.runtime.local_resource_url(self, 'static/css/html.css'))
 
         return frag
 
     def studio_view(self, context=None):  # pylint: disable=unused-argument
         """
         Return a fragment that contains the html for the Studio view.
         """
@@ -163,32 +156,33 @@
         ]
 
     def add_stylesheets(self, frag):
         """
         A helper method to add all necessary styles to the fragment.
         :param frag: The fragment that will hold the scripts.
         """
-        frag.add_css(self.resource_string('static/css/html.css'))
+        frag.add_css_url(self.runtime.local_resource_url(self, 'static/css/html.css'))
 
-        frag.add_css(self.resource_string('public/plugins/codemirror/codemirror-4.8/lib/codemirror.css'))
+        frag.add_css_url(self.runtime.local_resource_url(
+            self, 'public/plugins/codemirror/codemirror-4.8/lib/codemirror.css'))
 
     def add_scripts(self, frag):
         """
         A helper method to add all necessary scripts to the fragment.
         :param frag: The fragment that will hold the scripts.
         """
-        frag.add_javascript(self.resource_string('static/js/tinymce/tinymce.min.js'))
-        frag.add_javascript(self.resource_string('static/js/tinymce/themes/modern/theme.min.js'))
-        frag.add_javascript(self.resource_string('static/js/html.js'))
+        frag.add_javascript_url(self.runtime.local_resource_url(self, 'static/js/tinymce/tinymce.min.js'))
+        frag.add_javascript_url(self.runtime.local_resource_url(self, 'static/js/tinymce/themes/modern/theme.min.js'))
+        frag.add_javascript_url(self.runtime.local_resource_url(self, 'static/js/html.js'))
         frag.add_javascript(loader.load_unicode('public/studio_edit.js'))
 
         code_mirror_dir = 'public/plugins/codemirror/codemirror-4.8/'
 
-        frag.add_javascript(self.resource_string(code_mirror_dir + 'lib/codemirror.js'))
-        frag.add_javascript(self.resource_string(code_mirror_dir + 'mode/markdown/markdown.js'))
+        frag.add_javascript_url(self.runtime.local_resource_url(self, code_mirror_dir + 'lib/codemirror.js'))
+        frag.add_javascript_url(self.runtime.local_resource_url(self, code_mirror_dir + 'mode/markdown/markdown.js'))
 
     def get_editor_plugins(self):
         """
         This method will generate a list of external plugins urls to be used in TinyMCE editor.
         These plugins should live in `public` directory for us to generate URLs for.
 
         const PLUGINS_DIR = "/resource/html5/public/plugins/";
```

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/LICENSE` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/dialog.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/dialog/dialog.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/fullscreen.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/display/fullscreen.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/edit/matchbrackets.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/edit/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/search.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/search.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/searchcursor.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/search/searchcursor.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/selection/active-line.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/addon/selection/active-line.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.css` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/lib/codemirror.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/css/css.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/htmlmixed/htmlmixed.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/javascript/javascript.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/markdown/markdown.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/xml/xml.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/codemirror-4.8/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/plugin.min.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/plugin.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codemirror/source.html` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codemirror/source.html`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/css/prism.css` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/css/prism.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/js/prism.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/js/prism.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/codesample/plugin.min.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/codesample/plugin.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/image/plugin.min.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/image/plugin.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/link/plugin.min.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/link/plugin.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/lists/plugin.min.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/lists/plugin.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/plugins/textcolor/plugin.min.js` & `markdown-xblock-1.5.0/markdown_xblock/public/plugins/textcolor/plugin.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/content.inline.min.css` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/content.inline.min.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/content.min.css` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/content.min.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.eot` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.eot`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.svg` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.svg`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.ttf` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.ttf`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon-small.woff` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon-small.woff`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.eot` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.eot`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.svg` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.svg`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.ttf` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/fonts/icomoon.woff` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/fonts/icomoon.woff`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/img/loader.gif` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/img/loader.gif`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/skin.ie7.min.css` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/skin.ie7.min.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/skin.json` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/skin.json`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/public/skin/skin.min.css` & `markdown-xblock-1.5.0/markdown_xblock/public/skin/skin.min.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/static/css/pygments.css` & `markdown-xblock-1.5.0/markdown_xblock/static/css/pygments.css`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/static/html/studio.html` & `markdown-xblock-1.5.0/markdown_xblock/static/html/studio.html`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/static/js/html.js` & `markdown-xblock-1.5.0/markdown_xblock/static/js/html.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/themes/modern/theme.min.js` & `markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/themes/modern/theme.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/tinymce.js` & `markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/tinymce.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock/static/js/tinymce/tinymce.min.js` & `markdown-xblock-1.5.0/markdown_xblock/static/js/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `markdown-xblock-1.4.0/markdown_xblock.egg-info/SOURCES.txt` & `markdown-xblock-1.5.0/markdown_xblock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 releasenotes/notes/add-default-css-for-tables-3a53e02e8a350253.yaml
 releasenotes/notes/add_public_view-d24763b7941dc2b0.yaml
 releasenotes/notes/custom-css-classes-7984a9c95147d39c.yaml
 releasenotes/notes/export-md-to-file-ab1528b4c28cb2f0.yaml
 releasenotes/notes/fix-course-export-b35c78a22be0c6b5.yaml
 releasenotes/notes/missing-codemirror-files-d64ccb15d0faf640.yaml
 releasenotes/notes/pypi-release-3e4d5ceb7b6e252a.yaml
+releasenotes/notes/python-3.12-support-dac839f8d01ac6b9.yaml
 releasenotes/notes/refactor-ci-36abda8c15250d06.yaml
 releasenotes/notes/refactor-export-import-49bbf0e8a364f139.yaml
 releasenotes/notes/remove_py35-0b265861449b1753.yaml
 releasenotes/notes/safe_mode_replace_escape-40fdb78ec8aa5eff.yaml
 releasenotes/notes/show_in_read_only_mode-3af39459d5d56b33.yaml
 requirements/base.txt
 requirements/dev.txt
```

### Comparing `markdown-xblock-1.4.0/setup.py` & `markdown-xblock-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         'Topic :: Education :: Computer Aided Instruction (CAI)',
         'Topic :: Education',
     ],
     packages=[
         'markdown_xblock',
     ],
     install_requires=[
-        'XBlock',
+        'XBlock<=1.9',
         'markdown2>=2.3.9',
         'Pygments>=2.0.1'
     ],
     setup_requires=[
         'setuptools-scm',
     ],
     entry_points={
```

### Comparing `markdown-xblock-1.4.0/tests/test_basics.py` & `markdown-xblock-1.5.0/tests/test_basics.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,45 +2,51 @@
 Markdown XBlock tests
 """
 from __future__ import print_function
 
 import unittest
 
 from mock import Mock, patch
+from workbench.runtime import WorkbenchRuntime
 from xblock.field_data import DictFieldData
-from xblock.test.tools import TestRuntime
+from xblock.fields import ScopeIds
 
 from markdown2 import MarkdownError
 
 import markdown_xblock
 from markdown_xblock.html import DEFAULT_EXTRAS
 
 
 class TestMarkdownXBlock(unittest.TestCase):
     """
     Unit tests for `markdown_xblock`
     """
     def setUp(self):
-        self.runtime = TestRuntime()
+        block_type = 'markdown'
+        self.runtime = WorkbenchRuntime()
+        def_id = self.runtime.id_generator.create_definition(block_type)
+        usage_id = self.runtime.id_generator.create_usage(def_id)
+
+        self.scope_ids = ScopeIds('user', block_type, def_id, usage_id)
 
     def test_render(self):
         """
         Test a basic rendering with default settings.
         """
         field_data = DictFieldData({'data': '# This is h1'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         fragment = block.student_view()
         self.assertIn('<div class="markdown_xblock"><h1>This is h1</h1>\n</div>\n', fragment.content)
 
     def test_public_view(self):
         """
         Test public view rendering.
         """
         field_data = DictFieldData({'data': '# This is h1'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         student_view_fragment = block.student_view()
         self.assertIn('<div class="markdown_xblock"><h1>This is h1</h1>\n</div>\n',
                       student_view_fragment.content)
         public_view_fragment = block.public_view()
         self.assertIn('<div class="markdown_xblock"><h1>This is h1</h1>\n</div>\n',
                       public_view_fragment.content)
 
@@ -50,30 +56,30 @@
 
         Expects the content to be sanitized by injecting
         [HTML_REMOVED] in place of the HTML tags, and the sentence
         being wrapped in a <p> block (since the <h1> tags are no
         longer interpreted as HTML).
         """
         field_data = DictFieldData({'data': '<h1>This is h1</h1>'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         fragment = block.student_view()
         self.assertIn(
             '<div class="markdown_xblock"><p>[HTML_REMOVED]This is h1[HTML_REMOVED]</p>\n</div>\n',
             fragment.content
         )
 
     def test_render_invalid_safe_mode(self):
         """
         Test a basic rendering with default settings.
 
         Expects the rendering to fail since safe_mode is not set to
         one of 'replace', 'escape', True or False.
         """
         field_data = DictFieldData({'data': '<h1>This is h1</h1>'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": 'this is an invalid safe mode'
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             with self.assertRaises(MarkdownError):
@@ -85,15 +91,15 @@
 
         Expects the content to be sanitized by injecting
         [HTML_REMOVED] in place of the HTML tags, and the sentence
         being wrapped in a <p> block (since the <h1> tags are no
         longer interpreted as HTML).
         """
         field_data = DictFieldData({'data': '<h1>This is h1</h1>'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": 'replace'
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -108,15 +114,15 @@
 
         Expects the content to be sanitized by injecting
         [HTML_REMOVED] in place of the HTML tags, and the sentence
         being wrapped in a <p> block (since the <h1> tags are no
         longer interpreted as HTML).
         """
         field_data = DictFieldData({'data': '<h1>This is h1</h1>'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": True
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -130,15 +136,15 @@
         Test a basic rendering with safe_mode set to 'escape'
 
         Expects the content to be sanitized by escaping < and > with &lt; and &gt;
         and the sentence being wrapped in a <p> block (since the <h1> tags are
         no longer interpreted as HTML).
         """
         field_data = DictFieldData({'data': '<h1>This is h1</h1>'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": 'escape'
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -149,15 +155,15 @@
 
     def test_render_allow_inline_html(self):
         """
         Test a basic rendering with javascript enabled.
         Expects the content *not* to be sanitized.
         """
         field_data = DictFieldData({'data': '<h1>This is h1</h1>'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": False
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -167,15 +173,15 @@
     def test_render_url_safe_mode_replace(self):
         """
         Test rendering a URL with safe_mode set to 'replace'.
         """
         field_data = DictFieldData(
             {'data': '[test1](https://test.com/courses/course-v1:Org+Class+Version/about) [test2](https://test.com/courses/course-v1%3AOrg%2BClass%2BVersion/about)'}  # noqa: E501
         )
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": 'replace'
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -192,15 +198,15 @@
     def test_render_url_safe_mode_escape(self):
         """
         Test rendering a URL with safe_mode set to 'replace'.
         """
         field_data = DictFieldData(
             {'data': '[test1](https://test.com/courses/course-v1:Org+Class+Version/about) [test2](https://test.com/courses/course-v1%3AOrg%2BClass%2BVersion/about)'}  # noqa: E501
         )
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": 'escape'
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -217,15 +223,15 @@
     def test_render_url_no_safe_mode(self):
         """
         Test rendering a URL with safe_mode disabled.
         """
         field_data = DictFieldData(
             {'data': '[test](https://test.com/courses/course-v1:Org+Class+Version/about)'}
         )
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         settings = {
             "extras": DEFAULT_EXTRAS,
             "safe_mode": False
         }
         with patch('markdown_xblock.html.get_xblock_settings') as get_settings_mock:
             get_settings_mock.return_value = settings
             fragment = block.student_view()
@@ -235,42 +241,42 @@
             )
 
     def test_substitution_no_system(self):
         """
         Test that the substitution is not performed when `system` is not present inside XBlock.
         """
         field_data = DictFieldData({'data': '%%USER_ID%% %%COURSE_ID%%'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         fragment = block.student_view()
         self.assertIn('<div class="markdown_xblock"><p>%%USER_ID%% %%COURSE_ID%%</p>\n</div>\n', fragment.content)
 
     def test_substitution_not_found(self):
         """
         Test that the keywords are not replaced when they're not found.
         """
         field_data = DictFieldData({'data': 'USER_ID%% %%COURSE_ID%%'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         block.system = Mock(anonymous_student_id=None)
         fragment = block.student_view()
         self.assertIn('<div class="markdown_xblock"><p>USER_ID%% %%COURSE_ID%%</p>\n</div>\n', fragment.content)
 
     def test_user_id_substitution(self):
         """
         Test replacing %%USER_ID%% with anonymous user ID.
         """
         field_data = DictFieldData({'data': '%%USER_ID%%'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         block.system = Mock(anonymous_student_id='test_user')
         fragment = block.student_view()
         self.assertIn('<div class="markdown_xblock"><p>test_user</p>\n</div>\n', fragment.content)
 
     def test_course_id_substitution(self):
         """
         Test replacing %%COURSE_ID%% with HTML representation of course key.
         """
         field_data = DictFieldData({'data': '%%COURSE_ID%%'})
-        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, None)
+        block = markdown_xblock.MarkdownXBlock(self.runtime, field_data, scope_ids=self.scope_ids)
         course_locator_mock = Mock()
         course_locator_mock.html_id = Mock(return_value='test_course')
         block.system = Mock(course_id=course_locator_mock)
         fragment = block.student_view()
         self.assertIn('<div class="markdown_xblock"><p>test_course</p>\n</div>\n', fragment.content)
```

### Comparing `markdown-xblock-1.4.0/tox.ini` & `markdown-xblock-1.5.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tox]
-envlist = py38,flake8,report
+envlist = py{38,310,312},flake8,report
 
 [gh-actions]
 python =
     3.8: py38,flake8
+    3.10: py310,flake8
+    3.12: py312,flake8
 
 [flake8]
 ignore = E124
 max-line-length = 120
 
 [coverage:run]
 parallel = True
```

