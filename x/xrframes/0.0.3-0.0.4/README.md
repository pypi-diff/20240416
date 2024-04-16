# Comparing `tmp/xrframes-0.0.3.tar.gz` & `tmp/xrframes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrframes-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xrframes-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xrframes-0.0.3.tar` & `xrframes-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2024-04-08 15:12:20.359310 xrframes-0.0.3/LICENSE
--rw-r--r--   0        0        0     2490 2024-04-09 21:55:29.028989 xrframes-0.0.3/README.md
--rw-r--r--   0        0        0      774 2024-04-09 21:13:14.906424 xrframes-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      200 2024-04-10 20:10:07.753702 xrframes-0.0.3/xrframes/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-09 21:09:20.586622 xrframes-0.0.3/xrframes/_rich_dask.py
--rw-r--r--   0        0        0     1364 2024-04-09 21:09:21.332911 xrframes-0.0.3/xrframes/_rich_joblib.py
--rw-r--r--   0        0        0    14650 2024-04-10 20:08:45.918791 xrframes-0.0.3/xrframes/core.py
--rw-r--r--   0        0        0        0 2024-04-09 04:38:57.565418 xrframes-0.0.3/xrframes/py.typed
--rw-r--r--   0        0        0      278 2024-04-10 19:45:58.414851 xrframes-0.0.3/xrframes/util.py
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 xrframes-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-08 15:12:20.359310 xrframes-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2608 2024-04-16 19:31:37.043637 xrframes-0.0.4/README.md
+-rw-r--r--   0        0        0      928 2024-04-16 19:50:40.630494 xrframes-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-04-16 20:20:06.639966 xrframes-0.0.4/xrframes/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-09 21:09:20.586622 xrframes-0.0.4/xrframes/_rich_dask.py
+-rw-r--r--   0        0        0     1364 2024-04-09 21:09:21.332911 xrframes-0.0.4/xrframes/_rich_joblib.py
+-rw-r--r--   0        0        0    16382 2024-04-16 20:13:26.282971 xrframes-0.0.4/xrframes/core.py
+-rw-r--r--   0        0        0        0 2024-04-09 04:38:57.565418 xrframes-0.0.4/xrframes/py.typed
+-rw-r--r--   0        0        0     1913 2024-04-16 20:16:38.114812 xrframes-0.0.4/xrframes/util.py
+-rw-r--r--   0        0        0     2936 1970-01-01 00:00:00.000000 xrframes-0.0.4/PKG-INFO
```

### Comparing `xrframes-0.0.3/LICENSE` & `xrframes-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.3/README.md` & `xrframes-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: xrframes
+Version: 0.0.4
+Summary: Similar to ``xmovie``, make animations from xarray objects.
+Author-email: zmoon <zmoon92@gmail.com>
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: rich
+Project-URL: Home, https://github.com/zmoon/xrframes
+Project-URL: Source, https://github.com/zmoon/xrframes
+
 # xrframes
 
 [![Version on PyPI](https://img.shields.io/pypi/v/xrframes.svg)](https://pypi.org/project/xrframes/)
 [![Project Status: Concept – Minimal or no implementation has been done yet, or the repository is only intended to be a limited example, demo, or proof-of-concept.](https://www.repostatus.org/badges/latest/concept.svg)](https://www.repostatus.org/#concept)
 
 Similar to (and inspired by) [jbusecke/xmovie](https://github.com/jbusecke/xmovie),
 make animations from [xarray](https://xarray.dev/) objects
-by applying your plotting function along a dimension.
+by applying a [matplotlib](https://matplotlib.org/)-based plotting function along a dimension.
 
 ## Install
 
 ```sh
 pip install xrframes
 ```
 
@@ -71,7 +83,8 @@
 frames.write()  # serial
 frames.to_mp4("./ta_cartopy.mp4", fps=5)
 ```
 
 [^a]: `dask` on PyPI, `dask-core` on conda-forge, more info [here](https://docs.dask.org/en/stable/install.html)
 [^b]: `joblib` on PyPI and on conda-forge
 [^c]: `conda install -c conda-forge imagemagick ffmpeg`
+
```

### Comparing `xrframes-0.0.3/pyproject.toml` & `xrframes-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -30,7 +30,16 @@
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.black]
 line-length = 100
+
+[tool.mypy]
+files = [
+    "./test.py",
+    "./xrframes/**/*.py",
+]
+install_types = true
+ignore_missing_imports = true
+check_untyped_defs = true
```

### Comparing `xrframes-0.0.3/xrframes/_rich_dask.py` & `xrframes-0.0.4/xrframes/_rich_dask.py`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.3/xrframes/_rich_joblib.py` & `xrframes-0.0.4/xrframes/_rich_joblib.py`

 * *Files identical despite different names*

### Comparing `xrframes-0.0.3/xrframes/core.py` & `xrframes-0.0.4/xrframes/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from collections.abc import Hashable, Iterable
     from typing import Any, Callable
 
+    from IPython.display import Image, Video
     from matplotlib.figure import Figure
     from typing_extensions import Self
     from xarray import DataArray, Dataset
 
 
 class Frames:
 
@@ -52,14 +53,16 @@
 
             rand = str(uuid.uuid4()).split("-")[0]
             id_ = id_.replace("<rand>", rand)
         self.id_ = id_
 
         self.paths: list[Path] | None = None
 
+        self._anim_paths: list[Path] = []
+
     @classmethod
     def from_existing(cls, paths: str | Iterable[str | Path]) -> Frames:
         """Create a :class:`Frames` instance from existing frame files.
 
         This way you can call :meth:`to_mp4` and :meth:`to_gif`
         without calling :meth:`write` first, e.g. in a new session.
 
@@ -134,15 +137,15 @@
         s = StringIO()
         if p0.parent != Path("."):
             s.write(re.escape(p0.parent.as_posix()) + "/")
         s.write(re.escape(p0.name).replace(num, rf"[0-9]{{{nd}}}"))
 
         return s.getvalue()
 
-    def preview(self, frame: int = 0) -> Self:
+    def preview(self, frame: int = 0, **kwargs) -> Self:
         """Preview a frame.
 
         This calls the plotting function for the selected frame
         and thus can be used before :meth:`write` has been called.
 
         Note that ``plt.show()`` is not applied.
 
@@ -152,15 +155,15 @@
             Frame number to preview (plot).
         """
         if self.obj is None or self.func is None or self.dim is None:
             raise RuntimeError("`obj`, `func`, and `dim` must be set")
 
         if not 0 <= frame < self.obj.sizes[self.dim]:
             raise ValueError(f"frame number must be in [0, {self.obj.sizes[self.dim]})")
-        self.func(self.obj.isel({self.dim: frame}))
+        self.func(self.obj.isel({self.dim: frame}), **kwargs)
 
         return self
 
     def write(
         self,
         path=None,
         *,
@@ -367,23 +370,25 @@
                 )
                 progress.advance(task, 1)
                 progress.refresh()
         except subprocess.CalledProcessError as e:
             print(e.stderr.decode())
             raise
 
+        self._anim_paths.append(out)
+
         return None
 
     def to_gif(
         self,
         out: str | Path = "./movie.gif",
         *,
         fps: int = 10,
         scale: str = "100%",
-        magick: bool = True,
+        magick: bool | None = None,
         exe: str | Path = "convert",
     ) -> None:
         """Make a GIF from the PNG frames with ImageMagick.
 
         Parameters
         ----------
         fps
@@ -392,24 +397,37 @@
             Scaling applied when generating the output.
             For example
             ``'480x380'`` (maximum width and height in pixels, preserves original aspect ratio)
             or ``'50%'``.
         magick
             Use ``magick`` base command (new CLI for ImageMagick 7),
             i.e. ``magick convert`` instead of just ``convert``.
+            Default: ``True`` if ``magick`` is detected.
             Ignored if a custom `exe` is provived.
         exe
             Path to ``convert`` or ``magick``.
+            If detected to be a path to ``magick``, ``convert`` is added after it in the command.
+            If detected to be just ``convert`` (command), the `magick` setting will be considered,
+            but ignored if `exe` is a *path* to ``convert``.
+            Note that ``./convert`` (path in CWD), e.g., is treated as ``convert`` (command).
         """
         import subprocess
 
         from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
         out = Path(out).expanduser()
 
+        if magick is None:
+            try:
+                subprocess.run(["magick", "-version"], check=True, capture_output=True)
+            except FileNotFoundError:
+                magick = False
+            else:
+                magick = True
+
         exe = Path(exe)
 
         if self.paths is None:
             raise RuntimeError("call `write` first")
 
         files = [f.as_posix() for f in self.paths]
 
@@ -425,14 +443,16 @@
             *files,
             out.as_posix(),
         ]
         # fmt: on
 
         if magick and cmd[0] == "convert":
             cmd.insert(0, "magick")
+        elif exe.name.startswith("magick"):
+            cmd.insert(1, "convert")
 
         try:
             with Progress(
                 SpinnerColumn(finished_text="✔"),
                 r" [progress.description]{task.description}",
                 TimeElapsedColumn(),
             ) as progress:
@@ -444,16 +464,41 @@
                 )
                 progress.advance(task, 1)
                 progress.refresh()
         except subprocess.CalledProcessError as e:
             print(e.stderr.decode())
             raise
 
+        self._anim_paths.append(out)
+
         return None
 
+    def display(self, path: str | Path | None = None, **kwargs) -> Image | Video:
+        """Display the animation in a Jupyter notebook.
+
+        Parameters
+        ----------
+        path
+            By default, the last animation file created by :meth:`to_mp4` or :meth:`to_gif`,
+            but you can instead pass specify a specific file.
+        kwargs
+            Passed to :func:`IPython.display.Video` or :func:`IPython.display.Image`.
+        """
+        from .util import display
+
+        if path is None:
+            try:
+                p = self._anim_paths[-1]
+            except IndexError:
+                raise RuntimeError("call `to_mp4` or `to_gif` first")
+        else:
+            p = Path(path)
+
+        return display(p, **kwargs)
+
     def cleanup(self) -> Self:
         """Clean up (delete) the frame files associated with this instance.
 
         :attr:`paths` is reset to ``None``.
         """
         if self.paths is not None:
             for f in self.paths:
```

### Comparing `xrframes-0.0.3/PKG-INFO` & `xrframes-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,77 @@
-Metadata-Version: 2.1
-Name: xrframes
-Version: 0.0.3
-Summary: Similar to ``xmovie``, make animations from xarray objects.
-Author-email: zmoon <zmoon92@gmail.com>
-Requires-Python: ~=3.9
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: rich
-Project-URL: Home, https://github.com/zmoon/xrframes
-Project-URL: Source, https://github.com/zmoon/xrframes
-
-# xrframes
-
-[![Version on PyPI](https://img.shields.io/pypi/v/xrframes.svg)](https://pypi.org/project/xrframes/)
-[![Project Status: Concept – Minimal or no implementation has been done yet, or the repository is only intended to be a limited example, demo, or proof-of-concept.](https://www.repostatus.org/badges/latest/concept.svg)](https://www.repostatus.org/#concept)
-
-Similar to (and inspired by) [jbusecke/xmovie](https://github.com/jbusecke/xmovie),
-make animations from [xarray](https://xarray.dev/) objects
-by applying your plotting function along a dimension.
-
-## Install
-
-```sh
-pip install xrframes
-```
-
-Install and use Dask[^a] or joblib[^b] to parallelize the frame creation step.
-
-`.to_gif()` uses ImageMagick (`magick` or `convert` required on PATH);
-`.to_mp4()` uses FFmpeg (`ffmpeg` required on PATH).
-Both are available via conda-forge[^c], as well as other package managers.
-
-## Example
-
-Basic example, using just the xarray object's plot method:
-
-```python
-import xarray as xr
-from xrframes import Frames
-
-# Note: `pooch` required
-ta = xr.tutorial.open_dataset("air_temperature").air.isel(time=slice(0, 10))
-
-frames = Frames(ta, lambda da: da.plot(size=2.5, aspect=1.7), dim="time")
-frames.write(dpi=120)  # serial
-frames.to_gif("./ta_basic.gif", fps=5)
-```
-
-A bit fancier example with the same data, using Cartopy:
-
-```python
-import cartopy.crs as ccrs
-import cartopy.feature as cfeature
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import xarray as xr
-from xrframes import Frames
-
-# Note: `pooch` required
-ta = xr.tutorial.open_dataset("air_temperature").air.isel(time=slice(0, 10))
-
-proj = ccrs.Mercator()
-tran = ccrs.PlateCarree()
-
-def plot(da, **kwargs):
-    fig, ax = plt.subplots(figsize=(6, 3), layout="constrained", subplot_kw=dict(projection=proj))
-
-    ax.coastlines()
-    ax.add_feature(cfeature.BORDERS)
-    ax.add_feature(cfeature.STATES)
-    ax.gridlines(draw_labels=True)
-
-    da.plot.contourf(**kwargs, levels=np.arange(230, 305, 5), extend="both", ax=ax, transform=tran)
-
-    ax.set_title("")
-    ax.set_title(pd.Timestamp(da.time.item()).strftime(r"%Y-%m-%d %H:%M"), loc="left", size=10)
-
-    return fig
-
-frames = Frames(ta, plot, dim="time")
-frames.write()  # serial
-frames.to_mp4("./ta_cartopy.mp4", fps=5)
-```
-
-[^a]: `dask` on PyPI, `dask-core` on conda-forge, more info [here](https://docs.dask.org/en/stable/install.html)
-[^b]: `joblib` on PyPI and on conda-forge
-[^c]: `conda install -c conda-forge imagemagick ffmpeg`
-
+# xrframes
+
+[![Version on PyPI](https://img.shields.io/pypi/v/xrframes.svg)](https://pypi.org/project/xrframes/)
+[![Project Status: Concept – Minimal or no implementation has been done yet, or the repository is only intended to be a limited example, demo, or proof-of-concept.](https://www.repostatus.org/badges/latest/concept.svg)](https://www.repostatus.org/#concept)
+
+Similar to (and inspired by) [jbusecke/xmovie](https://github.com/jbusecke/xmovie),
+make animations from [xarray](https://xarray.dev/) objects
+by applying a [matplotlib](https://matplotlib.org/)-based plotting function along a dimension.
+
+## Install
+
+```sh
+pip install xrframes
+```
+
+Install and use Dask[^a] or joblib[^b] to parallelize the frame creation step.
+
+`.to_gif()` uses ImageMagick (`magick` or `convert` required on PATH);
+`.to_mp4()` uses FFmpeg (`ffmpeg` required on PATH).
+Both are available via conda-forge[^c], as well as other package managers.
+
+## Example
+
+Basic example, using just the xarray object's plot method:
+
+```python
+import xarray as xr
+from xrframes import Frames
+
+# Note: `pooch` required
+ta = xr.tutorial.open_dataset("air_temperature").air.isel(time=slice(0, 10))
+
+frames = Frames(ta, lambda da: da.plot(size=2.5, aspect=1.7), dim="time")
+frames.write(dpi=120)  # serial
+frames.to_gif("./ta_basic.gif", fps=5)
+```
+
+A bit fancier example with the same data, using Cartopy:
+
+```python
+import cartopy.crs as ccrs
+import cartopy.feature as cfeature
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import xarray as xr
+from xrframes import Frames
+
+# Note: `pooch` required
+ta = xr.tutorial.open_dataset("air_temperature").air.isel(time=slice(0, 10))
+
+proj = ccrs.Mercator()
+tran = ccrs.PlateCarree()
+
+def plot(da, **kwargs):
+    fig, ax = plt.subplots(figsize=(6, 3), layout="constrained", subplot_kw=dict(projection=proj))
+
+    ax.coastlines()
+    ax.add_feature(cfeature.BORDERS)
+    ax.add_feature(cfeature.STATES)
+    ax.gridlines(draw_labels=True)
+
+    da.plot.contourf(**kwargs, levels=np.arange(230, 305, 5), extend="both", ax=ax, transform=tran)
+
+    ax.set_title("")
+    ax.set_title(pd.Timestamp(da.time.item()).strftime(r"%Y-%m-%d %H:%M"), loc="left", size=10)
+
+    return fig
+
+frames = Frames(ta, plot, dim="time")
+frames.write()  # serial
+frames.to_mp4("./ta_cartopy.mp4", fps=5)
+```
+
+[^a]: `dask` on PyPI, `dask-core` on conda-forge, more info [here](https://docs.dask.org/en/stable/install.html)
+[^b]: `joblib` on PyPI and on conda-forge
+[^c]: `conda install -c conda-forge imagemagick ffmpeg`
```

