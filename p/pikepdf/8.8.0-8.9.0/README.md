# Comparing `tmp/pikepdf-8.8.0.tar.gz` & `tmp/pikepdf-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-8.8.0.tar", last modified: Sun Dec  3 02:02:59 2023, max compression
+gzip compressed data, was "pikepdf-8.9.0.tar", last modified: Sun Dec 10 23:26:49 2023, max compression
```

## Comparing `pikepdf-8.8.0.tar` & `pikepdf-8.9.0.tar`

### file list

```diff
@@ -1,197 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.476948 pikepdf-8.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-12-03 02:01:13.000000 pikepdf-8.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-03 02:01:13.000000 pikepdf-8.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-12-03 02:02:59.476948 pikepdf-8.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2023-12-03 02:01:13.000000 pikepdf-8.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.448948 pikepdf-8.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.448948 pikepdf-8.8.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/_ext/fix_pybind11_autodoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.448948 pikepdf-8.8.0/docs/_notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/_notebooks/pages.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.452948 pikepdf-8.8.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/api/filters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/api/settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/binary-wheels.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.452948 pikepdf-8.8.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   543264 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/28fish.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     8489 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/acrobat-attachments.png
--rw-r--r--   0 runner    (1001) docker     (127)    26172 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/congress_im0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/pdfcoords.svg
--rw-r--r--   0 runner    (1001) docker     (127)   148388 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/pike-cartoon.png
--rw-r--r--   0 runner    (1001) docker     (127)    88609 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/pike-release.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    32321 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/pike.png
--rw-r--r--   0 runner    (1001) docker     (127)    29276 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/pikemen.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    65692 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/save-pike.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   155993 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/images/sushi.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.452948 pikepdf-8.8.0/docs/references/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/references/arch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/references/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/references/debugging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/references/resources.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.456948 pikepdf-8.8.0/docs/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version0.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17003 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version1.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version3.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version4.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version6.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version7.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/releasenotes/version8.rst
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.456948 pikepdf-8.8.0/docs/topics/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/attachments.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/content_streams.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/encoding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/images.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/nametrees.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/outlines.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/overlays.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/page.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/pagelayout.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/pages.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/topics/streams.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2023-12-03 02:01:13.000000 pikepdf-8.8.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2023-12-03 02:01:13.000000 pikepdf-8.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-03 02:02:59.476948 pikepdf-8.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2023-12-03 02:01:13.000000 pikepdf-8.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.448948 pikepdf-8.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.460948 pikepdf-8.8.0/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/annotation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/embeddedfiles.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/jbig2-inl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/job.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/mmap_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/nametree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/numbertree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    43391 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/object.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/object_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/object_repr.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/page.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/parsers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/parsers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/pikepdf.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/pikepdf.h
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/pipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/pipeline.h
--rw-r--r--   0 runner    (1001) docker     (127)    37703 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/qpdf.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/qpdf_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15441 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/qpdf_pagelist.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/qpdf_pagelist.h
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/rectangle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/tokenfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/core/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.460948 pikepdf-8.8.0/src/pikepdf/
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_augments.py
--rw-r--r--   0 runner    (1001) docker     (127)    27801 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_cpphelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    60241 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_qpdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/jbig2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.464948 pikepdf-8.8.0/src/pikepdf/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/_content_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)    37931 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    32023 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/models/outlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-03 02:01:13.000000 pikepdf-8.8.0/src/pikepdf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.472948 pikepdf-8.8.0/src/pikepdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-12-03 02:02:59.000000 pikepdf-8.8.0/src/pikepdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-12-03 02:02:59.000000 pikepdf-8.8.0/src/pikepdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 02:02:59.000000 pikepdf-8.8.0/src/pikepdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-03 02:02:59.000000 pikepdf-8.8.0/src/pikepdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-03 02:02:59.000000 pikepdf-8.8.0/src/pikepdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.468948 pikepdf-8.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 02:02:59.472948 pikepdf-8.8.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/1biticc.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/Gray.icc
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/aquamarine-cie.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/aquamarine-cie.png
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/cmyk-jpeg.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    97969 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/congress-gray.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   193947 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/congress.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/content-stream-errors.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/form.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/formxobject.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/fourpages.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   296661 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/graph-encrypted.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   296322 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/graph.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/image-mono-inline.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/invalid_creationdate.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    20306 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/jbig2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    60332 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/jbig2global.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/newline-buffer-test.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/outlines.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pal-1bit-rgb.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pal-1bit-trivial.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pal.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)   533953 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pdfx.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    18471 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pike-flate-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pike-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pink-palette-icc.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/pink-palette-icc.png
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/rle.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   115546 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/sandwich.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_augments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_foreign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_formxobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    33373 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_image_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_io_psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_jbig2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    25174 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_nametree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_numbertree.py
--rw-r--r--   0 runner    (1001) docker     (127)    23537 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_objectlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    17194 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_outlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    15569 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13003 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_pdfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_private_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2023-12-03 02:01:13.000000 pikepdf-8.8.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.663727 pikepdf-8.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-12-10 23:24:59.000000 pikepdf-8.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-12-10 23:24:59.000000 pikepdf-8.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2023-12-10 23:26:49.663727 pikepdf-8.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2023-12-10 23:24:59.000000 pikepdf-8.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.635727 pikepdf-8.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.635727 pikepdf-8.9.0/docs/_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/_notebooks/pages.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.635727 pikepdf-8.9.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/api/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/api/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/binary-wheels.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.635727 pikepdf-8.9.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   543264 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/28fish.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/acrobat-attachments.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26172 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/congress_im0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/pdfcoords.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   148388 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/pike-cartoon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    88609 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/pike-release.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    32321 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/pike.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29276 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/pikemen.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    65692 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/save-pike.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   155993 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/images/sushi.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.639727 pikepdf-8.9.0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/references/arch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/references/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/references/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/references/resources.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.639727 pikepdf-8.9.0/docs/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17003 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13480 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version6.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version7.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/releasenotes/version8.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.639727 pikepdf-8.9.0/docs/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/attachments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/content_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/encoding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/images.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/nametrees.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/outlines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/overlays.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/page.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/pagelayout.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/pages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/security.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/topics/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2023-12-10 23:24:59.000000 pikepdf-8.9.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2023-12-10 23:24:59.000000 pikepdf-8.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 23:26:49.663727 pikepdf-8.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2023-12-10 23:24:59.000000 pikepdf-8.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.631727 pikepdf-8.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.643727 pikepdf-8.9.0/src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/annotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/embeddedfiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/jbig2-inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/mmap_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/nametree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/numbertree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35678 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/object_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/object_repr.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/page.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12689 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/parsers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/parsers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/pikepdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/pikepdf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/pipeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/pipeline.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26525 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/qpdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/qpdf_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11782 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/qpdf_pagelist.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/qpdf_pagelist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/rectangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/tokenfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/core/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.647727 pikepdf-8.9.0/src/pikepdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_augments.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116538 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_cpphelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26376 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_qpdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14938 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/jbig2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.647727 pikepdf-8.9.0/src/pikepdf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/_content_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37992 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32056 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15453 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/models/outlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-10 23:24:59.000000 pikepdf-8.9.0/src/pikepdf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.659727 pikepdf-8.9.0/src/pikepdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2023-12-10 23:26:49.000000 pikepdf-8.9.0/src/pikepdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2023-12-10 23:26:49.000000 pikepdf-8.9.0/src/pikepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 23:26:49.000000 pikepdf-8.9.0/src/pikepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-10 23:26:49.000000 pikepdf-8.9.0/src/pikepdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-10 23:26:49.000000 pikepdf-8.9.0/src/pikepdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.655727 pikepdf-8.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 23:26:49.659727 pikepdf-8.9.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/1biticc.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/Gray.icc
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/aquamarine-cie.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/aquamarine-cie.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/cmyk-jpeg.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    97969 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/congress-gray.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   193947 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/congress.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/content-stream-errors.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/form.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/formxobject.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/fourpages.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   296661 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/graph-encrypted.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   296322 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/image-mono-inline.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/invalid_creationdate.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    20306 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/jbig2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    60332 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/jbig2global.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/newline-buffer-test.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/outlines.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pal-1bit-rgb.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pal-1bit-trivial.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pal.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   533953 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pdfx.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    18471 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pike-flate-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pike-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pink-palette-icc.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/pink-palette-icc.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/rle.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   115546 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/sandwich.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_augments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_formxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33373 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_image_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_io_psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_jbig2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25174 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_nametree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_numbertree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23537 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_objectlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17194 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15569 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13003 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_pdfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_private_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2023-12-10 23:24:59.000000 pikepdf-8.9.0/tests/test_sanity.py
```

### Comparing `pikepdf-8.8.0/LICENSE.txt` & `pikepdf-8.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/PKG-INFO` & `pikepdf-8.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.8.0
+Version: 8.9.0
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
@@ -25,35 +25,30 @@
 Requires-Dist: Deprecated
 Requires-Dist: lxml>=4.8
 Requires-Dist: packaging
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: typer[all]; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: GitPython; extra == "docs"
-Requires-Dist: PyGithub; extra == "docs"
 Requires-Dist: Sphinx>=3; extra == "docs"
-Requires-Dist: ipython; extra == "docs"
-Requires-Dist: matplotlib; extra == "docs"
-Requires-Dist: pybind11; extra == "docs"
-Requires-Dist: requests; extra == "docs"
+Requires-Dist: sphinx-autoapi; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: sphinx-issues; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: mypy
 Requires-Dist: lxml-stubs; extra == "mypy"
 Requires-Dist: types-Pillow; extra == "mypy"
 Requires-Dist: types-requests; extra == "mypy"
 Requires-Dist: types-setuptools; extra == "mypy"
 Provides-Extra: test
 Requires-Dist: attrs>=20.2.0; extra == "test"
 Requires-Dist: coverage[toml]; extra == "test"
 Requires-Dist: hypothesis>=6.36; extra == "test"
-Requires-Dist: numpy>=1.21.0; extra == "test"
+Requires-Dist: numpy>=1.21.0; (platform_machine == "x86_64" or platform_python_implementation == "CPython") and extra == "test"
 Requires-Dist: psutil>=5.9; os_name != "nt" and extra == "test"
 Requires-Dist: pybind11; extra == "test"
 Requires-Dist: pytest>=6.2.5; extra == "test"
 Requires-Dist: pytest-cov>=3.0.0; extra == "test"
 Requires-Dist: pytest-timeout>=2.1.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.5.0; extra == "test"
 Requires-Dist: python-dateutil>=2.8.1; extra == "test"
```

### Comparing `pikepdf-8.8.0/README.md` & `pikepdf-8.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/Makefile` & `pikepdf-8.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/_notebooks/pages.ipynb` & `pikepdf-8.9.0/docs/_notebooks/pages.ipynb`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/28fish.jpg` & `pikepdf-8.9.0/docs/images/28fish.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/acrobat-attachments.png` & `pikepdf-8.9.0/docs/images/acrobat-attachments.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/congress_im0.jpg` & `pikepdf-8.9.0/docs/images/congress_im0.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/pdfcoords.svg` & `pikepdf-8.9.0/docs/images/pdfcoords.svg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/pike-cartoon.png` & `pikepdf-8.9.0/docs/images/pike-cartoon.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/pike-release.jpg` & `pikepdf-8.9.0/docs/images/pike-release.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/pike.png` & `pikepdf-8.9.0/docs/images/pike.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/pikemen.jpg` & `pikepdf-8.9.0/docs/images/pikemen.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/save-pike.jpg` & `pikepdf-8.9.0/docs/images/save-pike.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/images/sushi.jpg` & `pikepdf-8.9.0/docs/images/sushi.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/index.rst` & `pikepdf-8.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/installation.rst` & `pikepdf-8.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/make.bat` & `pikepdf-8.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/references/arch.rst` & `pikepdf-8.9.0/docs/references/arch.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/references/contributing.rst` & `pikepdf-8.9.0/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/references/debugging.rst` & `pikepdf-8.9.0/docs/references/debugging.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/references/resources.rst` & `pikepdf-8.9.0/docs/references/resources.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/index.rst` & `pikepdf-8.9.0/docs/releasenotes/index.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version0.rst` & `pikepdf-8.9.0/docs/releasenotes/version0.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version1.rst` & `pikepdf-8.9.0/docs/releasenotes/version1.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version2.rst` & `pikepdf-8.9.0/docs/releasenotes/version2.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version3.rst` & `pikepdf-8.9.0/docs/releasenotes/version3.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version4.rst` & `pikepdf-8.9.0/docs/releasenotes/version4.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version5.rst` & `pikepdf-8.9.0/docs/releasenotes/version5.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version6.rst` & `pikepdf-8.9.0/docs/releasenotes/version6.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version7.rst` & `pikepdf-8.9.0/docs/releasenotes/version7.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/releasenotes/version8.rst` & `pikepdf-8.9.0/docs/releasenotes/version8.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,20 @@
 
+v8.9.0
+======
+
+- Overhauled documentation. Previously the documentation could only be generated in
+  an environment where pikepdf was compiled and installed, since generating the final
+  result depended on executing pikepdf. Now, these dynamic features are removed and
+  the documentation is static. All documentation that was defined in C++ has been
+  pulled out and defined in Python stub files instead, which means compiled binaries
+  are no longer needed to access documentation. This change simplifies the generation of
+  documentation and makes it easier for IDEs to look up function signatures.
+- Similarly, typing is now defined only in Python stub files.
+
 v8.8.0
 ======
 
 - Added new ``pikepdf.canvas`` module with rudimentary content stream creation
   functions.
 
 v8.7.1
```

### Comparing `pikepdf-8.8.0/docs/topics/attachments.rst` & `pikepdf-8.9.0/docs/topics/attachments.rst`

 * *Files 20% similar despite different names*

```diff
@@ -5,46 +5,51 @@
 
 .. versionadded:: 3.0
 
 You can attach (or if you prefer, embed) any file to a PDF, including
 other PDFs. As a quick example, let's attach pikepdf's README.md file
 to one of its test files.
 
-.. ipython::
+.. doctest::
 
-    In [1]: from pikepdf import Pdf, AttachedFileSpec, Name, Dictionary, Array
+    >>> from pikepdf import Pdf, AttachedFileSpec, Name, Dictionary, Array
 
-    In [1]: from pathlib import Path
+    >>> from pathlib import Path
 
-    In [1]: pdf = Pdf.open('../tests/resources/fourpages.pdf')
+    >>> pdf = Pdf.open('../tests/resources/fourpages.pdf')
 
-    In [1]: filespec = AttachedFileSpec.from_filepath(pdf, Path('../README.md'))
+    >>> filespec = AttachedFileSpec.from_filepath(pdf, Path('../README.md'))
 
-    In [1]: pdf.attachments['README.md'] = filespec
+    >>> pdf.attachments['README.md'] = filespec
 
-    In [1]: pdf.attachments
+    >>> pdf.attachments
+    <pikepdf._core.Attachments with 1 attached files>
 
 This creates an attached file named ``README.md``, which holds the data in ``filespec``.
 Now we can retrieve the data.
 
-.. ipython::
+.. doctest::
 
-    In [1]: pdf.attachments['README.md']
+    >>> pdf.attachments['README.md']
+    <pikepdf._core.AttachedFileSpec for 'README.md', description ''>
 
-    In [1]: file = pdf.attachments['README.md'].get_file()
+    >>> file = pdf.attachments['README.md'].get_file()
 
-    In [1]: file.read_bytes()[:50]
+.. code-block:: python
+
+    >>> file.read_bytes()[...]
+    b'**pikepdf** is a Python library for reading and writing PDF files.'
 
 If the data used to create an attachment is in memory:
 
-.. ipython::
+.. doctest::
 
-    In [1]: memfilespec = AttachedFileSpec(pdf, b'Some text', mime_type='text/plain')
+    >>> memfilespec = AttachedFileSpec(pdf, b'Some text', mime_type='text/plain')
 
-    In [1]: pdf.attachments['plain.txt'] = memfilespec
+    >>> pdf.attachments['plain.txt'] = memfilespec
 
 
 General notes on attached files
 -------------------------------
 
 * If the main PDF is encrypted, any embedded files will be encrypted with the same
   encryption settings.
@@ -81,27 +86,27 @@
 -------------------------------
 
 You can also create PDF Annotations and Actions that contain attached files.
 
 Here is an example of an annotation that displays an icon. Clicking the icon
 prompt the user to view the attached document.
 
-.. ipython::
+.. doctest::
 
-  In [1]: pdf = Pdf.open('../tests/resources/fourpages.pdf')
+  >>> pdf = Pdf.open('../tests/resources/fourpages.pdf')
 
-  In [1]: filespec = AttachedFileSpec.from_filepath(pdf, Path('../README.md'))
+  >>> filespec = AttachedFileSpec.from_filepath(pdf, Path('../README.md'))
 
-  In [1]: pushpin = Dictionary(
-     ...:     Type=Name.Annot,
-     ...:     Subtype=Name.FileAttachment,
-     ...:     Name=Name.GraphPushPin,
-     ...:     FS=filespec.obj,
-     ...:     Rect=[2*72, 9*72, 3*72, 10*72],
-     ...: )
-
-  In [1]: pdf.pages[0].Annots = pdf.make_indirect(Array([
-     ...:     pushpin
-     ...: ]))
+  >>> pushpin = Dictionary(
+  ...     Type=Name.Annot,
+  ...     Subtype=Name.FileAttachment,
+  ...     Name=Name.GraphPushPin,
+  ...     FS=filespec.obj,
+  ...     Rect=[2*72, 9*72, 3*72, 10*72],
+  ... )
+
+  >>> pdf.pages[0].Annots = pdf.make_indirect(Array([
+  ...     pushpin
+  ... ]))
 
 Files that are referenced as Annotations and Actions do not need to be added
 to ``Pdf.attachments``. If they are, the file will be attached twice.
```

