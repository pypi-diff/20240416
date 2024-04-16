# Comparing `tmp/manim_slides-5.1.3.tar.gz` & `tmp/manim_slides-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_slides-5.1.3.tar", last modified: Fri Feb 16 13:01:18 2024, max compression
+gzip compressed data, was "manim_slides-5.1.4.tar", last modified: Tue Apr 16 15:37:41 2024, max compression
```

## Comparing `manim_slides-5.1.3.tar` & `manim_slides-5.1.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1078 2024-02-16 13:00:59.431347 manim_slides-5.1.3/LICENSE.md
--rw-r--r--   0        0        0     9757 2024-02-16 13:00:59.431347 manim_slides-5.1.3/README.md
--rw-r--r--   0        0        0     1639 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/__init__.py
--rw-r--r--   0        0        0     2550 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/__main__.py
--rw-r--r--   0        0        0       22 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/__version__.py
--rw-r--r--   0        0        0     2203 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/commons.py
--rw-r--r--   0        0        0    11054 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/config.py
--rw-r--r--   0        0        0    21534 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/convert.py
--rw-r--r--   0        0        0      110 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/defaults.py
--rw-r--r--   0        0        0        0 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/docs/__init__.py
--rw-r--r--   0        0        0    15912 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/docs/manim_slides_directive.py
--rw-r--r--   0        0        0    10431 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/ipython/ipython_magic.py
--rw-r--r--   0        0        0     1161 2024-02-16 13:00:59.431347 manim_slides-5.1.3/manim_slides/logger.py
--rw-r--r--   0        0        0     9927 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/present/__init__.py
--rw-r--r--   0        0        0    17860 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/present/player.py
--rw-r--r--   0        0        0      254 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/qt_utils.py
--rw-r--r--   0        0        0     1511 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/render.py
--rw-r--r--   0        0        0     7448 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/resources.py
--rw-r--r--   0        0        0     1317 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/slide/__init__.py
--rw-r--r--   0        0        0     5105 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/slide/animation.py
--rw-r--r--   0        0        0    20747 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/slide/base.py
--rw-r--r--   0        0        0     4430 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/slide/manim.py
--rw-r--r--   0        0        0     2129 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/slide/manimlib.py
--rw-r--r--   0        0        0        0 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/templates/__init__.py
--rw-r--r--   0        0        0    14662 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/templates/revealjs.html
--rw-r--r--   0        0        0     2994 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/utils.py
--rw-r--r--   0        0        0     2317 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/wizard/__init__.py
--rw-r--r--   0        0        0     3651 2024-02-16 13:00:59.435346 manim_slides-5.1.3/manim_slides/wizard/wizard.py
--rw-r--r--   0        0        0     3826 2024-02-16 13:01:18.271327 manim_slides-5.1.3/pyproject.toml
--rw-r--r--   0        0        0     2056 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/conftest.py
--rw-r--r--   0        0        0      834 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides.py
--rw-r--r--   0        0        0     1155 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/BasicSlide.json
--rw-r--r--   0        0        0    50327 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4
--rw-r--r--   0        0        0    45042 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4
--rw-r--r--   0        0        0    23621 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4
--rw-r--r--   0        0        0    23195 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4
--rw-r--r--   0        0        0    17527 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4
--rw-r--r--   0        0        0    17349 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4
--rw-r--r--   0        0        0    36367 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4
--rw-r--r--   0        0        0    30504 2024-02-16 13:00:59.443346 manim_slides-5.1.3/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4
--rw-r--r--   0        0        0    30504 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/data/video.mp4
--rw-r--r--   0        0        0    40695 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/data/video_data_uri.txt
--rw-r--r--   0        0        0     3469 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_base_slide.py
--rw-r--r--   0        0        0     3443 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_commons.py
--rw-r--r--   0        0        0     1103 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_config.py
--rw-r--r--   0        0        0     4446 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_convert.py
--rw-r--r--   0        0        0      249 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_defaults.py
--rw-r--r--   0        0        0     2972 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_main.py
--rw-r--r--   0        0        0     1987 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_manim.py
--rw-r--r--   0        0        0        7 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_player.py
--rw-r--r--   0        0        0     3982 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_present.py
--rw-r--r--   0        0        0      250 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_qt_utils.py
--rw-r--r--   0        0        0     9220 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_slide.py
--rw-r--r--   0        0        0      608 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_utils.py
--rw-r--r--   0        0        0     5074 2024-02-16 13:00:59.447346 manim_slides-5.1.3/tests/test_wizard.py
--rw-r--r--   0        0        0    12779 1970-01-01 00:00:00.000000 manim_slides-5.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-16 15:37:25.896284 manim_slides-5.1.4/LICENSE.md
+-rw-r--r--   0        0        0     9734 2024-04-16 15:37:25.896284 manim_slides-5.1.4/README.md
+-rw-r--r--   0        0        0     1639 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/__init__.py
+-rw-r--r--   0        0        0     2550 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/__version__.py
+-rw-r--r--   0        0        0     2203 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/commons.py
+-rw-r--r--   0        0        0    11054 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/config.py
+-rw-r--r--   0        0        0    21294 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/convert.py
+-rw-r--r--   0        0        0      110 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/docs/__init__.py
+-rw-r--r--   0        0        0    15913 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/docs/manim_slides_directive.py
+-rw-r--r--   0        0        0    10370 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/ipython/ipython_magic.py
+-rw-r--r--   0        0        0     1161 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/logger.py
+-rw-r--r--   0        0        0    10490 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/present/__init__.py
+-rw-r--r--   0        0        0    18068 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/present/player.py
+-rw-r--r--   0        0        0      254 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/qt_utils.py
+-rw-r--r--   0        0        0     1511 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/render.py
+-rw-r--r--   0        0        0     7448 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/resources.py
+-rw-r--r--   0        0        0     1317 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/__init__.py
+-rw-r--r--   0        0        0     5105 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/animation.py
+-rw-r--r--   0        0        0    20747 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/base.py
+-rw-r--r--   0        0        0     4432 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/manim.py
+-rw-r--r--   0        0        0     2129 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/slide/manimlib.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/templates/__init__.py
+-rw-r--r--   0        0        0    14662 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/templates/revealjs.html
+-rw-r--r--   0        0        0     4303 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/utils.py
+-rw-r--r--   0        0        0     2317 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/wizard/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-16 15:37:25.900284 manim_slides-5.1.4/manim_slides/wizard/wizard.py
+-rw-r--r--   0        0        0     3795 2024-04-16 15:37:41.840191 manim_slides-5.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2056 2024-04-16 15:37:25.908284 manim_slides-5.1.4/tests/conftest.py
+-rw-r--r--   0        0        0      834 2024-04-16 15:37:25.908284 manim_slides-5.1.4/tests/data/slides.py
+-rw-r--r--   0        0        0     1155 2024-04-16 15:37:25.908284 manim_slides-5.1.4/tests/data/slides/BasicSlide.json
+-rw-r--r--   0        0        0    50327 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4
+-rw-r--r--   0        0        0    45042 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4
+-rw-r--r--   0        0        0    23621 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4
+-rw-r--r--   0        0        0    23195 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4
+-rw-r--r--   0        0        0    17527 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4
+-rw-r--r--   0        0        0    17349 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4
+-rw-r--r--   0        0        0    36367 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4
+-rw-r--r--   0        0        0    30504 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4
+-rw-r--r--   0        0        0    30504 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/video.mp4
+-rw-r--r--   0        0        0    40695 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/data/video_data_uri.txt
+-rw-r--r--   0        0        0     3469 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_base_slide.py
+-rw-r--r--   0        0        0     3443 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_commons.py
+-rw-r--r--   0        0        0     1103 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_config.py
+-rw-r--r--   0        0        0     4574 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_convert.py
+-rw-r--r--   0        0        0      249 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_defaults.py
+-rw-r--r--   0        0        0     2972 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_main.py
+-rw-r--r--   0        0        0     1987 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_manim.py
+-rw-r--r--   0        0        0        7 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_player.py
+-rw-r--r--   0        0        0     3982 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_present.py
+-rw-r--r--   0        0        0      250 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_qt_utils.py
+-rw-r--r--   0        0        0     9508 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_slide.py
+-rw-r--r--   0        0        0      608 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_utils.py
+-rw-r--r--   0        0        0     5074 2024-04-16 15:37:25.912284 manim_slides-5.1.4/tests/test_wizard.py
+-rw-r--r--   0        0        0    12733 1970-01-01 00:00:00.000000 manim_slides-5.1.4/PKG-INFO
```

### Comparing `manim_slides-5.1.3/LICENSE.md` & `manim_slides-5.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/README.md` & `manim_slides-5.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 <!-- end contact -->
 
 [pypi-version-badge]: https://img.shields.io/pypi/v/manim-slides?label=manim-slides
 [pypi-version-url]: https://pypi.org/project/manim-slides/
 [pypi-python-version-badge]: https://img.shields.io/pypi/pyversions/manim-slides
 [pypi-download-badge]: https://img.shields.io/pypi/dm/manim-slides
 [documentation-badge]: https://readthedocs.org/projects/manim-slides/badge/?version=latest