### Comparing `pikepdf-8.8.0/docs/topics/content_streams.rst` & `pikepdf-8.9.0/docs/topics/content_streams.rst`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 -------------------------------
 
 To pretty-print a content stream, you can use parse and then unparse it. This
 converts it from binary data form to pikepdf objects and back. In the process,
 the content stream is cleaned up. Every instruction will be separated by a line
 break.
 
-.. ipython:: python
+.. doctest::
 
   with pikepdf.open("../tests/resources/congress.pdf") as pdf:
       page = pdf.pages[0]
       instructions = pikepdf.parse_content_stream(page)
       data = pikepdf.unparse_content_stream(instructions)
       print(data.decode('ascii'))
 
@@ -57,15 +57,15 @@
 
 How content streams draw images
 -------------------------------
 
 This example prints a typical content stream from a real file, which like the
 contrived example above, displays an actual image.
 
-.. ipython:: python
+.. doctest::
 
   with pikepdf.open("../tests/resources/congress.pdf") as pdf:
       page = pdf.pages[0]
       commands = []
       for operands, operator in pikepdf.parse_content_stream(page):
           print(f"Operands {operands}, operator {operator}")
           if operator == pikepdf.Operator('cm'):
@@ -96,15 +96,15 @@
 of this page. We're currently in a coordinate system where (0, 0) is the bottom
 left corner of the page, and (1, 1) is the top right corner. Without actually
 having to track the image's position, we can translate it by 0.25 of its
 dimensions (to create a border of 25% all around) and then scale it by 0.5.
 (We could also scale by 50%, and then translate by 50%, which would be 25% in
 the full image coordinate system.)
 
-.. ipython:: python
+.. doctest::
 
   new_matrix = matrix.translated(0.25, 0.25).scaled(0.5, 0.5)
   new_matrix
 
 On an important note, the PDF coordinate system is nailed to the **bottom left**
 corner of the page, and on y-axis, **up is positive**. That is, the coordinate
 system is more like the first quadrant of a Cartesian graph than the
@@ -118,15 +118,15 @@
 (Some PDF programs insert a command to "flip" the coordinate system, by
 translating to the top left corner and scaling by (1, -1).)
 
 After calculating our new matrix, we need to insert it back into the parsed
 content stream, "unparse" it to binary data, and replace the old content
 stream.
 
-.. ipython:: python
+.. doctest::
 
   commands[1][0] = pikepdf.Array(new_matrix)
   new_content_stream = pikepdf.unparse_content_stream(commands)
   new_content_stream
   page.Contents = pdf.make_stream(new_content_stream)
 
   # You could save the file here to see it
```

### Comparing `pikepdf-8.8.0/docs/topics/encoding.rst` & `pikepdf-8.9.0/docs/topics/encoding.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/topics/images.rst` & `pikepdf-8.9.0/docs/topics/images.rst`

 * *Files 16% similar despite different names*

```diff
@@ -25,46 +25,50 @@
 Playing with images
 -------------------
 
 pikepdf provides a helper class :class:`~pikepdf.PdfImage` for manipulating
 images in a PDF. The helper class helps manage the complexity of the image
 dictionaries.
 
-.. ipython::
+.. doctest::
 
-    In [1]: from pikepdf import Pdf, PdfImage, Name
+    >>> from pikepdf import Pdf, PdfImage, Name
 
-    In [1]: example = Pdf.open('../tests/resources/congress.pdf')
+    >>> example = Pdf.open('../tests/resources/congress.pdf')
 
-    In [1]: page1 = example.pages[0]
+    >>> page1 = example.pages[0]
 
-    In [1]: list(page1.images.keys())
+    >>> list(page1.images.keys())
+    ['/Im0']
 
-    In [1]: rawimage = page1.images['/Im0']  # The raw object/dictionary
+    >>> rawimage = page1.images['/Im0']  # The raw object/dictionary
 
-    In [1]: pdfimage = PdfImage(rawimage)
+    >>> pdfimage = PdfImage(rawimage)
 
-    In [1]: type(pdfimage)
+    >>> type(pdfimage)
+    <class 'pikepdf.models.image.PdfImage'>
 
 In Jupyter (or IPython with a suitable backend) the image will be
 displayed.
 
 |im0|
 
 .. |im0| image:: /images/congress_im0.jpg
   :width: 2in
 
 You can also inspect the properties of the image. The parameters are similar
 to Pillow's.
 
-.. ipython::
+.. doctest::
 
-    In [1]: pdfimage.colorspace
+    >>> pdfimage.colorspace
+    '/DeviceRGB'
 
-    In [1]: pdfimage.width, pdfimage.height
+    >>> pdfimage.width, pdfimage.height
+    (1000, 1520)
 
 .. note::
 
     ``.width`` and ``.height`` are the resolution of the image in pixels, not
     the size of the image in page coordinates. The size of the image in page
     coordinates is determined by the content stream.
 
@@ -75,28 +79,28 @@
 
 Extracting images is straightforward. :meth:`~pikepdf.PdfImage.extract_to` will
 extract images to a specified file prefix. The extension is determined while
 extracting and appended to the filename. Where possible, ``extract_to``
 writes compressed data directly to the stream without transcoding. (Transcoding
 lossy formats like JPEG can reduce their quality.)
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: pdfimage.extract_to(fileprefix='image')
-    Out[1]: 'image.jpg'
+    >>> pdfimage.extract_to(fileprefix='image')
+    'image.jpg'
 
 It also possible to extract to a writable Python stream using
 ``.extract_to(stream=...`)``.
 
 You can also retrieve the image as a Pillow image (this will transcode):
 
-.. ipython::
+.. doctest::
 
-    In [1]: type(pdfimage.as_pil_image())
+    >>> type(pdfimage.as_pil_image())
+    <class 'PIL.JpegImagePlugin.JpegImageFile'>
 
 Another way to view the image is using Pillow's ``Image.show()`` method.
 
 Not all image types can be extracted. Also, some PDFs describe an image with a
 mask, with transparency effects. pikepdf can only extract the images
 themselves, not rasterize them exactly as they would appear in a PDF viewer. In
 the vast majority of cases, however, the image can be extracted as it appears.
@@ -117,31 +121,31 @@
 
 Replacing an image
 ------------------
 
 In this example we extract an image and replace it with a grayscale
 equivalent.
 
-.. ipython::
+.. doctest::
 
-    In [1]: import zlib
+    >>> import zlib
 
-    In [1]: rawimage = pdfimage.obj
+    >>> rawimage = pdfimage.obj
 
-    In [1]: pillowimage = pdfimage.as_pil_image()
+    >>> pillowimage = pdfimage.as_pil_image()
 
-    In [1]: grayscale = pillowimage.convert('L')
+    >>> grayscale = pillowimage.convert('L')
 
-    In [1]: grayscale = grayscale.resize((32, 32))
+    >>> grayscale = grayscale.resize((32, 32))
 
-    In [1]: rawimage.write(zlib.compress(grayscale.tobytes()), filter=Name("/FlateDecode"))
+    >>> rawimage.write(zlib.compress(grayscale.tobytes()), filter=Name("/FlateDecode"))
 
-    In [1]: rawimage.ColorSpace = Name("/DeviceGray")
+    >>> rawimage.ColorSpace = Name("/DeviceGray")
 
-    In [1]: rawimage.Width, rawimage.Height = 32, 32
+    >>> rawimage.Width, rawimage.Height = 32, 32
 
 Notes on this example:
 
 * It is generally possible to use ``zlib.compress()`` to
   generate compressed image data, although this is not as efficient as using
   a program that knows it is preparing a PDF.
 
@@ -157,26 +161,26 @@
 The easy way to remove an image is to replace it with a 1x1 pixel transparent image.
 A transparent image can be created by setting the ``/ImageMask`` to true.
 
 Note that, if an image is referenced on multiple pages, this procedure only updates
 the occurrence on one page. If all references to the image are deleted, it should
 not be included in the output file.
 
-.. ipython::
+.. doctest::
 
-  In [1]: pdf = pikepdf.open('../tests/resources/sandwich.pdf')
+  >>> pdf = pikepdf.open('../tests/resources/sandwich.pdf')
 
-  In [1]: page = pdf.pages[0]
+  >>> page = pdf.pages[0]
 
-  In [1]: image_name, image = next(iter(page.images.items()))
+  >>> image_name, image = next(iter(page.images.items()))
 
-  In [1]: new_image = pdf.make_stream(b'\xff')
+  >>> new_image = pdf.make_stream(b'\xff')
 
-  In [1]: new_image.Width, new_image.Height = 1, 1
+  >>> new_image.Width, new_image.Height = 1, 1
 
-  In [1]: new_image.BitsPerComponent = 1
+  >>> new_image.BitsPerComponent = 1
 
-  In [1]: new_image.ImageMask = True
+  >>> new_image.ImageMask = True
 
-  In [1]: new_image.Decode = [0, 1]
+  >>> new_image.Decode = [0, 1]
 
-  In [1]: page.Resources.XObject[image_name] = new_image
+  >>> page.Resources.XObject[image_name] = new_image
```

### Comparing `pikepdf-8.8.0/docs/topics/metadata.rst` & `pikepdf-8.9.0/docs/topics/metadata.rst`

 * *Files 9% similar despite different names*

```diff
@@ -42,35 +42,35 @@
 management of this, use :meth:`pikepdf.Pdf.open_metadata`. The returned
 :class:`pikepdf.models.PdfMetadata` object may be used for reading, or entered
 with a ``with`` block to modify and commit changes. If you use this interface,
 pikepdf will synchronize changes to new and old metadata.
 
 A PDF must still be saved after metadata is changed.
 
-.. ipython::
+.. doctest::
 
-  In [1]: pdf = pikepdf.open('../tests/resources/sandwich.pdf')
+  >>> pdf = pikepdf.open('../tests/resources/sandwich.pdf')
 
-  In [2]: meta = pdf.open_metadata()
+  >>> meta = pdf.open_metadata()
 
-  In [3]: meta['xmp:CreatorTool']
-  Out[3]: 'ocrmypdf 5.3.3 / Tesseract OCR-PDF 3.05.01'
+  >>> meta['xmp:CreatorTool']
+  'ocrmypdf 5.3.3 / Tesseract OCR-PDF 3.05.01'
 
 If no XMP metadata exists, an empty XMP metadata container will be created.
 
 Open metadata in a ``with`` block to open it for editing. When the block is
 exited, changes are committed (updating XMP and the Document Info dictionary)
 and attached to the PDF object. The PDF must still be saved. If an exception
 occurs in the block, changes are discarded.
 
-.. ipython::
+.. doctest::
 
-  In [4]: with pdf.open_metadata() as meta:
-     ...:     meta['dc:title'] = "Let's change the title"
-     ...:
+  >>> with pdf.open_metadata() as meta:
+  ...     meta['dc:title'] = "Let's change the title"
+  ...
 
 The list of available metadata fields may be found in the `XMP Specification`_.
 
 Removing metadata items
 -----------------------
 
 After opening metadata, use ``del meta['dc:title']`` to delete a metadata entry.
@@ -81,22 +81,22 @@
 
 Checking PDF/A conformance
 --------------------------
 
 The metadata interface can also test if a file **claims** to be conformant
 to the PDF/A specification.
 
-.. ipython::
+.. doctest::
 
-  In [9]: pdf = pikepdf.open('../tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf')
+  >>> pdf = pikepdf.open('../tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf')
 
-  In [10]: meta = pdf.open_metadata()
+  >>> meta = pdf.open_metadata()
 
-  In [11]: meta.pdfa_status
-  Out[11]: '1B'
+  >>> meta.pdfa_status
+  '1B'
 
 .. note::
 
   Note that this property merely *tests* if the file claims to be conformant to
   the PDF/A standard. Use a tool such as `veraPDF`_ (official tool), or third party
   web services such as `PDFEN`_ or 3-HEIGHTS™ PDF `VALIDATOR`_ to verify conformance.
 
@@ -120,22 +120,23 @@
 
 Low-level XMP metadata access
 -----------------------------
 
 You can read the raw XMP metadata if desired. For example, one could extract it and
 edit it using the full featured ``python-xmp-toolkit`` library.
 
-.. ipython::
+.. doctest::
 
-   In [1]: xmp = pdf.Root.Metadata.read_bytes()
+   >>> xmp = pdf.Root.Metadata.read_bytes()
 
-   In [1]: type(xmp)
-   Out[1]: bytes
+   >>> type(xmp)
+   <class 'bytes'>
 
-   In [1]: print(xmp.decode())
+   >>> print(xmp.decode()[:len("<?xpacket")] + "...")
+   <?xpacket...
 
 Editing XMP with a generic XML library is probably not worth the trouble; the
 semantics are fairly complex.
 
 .. warning::
 
   Manually changes to XMP stream object will not be synchronized with live
@@ -147,20 +148,19 @@
 The Document Info block is an older, now deprecated object in which metadata
 may be stored. The Document Info is not attached to the /Root object.
 It may be accessed using the ``.docinfo`` property. If no Document Info exists,
 touching the ``.docinfo`` will properly initialize an empty one.
 
 Here is an example of a Document Info block.
 
-.. ipython::
+.. doctest::
 
-  In [12]: pdf = pikepdf.open('../tests/resources/sandwich.pdf')
+  >>> pdf = pikepdf.open('../tests/resources/sandwich.pdf')
 
-  In [12]: pdf.docinfo
-  Out[12]:
+  >>> pdf.docinfo
   pikepdf.Dictionary({
     "/CreationDate": "D:20170911132748-07'00'",
     "/Creator": "ocrmypdf 5.3.3 / Tesseract OCR-PDF 3.05.01",
     "/ModDate": "D:20170911132748-07'00'",
     "/Producer": "GPL Ghostscript 9.21"
   })
```

### Comparing `pikepdf-8.8.0/docs/topics/nametrees.rst` & `pikepdf-8.9.0/docs/topics/nametrees.rst`

 * *Files 16% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 * ``JavaScript``: embedded PDF JavaScript
 * ``Pages``: named pages
 * ``IDS``: digital identifiers
 
 Attached files (or embedded files) are managed in a name tree, but pikepdf
 provides an interface specifically for managing them. Use that instead.
 
-.. ipython::
+.. doctest::
 
-    In [1]: from pikepdf import Pdf, Page, NameTree
+    >>> from pikepdf import Pdf, Page, NameTree
 
-    In [1]: pdf = Pdf.open('../tests/resources/outlines.pdf')
+    >>> pdf = Pdf.open('../tests/resources/outlines.pdf')
 
-    In [1]: nt = NameTree(pdf.Root.Names.Dests)
+    >>> nt = NameTree(pdf.Root.Names.Dests)
 
-    In [1]: print([k for k in nt.keys()])
+    >>> print([k for k in nt.keys()])
+    ['0', '1', '2', '3', '4', '5', '6', '7', '8']
 
-    In [1]: nt['2'][0].objgen, nt['2'][1], nt['2'][2]
+    >>> nt['2'][0].objgen, nt['2'][1], nt['2'][2]
+    ((3, 0), pikepdf.Name("/XYZ"), Decimal('89.29'))
```

### Comparing `pikepdf-8.8.0/docs/topics/objects.rst` & `pikepdf-8.9.0/docs/topics/objects.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/topics/outlines.rst` & `pikepdf-8.9.0/docs/topics/outlines.rst`

 * *Files 20% similar despite different names*

```diff
@@ -9,51 +9,49 @@
 -----------------
 Outlines can be created from scratch, e.g. when assembling a set of PDF files
 into a single document.
 
 The following example adds outline entries referring to the 1st, 3rd and 9th page
 of an existing PDF.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: from pikepdf import Pdf, OutlineItem
+    >>> from pikepdf import Pdf, OutlineItem
 
-    In [1]: pdf = Pdf.open('document.pdf')
+    >>> pdf = Pdf.open('document.pdf')
 
-    In [1]: with pdf.open_outline() as outline:
-       ...:     outline.root.extend([
-       ...:         # Page counts are zero-based
-       ...:         OutlineItem('Section One', 0),
-       ...:         OutlineItem('Section Two', 2),
-       ...:         OutlineItem('Section Three', 8)
-       ...:     ])
+    >>> with pdf.open_outline() as outline:
+    ...     outline.root.extend([
+    ...         # Page counts are zero-based
+    ...         OutlineItem('Section One', 0),
+    ...         OutlineItem('Section Two', 2),
+    ...         OutlineItem('Section Three', 8)
+    ...     ])
 
-    In [1]: pdf.save('document_with_outline.pdf')
+    >>> pdf.save('document_with_outline.pdf')
 
 Another example, for automatically adding an entry for each file in a merged document:
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: from glob import glob
+    >>> from glob import glob
 
-    In [1]: pdf = Pdf.new()
+    >>> pdf = Pdf.new()
 
-    In [1]: page_count = 0
+    >>> page_count = 0
 
-    In [1]: with pdf.open_outline() as outline:
-       ...:     for file in glob('*.pdf'):
-       ...:         src = Pdf.open(file)
-       ...:         oi = OutlineItem(file, page_count)
-       ...:         outline.root.append(oi)
-       ...:         page_count += len(src.pages)
-       ...:         pdf.pages.extend(src.pages)
+    >>> with pdf.open_outline() as outline:
+    ...     for file in glob('*.pdf'):
+    ...         src = Pdf.open(file)
+    ...         oi = OutlineItem(file, page_count)
+    ...         outline.root.append(oi)
+    ...         page_count += len(src.pages)
+    ...         pdf.pages.extend(src.pages)
 
-    In [1]: pdf.save('merged.pdf')
+    >>> pdf.save('merged.pdf')
 
 Editing outlines
 ----------------
 Existing outlines can be edited. Entries can be moved and renamed without affecting
 the targets they refer to.
 
 Destinations
@@ -69,31 +67,28 @@
 * When creating new outline entries passing in a page number or reference name,
   the ``Dest`` attribute is used.
 * When editing an existing entry with an assigned action, it is left as-is, unless a
   ``destination`` is set. The latter is preferred if both are present.
 
 Creating a more detailed destination with page location:
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: oi = OutlineItem('First', 0, 'FitB', top=1000)
+    >>> oi = OutlineItem('First', 0, 'FitB', top=1000)
 
 The above will call ``make_page_destination`` when saving to a ``Pdf`` document,
 roughly equivalent to the following:
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: oi.destination = make_page_destination(pdf, 0, 'FitB', top=1000)
+    >>> oi.destination = make_page_destination(pdf, 0, 'FitB', top=1000)
 
 Outline structure
 ------------------
 For nesting outlines, add items to the ``children`` list of another ``OutlineItem``.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: with pdf.open_outline() as outline:
-       ...:     main_item = OutlineItem('Main', 0)
-       ...:     outline.root.append(main_item)
-       ...:     main_item.children.append(OutlineItem('A', 1))
+    >>> with pdf.open_outline() as outline:
+    ...     main_item = OutlineItem('Main', 0)
+    ...     outline.root.append(main_item)
+    ...     main_item.children.append(OutlineItem('A', 1))
```

### Comparing `pikepdf-8.8.0/docs/topics/overlays.rst` & `pikepdf-8.9.0/docs/topics/overlays.rst`

 * *Files 14% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 slides from a presentation to 4-up for reading and printing).
 
 If you are looking to merge pages from different PDFs, see :ref:`mergepdf`.
 
 In this example we use :meth:`pikepdf.Page.add_overlay` to draw a thumbnail of
 of the second page onto the first page.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: from pikepdf import Pdf, Page, Rectangle
+    >>> from pikepdf import Pdf, Page, Rectangle
 
-    In [1]: pdf = Pdf.open(...)
+    >>> pdf = Pdf.open(...)
 
-    In [1]: destination_page = Page(pdf.pages[0])
+    >>> destination_page = Page(pdf.pages[0])
 
-    In [1]: thumbnail = Page(pdf.pages[1])
+    >>> thumbnail = Page(pdf.pages[1])
 
-    In [1]: destination_page.add_overlay(thumbnail, Rectangle(0, 0, 300, 300))
+    >>> destination_page.add_overlay(thumbnail, Rectangle(0, 0, 300, 300))
 
-    In [1]: pdf.save("page1_with_page2_thumbnail.pdf")
+    >>> pdf.save("page1_with_page2_thumbnail.pdf")
 
 The :class:`pikepdf.Rectangle` specifies the position on the target page into which
 the other page can be drawn. The object will be drawn centered in a way that
 fills as much space as possible while preserving aspect ratio.
 
 Use :meth:`pikepdf.Page.add_underlay` instead if you want content drawn underneath.
 It is possible content drawn this way will be overdrawn by other objects.
```

### Comparing `pikepdf-8.8.0/docs/topics/pagelayout.rst` & `pikepdf-8.9.0/docs/topics/pagelayout.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/topics/security.rst` & `pikepdf-8.9.0/docs/topics/security.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/topics/streams.rst` & `pikepdf-8.9.0/docs/topics/streams.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/docs/tutorial.rst` & `pikepdf-8.9.0/docs/tutorial.rst`

 * *Files 22% similar despite different names*

```diff
@@ -61,48 +61,47 @@
 
 Manipulating pages is fundamental to PDFs. pikepdf presents the pages in a PDF
 through the :attr:`pikepdf.Pdf.pages` property, which follows the ``list``
 protocol. As such page numbers begin at 0.
 
 Let’s open a simple PDF that contains four pages.
 
-.. ipython::
+.. doctest::
 
-    In [1]: from pikepdf import Pdf
+    >>> from pikepdf import Pdf
 
-    In [2]: pdf = Pdf.open('../tests/resources/fourpages.pdf')
+    >>> pdf = Pdf.open('../tests/resources/fourpages.pdf')
 
 How many pages?
 
-.. ipython::
+.. doctest::
 
-    In [2]: len(pdf.pages)
+    >>> len(pdf.pages)
+    4
 
 pikepdf integrates with IPython and Jupyter's rich object APIs so that you can
 view PDFs, PDF pages, or images within PDF in a IPython window or Jupyter
 notebook. This makes it easier to test visual changes.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: pdf
-    Out[1]: « In Jupyter you would see the PDF here »
+    >>> pdf
+    « In Jupyter you would see the PDF here »
 
-    In [1]: pdf.pages[0]
-    Out[1]: « In Jupyter you would see an image of the PDF page here »
+    >>> pdf.pages[0]
+    « In Jupyter you would see an image of the PDF page here »
 
 You can also examine individual pages, which we’ll explore in the next
 section. Suffice to say that you can access pages by indexing them and
 slicing them.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: pdf.pages[0]
-    Out[1]: « In Jupyter you would see an image of the PDF page here »
+    >>> pdf.pages[0]
+    « In Jupyter you would see an image of the PDF page here »
 
 .. note::
 
     :meth:`pikepdf.Pdf.open` can open almost all types of encrypted PDF! Just
     provide the ``password=`` keyword argument.
 
 For more details on document assembly, see
@@ -115,82 +114,114 @@
 structure much like a Python ``dict`` or ``attrdict``. The major difference is
 that the keys can only be **names**, and the values can only be PDF types, including
 other dictionaries.
 
 PDF dictionaries are represented as :class:`pikepdf.Dictionary` objects, and names
 are of type :class:`pikepdf.Name`.
 
-.. ipython::
+.. doctest::
 
-    In [1]: from pikepdf import Pdf
+    >>> from pikepdf import Pdf
 
-    In [1]: example = Pdf.open('../tests/resources/congress.pdf')
+    >>> example = Pdf.open('../tests/resources/congress.pdf')
 
-    In [1]: example.Root  # Show the document's root dictionary
+    >>> example.Root  # Show the document's root dictionary
+    pikepdf.Dictionary(Type="/Catalog")({
+      "/Pages": {
+        "/Count": 1,
+        "/Kids": [ <Pdf.pages.from_objgen(4,0)> ],
+        "/Type": "/Pages"
+      },
+      "/Type": "/Catalog"
+    })
 
 Page dictionaries
 -----------------
 
 A page in a PDF is just a dictionary with certain required keys that is
 referenced by the PDF's "page tree". (pikepdf manages the page tree for you,
 and wraps page dictionaries to provide special functions
 that help with managing pages.) A :class:`pikepdf.Page` is a wrapper around a PDF
 page dictionary that provides many useful functions for working on pages.
 
-.. ipython::
+.. doctest::
 
-    In [1]: from pikepdf import Pdf
+    >>> from pikepdf import Pdf
 
-    In [1]: example = Pdf.open('../tests/resources/congress.pdf')
+    >>> example = Pdf.open('../tests/resources/congress.pdf')
 
-    In [1]: page1 = example.pages[0]
+    >>> page1 = example.pages[0]
 
-    In [1]: obj_page1 = page1.obj
-
-    In [1]: obj_page1
+    >>> obj_page1 = page1.obj
+
+    >>> obj_page1
+    <pikepdf.Dictionary(Type="/Page")({
+      "/Contents": pikepdf.Stream(owner=<...>, data=b'q\n200.0000 0 0 304.0'..., {
+        "/Length": 50
+      }),
+      "/MediaBox": [ 0, 0, 200, 304 ],
+      "/Parent": <reference to /Pages>,
+      "/Resources": {
+        "/XObject": {
+          "/Im0": pikepdf.Stream(owner=<...>, data=<...>, {
+            "/BitsPerComponent": 8,
+            "/ColorSpace": "/DeviceRGB",
+            "/Filter": [ "/DCTDecode" ],
+            "/Height": 1520,
+            "/Length": 192956,
+            "/Subtype": "/Image",
+            "/Type": "/XObject",
+            "/Width": 1000
+          })
+        }
+      },
+      "/Type": "/Page"
+    })>
 
 repr() output
 -------------
 
 Let's observe the page's ``repr()`` output:
 
-.. ipython::
+.. doctest::
 
-    In [1]: repr(page1)
+    >>> repr(page1)
+    '<pikepdf.Page({\n  "/Contents": pikepdf.Stream(owner=<...>, data=b\'q\\n200.0000 0 0 304.0\'..., {\n    "/Length": 50\n  }),\n  "/MediaBox": [ 0, 0, 200, 304 ],\n  "/Parent": <reference to /Pages>,\n  "/Resources": {\n    "/XObject": {\n      "/Im0": pikepdf.Stream(owner=<...>, data=<...>, {\n        "/BitsPerComponent": 8,\n        "/ColorSpace": "/DeviceRGB",\n        "/Filter": [ "/DCTDecode" ],\n        "/Height": 1520,\n        "/Length": 192956,\n        "/Subtype": "/Image",\n        "/Type": "/XObject",\n        "/Width": 1000\n      })\n    }\n  },\n  "/Type": "/Page"\n})>'
 
 The angle brackets in the output indicate that this object cannot be constructed
 with a Python expression because it contains a reference. When angle brackets
 are omitted from the ``repr()`` of a pikepdf object, then the object can be
 replicated with a Python expression, such as ``eval(repr(x)) == x``. Pages
 typically have indirect references to themselves and other pages, so they
 cannot be represented as an expression.
 
 Item and attribute notation
 ---------------------------
 
 Dictionary keys may be looked up using attributes (``page1.Type``) or
 keys (``page1['/Type']``).
 
-.. ipython::
+.. doctest::
 
-    In [1]: page1.Type      # preferred notation for standard PDF names
+    >>> page1.Type      # preferred notation for standard PDF names
+    pikepdf.Name("/Page")
 
-    In [1]: page1['/Type']  # also works
+    >>> page1['/Type']  # also works
+    pikepdf.Name("/Page")
 
 By convention, pikepdf uses attribute notation for standard names (the names
 that are normally part of a dictionary, according to the |pdfrm|),
 and item notation for names that may not always appear. For example, the images
 belong to a page always appear at ``page.Resources.XObject`` but the names
 of images are arbitrarily chosen by whatever software generates the PDF (``/Im0``,
 in this case). (Whenever expressed as strings, names begin with ``/``.)
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: page1.Resources.XObject['/Im0']
+    >>> page1.Resources.XObject['/Im0']
 
 Item notation here would be quite cumbersome:
 ``['/Resources']['/XObject]['/Im0']`` (not recommended).
 
 Attribute notation is convenient, but not robust if elements are missing. For
 elements that are not always present, you can use ``.get()``, which behaves like
 ``dict.get()`` in core Python.  A library such as `glom
@@ -201,39 +232,39 @@
 are for. See :ref:`Working with pages <work_with_pages>` for details.)
 
 Deleting pages
 --------------
 
 Removing pages is easy too.
 
-.. ipython::
+.. doctest::
 
-    In [1]: del pdf.pages[1:3]  # Remove pages 2-3 labeled "second page" and "third page"
+    >>> del pdf.pages[1:3]  # Remove pages 2-3 labeled "second page" and "third page"
 
-.. ipython::
+.. doctest::
 
-    In [1]: len(pdf.pages)
+    >>> len(pdf.pages)
+    2
 
 Saving changes
 --------------
 
 .. figure:: /images/save-pike.jpg
    :align: right
    :alt: Sign that reads "Help the pike survive"
    :figwidth: 40%
 
    Saving pike.
 
 Naturally, you can save your changes with :meth:`pikepdf.Pdf.save`.
 ``filename`` can be a :class:`pathlib.Path`, which we accept everywhere.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: pdf.save('output.pdf')
+    >>> pdf.save('output.pdf')
 
 You may save a file multiple times, and you may continue modifying it after
 saving. For example, you could create an unencrypted version of document, then
 apply a watermark, and create an encrypted version.
 
 .. note::
 
@@ -247,46 +278,43 @@
 
 To save an encrypted (password protected) PDF, use a :class:`pikepdf.Encryption`
 object to specify the encryption settings. By default, pikepdf selects the
 strongest security handler and algorithm (AES-256), but allows full access to
 modify file contents. A :class:`pikepdf.Permissions` object can be used to
 specify restrictions.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: no_extracting = pikepdf.Permissions(extract=False)
+    >>> no_extracting = pikepdf.Permissions(extract=False)
 
-    In [1]: pdf.save('encrypted.pdf', encryption=pikepdf.Encryption(
-       ...:      user="user password", owner="owner password", allow=no_extracting
-       ...: ))
+    >>> pdf.save('encrypted.pdf', encryption=pikepdf.Encryption(
+    ...      user="user password", owner="owner password", allow=no_extracting
+    ... ))
 
 Refer to our :ref:`security documentation <security>` for more information on
 user/owner passwords and PDF permissions.
 
 Running QPDF through Jobs
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 pikepdf can access all of the features of the qpdf command line program, and
 can even execute qpdf-like command lines.
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: from pikepdf import Job
+    >>> from pikepdf import Job
 
-    In [1]: Job(['pikepdf', '--check', '../tests/resources/fourpages.pdf'])
+    >>> Job(['pikepdf', '--check', '../tests/resources/fourpages.pdf'])
 
 You can also specify jobs in QPDF Job JSON:
 
-.. ipython::
-    :verbatim:
+.. code-block:: python
 
-    In [1]: job_json = {'inputFile': '../tests/resources/fourpages.pdf', 'check': ''}
+    >>> job_json = {'inputFile': '../tests/resources/fourpages.pdf', 'check': ''}
 