-[documentation-url]: https://manim-slides.readthedocs.io/en/latest/?badge=latest
+[documentation-url]: https://manim-slides.readthedocs.io/
 [doi-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.8215167.svg
 [doi-url]: https://doi.org/10.5281/zenodo.8215167
 [jose-badge]: https://jose.theoj.org/papers/10.21105/jose.00206/status.svg
 [jose-url]: https://doi.org/10.21105/jose.00206
 [codecov-badge]: https://codecov.io/gh/jeertmans/manim-slides/branch/main/graph/badge.svg?token=8P4DY9JCE4
 [codecov-url]: https://codecov.io/gh/jeertmans/manim-slides
 [binder-badge]: https://mybinder.org/badge_logo.svg
```

### Comparing `manim_slides-5.1.3/manim_slides/__init__.py` & `manim_slides-5.1.4/manim_slides/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/__main__.py` & `manim_slides-5.1.4/manim_slides/__main__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/commons.py` & `manim_slides-5.1.4/manim_slides/commons.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/config.py` & `manim_slides-5.1.4/manim_slides/config.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/convert.py` & `manim_slides-5.1.4/manim_slides/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import os
 import platform
 import subprocess
 import sys
 import tempfile
 import webbrowser
 from base64 import b64encode
+from collections import deque
 from enum import Enum
 from importlib import resources
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
+import av
 import click
-import cv2
 import pptx
 from click import Context, Parameter
 from jinja2 import Template
 from lxml import etree
 from PIL import Image
 from pydantic import (
     BaseModel,
@@ -75,19 +76,31 @@
     mime_type = mimetypes.guess_type(file)[0] or "video/mp4"
 
     return f"data:{mime_type};base64,{b64}"
 
 
 def get_duration_ms(file: Path) -> float:
     """Read a video and return its duration in milliseconds."""
-    cap = cv2.VideoCapture(str(file))
-    fps: int = cap.get(cv2.CAP_PROP_FPS)
-    frame_count: int = cap.get(cv2.CAP_PROP_FRAME_COUNT)
+    with av.open(str(file)) as container:
+        video = container.streams.video[0]
 
-    return 1000 * frame_count / fps
+        return float(1000 * video.duration * video.time_base)
+
+
+def read_image_from_video_file(file: Path, frame_index: "FrameIndex") -> Image:
+    """Read a image from a video file at a given index."""
+    with av.open(str(file)) as container:
+        frames = container.decode(video=0)
+
+        if frame_index == FrameIndex.last:
+            (frame,) = deque(frames, 1)
+        else:
+            frame = next(frames)
+
+        return frame.to_image()
 
 
 class Converter(BaseModel):  # type: ignore
     presentation_configs: conlist(PresentationConfig, min_length=1)  # type: ignore[valid-type]
     assets_dir: str = "{basename}_assets"
     template: Optional[Path] = None
 
@@ -351,15 +364,15 @@
     view_distance: int = 3
     mobile_view_distance: int = 2
     display: Display = Display.block
     hide_inactive_cursor: JsBool = JsBool.true
     hide_cursor_time: int = 5000
     # Appearance options from RevealJS
     background_color: Color = "black"
-    reveal_version: str = "4.6.1"
+    reveal_version: str = "5.1.0"
     reveal_theme: RevealTheme = RevealTheme.black
     title: str = "Manim Slides"
     # Pydantic options
     model_config = ConfigDict(use_enum_values=True, extra="forbid")
 
     def load_template(self) -> str:
         """Return the RevealJS HTML template as a string."""
@@ -434,31 +447,14 @@
     model_config = ConfigDict(use_enum_values=True, extra="forbid")
 
     def open(self, file: Path) -> None:
         return open_with_default(file)
 
     def convert_to(self, dest: Path) -> None:
         """Convert this configuration into a PDF presentation, saved to DEST."""
-
-        def read_image_from_video_file(file: Path, frame_index: FrameIndex) -> Image:
-            cap = cv2.VideoCapture(str(file))
-
-            if frame_index == FrameIndex.last:
-                index = cap.get(cv2.CAP_PROP_FRAME_COUNT)
-                cap.set(cv2.CAP_PROP_POS_FRAMES, index - 1)
-
-            ret, frame = cap.read()
-            cap.release()
-
-            if ret:
-                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-                return Image.fromarray(frame)
-            else:
-                raise ValueError("Failed to read {image_index} image from video file")
-
         images = []
 
         for i, presentation_config in enumerate(self.presentation_configs):
             for slide_config in tqdm(
                 presentation_config.slides,
                 desc=f"Generating video slides for config {i + 1}",
                 leave=False,
@@ -486,15 +482,15 @@
     auto_play_media: bool = True
     poster_frame_image: Optional[FilePath] = None
     model_config = ConfigDict(use_enum_values=True, extra="forbid")
 
     def open(self, file: Path) -> None:
         return open_with_default(file)
 
-    def convert_to(self, dest: Path) -> None:  # noqa: C901
+    def convert_to(self, dest: Path) -> None:
         """Convert this configuration into a PowerPoint presentation, saved to DEST."""
         prs = pptx.Presentation()
         prs.slide_width = self.width * 9525
         prs.slide_height = self.height * 9525
 
         layout = prs.slide_layouts[6]  # Should be blank
 
@@ -515,61 +511,56 @@
                 ctn = xpath(el_cnt.getparent().getparent(), ".//p:cTn")[0]
                 ctn.set("repeatCount", "indefinite")
 
         def xpath(el: etree.Element, query: str) -> etree.XPath:
             nsmap = {"p": "http://schemas.openxmlformats.org/presentationml/2006/main"}
             return etree.ElementBase.xpath(el, query, namespaces=nsmap)
 
-        def save_first_image_from_video_file(file: Path) -> Optional[str]:
-            cap = cv2.VideoCapture(file.as_posix())
-            ret, frame = cap.read()
-            cap.release()
-
-            if ret:
-                f = tempfile.NamedTemporaryFile(mode="w", delete=False, suffix=".png")
-                cv2.imwrite(f.name, frame)
-                f.close()
-                return f.name
-            else:
-                logger.warn("Failed to read first image from video file")
-                return None
-
-        for i, presentation_config in enumerate(self.presentation_configs):
-            for slide_config in tqdm(
-                presentation_config.slides,
-                desc=f"Generating video slides for config {i + 1}",
-                leave=False,
-            ):
-                file = slide_config.file
-
-                mime_type = mimetypes.guess_type(file)[0]
+        with tempfile.TemporaryDirectory() as directory_name:
+            directory = Path(directory_name)
+            frame_number = 0
+            for i, presentation_config in enumerate(self.presentation_configs):
+                for slide_config in tqdm(
+                    presentation_config.slides,
+                    desc=f"Generating video slides for config {i + 1}",
+                    leave=False,
+                ):
+                    file = slide_config.file
+
+                    mime_type = mimetypes.guess_type(file)[0]
+
+                    if self.poster_frame_image is None:
+                        poster_frame_image = str(directory / f"{frame_number}.png")
+                        image = read_image_from_video_file(
+                            file, frame_index=FrameIndex.first
+                        )
+                        image.save(poster_frame_image)
+
+                        frame_number += 1
+                    else:
+                        poster_frame_image = str(self.poster_frame_image)
+
+                    slide = prs.slides.add_slide(layout)
+                    movie = slide.shapes.add_movie(
+                        str(file),
+                        self.left,
+                        self.top,
+                        self.width * 9525,
+                        self.height * 9525,
+                        poster_frame_image=poster_frame_image,
+                        mime_type=mime_type,
+                    )
+                    if slide_config.notes != "":
+                        slide.notes_slide.notes_text_frame.text = slide_config.notes
 
-                if self.poster_frame_image is None:
-                    poster_frame_image = save_first_image_from_video_file(file)
-                else:
-                    poster_frame_image = str(self.poster_frame_image)
-
-                slide = prs.slides.add_slide(layout)
-                movie = slide.shapes.add_movie(
-                    str(file),
-                    self.left,
-                    self.top,
-                    self.width * 9525,
-                    self.height * 9525,
-                    poster_frame_image=poster_frame_image,
-                    mime_type=mime_type,
-                )
-                if slide_config.notes != "":
-                    slide.notes_slide.notes_text_frame.text = slide_config.notes
+                    if self.auto_play_media:
+                        auto_play_media(movie, loop=slide_config.loop)
 
-                if self.auto_play_media:
-                    auto_play_media(movie, loop=slide_config.loop)
-
-        dest.parent.mkdir(parents=True, exist_ok=True)
-        prs.save(dest)
+            dest.parent.mkdir(parents=True, exist_ok=True)
+            prs.save(dest)
 
 
 def show_config_options(function: Callable[..., Any]) -> Callable[..., Any]:
     """Wrap a function to add a `--show-config` option."""
 
     def callback(ctx: Context, param: Parameter, value: bool) -> None:
         if not value or ctx.resilient_parsing:
```

### Comparing `manim_slides-5.1.3/manim_slides/docs/manim_slides_directive.py` & `manim_slides-5.1.4/manim_slides/docs/manim_slides_directive.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
             self.play(text.animate.scale(2))
 
             self.next_slide()
             self.zoom(text)
 
 
 """  # noqa: D400, D415
+
 from __future__ import annotations
 
 import csv
 import itertools as it
 import re
 import shlex
 import sys
```

### Comparing `manim_slides-5.1.3/manim_slides/ipython/ipython_magic.py` & `manim_slides-5.1.4/manim_slides/ipython/ipython_magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,17 +245,15 @@
                 result = HTML(
                     """<div style="position:relative;padding-bottom:56.25%;"><iframe style="width:100%;height:100%;position:absolute;left:0px;top:0px;" frameborder="0" width="100%" height="100%" allowfullscreen allow="autoplay" srcdoc="{srcdoc}"></iframe></div>""".format(
                         srcdoc=tmpfile.read_text().replace('"', "'")
                     )
                 )
             else:
                 result = HTML(
-                    """<div style="position:relative;padding-bottom:56.25%;"><iframe style="width:100%;height:100%;position:absolute;left:0px;top:0px;" frameborder="0" width="100%" height="100%" allowfullscreen allow="autoplay" src="{src}"></iframe></div>""".format(
-                        src=tmpfile.as_posix()
-                    )
+                    f"""<div style="position:relative;padding-bottom:56.25%;"><iframe style="width:100%;height:100%;position:absolute;left:0px;top:0px;" frameborder="0" width="100%" height="100%" allowfullscreen allow="autoplay" src="{tmpfile.as_posix()}"></iframe></div>"""
                 )
 
             display(result)
 
     def add_additional_args(self, args: list[str]) -> list[str]:
         additional_args = ["--jupyter"]
         # Use webm to support transparency
```

### Comparing `manim_slides-5.1.3/manim_slides/logger.py` & `manim_slides-5.1.4/manim_slides/logger.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/present/__init__.py` & `manim_slides-5.1.4/manim_slides/present/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,14 +238,22 @@
     help="If set, pressing next will turn any looping slide into a play slide.",
 )
 @click.option(
     "--hide-info-window",
     is_flag=True,
     help="Hide info window.",
 )
+@click.option(
+    "--info-window-screen",
+    "info_window_screen_number",
+    metavar="NUMBER",
+    type=int,
+    default=None,
+    help="Put info window on the given screen (a.k.a. display).",
+)
 @click.help_option("-h", "--help")
 @verbosity_option
 def present(
     scenes: List[str],
     config_path: Path,
     folder: Path,
     start_paused: bool,
@@ -257,14 +265,15 @@
     start_at: Tuple[Optional[int], Optional[int], Optional[int]],
     start_at_scene_number: int,
     start_at_slide_number: int,
     screen_number: Optional[int],
     playback_rate: float,
     next_terminates_loop: bool,
     hide_info_window: bool,
+    info_window_screen_number: Optional[int],
 ) -> None:
     """
     Present SCENE(s), one at a time, in order.
 
     Each SCENE parameter must be the name of a Manim scene,
     with existing SCENE.json config file.
 
@@ -291,40 +300,48 @@
         start_at_scene_number = start_at[0]
 
     if start_at[1]:
         start_at_slide_number = start_at[1]
 
     warn_if_non_desirable_pyside6_version()
 
+    from qtpy.QtCore import Qt
+    from qtpy.QtGui import QScreen
+
     from ..qt_utils import qapp
+    from .player import Player
 
     app = qapp()
     app.setApplicationName("Manim Slides")
 
-    if screen_number is not None:
+    def get_screen(number: int) -> Optional[QScreen]:
         try:
-            screen = app.screens()[screen_number]
+            return app.screens()[number]
         except IndexError:
             logger.error(
-                f"Invalid screen number {screen_number}, "
+                f"Invalid screen number {number}, "
                 f"allowed values are from 0 to {len(app.screens())-1} (incl.)"
             )
-            screen = None
+            return None
+
+    if screen_number is not None:
+        screen = get_screen(screen_number)
     else:
         screen = None
 
-    from qtpy.QtCore import Qt
+    if info_window_screen_number is not None:
+        info_window_screen = get_screen(info_window_screen_number)
+    else:
+        info_window_screen = None
 
     aspect_ratio_modes = {
         "keep": Qt.KeepAspectRatio,
         "ignore": Qt.IgnoreAspectRatio,
     }
 
-    from .player import Player
-
     player = Player(
         config,
         presentation_configs,
         start_paused=start_paused,
         full_screen=full_screen,
         skip_all=skip_all,
         exit_after_last_slide=exit_after_last_slide,
@@ -332,13 +349,14 @@
         aspect_ratio_mode=aspect_ratio_modes[aspect_ratio],
         presentation_index=start_at_scene_number,
         slide_index=start_at_slide_number,
         screen=screen,
         playback_rate=playback_rate,
         next_terminates_loop=next_terminates_loop,
         hide_info_window=hide_info_window,
+        info_window_screen=info_window_screen,
     )
 
     player.show()
 
     signal.signal(signal.SIGINT, signal.SIG_DFL)
     sys.exit(app.exec())
```

### Comparing `manim_slides-5.1.3/manim_slides/present/player.py` & `manim_slides-5.1.4/manim_slides/present/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from pathlib import Path
 from typing import List, Optional
 
 from qtpy.QtCore import Qt, QTimer, QUrl, Signal, Slot
 from qtpy.QtGui import QCloseEvent, QIcon, QKeyEvent, QScreen
-from qtpy.QtMultimedia import QMediaPlayer
+from qtpy.QtMultimedia import QAudioOutput, QMediaPlayer
 from qtpy.QtMultimediaWidgets import QVideoWidget
 from qtpy.QtWidgets import (
     QHBoxLayout,
     QLabel,
     QMainWindow,
     QVBoxLayout,
     QWidget,
@@ -179,14 +179,15 @@
         aspect_ratio_mode: Qt.AspectRatioMode = Qt.KeepAspectRatio,
         presentation_index: int = 0,
         slide_index: int = 0,
         screen: Optional[QScreen] = None,
         playback_rate: float = 1.0,
         next_terminates_loop: bool = False,
         hide_info_window: bool = False,
+        info_window_screen: Optional[QScreen] = None,
     ):
         super().__init__()
 
         # Wizard's config
 
         self.config = config
 
@@ -221,28 +222,32 @@
         if hide_mouse:
             self.setCursor(Qt.BlankCursor)
 
         self.setWindowTitle(WINDOW_NAME)
         self.icon = QIcon(":/icon.png")
         self.setWindowIcon(self.icon)
 
+        self.audio_output = QAudioOutput()
         self.video_widget = QVideoWidget()
         self.video_sink = self.video_widget.videoSink()
         self.video_widget.setAspectRatioMode(aspect_ratio_mode)
         self.setCentralWidget(self.video_widget)
 
         self.media_player = QMediaPlayer(self)
+        self.media_player.setAudioOutput(self.audio_output)
         self.media_player.setVideoOutput(self.video_widget)
         self.playback_rate = playback_rate
 
         self.presentation_changed.connect(self.presentation_changed_callback)
         self.slide_changed.connect(self.slide_changed_callback)
 
         self.info = Info(
-            full_screen=full_screen, aspect_ratio_mode=aspect_ratio_mode, screen=screen
+            full_screen=full_screen,
+            aspect_ratio_mode=aspect_ratio_mode,
+            screen=info_window_screen,
         )
         self.info.close_event.connect(self.closeEvent)
         self.info.key_press_event.connect(self.keyPressEvent)
         self.video_sink.videoFrameChanged.connect(
             lambda frame: self.info.video_sink.setVideoFrame(frame)
         )
         self.hide_info_window = hide_info_window
```

### Comparing `manim_slides-5.1.3/manim_slides/render.py` & `manim_slides-5.1.4/manim_slides/render.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/resources.py` & `manim_slides-5.1.4/manim_slides/resources.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/slide/__init__.py` & `manim_slides-5.1.4/manim_slides/slide/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/slide/animation.py` & `manim_slides-5.1.4/manim_slides/slide/animation.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/slide/base.py` & `manim_slides-5.1.4/manim_slides/slide/base.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/slide/manim.py` & `manim_slides-5.1.4/manim_slides/slide/manim.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     @property
     def _frame_width(self) -> float:
         return config["frame_width"]  # type: ignore
 
     @property
     def _background_color(self) -> str:
-        color = config["background_color"]
+        color = self.camera.background_color
         if hex_color := getattr(color, "hex", None):
             return hex_color  # type: ignore
         else:  # manim>=0.18, see https://github.com/ManimCommunity/manim/pull/3020
             return color.to_hex()  # type: ignore
 
     @property
     def _resolution(self) -> Tuple[int, int]:
```

### Comparing `manim_slides-5.1.3/manim_slides/slide/manimlib.py` & `manim_slides-5.1.4/manim_slides/slide/manimlib.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/templates/revealjs.html` & `manim_slides-5.1.4/manim_slides/templates/revealjs.html`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/wizard/__init__.py` & `manim_slides-5.1.4/manim_slides/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/manim_slides/wizard/wizard.py` & `manim_slides-5.1.4/manim_slides/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/pyproject.toml` & `manim_slides-5.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 dependencies = [
     "av>=9.0.0",
     "click>=8.1.3",
     "click-default-group>=1.2.2",
     "jinja2>=3.1.2",
     "lxml>=4.9.2",
     "numpy>=1.19",
-    "opencv-python>=4.6.0.66",
     "pillow>=9.5.0",
     "pydantic>=2.0.1",
     "pydantic-extra-types>=2.0.0",
     "python-pptx>=0.6.21",
     "qtpy>=2.4.1",
     "requests>=2.28.1",
     "rich>=13.3.2",
@@ -46,15 +45,15 @@
     "slides",
     "plugin",
     "manimgl",
 ]
 name = "manim-slides"
 readme = "README.md"
 requires-python = ">=3.9,<3.13"
-version = "5.1.3"
+version = "5.1.4"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 docs = [
     "manim-slides[magic,sphinx-directive]",
```

### Comparing `manim_slides-5.1.3/tests/conftest.py` & `manim_slides-5.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides.py` & `manim_slides-5.1.4/tests/data/slides.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/BasicSlide.json` & `manim_slides-5.1.4/tests/data/slides/BasicSlide.json`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/28bf32c4df2711b07b765a647667059683133b3c45291f34692be0c845f75511_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/5060f74bee3cb2e40a399a023e0120b3f91d348a9867c7f401db54ea337de97c_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/7a5de547a0b5de2230ff3451dd680425cf0a7ea065b31e8f92b5e93527694077_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4` & `manim_slides-5.1.4/tests/data/slides/files/BasicSlide/c7d0d9ccbf764d32bf316451f2d00607b8f12893e64afe215041a8aedceeb368_reversed.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/video.mp4` & `manim_slides-5.1.4/tests/data/video.mp4`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/data/video_data_uri.txt` & `manim_slides-5.1.4/tests/data/video_data_uri.txt`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_base_slide.py` & `manim_slides-5.1.4/tests/test_base_slide.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_commons.py` & `manim_slides-5.1.4/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_config.py` & `manim_slides-5.1.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_convert.py` & `manim_slides-5.1.4/tests/test_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,19 +149,22 @@
         out_file = tmp_path / "slides.html"
         RevealJS(presentation_configs=[presentation_config]).convert_to(out_file)
         assert out_file.exists()
         assert Path(tmp_path / "slides_assets").is_dir()
         file_contents = Path(out_file).read_text()
         assert "manim" in file_contents.casefold()
 
+    @pytest.mark.parametrize("frame_index", ("first", "last"))
     def test_pdf_converter(
-        self, tmp_path: Path, presentation_config: PresentationConfig
+        self, frame_index: str, tmp_path: Path, presentation_config: PresentationConfig
     ) -> None:
         out_file = tmp_path / "slides.pdf"
-        PDF(presentation_configs=[presentation_config]).convert_to(out_file)
+        PDF(
+            presentation_configs=[presentation_config], frame_index=frame_index
+        ).convert_to(out_file)
         assert out_file.exists()
 
     def test_converter_no_presentation_config(self) -> None:
         with pytest.raises(ValidationError):
             Converter(presentation_configs=[])
 
     def test_pptx_converter(
```

### Comparing `manim_slides-5.1.3/tests/test_main.py` & `manim_slides-5.1.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_manim.py` & `manim_slides-5.1.4/tests/test_manim.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_present.py` & `manim_slides-5.1.4/tests/test_present.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_slide.py` & `manim_slides-5.1.4/tests/test_slide.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 from pathlib import Path
 
 import numpy as np
 import pytest
 from click.testing import CliRunner
 from manim import (
+    BLACK,
     BLUE,
     DOWN,
     LEFT,
     ORIGIN,
     RIGHT,
     UP,
     Circle,
@@ -104,14 +105,21 @@
             assert self._output_folder == FOLDER_PATH
             assert len(self._slides) == 0
             assert self._current_slide == 1
             assert self._start_animation == 0
             assert len(self._canvas) == 0
             assert self._wait_time_between_slides == 0.0
 
+    @assert_constructs
+    class TestBackgroundColor(Slide):
+        def construct(self) -> None:
+            assert self._background_color == BLACK.to_hex()  # DEFAULT
+            self.camera.background_color = BLUE
+            assert self._background_color == BLUE.to_hex()
+
     @assert_renders
     class TestMultipleAnimationsInLastSlide(Slide):
         """Check against solution for issue #161."""
 
         def construct(self) -> None:
             circle = Circle(color=BLUE)
             dot = Dot()
```

### Comparing `manim_slides-5.1.3/tests/test_utils.py` & `manim_slides-5.1.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/tests/test_wizard.py` & `manim_slides-5.1.4/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `manim_slides-5.1.3/PKG-INFO` & `manim_slides-5.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: manim-slides
-Version: 5.1.3
+Version: 5.1.4
 Summary: Tool for live presentations using manim
-Keywords: manim slides plugin manimgl
-Author-Email: Jérome Eertmans <jeertmans@icloud.com>
+Keywords: manim,slides,plugin,manimgl
+Author-Email: =?utf-8?q?J=C3=A9rome_Eertmans?= <jeertmans@icloud.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,14 @@
 Requires-Python: <3.13,>=3.9
 Requires-Dist: av>=9.0.0
 Requires-Dist: click>=8.1.3
 Requires-Dist: click-default-group>=1.2.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: numpy>=1.19
-Requires-Dist: opencv-python>=4.6.0.66
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-extra-types>=2.0.0
 Requires-Dist: python-pptx>=0.6.21
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: requests>=2.28.1
 Requires-Dist: rich>=13.3.2
@@ -294,15 +293,15 @@
 <!-- end contact -->
 
 [pypi-version-badge]: https://img.shields.io/pypi/v/manim-slides?label=manim-slides
 [pypi-version-url]: https://pypi.org/project/manim-slides/
 [pypi-python-version-badge]: https://img.shields.io/pypi/pyversions/manim-slides
 [pypi-download-badge]: https://img.shields.io/pypi/dm/manim-slides
 [documentation-badge]: https://readthedocs.org/projects/manim-slides/badge/?version=latest
-[documentation-url]: https://manim-slides.readthedocs.io/en/latest/?badge=latest
+[documentation-url]: https://manim-slides.readthedocs.io/
 [doi-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.8215167.svg
 [doi-url]: https://doi.org/10.5281/zenodo.8215167
 [jose-badge]: https://jose.theoj.org/papers/10.21105/jose.00206/status.svg
 [jose-url]: https://doi.org/10.21105/jose.00206
 [codecov-badge]: https://codecov.io/gh/jeertmans/manim-slides/branch/main/graph/badge.svg?token=8P4DY9JCE4
 [codecov-url]: https://codecov.io/gh/jeertmans/manim-slides
 [binder-badge]: https://mybinder.org/badge_logo.svg
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