-    In [1]: Job(job_json).run()
+    >>> Job(job_json).run()
 
 Next steps
 ----------
 
 Have a look at pikepdf topics that interest you, or jump to our detailed API
 reference...
```

### Comparing `pikepdf-8.8.0/pyproject.toml` & `pikepdf-8.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools >= 61", "wheel >= 0.37", "pybind11 >= 2.10.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pikepdf"
-version = "8.8.0"
+version = "8.9.0"
 description = "Read and write PDFs with Python, powered by qpdf"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["PDF"]
 authors = [{ name = "James R. Barlow", email = "james@purplerock.ca" }]
 license = { text = "MPL-2.0" }
 classifiers = [
@@ -32,32 +32,27 @@
 documentation = "https://pikepdf.readthedocs.io/"
 repository = "https://github.com/pikepdf/pikepdf"
 changelog = "https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html"
 
 [project.optional-dependencies]
 dev = ["pre-commit", "typer[all]"]
 docs = [
-  "GitPython",
-  "PyGithub",
   "Sphinx>=3",
-  "ipython",
-  "matplotlib",
-  "pybind11",
-  "requests",
+  "sphinx-autoapi",
   "sphinx-design",
   "sphinx-issues",
   "sphinx-rtd-theme",
   "tomli;python_version < '3.11'",
 ]
 mypy = ["lxml-stubs", "types-Pillow", "types-requests", "types-setuptools"]
 test = [
   "attrs>=20.2.0",
   "coverage[toml]",
   "hypothesis>=6.36",
-  "numpy>=1.21.0",
+  "numpy>=1.21.0; platform_machine == 'x86_64' or platform_python_implementation == 'CPython'",
   "psutil>=5.9; os_name != 'nt'",
   "pybind11",
   "pytest>=6.2.5",
   "pytest-cov>=3.0.0",
   "pytest-timeout>=2.1.0",
   "pytest-xdist>=2.5.0",
   "python-dateutil>=2.8.1",
@@ -163,15 +158,15 @@
 minversion = "6.0"
 norecursedirs = ["lib", ".pc", ".git", "venv"]
 testpaths = ["tests"]
 addopts = "-n auto"
 
 [tool.coverage.run]
 concurrency = ["multiprocessing"]
-omit = ["src/pikepdf/_qpdf.py"]  # Remove in pikepdf 9
+omit = ["src/pikepdf/_qpdf.py"]   # Remove in pikepdf 9
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_lines = [
   # Have to re-enable the standard pragma
   "pragma: no cover",
   # Don't complain if tests don't hit defensive assertion code:
```

### Comparing `pikepdf-8.8.0/setup.py` & `pikepdf-8.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/embeddedfiles.cpp` & `pikepdf-8.9.0/src/core/page.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,181 +1,193 @@
 // SPDX-FileCopyrightText: 2022 James R. Barlow
 // SPDX-License-Identifier: MPL-2.0
 
-#include <qpdf/Constants.h>
-#include <qpdf/Types.h>
-#include <qpdf/DLL.h>
-#include <qpdf/QPDFExc.hh>
-#include <qpdf/QPDFFileSpecObjectHelper.hh>
-#include <qpdf/QPDFEFStreamObjectHelper.hh>
-#include <qpdf/QPDFEmbeddedFileDocumentHelper.hh>
-
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
+#include <sstream>
+#include <iostream>
+#include <iomanip>
+#include <cctype>
 
 #include "pikepdf.h"
-#include "pipeline.h"
+#include "parsers.h"
+
+#include <qpdf/QPDFPageObjectHelper.hh>
+#include <qpdf/QPDFPageLabelDocumentHelper.hh>
+#include <qpdf/Pipeline.hh>
+#include <qpdf/Pl_Buffer.hh>
 
-void init_embeddedfiles(py::module_ &m)
+py::size_t page_index(QPDF &owner, QPDFObjectHandle page)
 {
-    py::class_<QPDFFileSpecObjectHelper,
-        std::shared_ptr<QPDFFileSpecObjectHelper>,
-        QPDFObjectHelper>(m, "AttachedFileSpec") // /Type /Filespec
-        .def(py::init([](QPDF &q,
-                          py::bytes data,
-                          std::string description,
-                          std::string filename,
-                          std::string mime_type,
-                          std::string creation_date,
-                          std::string mod_date,
-                          QPDFObjectHandle &relationship) {
-            auto efstream =
-                QPDFEFStreamObjectHelper::createEFStream(q, std::string(data));
-            auto filespec =
-                QPDFFileSpecObjectHelper::createFileSpec(q, filename, efstream);
-
-            if (!description.empty())
-                filespec.setDescription(description);
-            if (!mime_type.empty())
-                efstream.setSubtype(mime_type);
-            if (!creation_date.empty())
-                efstream.setCreationDate(creation_date);
-            if (!mod_date.empty())
-                efstream.setModDate(mod_date);
-
-            if (relationship.isName()) {
-                filespec.getObjectHandle().replaceKey("/AFRelationship", relationship);
-            }
-
-            return filespec;
-        }),
-            py::keep_alive<0, 1>(), // LCOV_EXCL_LINE
-            py::arg("q"),
-            py::arg("data"),
-            py::kw_only(), // LCOV_EXCL_LINE
-            py::arg("description")   = std::string(""),
-            py::arg("filename")      = std::string(""),
-            py::arg("mime_type")     = std::string(""),
-            py::arg("creation_date") = std::string(""),
-            py::arg("mod_date")      = std::string(""),
-            py::arg("relationship")  = QPDFObjectHandle::newName("/Unspecified"),
-            R"~~~(
-            Construct a attached file spec from data in memory.
-
-            To construct a file spec from a file on the computer's file system,
-            use :meth:`from_filepath`.
-
-            Args:
-                data: Resource to load.
-                description: Any description text for the attachment. May be
-                    shown in PDF viewers.
-                filename: Filename to display in PDF viewers.
-                mime_type: Helps PDF viewers decide how to display the information.
-                creation_date: PDF date string for when this file was created.
-                mod_date: PDF date string for when this file was last modified.
-                relationship: A :class:`pikepdf.Name` indicating the relationship
-                    of this file to the document. Canonically, this should be a name
-                    from the PDF specification:
-                    Source, Data, Alternative, Supplement, EncryptedPayload, FormData,
-                    Schema, Unspecified. If omitted, Unspecified is used.
-            )~~~")
-        .def_property("description",
-            &QPDFFileSpecObjectHelper::getDescription,
-            &QPDFFileSpecObjectHelper::setDescription, // LCOV_EXCL_LINE
-            "Description text associated with the embedded file.")
-        .def_property(
-            "filename",
-            [](QPDFFileSpecObjectHelper &spec) { return spec.getFilename(); },
-            [](QPDFFileSpecObjectHelper &spec, std::string const &value) {
-                spec.setFilename(value);
-            },
-            R"~~~(
-            The main filename for this file spec.
-
-            In priority order, getting this returns the first of /UF, /F, /Unix,
-            /DOS, /Mac if multiple filenames are set. Setting this will set a UTF-8
-            encoded Unicode filename and write it to /UF.
-            )~~~")
-        .def(
-            "get_all_filenames",
-            [](QPDFFileSpecObjectHelper &spec) -> py::dict {
-                auto filenames = spec.getFilenames();
-                py::dict result;
-                for (auto key_filename : filenames) {
-                    auto key                      = key_filename.first;
-                    auto filename                 = key_filename.second;
-                    auto key_as_name              = QPDFObjectHandle::newName(key);
-                    result[py::cast(key_as_name)] = py::bytes(filename);
+    if (&owner != page.getOwningQPDF())
+        throw py::value_error("Page is not in this Pdf");
+
+    int idx;
+    try {
+        idx = owner.findPage(page);
+    } catch (const QPDFExc &e) {
+        if (std::string(e.what()).find("page object not referenced") >= 0)
+            throw py::value_error("Page is not consistently registered with Pdf");
+        throw e;
+    }
+    if (idx < 0) {
+        // LCOV_EXCL_START
+        throw std::logic_error("Page index is negative");
+        // LCOV_EXCL_STOP
+    }
+
+    return idx;
+}
+
+std::string label_string_from_dict(QPDFObjectHandle label_dict)
+{
+    auto impl =
+        py::module_::import("pikepdf._cpphelpers").attr("label_from_label_dict");
+    py::str result = impl(label_dict);
+    return result;
+}
+
+void init_page(py::module_ &m)
+{
+    py::class_<QPDFPageObjectHelper,
+        std::shared_ptr<QPDFPageObjectHelper>,
+        QPDFObjectHelper>(m, "Page")
+        .def(py::init<QPDFObjectHandle &>())
+        .def(py::init([](QPDFPageObjectHelper &poh) {
+            return QPDFPageObjectHelper(poh.getObjectHandle());
+        }))
+        .def(
+            "__copy__", [](QPDFPageObjectHelper &poh) { return poh.shallowCopyPage(); })
+        .def_property_readonly("_images", &QPDFPageObjectHelper::getImages)
+        .def_property_readonly("_form_xobjects", &QPDFPageObjectHelper::getFormXObjects)
+        .def("_get_mediabox", &QPDFPageObjectHelper::getMediaBox)
+        .def("_get_artbox", &QPDFPageObjectHelper::getArtBox)
+        .def("_get_bleedbox", &QPDFPageObjectHelper::getBleedBox)
+        .def("_get_cropbox", &QPDFPageObjectHelper::getCropBox)
+        .def("_get_trimbox", &QPDFPageObjectHelper::getTrimBox)
+        .def(
+            "externalize_inline_images",
+            [](QPDFPageObjectHelper &poh, size_t min_size = 0, bool shallow = false) {
+                return poh.externalizeInlineImages(min_size, shallow);
+            },
+            py::arg("min_size") = 0,
+            py::arg("shallow")  = false)
+        .def("rotate",
+            &QPDFPageObjectHelper::rotatePage,
+            py::arg("angle"),
+            py::arg("relative"))
+        .def("contents_coalesce",
+            &QPDFPageObjectHelper::coalesceContentStreams // LCOV_EXCL_LINE
+            )
+        .def(
+            "_contents_add",
+            [](QPDFPageObjectHelper &poh, QPDFObjectHandle &contents, bool prepend) {
+                return poh.addPageContents(contents, prepend);
+            },
+            py::arg("contents"), // LCOV_EXCL_LINE
+            py::kw_only(),
+            py::arg("prepend") = false)
+        .def(
+            "_contents_add",
+            [](QPDFPageObjectHelper &poh, py::bytes contents, bool prepend) {
+                auto q = poh.getObjectHandle().getOwningQPDF();
+                if (!q) {
+                    // LCOV_EXCL_START
+                    throw std::logic_error("QPDFPageObjectHelper not attached to QPDF");
+                    // LCOV_EXCL_STOP
                 }
-                return result;
+                auto stream = QPDFObjectHandle::newStream(q, contents);
+                return poh.addPageContents(stream, prepend);
             },
-            R"~~~(
-            Return a Python dictionary that describes all filenames.
-
-            The returned dictionary is not a pikepdf Object.
+            py::arg("contents"),
+            py::kw_only(),
+            py::arg("prepend") = false)
+        .def("remove_unreferenced_resources",
+            &QPDFPageObjectHelper::removeUnreferencedResources // LCOV_EXCL_LINE
+            )
+        .def("as_form_xobject",
+            &QPDFPageObjectHelper::getFormXObjectForPage, // LCOV_EXCL_LINE
+            py::arg("handle_transformations") = true)
+        .def(
+            "calc_form_xobject_placement",
+            [](QPDFPageObjectHelper &poh,
+                QPDFObjectHandle formx,
+                QPDFObjectHandle name,
+                QPDFObjectHandle::Rectangle rect,
+                bool invert_transformations,
+                bool allow_shrink,
+                bool allow_expand) -> py::bytes {
+                return py::bytes(poh.placeFormXObject(formx,
+                    name.getName(),
+                    rect,
+                    invert_transformations,
+                    allow_shrink,
+                    allow_expand));
+            },
+            py::arg("formx"), // LCOV_EXCL_LINE
+            py::arg("name"),
+            py::arg("rect"),
+            py::kw_only(), // LCOV_EXCL_LINE
+            py::arg("invert_transformations") = true,
+            py::arg("allow_shrink")           = true,
+            py::arg("allow_expand")           = false)
+        .def(
+            "get_filtered_contents",
+            [](QPDFPageObjectHelper &poh,
+                QPDFObjectHandle::TokenFilter &tf) -> py::bytes {
+                Pl_Buffer pl_buffer("filter_page");
+                poh.filterContents(&tf, &pl_buffer);
+
+                // Hold .getBuffer in unique_ptr to ensure it is deleted.
+                // QPDF makes a copy and expects us to delete it.
+                std::unique_ptr<Buffer> buf(pl_buffer.getBuffer());
+                auto data = reinterpret_cast<const char *>(buf->getBuffer());
+                auto size = buf->getSize();
+                return py::bytes(data, size);
+            },
+            py::arg("tf") // LCOV_EXCL_LINE
+            )
+        .def(
+            "add_content_token_filter",
+            [](QPDFPageObjectHelper &poh,
+                std::shared_ptr<QPDFObjectHandle::TokenFilter> tf) {
+                // TokenFilters may be processed after the Python objects have gone
+                // out of scope, so we need to keep them alive by attaching them to
+                // the corresponding QPDF object.
+                // Standard py::keep_alive<> won't cut it. We could make this
+                // function require a Pdf, or move it to the Pdf.
+                auto pyqpdf = py::cast(poh.getObjectHandle().getOwningQPDF());
+                auto pytf   = py::cast(tf);
+                py::detail::keep_alive_impl(pyqpdf, pytf);
 
-            Multiple filenames are generally a holdover from the pre-Unicode era.
-            Modern PDFs can generally set UTF-8 filenames and avoid using
-            punctuation or other marks that are forbidden in filenames.
-            )~~~")
-        .def(
-            "get_file",
-            [](QPDFFileSpecObjectHelper &spec) {
-                return QPDFEFStreamObjectHelper(spec.getEmbeddedFileStream());
-            },
-            py::return_value_policy::reference_internal,
-            R"~~~(
-            Return the primary (usually only) attached file.
-            )~~~")
-        .def(
-            "get_file",
-            [](QPDFFileSpecObjectHelper &spec, QPDFObjectHandle &name) {
-                if (!name.isName())
-                    throw py::type_error("Argument must be a pikepdf.Name");
-                return QPDFEFStreamObjectHelper(
-                    spec.getEmbeddedFileStream(name.getName()));
-            },
-            py::return_value_policy::reference_internal,
-            R"~~~(
-            Return an attached file selected by :class:`pikepdf.Name`.
-
-            Typical names would be ``/UF`` and ``/F``. See |pdfrm| for other obsolete
-            names.
-            )~~~");
-
-    py::class_<QPDFEFStreamObjectHelper,
-        std::shared_ptr<QPDFEFStreamObjectHelper>,
-        QPDFObjectHelper>(m, "AttachedFile") // /Type /EmbeddedFile
-        .def_property_readonly("size",
-            &QPDFEFStreamObjectHelper::getSize, // LCOV_EXCL_LINE
-            "Get length of the attached file in bytes according to the PDF creator.")
-        .def_property("mime_type",
-            &QPDFEFStreamObjectHelper::getSubtype,
-            &QPDFEFStreamObjectHelper::setSubtype, // LCOV_EXCL_LINE
-            "Get the MIME type of the attached file according to the PDF creator.")
-        .def_property_readonly(
-            "md5",
-            [](QPDFEFStreamObjectHelper &efstream) {
-                return py::bytes(efstream.getChecksum());
-            },
-            "Get the MD5 checksum of the attached file according to the PDF creator.")
-        .def_property("_creation_date",
-            &QPDFEFStreamObjectHelper::getCreationDate,
-            &QPDFEFStreamObjectHelper::setCreationDate)
-        .def_property("_mod_date",
-            &QPDFEFStreamObjectHelper::getModDate,
-            &QPDFEFStreamObjectHelper::setModDate);
-
-    py::class_<QPDFEmbeddedFileDocumentHelper>(m, "Attachments")
-        .def_property_readonly(
-            "_has_embedded_files", &QPDFEmbeddedFileDocumentHelper::hasEmbeddedFiles)
-        .def("_get_all_filespecs",
-            &QPDFEmbeddedFileDocumentHelper::getEmbeddedFiles,
-            py::return_value_policy::reference_internal)
-        .def("_get_filespec",
-            &QPDFEmbeddedFileDocumentHelper::getEmbeddedFile,
-            py::return_value_policy::reference_internal)
-        .def("_add_replace_filespec",
-            &QPDFEmbeddedFileDocumentHelper::replaceEmbeddedFile,
-            py::keep_alive<0, 2>())
-        .def("_remove_filespec", &QPDFEmbeddedFileDocumentHelper::removeEmbeddedFile);
-}
+                poh.addContentTokenFilter(tf);
+            },
+            py::arg("tf"))
+        .def(
+            "parse_contents",
+            [](QPDFPageObjectHelper &poh, PyParserCallbacks &stream_parser) {
+                poh.parseContents(&stream_parser);
+            },
+            py::arg("stream_parser"))
+        .def_property_readonly("index",
+            [](QPDFPageObjectHelper &poh) {
+                auto this_page = poh.getObjectHandle();
+                auto p_owner   = this_page.getOwningQPDF();
+                if (!p_owner)
+                    throw py::value_error("Page is not attached to a Pdf");
+                auto &owner = *p_owner;
+                return page_index(owner, this_page);
+            })
+        .def_property_readonly("label", [](QPDFPageObjectHelper &poh) {
+            auto this_page = poh.getObjectHandle();
+            auto p_owner   = this_page.getOwningQPDF();
+            if (!p_owner)
+                throw py::value_error("Page is not attached to a Pdf");
+            auto &owner = *p_owner;
+            auto index  = page_index(owner, this_page);
+
+            QPDFPageLabelDocumentHelper pldh(owner);
+            auto label_dict = pldh.getLabelForPage(index);
+            if (label_dict.isNull())
+                return std::to_string(index + 1);
+
+            return label_string_from_dict(label_dict);
+        });
+}
```

### Comparing `pikepdf-8.8.0/src/core/jbig2-inl.h` & `pikepdf-8.9.0/src/core/jbig2-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/logger.cpp` & `pikepdf-8.9.0/src/core/logger.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/mmap_inputsource-inl.h` & `pikepdf-8.9.0/src/core/mmap_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/nametree.cpp` & `pikepdf-8.9.0/src/core/nametree.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -31,31 +31,16 @@
             "new",
             [](QPDF &pdf, bool auto_repair = true) {
                 return NameTree::newEmpty(pdf, auto_repair);
             },
             py::arg("pdf"), // LCOV_EXCL_LINE
             py::kw_only(),
             py::arg("auto_repair") = true,
-            py::keep_alive<0, 1>(),
-            R"~~~(
-                Create a new NameTree in the provided Pdf.
-
-                You will probably need to insert the name tree in the PDF's
-                catalog. For example, to insert this name tree in
-                /Root /Names /Dests:
-
-                .. code-block:: python
-
-                    nt = NameTree.new(pdf)
-                    pdf.Root.Names.Dests = nt.obj
-            )~~~")
-        .def_property_readonly(
-            "obj",
-            [](NameTree &nt) { return nt.getObjectHandle(); },
-            "Returns the underlying root object for this name tree.")
+            py::keep_alive<0, 1>())
+        .def_property_readonly("obj", [](NameTree &nt) { return nt.getObjectHandle(); })
         .def(
             "__eq__",
             [](NameTree &self, NameTree &other) {
                 return objecthandle_equal(
                     self.getObjectHandle(), other.getObjectHandle());
             },
             py::is_operator())
```

### Comparing `pikepdf-8.8.0/src/core/numbertree.cpp` & `pikepdf-8.9.0/src/core/numbertree.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -34,27 +34,15 @@
             "new",
             [](QPDF &pdf, bool auto_repair = true) {
                 return NumberTree::newEmpty(pdf, auto_repair);
             },
             py::arg("pdf"), // LCOV_EXCL_LINE
             py::kw_only(),
             py::arg("auto_repair") = true,
-            py::keep_alive<0, 1>(),
-            R"~~~(
-                Create a new NumberTree in the provided Pdf.
-
-                You will probably need to insert the number tree in the PDF's
-                catalog. For example, to insert this number tree in 
-                /Root /PageLabels:
-
-                .. code-block:: python
-
-                    nt = NumberTree.new(pdf)
-                    pdf.Root.PageLabels = nt.obj
-            )~~~")
+            py::keep_alive<0, 1>())
         .def("__contains__",
             [](NumberTree &nt, numtree_number idx) { return nt.hasIndex(idx); })
         .def("__contains__", [](NumberTree &nt, py::object idx) { return false; })
         .def("__getitem__",
             [](NumberTree &nt, numtree_number key) {
                 QPDFObjectHandle oh;
                 if (nt.findObject(key, oh)) // writes to 'oh'
```

### Comparing `pikepdf-8.8.0/src/core/object.cpp` & `pikepdf-8.9.0/src/core/object.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -322,53 +322,35 @@
         .def_property_readonly("_type_code", &QPDFObjectHandle::getTypeCode)
         .def_property_readonly("_type_name", &QPDFObjectHandle::getTypeName)
         .def(
             "is_owned_by",
             [](QPDFObjectHandle &h, QPDF &possible_owner) {
                 return (h.getOwningQPDF() == &possible_owner);
             },
-            "Test if this object is owned by the indicated *possible_owner*.",
             py::arg("possible_owner"))
-        .def(
-            "same_owner_as",
+        .def("same_owner_as",
             [](QPDFObjectHandle &self, QPDFObjectHandle &other) {
                 return self.getOwningQPDF() == other.getOwningQPDF();
-            },
-            "Test if two objects are owned by the same :class:`pikepdf.Pdf`.")
-        .def(
-            "with_same_owner_as",
+            })
+        .def("with_same_owner_as",
             [](QPDFObjectHandle &self, QPDFObjectHandle &other) {
                 QPDF *self_owner  = self.getOwningQPDF();
                 QPDF *other_owner = other.getOwningQPDF();
 
                 if (self_owner == other_owner)
                     return self;
                 if (!other_owner)
                     throw py::value_error(
                         "with_same_owner_as() called for object that has no owner");
                 if (!self.isIndirect())
                     return other_owner->makeIndirectObject(self);
 
                 auto self_in_other = other_owner->copyForeignObject(self);
                 return self_in_other;
-            },
-            R"~~~(
-                Returns an object that is owned by the same Pdf that owns the *other* object.
-
-                If the objects already have the same owner, this object is returned.
-                If the *other* object has a different owner, then a copy is created
-                that is owned by *other*'s owner. If this object is a direct object
-                (no owner), then an indirect object is created that is owned by
-                *other*. An exception is thrown if *other* is a direct object.
-
-                This method may be convenient when a reference to the Pdf is not
-                available.
-
-                .. versionadded:: 2.14
-            )~~~")
+            })
         .def_property_readonly("is_indirect", &QPDFObjectHandle::isIndirect)
         .def("__repr__", &objecthandle_repr)
         .def("__hash__",
             [](QPDFObjectHandle &self) -> py::int_ {
                 // Objects which compare equal must have the same hash value
                 switch (self.getTypeCode()) {
                 case qpdf_object_type_e::ot_string:
@@ -499,48 +481,39 @@
             [](QPDFObjectHandle &h, std::string const &key) {
                 return object_get_key(h, key);
             })
         .def("__getitem__",
             [](QPDFObjectHandle &h, QPDFObjectHandle &name) {
                 return object_get_key(h, name.getName());
             })
-        .def(
-            "__setitem__",
+        .def("__setitem__",
             [](QPDFObjectHandle &h, std::string const &key, QPDFObjectHandle &value) {
                 object_set_key(h, key, value);
-            },
-            "assign dictionary key to new object")
-        .def(
-            "__setitem__",
+            })
+        .def("__setitem__",
             [](QPDFObjectHandle &h, QPDFObjectHandle &name, QPDFObjectHandle &value) {
                 object_set_key(h, name.getName(), value);
-            },
-            "assign dictionary key to new object")
+            })
         .def("__setitem__",
             [](QPDFObjectHandle &h, std::string const &key, py::object pyvalue) {
                 auto value = objecthandle_encode(pyvalue);
                 object_set_key(h, key, value);
             })
         .def("__setitem__",
             [](QPDFObjectHandle &h, QPDFObjectHandle &name, py::object pyvalue) {
                 auto value = objecthandle_encode(pyvalue);
                 object_set_key(h, name.getName(), value);
             })
-        .def(
-            "__delitem__",
-            [](QPDFObjectHandle &h, std::string const &key) { object_del_key(h, key); },
-            "delete a dictionary key")
-        .def(
-            "__delitem__",
+        .def("__delitem__",
+            [](QPDFObjectHandle &h, std::string const &key) { object_del_key(h, key); })
+        .def("__delitem__",
             [](QPDFObjectHandle &h, QPDFObjectHandle &name) {
                 object_del_key(h, name.getName());
-            },
-            "delete a dictionary key")
-        .def(
-            "__getattr__",
+            })
+        .def("__getattr__",
             [](QPDFObjectHandle &h, std::string const &name) {
                 QPDFObjectHandle value;
                 std::string key = "/" + name;
                 try {
                     value = object_get_key(h, key);
                 } catch (const py::key_error &e) {
                     if (std::isupper(name[0]))
@@ -549,37 +522,33 @@
                         throw py::attribute_error(name);
                 } catch (const py::value_error &e) {
                     if (name == std::string("__name__"))
                         throw py::attribute_error(name);
                     throw;
                 }
                 return value;
-            },
-            "attribute lookup name")
+            })
         .def_property("stream_dict",
             &QPDFObjectHandle::getDict,
             &QPDFObjectHandle::replaceDict,
-            "Access the dictionary key-values for a :class:`pikepdf.Stream`.",
             py::return_value_policy::reference_internal)
-        .def(
-            "__setattr__",
+        .def("__setattr__",
             [](QPDFObjectHandle &h, std::string const &name, py::object pyvalue) {
                 if (h.isDictionary() || (h.isStream() && name != "stream_dict")) {
                     // Map attribute assignment to setting dictionary key
                     std::string key = "/" + name;
                     auto value      = objecthandle_encode(pyvalue);
                     object_set_key(h, key, value);
                     return;
                 }
 
                 // If we don't have a special rule, do object.__setattr__()
                 py::object baseobj = py::module_::import("builtins").attr("object");
                 baseobj.attr("__setattr__")(py::cast(h), py::str(name), pyvalue);
-            },
-            "attribute access")
+            })
         .def("__delattr__",
             [](QPDFObjectHandle &h, std::string const &name) {
                 std::string key = "/" + name;
                 object_del_key(h, key);
             })
         .def("__dir__",
             [](QPDFObjectHandle &h) {
@@ -605,42 +574,35 @@
                 try {
                     value = object_get_key(h, key);
                 } catch (const py::key_error &) {
                     return default_;
                 }
                 return py::cast(value);
             },
-            "For ``pikepdf.Dictionary`` or ``pikepdf.Stream`` objects, behave as "
-            "``dict.get(key, default=None)``",
             py::arg("key"),
             py::arg("default") = py::none())
         .def(
             "get",
             [](QPDFObjectHandle &h, QPDFObjectHandle &name, py::object default_) {
                 QPDFObjectHandle value;
                 try {
                     value = object_get_key(h, name.getName());
                 } catch (const py::key_error &) {
                     return default_;
                 }
                 return py::cast(value);
             },
-            "For ``pikepdf.Dictionary`` or ``pikepdf.Stream`` objects, behave as "
-            "``dict.get(key, default=None)``",
             py::arg("key"),
             py::arg("default") = py::none())
-        .def(
-            "keys",
+        .def("keys",
             [](QPDFObjectHandle &h) {
                 if (h.isStream())
                     return h.getDict().getKeys();
                 return h.getKeys();
-            },
-            "For ``pikepdf.Dictionary`` or ``pikepdf.Stream`` objects, obtain the "
-            "keys.")
+            })
         .def("__contains__",
             [](QPDFObjectHandle &h, QPDFObjectHandle &key) {
                 if (h.isArray()) {
                     return array_has_item(h, key);
                 }
                 if (!key.isName())
                     throw py::type_error("Dictionaries can only contain Names");
@@ -736,105 +698,73 @@
                 h.setArrayItem(u_index, value);
             })
         .def("__delitem__",
             [](QPDFObjectHandle &h, int index) {
                 auto u_index = list_range_check(h, index);
                 h.eraseItem(u_index);
             })
-        .def(
-            "wrap_in_array",
-            [](QPDFObjectHandle &h) { return h.wrapInArray(); },
-            "Return the object wrapped in an array if not already an array.")
-        .def(
-            "append",
+        .def("wrap_in_array", [](QPDFObjectHandle &h) { return h.wrapInArray(); })
+        .def("append",
             [](QPDFObjectHandle &h, py::object pyitem) {
                 auto item = objecthandle_encode(pyitem);
                 return h.appendItem(item);
-            },
-            "Append another object to an array; fails if the object is not an array.")
-        .def(
-            "extend",
+            })
+        .def("extend",
             [](QPDFObjectHandle &h, py::iterable iter) {
                 for (auto item : iter) {
                     h.appendItem(objecthandle_encode(item));
                 }
-            },
-            "Extend a pikepdf.Array with an iterable of other objects.")
+            })
         .def_property_readonly("is_rectangle",
-            &QPDFObjectHandle::isRectangle, // LCOV_EXCL_LINE
-            "Returns True if the object is a rectangle (an array of 4 numbers)")
+            &QPDFObjectHandle::isRectangle // LCOV_EXCL_LINE
+            )
         .def(
             "get_stream_buffer",
             [](QPDFObjectHandle &h, qpdf_stream_decode_level_e decode_level) {
                 return get_stream_data(h, decode_level);
             },
-            "Return a buffer protocol buffer describing the decoded stream.",
             py::arg("decode_level") = qpdf_dl_generalized)
-        .def(
-            "get_raw_stream_buffer",
-            [](QPDFObjectHandle &h) { return h.getRawStreamData(); },
-            "Return a buffer protocol buffer describing the raw, encoded stream")
+        .def("get_raw_stream_buffer",
+            [](QPDFObjectHandle &h) { return h.getRawStreamData(); })
         .def(
             "read_bytes",
             [](QPDFObjectHandle &h, qpdf_stream_decode_level_e decode_level) {
                 auto buf = get_stream_data(h, decode_level);
                 return py::bytes((const char *)buf->getBuffer(), buf->getSize());
             },
-            "Decode and read the content stream associated with this object.",
             py::arg("decode_level") = qpdf_dl_generalized)
-        .def(
-            "read_raw_bytes",
+        .def("read_raw_bytes",
             [](QPDFObjectHandle &h) {
                 auto buf = h.getRawStreamData();
                 // py::bytes will make a copy of the buffer, so releasing is fine
                 return py::bytes((const char *)buf->getBuffer(), buf->getSize());
-            },
-            "Read the content stream associated with this object without decoding")
+            })
         .def(
             "_write",
             [](QPDFObjectHandle &h,
                 py::bytes data,
                 py::object filter,
                 py::object decode_parms) {
                 std::string sdata               = data;
                 QPDFObjectHandle h_filter       = objecthandle_encode(filter);
                 QPDFObjectHandle h_decode_parms = objecthandle_encode(decode_parms);
                 h.replaceStreamData(sdata, h_filter, h_decode_parms);
             },
-            R"~~~(
-            Low level write/replace stream data without argument checking. Use .write().
-            )~~~",
             py::arg("data"),
             py::arg("filter"),
             py::arg("decode_parms"))
         .def("_inline_image_raw_bytes",
             [](QPDFObjectHandle &h) { return py::bytes(h.getInlineImageValue()); })
         .def_property_readonly("_objgen", &object_get_objgen)
-        .def_property_readonly("objgen",
-            &object_get_objgen,
-            R"~~~(
-            Return the object-generation number pair for this object.
-
-            If this is a direct object, then the returned value is ``(0, 0)``.
-            By definition, if this is an indirect object, it has a "objgen",
-            and can be looked up using this in the cross-reference (xref) table.
-            Direct objects cannot necessarily be looked up.
-
-            The generation number is usually 0, except for PDFs that have been
-            incrementally updated. Incrementally updated PDFs are now uncommon,
-            since it does not take too long for modern CPUs to reconstruct an
-            entire PDF. pikepdf will consolidate all incremental updates
-            when saving.
-            )~~~")
+        .def_property_readonly("objgen", &object_get_objgen)
         .def_static(
             "parse",
             [](std::string const &stream, std::string const &description) {
                 return QPDFObjectHandle::parse(stream, description);
             },
-            "Parse PDF binary representation into PDF objects.",
             py::arg("stream"),
             py::arg("description") = "")
         .def("_parse_page_contents",
             &QPDFObjectHandle::parsePageContents,
             "Helper for parsing page contents; use ``pikepdf.parse_content_stream``.")
         .def("_parse_page_contents_grouped",
             [](QPDFObjectHandle &h, std::string const &whitelist) {
@@ -858,201 +788,92 @@
         .def(
             "unparse",
             [](QPDFObjectHandle &h, bool resolved) -> py::bytes {
                 if (resolved)
                     return h.unparseResolved();
                 return h.unparse();
             },
-            py::arg("resolved") = false,
-            R"~~~(
-            Convert PDF objects into their binary representation, optionally
-            resolving indirect objects.
-
-            If you want to unparse content streams, which are a collection of
-            objects that need special treatment, use
-            :func:`pikepdf.unparse_content_stream` instead.
-
-            Returns ``bytes()`` that can be used with :meth:`Object.parse`
-            to reconstruct the ``pikepdf.Object``. If reconstruction is not possible,
-            a relative object reference is returned, such as ``4 0 R``.
-
-            Args:
-                resolved: If True, deference indirect objects where possible.
-            )~~~")
+            py::arg("resolved") = false)
         .def(
             "to_json",
             [](QPDFObjectHandle &h,
                 bool dereference   = false,
                 int schema_version = 2) -> py::bytes {
                 return h.getJSON(schema_version, dereference).unparse();
             },
             py::arg("dereference")    = false,
-            py::arg("schema_version") = 2,
-            R"~~~(
-            Convert to a QPDF JSON representation of the object.
-
-            See the QPDF manual for a description of its JSON representation.
-            https://qpdf.readthedocs.io/en/stable/json.html#qpdf-json-format
+            py::arg("schema_version") = 2); // end of QPDFObjectHandle bindings
 
-            Not necessarily compatible with other PDF-JSON representations that
-            exist in the wild.
-
-            * Names are encoded as UTF-8 strings
-            * Indirect references are encoded as strings containing ``obj gen R``
-            * Strings are encoded as UTF-8 strings with unrepresentable binary
-              characters encoded as ``\uHHHH``
-            * Encoding streams just encodes the stream's dictionary; the stream
-              data is not represented
-            * Object types that are only valid in content streams (inline
-              image, operator) as well as "reserved" objects are not
-              representable and will be serialized as ``null``.
-
-            Args:
-                dereference (bool): If True, dereference the object if this is an
-                    indirect object.
-                schema_version (int): The version of the JSON schema. Defaults to 2.
-
-            Returns:
-                JSON bytestring of object. The object is UTF-8 encoded
-                and may be decoded to a Python str that represents the binary
-                values ``\x00-\xFF`` as ``U+0000`` to ``U+00FF``; that is,
-                it may contain mojibake.
-
-            .. versionchanged:: 6.0
-                Added *schema_version*.
-            )~~~"); // end of QPDFObjectHandle bindings
-
-    m.def("_new_boolean", &QPDFObjectHandle::newBool, "Construct a PDF Boolean object");
-    m.def("_new_integer",
-        &QPDFObjectHandle::newInteger,
-        "Construct a PDF Integer object");
-    m.def(
-        "_new_real",
-        [](const std::string &value) { return QPDFObjectHandle::newReal(value); },
-        "Construct a PDF Real value, that is, a decimal number");
+    m.def("_new_boolean", &QPDFObjectHandle::newBool);
+    m.def("_new_integer", &QPDFObjectHandle::newInteger);
+    m.def("_new_real",
+        [](const std::string &value) { return QPDFObjectHandle::newReal(value); });
     m.def(
         "_new_real",
         [](double value, uint places) {
             return QPDFObjectHandle::newReal(value, places);
         },
-        "Construct PDF real",
         py::arg("value"),
         py::arg("places") = 0);
-    m.def(
-        "_new_name",
-        [](const std::string &s) {
-            if (s.length() < 2)
-                throw py::value_error("Name must be at least one character long");
-            if (s.at(0) != '/')
-                throw py::value_error("Name objects must begin with '/'");
-            return QPDFObjectHandle::newName(s);
-        },
-        "Create a Name from a string. Must begin with '/'. All other characters "
-        "except null are valid.");
-    m.def(
-        "_new_string",
-        [](const std::string &s) { return QPDFObjectHandle::newString(s); },
-        "Construct a PDF String object.");
-    m.def(
-        "_new_string_utf8",
-        [](const std::string &utf8) {
-            return QPDFObjectHandle::newUnicodeString(utf8);
-        },
-        "Construct a PDF String object from UTF-8 bytes.");
-    m.def(
-        "_new_array",
-        [](py::iterable iterable) {
-            return QPDFObjectHandle::newArray(array_builder(iterable));
-        },
-        "Construct a PDF Array object from an iterable of PDF objects or types "
-        "that can be coerced to PDF objects.");
-    m.def(
-        "_new_dictionary",
-        [](py::dict dict) {
-            return QPDFObjectHandle::newDictionary(dict_builder(dict));
-        },
-        "Construct a PDF Dictionary from a mapping of PDF objects or Python types "
-        "that can be coerced to PDF objects.");
-    m.def(
-        "_new_stream",
-        [](QPDF &owner, py::bytes data) {
-            // This makes a copy of the data
-            return QPDFObjectHandle::newStream(&owner, data);
-        },
-        "Construct a PDF Stream object from binary data");
+    m.def("_new_name", [](const std::string &s) {
+        if (s.length() < 2)
+            throw py::value_error("Name must be at least one character long");
+        if (s.at(0) != '/')
+            throw py::value_error("Name objects must begin with '/'");
+        return QPDFObjectHandle::newName(s);
+    });
+    m.def("_new_string",
+        [](const std::string &s) { return QPDFObjectHandle::newString(s); });
+    m.def("_new_string_utf8", [](const std::string &utf8) {
+        return QPDFObjectHandle::newUnicodeString(utf8);
+    });
+    m.def("_new_array", [](py::iterable iterable) {
+        return QPDFObjectHandle::newArray(array_builder(iterable));
+    });
+    m.def("_new_dictionary", [](py::dict dict) {
+        return QPDFObjectHandle::newDictionary(dict_builder(dict));
+    });
+    m.def("_new_stream", [](QPDF &owner, py::bytes data) {
+        // This makes a copy of the data
+        return QPDFObjectHandle::newStream(&owner, data);
+    });
     m.def(
         "_new_operator",
         [](const std::string &op) { return QPDFObjectHandle::newOperator(op); },
-        "Construct a PDF Operator object for use in content streams.",
         py::arg("op"));
     m.def("_Null", &QPDFObjectHandle::newNull, "Construct a PDF Null object");
 
-    py::class_<QPDFObjectHandle::ParserCallbacks, PyParserCallbacks>(m,
-        "StreamParser",
-        R"~~~(
-            A simple content stream parser, which must be subclassed to be used.
-
-            In practice, the performance of this class may be quite poor on long
-            content streams because it creates objects and involves multiple
-            function calls for every object in a content stream, some of which
-            may be only a single byte long.
-
-            Consider instead using :func:`pikepdf.parse_content_stream`.
-        )~~~")
+    py::class_<QPDFObjectHandle::ParserCallbacks, PyParserCallbacks>(m, "StreamParser")
         .def(py::init<>(), "You must call ``super.__init__()`` in subclasses.")
         // LCOV_EXCL_START
         // coverage misses the virtual function call ::handleObject here.
-        .def(
-            "handle_object",
+        .def("handle_object",
             [](QPDFObjectHandle::ParserCallbacks &parsercallbacks,
                 QPDFObjectHandle &h,
                 size_t offset,
-                size_t length) { parsercallbacks.handleObject(h, offset, length); },
-            R"~~~(
-                This is an abstract method that must be overloaded in a subclass.
-
-                This function will be called back once for each object that is
-                parsed in the content stream.
-            )~~~")
+                size_t length) { parsercallbacks.handleObject(h, offset, length); })
         // LCOV_EXCL_STOP
-        .def("handle_eof",
-            &QPDFObjectHandle::ParserCallbacks::handleEOF,
-            R"~~~(
-                This is an abstract method that may be overloaded in a subclass.
-
-                Called at the end of a content stream.
-            )~~~");
+        .def("handle_eof", &QPDFObjectHandle::ParserCallbacks::handleEOF);
 
     // Since QPDFEmbeddedFileDocumentHelper::getEmbeddedFiles returns
     // std::map<std::string, std::shared_ptr<QPDFFileSpecObjectHelper>>
     // we must ensure that the entire QPDFObjectHelper type hierarchy is held in
     // std::shared_ptr or repackage that interface so it does not return a
     // std::shared_ptr<QPDFFileSpecObjectHelper>> to Python.
-    py::class_<QPDFObjectHelper, std::shared_ptr<QPDFObjectHelper>>(m,
-        "ObjectHelper",
-        R"~~~(
-            Base class for wrapper/helper around an Object.
-
-            Used to expose additional functionality specific to that object type.
-        )~~~")
+    py::class_<QPDFObjectHelper, std::shared_ptr<QPDFObjectHelper>>(m, "ObjectHelper")
         .def(
             "__eq__",
             [](QPDFObjectHelper &self, QPDFObjectHelper &other) {
                 // Pages that are copies
                 return objecthandle_equal(
                     self.getObjectHandle(), other.getObjectHandle());
             },
             py::is_operator())
-        .def_property_readonly(
-            "obj",
-            [](QPDFObjectHelper &poh) -> QPDFObjectHandle {
-                return poh.getObjectHandle();
-            },
-            R"~~~(
-                Get the underlying :class:`pikepdf.Object`.
-            )~~~");
+        .def_property_readonly("obj", [](QPDFObjectHelper &poh) -> QPDFObjectHandle {
+            return poh.getObjectHandle();
+        });
 
     m.def("_encode", [](py::handle handle) { return objecthandle_encode(handle); });
     m.def("unparse", [](py::object obj) -> py::bytes {
         return objecthandle_encode(obj).unparseBinary();
     });
 } // init_object
```

### Comparing `pikepdf-8.8.0/src/core/object_convert.cpp` & `pikepdf-8.9.0/src/core/object_convert.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/object_repr.cpp` & `pikepdf-8.9.0/src/core/object_repr.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -287,14 +287,18 @@
     }
 
     return ss.str();
 }
 
 std::string objecthandle_repr(QPDFObjectHandle h)
 {
+    // While we would normally expect a repr function to be a constant,
+    // accessing the repr of an object can trigger dereferencing of indirect objects
+    // and loading data from the source PDF. Thus, it is not constant.
+
     if (h.isDestroyed()) {
         return std::string("<Object was inside a closed or deleted pikepdf.Pdf>");
     }
     if (h.isScalar() || h.isOperator()) {
         // qpdf does not consider Operator a scalar but it is as far we
         // are concerned here
         return objecthandle_repr_typename_and_value(h);
```

### Comparing `pikepdf-8.8.0/src/core/parsers.cpp` & `pikepdf-8.9.0/src/core/parsers.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,68 @@
     PYBIND11_OVERRIDE_PURE_NAME(void,
         QPDFObjectHandle::ParserCallbacks,
         "handle_eof", /* Python name */
         handleEOF,    /* C++ name; trailing comma needed for macro */
     );
 }
 
+void check_operand(QPDFObjectHandle obj)
+{
+    switch (obj.getTypeCode()) {
+    case qpdf_object_type_e::ot_null:
+    case qpdf_object_type_e::ot_boolean:
+    case qpdf_object_type_e::ot_integer:
+    case qpdf_object_type_e::ot_real:
+    case qpdf_object_type_e::ot_name:
+    case qpdf_object_type_e::ot_string:
+    case qpdf_object_type_e::ot_inlineimage:
+        break;
+    case qpdf_object_type_e::ot_array: {
+        if (obj.isIndirect()) {
+            throw py::type_error(
+                "Indirect arrays are not allowed in content stream instructions");
+        }
+        for (auto &inner : obj.aitems()) {
+            check_operand(inner);
+        }
+        break;
+    }
+    case qpdf_object_type_e::ot_dictionary: {
+        if (obj.isIndirect()) {
+            throw py::type_error(
+                "Indirect dictionaries are not allowed in content stream instructions");
+        }
+        for (auto &kv : obj.ditems()) {
+            check_operand(kv.second);
+        }
+        break;
+    }
+    case qpdf_object_type_e::ot_stream:
+        throw py::type_error("Streams are not allowed in content stream instructions");
+    default: {
+        throw py::type_error("Only scalar types, arrays, and dictionaries are allowed "
+                             "in content streams.");
+    }
+    }
+}
+
+void check_objects_in_operands(std::vector<QPDFObjectHandle> &operands)
+{
+    for (QPDFObjectHandle &obj : operands) {
+        check_operand(obj);
+    }
+}
+
 ContentStreamInstruction::ContentStreamInstruction(
     ObjectList operands, QPDFObjectHandle operator_)
     : operands(operands), operator_(operator_)
 {
     if (!this->operator_.isOperator())
         throw py::type_error("operator parameter must be a pikepdf.Operator");
+    check_objects_in_operands(this->operands);
 }
 
 std::ostream &operator<<(std::ostream &os, ContentStreamInstruction &csi)
 {
     for (QPDFObjectHandle &obj : csi.operands) {
         os << obj.unparseBinary() << " ";
     }
@@ -183,17 +231,17 @@
             op        = QPDFObjectHandle::newOperator(std::string(s).c_str());
         } else if (py::isinstance<py::bytes>(operator_)) {
             py::bytes s = py::reinterpret_borrow<py::bytes>(operator_);
             op          = QPDFObjectHandle::newOperator(std::string(s).c_str());
         } else {
             op = operator_.cast<QPDFObjectHandle>();
             if (!op.isOperator()) {
-                errmsg
-                    << "At content stream instruction " << n
-                    << ", the operator is not of type pikepdf.Operator, bytes or str";
+                errmsg << "At content stream instruction " << n
+                       << ", the operator is not of type pikepdf.Operator, bytes "
+                          "or str";
                 throw py::type_error(errmsg.str());
             }
         }
 
         if (op.getOperatorValue() == std::string("INLINE IMAGE")) {
             auto operands     = py::reinterpret_borrow<py::sequence>(operands_op[0]);
             py::object iimage = operands[0];
@@ -219,14 +267,17 @@
     return py::bytes(ss.str());
 }
 
 void init_parsers(py::module_ &m)
 {
     py::class_<ContentStreamInstruction>(m, "ContentStreamInstruction")
         .def(py::init<const ContentStreamInstruction &>())
+        .def(py::init([](ObjectList operands, QPDFObjectHandle operator_) {
+            return ContentStreamInstruction(operands, operator_);
+        }))
         .def(py::init([](py::iterable operands, QPDFObjectHandle operator_) {
             ObjectList newlist;
             for (auto &item : operands) {
                 newlist.push_back(objecthandle_encode(item));
             }
             return ContentStreamInstruction(newlist, operator_);
         }))
```

### Comparing `pikepdf-8.8.0/src/core/parsers.h` & `pikepdf-8.9.0/src/core/parsers.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/pikepdf.cpp` & `pikepdf-8.9.0/src/core/pikepdf.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -155,52 +155,40 @@
             "_translate_qpdf_logic_error",
             [](std::string s) { return translate_qpdf_logic_error(s).first; },
             "Used to test interpretation of QPDF errors.")
         .def(
             "_log_info",
             [](std::string s) { return get_pikepdf_logger()->info(s); },
             "Used to test routing of QPDF's logger to Python logging.")
-        .def(
-            "set_decimal_precision",
+        .def("set_decimal_precision",
             [](uint prec) {
                 DECIMAL_PRECISION = prec;
                 return DECIMAL_PRECISION;
-            },
-            "Set the number of decimal digits to use when converting floats.")
-        .def(
-            "get_decimal_precision",
-            []() { return DECIMAL_PRECISION; },
-            "Get the number of decimal digits to use when converting floats.")
+            })
+        .def("get_decimal_precision", []() { return DECIMAL_PRECISION; })
         .def(
             "get_access_default_mmap",
             []() { return MMAP_DEFAULT; },
             "Return True if default access is to use mmap.")
         .def(
             "set_access_default_mmap",
             [](bool mmap) {
                 MMAP_DEFAULT = mmap;
                 return MMAP_DEFAULT;
             },
             "If True, ``pikepdf.open(...access_mode=access_default)`` will use mmap.")
-        .def(
-            "set_flate_compression_level",
+        .def("set_flate_compression_level",
             [](int level) {
                 if (-1 <= level && level <= 9) {
                     Pl_Flate::setCompressionLevel(level);
                     return level;
                 }
                 throw py::value_error(
                     "Flate compression level must be between 0 and 9 (or -1)");
-            },
-            R"~~~(
-            Set the compression level whenever the Flate compression algorithm is used.
-
-            Args:
-                level: -1 (default), 0 (no compression), 1 to 9 (increasing compression)
-            )~~~")
+            })
         .def("_unparse_content_stream", unparse_content_stream);
 
     // -- Exceptions --
     static py::exception<QPDFExc> exc_main(m, "PdfError");
     static py::exception<QPDFExc> exc_password(m, "PasswordError");
     static py::exception<QPDFExc> exc_datadecoding(m, "DataDecodingError");
     static py::exception<QPDFUsage> exc_usage(m, "JobUsageError");
```

### Comparing `pikepdf-8.8.0/src/core/pikepdf.h` & `pikepdf-8.9.0/src/core/pikepdf.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/pipeline.cpp` & `pikepdf-8.9.0/src/core/pipeline.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/pipeline.h` & `pikepdf-8.9.0/src/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/qpdf_inputsource-inl.h` & `pikepdf-8.9.0/src/core/qpdf_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/core/qpdf_pagelist.h` & `pikepdf-8.9.0/src/core/qpdf_pagelist.h`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/__init__.py` & `pikepdf-8.9.0/src/pikepdf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """A library for manipulating PDFs."""
 
 # isort:skip_file
 
 from __future__ import annotations
 
-__version__ = "8.8.0"
+from ._version import __version__
 
 try:
     from . import _core
 except ImportError as _e:  # pragma: no cover
     _msg = "pikepdf's extension library failed to import"
     raise ImportError(_msg) from _e
```

### Comparing `pikepdf-8.8.0/src/pikepdf/_augments.py` & `pikepdf-8.9.0/src/pikepdf/_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/_cpphelpers.py` & `pikepdf-8.9.0/src/pikepdf/_cpphelpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from typing import TYPE_CHECKING, Callable
 from warnings import warn
 
 from pikepdf.objects import Name
 
 if TYPE_CHECKING:
-    from pikepdf import Dictionary, Pdf
+    from pikepdf._core import Pdf
+    from pikepdf.objects import Dictionary
 
 
 def update_xmp_pdfversion(pdf: Pdf, version: str) -> None:
     """Update XMP metadata to specified PDF version."""
     if Name.Metadata not in pdf.Root:
         return  # Don't create an empty XMP object just to store the version
```

### Comparing `pikepdf-8.8.0/src/pikepdf/_io.py` & `pikepdf-8.9.0/src/pikepdf/_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/_qpdf.py` & `pikepdf-8.9.0/src/pikepdf/_qpdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/_xml.py` & `pikepdf-8.9.0/src/pikepdf/_xml.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/canvas.py` & `pikepdf-8.9.0/src/pikepdf/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 from enum import Enum
 from io import BytesIO
 from pathlib import Path
 
 from PIL import Image
 
 from pikepdf import (
+    Array,
     ContentStreamInstruction,
     Dictionary,
     Matrix,
     Name,
     Operator,
     Pdf,
     unparse_content_stream,
 )
+from pikepdf.objects import String
 
 log = logging.getLogger(__name__)
 
 
 Color = namedtuple('Color', ['red', 'green', 'blue', 'alpha'])
 
 BLACK = Color(0, 0, 0, 1)
@@ -68,15 +70,15 @@
 
 
 class Helvetica(Font):
     """Helvetica font."""
 
     def text_width(self, text: str, fontsize: float) -> float:
         """Estimate the width of a text string when rendered with the given font."""
-        return len(text) * fontsize
+        raise NotImplementedError()
 
     def register(self, pdf: Pdf) -> Dictionary:
         """Register the font."""
         return Dictionary(
             BaseFont=Name.Helvetica,
             Type=Name.Font,
             Subtype=Name.Type1,
@@ -167,18 +169,22 @@
 
     def set_text_horizontal_scaling(self, scale: float):
         """Set text horizontal scaling."""
         inst = ContentStreamInstruction([scale], Operator("Tz"))
         self._append(inst)
         return self
 
-    def show_text(self, text: str):
-        """Show text."""
-        encoded = text.encode("utf-16be")
-        inst = ContentStreamInstruction([[encoded]], Operator("TJ"))
+    def show_text(self, encoded: bytes):
+        """Show text.
+
+        The text must be encoded in character codes expected by the font.
+        """
+        # [ <text string> ] TJ
+        # operands need to be enclosed in Array
+        inst = ContentStreamInstruction([Array([String(encoded)])], Operator("TJ"))
         self._append(inst)
         return self
 
     def move_cursor(self, dx, dy):
         """Move cursor."""
         inst = ContentStreamInstruction([dx, dy], Operator("Td"))
         self._append(inst)
@@ -381,15 +387,14 @@
         self.page_size = page_size
         self._pdf = Pdf.new()
         self._page = self._pdf.add_blank_page(page_size=page_size)
         self._page.Resources = Dictionary(Font=Dictionary(), XObject=Dictionary())
         self._cs = ContentStreamBuilder()
         self._images: list[LoadedImage] = []
         self._accessor = _CanvasAccessor(self._cs, self._images)
-        self._stack_depth = 0
         self.do.push()
 
     def add_font(self, resource_name: Name, font: Font):
         """Add a font to the page."""
         self._page.Resources.Font[resource_name] = font.register(self._pdf)
 
     @property
@@ -409,15 +414,15 @@
             Subtype=Name.Image,
             BitsPerComponent=1 if li.image.mode == '1' else 8,
         )
 
     def to_pdf(self) -> Pdf:
         """Render the canvas as a single page PDF."""
         self.do.pop()
-        if self._stack_depth != 0:
+        if self._accessor._stack_depth != 0:
             log.warning(
                 "Graphics state stack is not empty when page saved - "
                 "rendering may be incorrect"
             )
         self._page.Contents = self._pdf.make_stream(self._cs.build())
         for li in self._images:
             self._page.Resources.XObject[li.name] = self._save_image(li)
@@ -451,21 +456,32 @@
         return self
 
     def text_transform(self, matrix: Matrix):
         """Set text matrix."""
         self._cs.set_text_matrix(matrix)
         return self
 
-    def show(self, text: str):
-        """Show text."""
+    def show(self, text: str | bytes):
+        """Show text.
+
+        The text must be encoded in character codes expected by the font.
+        If a text string is passed, it will be encoded as UTF-16BE.
+        Text rendering will not work properly if the font's character
+        codes are not consistent with UTF-16BE. This is a rudimentary
+        interface. You've been warned.
+        """
+        if isinstance(text, str):
+            encoded = b"\xfe\xff" + text.encode("utf-16be")
+        else:
+            encoded = text
         if self._direction == TextDirection.LTR:
-            self._cs.show_text(text)
+            self._cs.show_text(encoded)
         else:
             self._cs.begin_marked_content(Name.ReversedChars)
-            self._cs.show_text(text)
+            self._cs.show_text(encoded)
             self._cs.end_marked_content()
         return self
 
     def horiz_scale(self, scale):
         """Set text horizontal scaling."""
         self._cs.set_text_horizontal_scaling(scale)
         return self
```

### Comparing `pikepdf-8.8.0/src/pikepdf/codec.py` & `pikepdf-8.9.0/src/pikepdf/codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/jbig2.py` & `pikepdf-8.9.0/src/pikepdf/jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/models/__init__.py` & `pikepdf-8.9.0/src/pikepdf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/models/_content_stream.py` & `pikepdf-8.9.0/src/pikepdf/models/_content_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,33 @@
 
 """Content stream parsing."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Collection, List, Tuple, Union, cast
 
-from pikepdf import Object, ObjectType, Operator, Page, PdfError, _core
+from pikepdf._core import (
+    ContentStreamInlineImage,
+    ContentStreamInstruction,
+    Object,
+    ObjectType,
+    Page,
+    PdfError,
+    _unparse_content_stream,
+)
+from pikepdf.objects import Operator
 
 if TYPE_CHECKING:
     from pikepdf.models.image import PdfInlineImage
 
 # Operands, Operator
 _OldContentStreamOperands = Collection[Union[Object, 'PdfInlineImage']]
 _OldContentStreamInstructions = Tuple[_OldContentStreamOperands, Operator]
 
-ContentStreamInstructions = Union[
-    _core.ContentStreamInstruction, _core.ContentStreamInlineImage
-]
+ContentStreamInstructions = Union[ContentStreamInstruction, ContentStreamInlineImage]
 
 UnparseableContentStreamInstructions = Union[
     ContentStreamInstructions, _OldContentStreamInstructions
 ]
 
 
 class PdfParsingError(Exception):
@@ -59,18 +66,22 @@
         operators: A space-separated string of operators to whitelist.
             For example 'q Q cm Do' will return only operators
             that pertain to drawing images. Use 'BI ID EI' for inline images.
             All other operators and associated tokens are ignored. If blank,
             all tokens are accepted.
 
     Example:
-        >>> with pikepdf.Pdf.open(input_pdf) as pdf:
-        >>>     page = pdf.pages[0]
-        >>>     for operands, command in parse_content_stream(page):
-        >>>         print(command)
+        >>> with pikepdf.Pdf.open("../tests/resources/pal-1bit-trivial.pdf") as pdf:
+        ...     page = pdf.pages[0]
+        ...     for operands, command in pikepdf.parse_content_stream(page):
+        ...         print(command)
+        q
+        cm
+        Do
+        Q
 
     .. versionchanged:: 3.0
         Returns a list of ``ContentStreamInstructions`` instead of a list
         of (operand, operator) tuples. The returned items are duck-type compatible
         with the previous returned items.
     """
     if not isinstance(page_or_stream, (Object, Page)):
@@ -125,12 +136,12 @@
 
     .. versionchanged:: 3.0
         Now accept collections that contain any mixture of
         ``ContentStreamInstruction``, ``ContentStreamInlineImage``, and the older
         operand-operator tuples from pikepdf 2.x.
     """
     try:
-        return _core._unparse_content_stream(instructions)
+        return _unparse_content_stream(instructions)
     except (ValueError, TypeError, RuntimeError) as e:
         raise PdfParsingError(
             "While unparsing a content stream, an error occurred"
         ) from e
```

### Comparing `pikepdf-8.8.0/src/pikepdf/models/_transcoding.py` & `pikepdf-8.9.0/src/pikepdf/models/_transcoding.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/models/encryption.py` & `pikepdf-8.9.0/src/pikepdf/models/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,22 @@
     developers to enforce them as they see fit.
 
     Unencrypted PDFs implicitly have all permissions allowed. Permissions can
     only be changed when a PDF is saved.
     """
 
     accessibility: bool = True
-    """Can users use screen readers and accessibility tools to read the PDF?"""
+    """Deprecated in PDF 2.0. Formerly used to block accessibility tools.
+
+    In older versions of the PDF specification, it was possible to request
+    a PDF reader to block a user's right to use accessibility tools. Modern
+    PDF readers do not support this archaic feature and always allow accessibility
+    tools to be used. The only purpose of this permission is to provide
+    testing of this deprecated feature.
+    """
 
     extract: bool = True
     """Can users extract contents?"""
 
     modify_annotation: bool = True
     """Can users modify annotations?"""
```

### Comparing `pikepdf-8.8.0/src/pikepdf/models/image.py` & `pikepdf-8.9.0/src/pikepdf/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,26 @@
 from pathlib import Path
 from shutil import copyfileobj
 from typing import Any, BinaryIO, Callable, NamedTuple, TypeVar, Union, cast
 
 from PIL import Image
 from PIL.ImageCms import ImageCmsProfile
 
-from pikepdf import (
+from pikepdf import jbig2
+from pikepdf._core import Buffer, Pdf, PdfError, StreamDecodeLevel
+from pikepdf._exceptions import DependencyError
+from pikepdf.models import _transcoding
+from pikepdf.objects import (
     Array,
     Dictionary,
     Name,
     Object,
-    Pdf,
-    PdfError,
     Stream,
-    StreamDecodeLevel,
     String,
-    jbig2,
 )
-from pikepdf._core import Buffer
-from pikepdf._exceptions import DependencyError
-from pikepdf.models import _transcoding
 
 T = TypeVar('T')
 
 if sys.version_info >= (3, 9):
     RGBDecodeArray = tuple[float, float, float, float, float, float]
     GrayDecodeArray = tuple[float, float]
     CMYKDecodeArray = tuple[float, float, float, float, float, float, float, float]
@@ -679,18 +676,18 @@
         extracted, users should not assume what format they are getting back.
         When saving the image to a file, use a temporary filename, and then
         rename the file to its final name based on the returned file extension.
 
         Images might be saved as any of .png, .jpg, or .tiff.
 
         Examples:
-            >>> im.extract_to(stream=bytes_io)
+            >>> im.extract_to(stream=bytes_io)  # doctest: +SKIP
             '.png'
 
-            >>> im.extract_to(fileprefix='/tmp/image00')
+            >>> im.extract_to(fileprefix='/tmp/image00')  # doctest: +SKIP
             '/tmp/image00.jpg'
 
         Args:
             stream: Writable stream to write data to.
             fileprefix (str or Path): The path to write the extracted image to,
                 without the file extension.
 
@@ -1019,15 +1016,15 @@
         tmppdf.pages[0].contents_add(
             f'{self.width} 0 0 {self.height} 0 0 cm'.encode('ascii'), prepend=True
         )
         tmppdf.pages[0].contents_add(self.unparse())
 
         # ...externalize it,
         tmppdf.pages[0].externalize_inline_images()
-        raw_img = next(im for im in tmppdf.pages[0].images.values())
+        raw_img = cast(Stream, next(im for im in tmppdf.pages[0].images.values()))
 
         # ...then use the regular PdfImage API to extract it.
         img = PdfImage(raw_img)
         img._set_pdf_source(tmppdf)  # Hold tmppdf open while PdfImage exists
         return img
 
     def as_pil_image(self) -> Image.Image:
```

### Comparing `pikepdf-8.8.0/src/pikepdf/models/matrix.py` & `pikepdf-8.9.0/src/pikepdf/models/matrix.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/src/pikepdf/models/metadata.py` & `pikepdf-8.9.0/src/pikepdf/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from io import BytesIO
 from typing import TYPE_CHECKING, Any, Callable, NamedTuple, Set
 from warnings import warn
 
 from lxml import etree
 from lxml.etree import QName, XMLSyntaxError
 
-from .. import Name, Stream, String
-from .. import __version__ as pikepdf_version
-from .._xml import parse_xml
+from pikepdf._version import __version__ as pikepdf_version
+from pikepdf._xml import parse_xml
+from pikepdf.objects import Name, Stream, String
 
 if sys.version_info < (3, 9):  # pragma: no cover
     from typing import Iterable, MutableMapping
 else:
     from collections.abc import Iterable, MutableMapping
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -330,15 +330,15 @@
 
     See the XMP specification for details of allowable fields.
 
     To update metadata, use a with block.
 
     Example:
         >>> with pdf.open_metadata() as records:
-                records['dc:title'] = 'New Title'
+        ...     records['dc:title'] = 'New Title'
 
     See Also:
         :meth:`pikepdf.Pdf.open_metadata`
     """
 
     DOCINFO_MAPPING: list[DocinfoMapping] = [
         DocinfoMapping(XMP_NS_DC, 'creator', Name.Author, AuthorConverter),
```

### Comparing `pikepdf-8.8.0/src/pikepdf/models/outlines.py` & `pikepdf-8.9.0/src/pikepdf/models/outlines.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from __future__ import annotations
 
 from enum import Enum
 from itertools import chain
 from typing import Iterable, List, cast
 
-from pikepdf import Array, Dictionary, Name, Object, Page, Pdf, String
+from pikepdf._core import Page, Pdf
+from pikepdf.objects import Array, Dictionary, Name, Object, String
 
 
 class PageLocation(Enum):
     """Page view location definitions, from PDF spec."""
 
     XYZ = 1
     Fit = 2
```

### Comparing `pikepdf-8.8.0/src/pikepdf/objects.py` & `pikepdf-8.9.0/src/pikepdf/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,27 +102,37 @@
             raise TypeError("Name should be str")
         if isinstance(name, Name):
             return name  # Names are immutable so we can return a reference
         return _core._new_name(name)
 
     @classmethod
     def random(cls, len_: int = 16, prefix: str = '') -> Name:
-        """Generate a cryptographically strong random, valid PDF Name.
+        """Generate a cryptographically strong, random, valid PDF Name.
+
+        If you are inserting a new name into a PDF (for example,
+        name for a new image), you can use this function to generate a
+        cryptographically strong random name that is almost certainly already
+        not already in the PDF, and not colliding with other existing names.
 
         This function uses Python's secrets.token_urlsafe, which returns a
         URL-safe encoded random number of the desired length. An optional
         *prefix* may be prepended. (The encoding is ultimately done with
         :func:`base64.urlsafe_b64encode`.) Serendipitously, URL-safe is also
         PDF-safe.
 
         When the length parameter is 16 (16 random bytes or 128 bits), the result
         is probably globally unique and can be treated as never colliding with
         other names.
 
-        The length of the string may vary because it is encoded.
+        The length of the returned string may vary because it is encoded,
+        but will always have ``8 * len_`` random bits.
+
+        Args:
+            len_: The length of the random string.
+            prefix: A prefix to prepend to the random string.
         """
         random_string = token_urlsafe(len_)
         return _core._new_name(f"/{prefix}{random_string}")
 
 
 class Operator(Object, metaclass=_ObjectMeta):
     """Construct an operator for use in a content stream.
@@ -151,17 +161,14 @@
 
     def __new__(cls, s: str | bytes) -> String:
         """Construct a PDF String.
 
         Args:
             s: The string to use. String will be encoded for
                 PDF, bytes will be constructed without encoding.
-
-        Return type:
-            pikepdf.String
         """
         if isinstance(s, bytes):
             return _core._new_string(s)
         return _core._new_string_utf8(s)
 
 
 class Array(Object, metaclass=_ObjectMeta):
@@ -171,17 +178,14 @@
 
     def __new__(cls, a: Iterable | Rectangle | Matrix | None = None) -> Array:
         """Construct a PDF Array.
 
         Args:
             a: An iterable of objects. All objects must be either
                 `pikepdf.Object` or convertible to `pikepdf.Object`.
-
-        Return type:
-            pikepdf.Array
         """
         if isinstance(a, (str, bytes)):
             raise TypeError('Strings cannot be converted to arrays of chars')
 
         if a is None:
             a = []
         elif isinstance(a, (Rectangle, Matrix)):
@@ -208,17 +212,14 @@
             pikepdf.Dictionary({'/NameOne': 1, '/NameTwo': 'Two'})
 
             pikepdf.Dictionary(NameOne=1, NameTwo='Two')
 
         In either case, the keys must be strings, and the strings
         correspond to the desired Names in the PDF Dictionary. The values
         must all be convertible to `pikepdf.Object`.
-
-        Return type:
-            pikepdf.Dictionary
         """
         if kwargs and d is not None:
             raise ValueError('Cannot use both a mapping object and keyword args')
         if kwargs:
             # Add leading slash
             # Allows Dictionary(MediaBox=(0,0,1,1), Type=Name('/Page')...
             return _core._new_dictionary({('/' + k): v for k, v in kwargs.items()})
@@ -257,28 +258,29 @@
                 dictionary.
             kwargs: Keyword arguments that will define the stream dictionary. Do not set
                 /Length here as pikepdf will manage this value. Set /Filter
                 if the data is already encoded in some format.
 
         Examples:
             Using kwargs:
+                >>> pdf = pikepdf.Pdf.new()
                 >>> s1 = pikepdf.Stream(
-                        pdf,
-                        b"uncompressed image data",
-                        BitsPerComponent=8,
-                        ColorSpace=Name.DeviceRGB,
-                        ...
-                    )
+                ...     pdf,
+                ...     b"uncompressed image data",
+                ...     BitsPerComponent=8,
+                ...     ColorSpace=pikepdf.Name.DeviceRGB,
+                ... )
             Using dict:
-                >>> d = pikepdf.Dictionary(...)
+                >>> pdf = pikepdf.Pdf.new()
+                >>> d = pikepdf.Dictionary(Key1=1, Key2=2)
                 >>> s2 = pikepdf.Stream(
-                        pdf,
-                        b"data",
-                        d
-                    )
+                ...     pdf,
+                ...     b"data",
+                ...     d
+                ... )
 
         .. versionchanged:: 2.2
             Support creation of ``pikepdf.Stream`` from existing dictionary.
 
         .. versionchanged:: 3.0
             ``obj`` argument was removed; use ``data``.
         """
```

### Comparing `pikepdf-8.8.0/src/pikepdf.egg-info/PKG-INFO` & `pikepdf-8.9.0/src/pikepdf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 8.8.0
+Version: 8.9.0
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
@@ -25,35 +25,30 @@
 Requires-Dist: Deprecated
 Requires-Dist: lxml>=4.8
 Requires-Dist: packaging
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: typer[all]; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: GitPython; extra == "docs"
-Requires-Dist: PyGithub; extra == "docs"
 Requires-Dist: Sphinx>=3; extra == "docs"
-Requires-Dist: ipython; extra == "docs"
-Requires-Dist: matplotlib; extra == "docs"
-Requires-Dist: pybind11; extra == "docs"
-Requires-Dist: requests; extra == "docs"
+Requires-Dist: sphinx-autoapi; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: sphinx-issues; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Provides-Extra: mypy
 Requires-Dist: lxml-stubs; extra == "mypy"
 Requires-Dist: types-Pillow; extra == "mypy"
 Requires-Dist: types-requests; extra == "mypy"
 Requires-Dist: types-setuptools; extra == "mypy"
 Provides-Extra: test
 Requires-Dist: attrs>=20.2.0; extra == "test"
 Requires-Dist: coverage[toml]; extra == "test"
 Requires-Dist: hypothesis>=6.36; extra == "test"
-Requires-Dist: numpy>=1.21.0; extra == "test"
+Requires-Dist: numpy>=1.21.0; (platform_machine == "x86_64" or platform_python_implementation == "CPython") and extra == "test"
 Requires-Dist: psutil>=5.9; os_name != "nt" and extra == "test"
 Requires-Dist: pybind11; extra == "test"
 Requires-Dist: pytest>=6.2.5; extra == "test"
 Requires-Dist: pytest-cov>=3.0.0; extra == "test"
 Requires-Dist: pytest-timeout>=2.1.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.5.0; extra == "test"
 Requires-Dist: python-dateutil>=2.8.1; extra == "test"
```

### Comparing `pikepdf-8.8.0/src/pikepdf.egg-info/SOURCES.txt` & `pikepdf-8.9.0/src/pikepdf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 docs/binary-wheels.csv
 docs/conf.py
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/requirements.txt
 docs/tutorial.rst
-docs/_ext/fix_pybind11_autodoc.py
 docs/_notebooks/pages.ipynb
 docs/api/exceptions.rst
 docs/api/filters.rst
 docs/api/main.rst
 docs/api/models.rst
 docs/api/settings.rst
 docs/images/28fish.jpg
@@ -86,14 +85,15 @@
 src/pikepdf/_augments.py
 src/pikepdf/_core.pyi
 src/pikepdf/_cpphelpers.py
 src/pikepdf/_exceptions.py
 src/pikepdf/_io.py
 src/pikepdf/_methods.py
 src/pikepdf/_qpdf.py
+src/pikepdf/_version.py
 src/pikepdf/_xml.py
 src/pikepdf/canvas.py
 src/pikepdf/codec.py
 src/pikepdf/jbig2.py
 src/pikepdf/objects.py
 src/pikepdf/py.typed
 src/pikepdf/settings.py
```

### Comparing `pikepdf-8.8.0/src/pikepdf.egg-info/requires.txt` & `pikepdf-8.9.0/src/pikepdf.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 packaging
 
 [dev]
 pre-commit
 typer[all]
 
 [docs]
-GitPython
-PyGithub
 Sphinx>=3
-ipython
-matplotlib
-pybind11
-requests
+sphinx-autoapi
 sphinx-design
 sphinx-issues
 sphinx-rtd-theme
 
 [docs:python_version < "3.11"]
 tomli
 
@@ -28,23 +23,25 @@
 types-requests
 types-setuptools
 
 [test]
 attrs>=20.2.0
 coverage[toml]
 hypothesis>=6.36
-numpy>=1.21.0
 pybind11
 pytest>=6.2.5
 pytest-cov>=3.0.0
 pytest-timeout>=2.1.0
 pytest-xdist>=2.5.0
 python-dateutil>=2.8.1
 
 [test:os_name != "nt"]
 psutil>=5.9
 
 [test:os_name != "nt" and platform_machine == "x86_64"]
 python-xmp-toolkit>=2.0.1
 
+[test:platform_machine == "x86_64" or platform_python_implementation == "CPython"]
+numpy>=1.21.0
+
 [test:python_version < "3.11"]
 tomli
```

### Comparing `pikepdf-8.8.0/tests/conftest.py` & `pikepdf-8.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/1biticc.pdf` & `pikepdf-8.9.0/tests/resources/1biticc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/aquamarine-cie.pdf` & `pikepdf-8.9.0/tests/resources/aquamarine-cie.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/aquamarine-cie.png` & `pikepdf-8.9.0/tests/resources/aquamarine-cie.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/cmyk-jpeg.pdf` & `pikepdf-8.9.0/tests/resources/cmyk-jpeg.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/congress-gray.pdf` & `pikepdf-8.9.0/tests/resources/congress-gray.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/congress.pdf` & `pikepdf-8.9.0/tests/resources/congress.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/content-stream-errors.pdf` & `pikepdf-8.9.0/tests/resources/content-stream-errors.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/form.pdf` & `pikepdf-8.9.0/tests/resources/form.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/formxobject.pdf` & `pikepdf-8.9.0/tests/resources/formxobject.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/fourpages.pdf` & `pikepdf-8.9.0/tests/resources/fourpages.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/graph-encrypted.pdf` & `pikepdf-8.9.0/tests/resources/graph-encrypted.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/graph.pdf` & `pikepdf-8.9.0/tests/resources/graph.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/image-mono-inline.pdf` & `pikepdf-8.9.0/tests/resources/image-mono-inline.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/invalid_creationdate.pdf` & `pikepdf-8.9.0/tests/resources/invalid_creationdate.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/jbig2.pdf` & `pikepdf-8.9.0/tests/resources/jbig2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/jbig2global.pdf` & `pikepdf-8.9.0/tests/resources/jbig2global.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/newline-buffer-test.pdf` & `pikepdf-8.9.0/tests/resources/newline-buffer-test.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/outlines.pdf` & `pikepdf-8.9.0/tests/resources/outlines.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pal-1bit-rgb.pdf` & `pikepdf-8.9.0/tests/resources/pal-1bit-rgb.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pal-1bit-trivial.pdf` & `pikepdf-8.9.0/tests/resources/pal-1bit-trivial.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pal.pdf` & `pikepdf-8.9.0/tests/resources/pal.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pdfx.pdf` & `pikepdf-8.9.0/tests/resources/pdfx.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pike-flate-jp2.pdf` & `pikepdf-8.9.0/tests/resources/pike-flate-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pike-jp2.pdf` & `pikepdf-8.9.0/tests/resources/pike-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pink-palette-icc.pdf` & `pikepdf-8.9.0/tests/resources/pink-palette-icc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/pink-palette-icc.png` & `pikepdf-8.9.0/tests/resources/pink-palette-icc.png`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/rle.pdf` & `pikepdf-8.9.0/tests/resources/rle.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/sandwich.pdf` & `pikepdf-8.9.0/tests/resources/sandwich.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf` & `pikepdf-8.9.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf` & `pikepdf-8.9.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_annotation.py` & `pikepdf-8.9.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_attachments.py` & `pikepdf-8.9.0/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_augments.py` & `pikepdf-8.9.0/tests/test_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_codec.py` & `pikepdf-8.9.0/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_decimal.py` & `pikepdf-8.9.0/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_dictionary.py` & `pikepdf-8.9.0/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_encrypt.py` & `pikepdf-8.9.0/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_errors.py` & `pikepdf-8.9.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_filters.py` & `pikepdf-8.9.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_foreign.py` & `pikepdf-8.9.0/tests/test_foreign.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_formxobject.py` & `pikepdf-8.9.0/tests/test_formxobject.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_image_access.py` & `pikepdf-8.9.0/tests/test_image_access.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_io.py` & `pikepdf-8.9.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_io_psutil.py` & `pikepdf-8.9.0/tests/test_io_psutil.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_ipython.py` & `pikepdf-8.9.0/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_jbig2.py` & `pikepdf-8.9.0/tests/test_jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_job.py` & `pikepdf-8.9.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_matrix.py` & `pikepdf-8.9.0/tests/test_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         assert m != 'not matrix'
 
     def test_matrix_encode(self):
         m = PdfMatrix(1, 0, 0, 1, 0, 0)
         assert m.encode() == b'1.000000 0.000000 0.000000 1.000000 0.000000 0.000000'
 
     def test_matrix_inverse(self):
+        _np = pytest.importorskip('numpy')
         m = PdfMatrix(2, 0, 0, 1, 0, 3)
         minv_m = m.inverse() @ m
         assert allclose(minv_m, PdfMatrix.identity())
 
     def test_numpy(self):
         np = pytest.importorskip('numpy')
```

### Comparing `pikepdf-8.8.0/tests/test_metadata.py` & `pikepdf-8.9.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_nametree.py` & `pikepdf-8.9.0/tests/test_nametree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_numbertree.py` & `pikepdf-8.9.0/tests/test_numbertree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_object.py` & `pikepdf-8.9.0/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_objectlist.py` & `pikepdf-8.9.0/tests/test_objectlist.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_outlines.py` & `pikepdf-8.9.0/tests/test_outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_page.py` & `pikepdf-8.9.0/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_pages.py` & `pikepdf-8.9.0/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_parsers.py` & `pikepdf-8.9.0/tests/test_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     Stream,
     _core,
     parse_content_stream,
     unparse_content_stream,
 )
 from pikepdf._core import StreamParser
 from pikepdf.models import PdfParsingError
+from pikepdf.objects import Array
 
 # pylint: disable=useless-super-delegation,redefined-outer-name
 
 
 @pytest.fixture
 def graph(resources):
     yield Pdf.open(resources / 'graph.pdf')
@@ -314,7 +315,21 @@
             )
 
     def test_accepts_all_lists(self):
         unparse_content_stream([[[], b'Q']])
 
     def test_accepts_all_tuples(self):
         unparse_content_stream((((Name.Foo,), b'/Do'),))
+
+
+class TestBadSingleInstructions:
+    def test_indirect_object(self):
+        p = pikepdf.new()
+        arr = p.make_indirect(Array([42]))
+        d = p.make_indirect(Dictionary(Foo=Name.Bar))
+        stream = p.make_stream(b'test stream')
+        with pytest.raises(TypeError):
+            ContentStreamInstruction([arr], Operator('Do'))
+        with pytest.raises(TypeError):
+            ContentStreamInstruction([d], Operator('Do'))
+        with pytest.raises(TypeError):
+            ContentStreamInstruction([Name.Him, stream], Operator('Do'))
```

### Comparing `pikepdf-8.8.0/tests/test_pdf.py` & `pikepdf-8.9.0/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_pdfa.py` & `pikepdf-8.9.0/tests/test_pdfa.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_private_pdfs.py` & `pikepdf-8.9.0/tests/test_private_pdfs.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_rectangle.py` & `pikepdf-8.9.0/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_refcount.py` & `pikepdf-8.9.0/tests/test_refcount.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_repr.py` & `pikepdf-8.9.0/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `pikepdf-8.8.0/tests/test_sanity.py` & `pikepdf-8.9.0/tests/test_sanity.py`

 * *Files identical despite different names*

