# Comparing `tmp/octarine3d-0.1.1.tar.gz` & `tmp/octarine3d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octarine3d-0.1.1.tar", last modified: Sun Apr  7 11:37:27 2024, max compression
+gzip compressed data, was "octarine3d-0.1.2.tar", last modified: Tue Apr 16 14:00:37 2024, max compression
```

## Comparing `octarine3d-0.1.1.tar` & `octarine3d-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:27.732447 octarine3d-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-07 11:37:25.000000 octarine3d-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-07 11:37:27.732447 octarine3d-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-07 11:37:25.000000 octarine3d-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:27.732447 octarine3d-0.1.1/octarine/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-04-07 11:37:25.000000 octarine3d-0.1.1/octarine/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:27.732447 octarine3d-0.1.1/octarine3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 11:37:27.000000 octarine3d-0.1.1/octarine3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 11:37:25.000000 octarine3d-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:37:27.732447 octarine3d-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-07 11:37:25.000000 octarine3d-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:00:37.594943 octarine3d-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-16 14:00:32.000000 octarine3d-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-16 14:00:37.594943 octarine3d-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-16 14:00:32.000000 octarine3d-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:00:37.590943 octarine3d-0.1.2/octarine/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41162 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20173 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:00:37.590943 octarine3d-0.1.2/octarine3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 14:00:32.000000 octarine3d-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:00:37.594943 octarine3d-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-16 14:00:32.000000 octarine3d-0.1.2/setup.py
```

### Comparing `octarine3d-0.1.1/LICENSE` & `octarine3d-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.1/octarine/config.py` & `octarine3d-0.1.2/octarine/config.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.1/octarine/controls.py` & `octarine3d-0.1.2/octarine/controls.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.1/octarine/conversion.py` & `octarine3d-0.1.2/octarine/conversion.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.1/octarine/utils.py` & `octarine3d-0.1.2/octarine/utils.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.1/octarine/viewer.py` & `octarine3d-0.1.2/octarine/viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import png
 import cmap
 import uuid
-import wgpu
 import random
 import inspect
 
 import numpy as np
 import pygfx as gfx
 
 from functools import wraps
@@ -15,15 +14,15 @@
 from wgpu.gui.offscreen import WgpuCanvas as WgpuCanvasOffscreen
 
 from .visuals import mesh2gfx, volume2gfx, points2gfx, lines2gfx
 from .conversion import get_converter
 from . import utils, config
 
 
-__all__ = ['Viewer']
+__all__ = ["Viewer"]
 
 logger = config.get_logger(__name__)
 
 # TODO
 # - add styles for viewer (lights, background, etc.) - e.g. .set_style(dark)
 #   - e.g. material.metalness = 2 looks good for background meshes
 #   - metalness = 1 with roughness = 0 makes for funky looking neurons
@@ -31,22 +30,34 @@
 # - make Viewer reactive (see reactive_rendering.py) to save
 #   resources when not actively using the viewer - might help in Jupyter?
 # [/] add specialised methods for adding neurons, volumes, etc. to the viewer
 # - move lights to just outside the scene's bounding box (maybe use decorator?)
 #   whenever we add/remove objects
 
 
-def update_legend(func):
-    """Decorator to update legend after function call."""
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        func(*args, **kwargs)
-        if args[0].controls:
-            args[0].controls.update_legend()
-    return wrapper
+def update_viewer(legend=True, bounds=True):
+    def outer(func):
+        """Decorator to update legend."""
+
+        @wraps(func)
+        def inner(*args, **kwargs):
+            func(*args, **kwargs)
+            if legend:
+                if getattr(args[0], "controls", None):
+                    args[0].controls.update_legend()
+                if getattr(args[0], "widget", None):
+                    if args[0].widget.toolbar:
+                        args[0].widget.toolbar.update_legend()
+            if bounds:
+                if getattr(args[0], "show_bounds", False):
+                    args[0].update_bounds()
+
+        return inner
+
+    return outer
 
 
 class Viewer:
     """PyGFX 3D viewer.
 
     Parameters
     ----------
@@ -55,101 +66,113 @@
                 want a screenshot.
     title :     str, optional
                 Title of the viewer window.
     max_fps :   int, optional
                 Maximum frames per second to render.
     size :      tuple, optional
                 Size of the viewer window.
+    camera :    "ortho" | "perspective", optional
     show :      bool, optional
-                Whether to immediately show the viewer.
-    show_controls : bool, optional
-                If True, will show the controls widget.
-                You can always show/hide the controls with
-                ``viewer.show_controls()`` and ``viewer.hide_controls()``.
+                Whether to immediately show the viewer. Note that this has no
+                effect in Jupyter. There you will have to call ``.show()`` manually
+                on the last line of a cell for the viewer to appear.
     **kwargs
                 Keyword arguments are passed through to ``WgpuCanvas``.
 
     """
+
     # Palette used for assigning colors to objects
-    palette='seaborn:tab10'
+    palette = "seaborn:tab10"
 
-    def __init__(self,
-                 offscreen=False,
-                 title='Octarine Viewer',
-                 max_fps=30,
-                 size=None,
-                 show=True,
-                 show_controls=False,
-                 **kwargs):
+    def __init__(
+        self,
+        offscreen=False,
+        title="Octarine Viewer",
+        max_fps=30,
+        camera="ortho",
+        size=None,
+        show=True,
+        **kwargs,
+    ):
         # Check if we're running in an IPython environment
-        if utils._type_of_script() == 'ipython':
+        if utils._type_of_script() == "ipython":
             ip = get_ipython()  # noqa: F821
             if not ip.active_eventloop:
                 # ip.enable_gui('qt6')
-                raise ValueError('IPython event loop not running. Please use e.g. "%gui qt" to hook into the event loop.')
+                raise ValueError(
+                    'IPython event loop not running. Please use e.g. "%gui qt" to hook into the event loop.'
+                )
 
         self._title = title
 
         # Update some defaults as necessary
-        defaults = {'title': title, 'max_fps': max_fps, 'size': size}
+        defaults = {"title": title, "max_fps": max_fps, "size": size}
         defaults.update(kwargs)
 
         # If we're running in headless mode (primarily for tests on CI) we will
         # simply not initialize the gfx objects. Not ideal but it turns
         # out to be very annoying to correctly setup on Github Actions.
-        if getattr(config, 'HEADLESS', False):
+        if getattr(config, "HEADLESS", False):
             return
 
         if not offscreen:
             self.canvas = WgpuCanvas(**defaults)
         else:
             self.canvas = WgpuCanvasOffscreen(**defaults)
 
         # There is a bug in pygfx 0.1.18 that causes the renderer to crash
         # when using a Jupyter canvas without explicitly setting the pixel_ratio.
         # This is already fixed in main but for now:
         if self._is_jupyter:
-            self.renderer = gfx.renderers.WgpuRenderer(self.canvas, show_fps=False, pixel_ratio=2)
+            self.renderer = gfx.renderers.WgpuRenderer(
+                self.canvas, show_fps=False, pixel_ratio=2
+            )
         else:
             self.renderer = gfx.renderers.WgpuRenderer(self.canvas, show_fps=False)
 
         # Set up a default scene
         self.scene = gfx.Scene()
         self.scene.add(gfx.AmbientLight(intensity=0.5))
         self.scene.add(gfx.PointLight(intensity=4))
         # Adjust shadow bias (this helps with shadow acne)
         self.scene.children[-1].shadow.bias = 0.0000005
 
         # Modify the light
         light = self.scene.children[-1]
         light.local.z = -10000  # move light forward
-        light.local.euler_x = 2.5 # rotate light
+        light.local.euler_x = 2.5  # rotate light
 
         # Set up a default background
         self._background = gfx.BackgroundMaterial((0, 0, 0))
         self.scene.add(gfx.Background(None, self._background))
 
         # Add camera
-        self.camera = gfx.OrthographicCamera()
-        #self.camera.show_object(scene, scale=1.4)
+        if camera == "ortho":
+            self.camera = gfx.OrthographicCamera()
+        elif camera == "perspective":
+            self.camera = gfx.PerspectiveCamera()
+        else:
+            raise ValueError(f"Unknown camera type: {camera}")
 
         # Add controller
-        self.controller = gfx.TrackballController(self.camera, register_events=self.renderer)
+        self.controller = gfx.TrackballController(
+            self.camera, register_events=self.renderer
+        )
 
         # Stats
         self.stats = gfx.Stats(self.renderer)
         self._show_fps = False
 
         # Setup key events
         self.key_events = {}
-        self.key_events['1'] = lambda : self.set_view('XY')
-        self.key_events['2'] = lambda : self.set_view('XZ')
-        self.key_events['3'] = lambda : self.set_view('YZ')
-        self.key_events['f'] = lambda : self._toggle_fps()
-        self.key_events['c'] = lambda : self._toggle_controls()
+        self.key_events["1"] = lambda: self.set_view("XY")
+        self.key_events["2"] = lambda: self.set_view("XZ")
+        self.key_events["3"] = lambda: self.set_view("YZ")
+        self.key_events["f"] = lambda: self._toggle_fps()
+        self.key_events["c"] = lambda: self._toggle_controls()
 
         def _keydown(event):
             """Handle key presses."""
             if event.key in self.key_events:
                 self.key_events[event.key]()
 
         # Register events
@@ -157,29 +180,27 @@
 
         # Finally, setting some variables
         self._show_bounds = False
         self._shadows = False
         self._animations = []
 
         # This starts the animation loop
-        if show:
+        if show and not self._is_jupyter:
             self.show()
 
-            # Add controls
-            if show_controls:
-                self.show_controls()
-
     def _animate(self):
         """Animate the scene."""
         to_remove = []
         for i, func in enumerate(self._animations):
             try:
                 func()
             except BaseException as e:
-                logger.error(f'Removing animation function {func} because of error: {e}')
+                logger.error(
+                    f"Removing animation function {func} because of error: {e}"
+                )
                 to_remove.append(i)
         for i in to_remove[::-1]:
             self.remove_animation(i)
 
         if self._show_fps:
             with self.stats:
                 self.renderer.render(self.scene, self.camera, flush=False)
@@ -188,26 +209,29 @@
             self.renderer.render(self.scene, self.camera)
         self.canvas.request_draw()
 
     def _next_color(self):
         """Return next color in the colormap."""
         # Cache the full palette. N.B. that ordering of colors in cmap depends on
         # the number of colors requested - i.e. we can't just grab the last color.
-        if not hasattr(self, '__cached_palette') or self.palette != self.__cached_palette:
+        if (
+            not hasattr(self, "__cached_palette")
+            or self.palette != self.__cached_palette
+        ):
             self.__cached_colors = list(cmap.Colormap(self.palette).iter_colors())
             self.__cached_palette = self.palette
 
         return self.__cached_colors[len(self.objects) % len(self.__cached_colors)]
 
-    def _next_label(self, prefix='Object'):
+    def _next_label(self, prefix="Object"):
         """Return next label."""
-        existing = [o for o in self.objects if o.startswith(prefix)]
+        existing = [o for o in self.objects if str(o).startswith(prefix)]
         if len(existing) == 0:
             return prefix
-        return f'{prefix}.{len(existing) + 1:03}'
+        return f"{prefix}.{len(existing) + 1:03}"
 
     def __getitem__(self, key):
         """Get item."""
         return self.objects[key]
 
     def __contains__(self, key):
         """Check if object is on canvas."""
@@ -216,15 +240,15 @@
     def __len__(self):
         """Return number of objects on canvas."""
         return len(self._object_ids)
 
     @property
     def controls(self):
         """Return the controls widget."""
-        return getattr(self, '_controls', None)
+        return getattr(self, "_controls", None)
 
     @property
     def visible(self):
         """List IDs of currently visible objects."""
         objects = self.objects  # grab this only once to speed things up
         return [s for s in objects if objects[s][0].visible]
 
@@ -234,27 +258,27 @@
         objects = self.objects  # grab this only once to speed things up
         return [s for s in objects if not objects[s][0].visible]
 
     @property
     def pinned(self):
         """List IDs of currently pinned objects."""
         objects = self.objects  # grab this only once to speed things up
-        return [s for s in objects if getattr(objects[s][0], '_pinned', False)]
+        return [s for s in objects if getattr(objects[s][0], "_pinned", False)]
 
     @property
     def selected(self):
         """Return IDs of or set selected objects."""
         return self.__selected
 
     @selected.setter
     def selected(self, val):
         val = utils.make_iterable(val)
 
         objects = self.objects  # grab once to speed things up
-        logger.debug(f'{len(val)} objects selected ({len(self.selected)} previously)')
+        logger.debug(f"{len(val)} objects selected ({len(self.selected)} previously)")
         # First un-highlight neurons no more selected
         for s in [s for s in self.__selected if s not in val]:
             for v in objects[s]:
                 if isinstance(v, gfx.Mesh):
                     v.color = v._stored_color
                 else:
                     v.set_data(color=v._stored_color)
@@ -277,15 +301,15 @@
         # Update legend
         if self.show_legend:
             self.update_legend()
 
         # Update data text
         # Currently only the development version of vispy supports escape
         # character (e.g. \n)
-        t = '| '.join([f'{objects[s][0]._name} - #{s}' for s in self.__selected])
+        t = "| ".join([f"{objects[s][0]._name} - #{s}" for s in self.__selected])
         self._data_text.text = t
 
     @property
     def size(self):
         """Return size of the canvas."""
         return self.canvas.get_logical_size()
 
@@ -300,45 +324,45 @@
         """Return shadow state."""
         return self._shadows
 
     @shadows.setter
     def shadows(self, v):
         """Set shadow state."""
         if not isinstance(v, bool):
-            raise TypeError(f'Expected bool, got {type(v)}')
+            raise TypeError(f"Expected bool, got {type(v)}")
 
         def set_shadow(obj, state):
-            if hasattr(obj, 'cast_shadow'):
+            if hasattr(obj, "cast_shadow"):
                 obj.cast_shadow = state
-            if hasattr(obj, 'receive_shadow'):
+            if hasattr(obj, "receive_shadow"):
                 obj.receive_shadow = state
 
         if v != self._shadows:
             self._shadows = v
             for vis in self.visuals:
                 set_shadow(vis, v)
 
             for ch in self.scene.children:
                 if isinstance(ch, gfx.PointLight):
                     ch.cast_shadow = v
 
-            #self.scene.traverse(lambda x: set_shadow(x, v))
+            # self.scene.traverse(lambda x: set_shadow(x, v))
 
     @property
     def visuals(self):
         """List of all visuals on this canvas."""
-        return [c for c in self.scene.children if hasattr(c, '_object_id')]
+        return [c for c in self.scene.children if hasattr(c, "_object_id")]
 
     @property
     def bounds(self):
         """Bounds of all currently visuals (visible and invisible)."""
         bounds = []
         for vis in self.visuals:
             # Skip the bounding box itself
-            if getattr(vis, '_object_id', '') == 'boundingbox':
+            if getattr(vis, "_object_id", "") == "boundingbox":
                 continue
 
             try:
                 bounds.append(vis._bounds)
             except BaseException:
                 pass
 
@@ -373,38 +397,40 @@
         return isinstance(self.canvas, WgpuCanvasOffscreen)
 
     @property
     def _object_ids(self):
         """All object IDs on this canvas in order of addition."""
         obj_ids = []
         for v in self.visuals:
-            if hasattr(v, '_object_id'):
+            if hasattr(v, "_object_id"):
                 obj_ids.append(v._object_id)
         return sorted(set(obj_ids), key=lambda x: obj_ids.index(x))
 
     @property
     def objects(self):
         """Ordered dictionary {name->[visuals]} of all objects in order of addition."""
         objects = OrderedDict()
         for ob in self._object_ids:
-            objects[ob] = [v for v in self.visuals if getattr(v, '_object_id', None) == ob]
+            objects[ob] = [
+                v for v in self.visuals if getattr(v, "_object_id", None) == ob
+            ]
 
         return objects
 
     def add_animation(self, x):
         """Add animation function to the Viewer.
 
         Parameters
         ----------
         x :     callable
                 Function to add to the animation loop.
 
         """
         if not callable(x):
-            raise TypeError(f'Expected callable, got {type(x)}')
+            raise TypeError(f"Expected callable, got {type(x)}")
 
         self._animations.append(x)
 
     def remove_animation(self, x):
         """Remove animation function from the Viewer.
 
         Parameters
@@ -415,101 +441,119 @@
 
         """
         if callable(x):
             self._animations.remove(x)
         elif isinstance(x, int):
             self._animations.pop(x)
         else:
-            raise TypeError(f'Expected callable or index (int), got {type(x)}')
+            raise TypeError(f"Expected callable or index (int), got {type(x)}")
 
-    def show(self, use_sidecar=False):
+    def show(self, use_sidecar=False, toolbar=False):
         """Show viewer.
 
         Parameters
         ----------
+
+        For Jupyter lab only:
+
         use_sidecar : bool
-                      For Jupyter lab only: if True, will use the Sidecar
-                      extension to display the viewer outside the notebooks.
-                      Will throw an error if Sidecar is not installed.
+                      If True, will use the Sidecar extension to display the
+                      viewer outside the notebooks. Will throw an error if
+                      Sidecar is not installed.
+        toolbar :     bool
+                      If True, will show a toolbar. You can always show/hide
+                      the toolbar with ``viewer.show_controls()`` and
+                      ``viewer.hide_controls()``, or the `c` hotkey.
 
         """
         # This is for e.g. headless testing
-        if getattr(config, 'HEADLESS', False):
+        if getattr(config, "HEADLESS", False):
             logger.info("Viewer widget not shown - running in headless mode.")
             return
 
         # Start the animation loop
         self.canvas.request_draw(self._animate)
 
         # If this is an offscreen canvas, we don't need to show anything
         if isinstance(self.canvas, WgpuCanvasOffscreen):
             return
         # In terminal we can just show the window
         elif not self._is_jupyter:
             self.canvas.show()
         # For Jupyter we need to wrap the canvas in a widget
         else:
-            if not hasattr(self, 'widget'):
-                from .jupyter import JupyterOutput
-                # Construct the widget
-                self.widget = JupyterOutput(self, use_sidecar=use_sidecar, sidecar_kwargs={'title': self._title})
+            # if not hasattr(self, 'widget'):
+            from .jupyter import JupyterOutput
+
+            # Construct the widget
+            self.widget = JupyterOutput(
+                self,
+                use_sidecar=use_sidecar,
+                toolbar=toolbar,
+                sidecar_kwargs={"title": self._title},
+            )
             return self.widget
 
     def show_controls(self):
         """Show controls."""
         if self._is_jupyter:
-            logger.warning('Controls are not (yet) supported in Jupyter.')
-            return
+            if self.widget.toolbar:
+                self.widget.toolbar.show()
+        else:
+            if not hasattr(self, "_controls"):
+                from .controls import Controls
 
-        if not hasattr(self, '_controls'):
-            from .controls import Controls
-            self._controls = Controls(self)
-        self._controls.show()
+                self._controls = Controls(self)
+            self._controls.show()
 
     def hide_controls(self):
         """Hide controls."""
-        if not hasattr(self, '_controls'):
-            return
-        self._controls.hide()
+        if self._is_jupyter:
+            if self.widget.toolbar:
+                self.widget.toolbar.hide()
+        else:
+            if hasattr(self, "_controls"):
+                self._controls.hide()
 
     def _toggle_controls(self):
         """Switch controls on and off."""
-        if not hasattr(self, '_controls'):
-            self.show_controls()
-        elif self._controls.isVisible():
-            self.hide_controls()
+        if self._is_jupyter:
+            if self.widget.toolbar:
+                self.widget.toolbar.toggle()
         else:
-            self.show_controls()
+            if not hasattr(self, "_controls"):
+                self.show_controls()
+            elif self._controls.isVisible():
+                self.hide_controls()
+            else:
+                self.show_controls()
 
-    @update_legend
+    @update_viewer(legend=True, bounds=True)
     def clear(self):
         """Clear canvas of objects (expects lights and background)."""
         # Skip if running in headless mode
-        if getattr(config, 'HEADLESS', False):
+        if getattr(config, "HEADLESS", False):
             return
 
         # Remove everything but the lights and backgrounds
         self.scene.remove(*self.visuals)
 
-    @update_legend
+    @update_viewer(legend=True, bounds=True)
     def remove_objects(self, to_remove):
         """Remove given neurons/visuals from canvas."""
         to_remove = utils.make_iterable(to_remove)
 
         for vis in self.scene.children:
             if vis in to_remove:
                 self.scene.children.remove(vis)
-            elif hasattr(vis, '_object_id'):
+            elif hasattr(vis, "_object_id"):
                 if vis._object_id in to_remove:
                     self.scene.children.remove(vis)
 
-        if self.show_bounds:
-            self.update_bounds()
-
-    @update_legend
+    @update_viewer(legend=True, bounds=True)
     def pop(self, N=1):
         """Remove the most recently added N visuals."""
         for vis in list(self.objects.values())[-N:]:
             self.remove_objects(vis)
 
     @property
     def show_bounds(self):
@@ -519,42 +563,42 @@
     def toggle_bounds(self):
         """Toggle bounding box."""
         self.show_bounds = not self.show_bounds
 
     @show_bounds.setter
     def show_bounds(self, v):
         if not isinstance(v, bool):
-            raise TypeError(f'Need bool, got {type(v)}')
+            raise TypeError(f"Need bool, got {type(v)}")
 
         self._show_bounds = v
 
         if self.show_bounds:
             self.update_bounds()
         else:
             self.remove_bounds()
 
     def remove_bounds(self):
         """Remove bounding box visual."""
         self._show_bounds = False
         for v in self.visuals:
-            if getattr(v, '_object_type', '') == 'boundingbox':
+            if getattr(v, "_object_type", "") == "boundingbox":
                 self.remove_objects(v)
 
     def resize(self, size):
         """Resize canvas.
 
         Parameters
         ----------
         size :  (width, height) tuple
                 New size of the canvas.
         """
         assert len(size) == 2
         self.canvas.set_logical_size(*size)
 
-    def update_bounds(self, color='w', width=1):
+    def update_bounds(self, color="w", width=1):
         """Update bounding box visual."""
         # Remove any existing visual
         self.remove_bounds()
 
         self._show_bounds = True
 
         # Skip if no visual on canvas
@@ -563,30 +607,27 @@
             return
 
         # Create box visual
         box = gfx.BoxHelper()
         box.set_transform_by_aabb(bounds)
 
         # Add custom attributes
-        box._object_type = 'boundingbox'
+        box._object_type = "boundingbox"
         box._object_id = uuid.uuid4()
 
         self.scene.add(box)
 
     def center_camera(self):
         """Center camera on visuals."""
         if len(self):
             self.camera.show_object(
-                self.scene,
-                scale=1,
-                view_dir=(0., 0., 1.),
-                up=(0., -1., 0.)
-                )
+                self.scene, scale=1, view_dir=(0.0, 0.0, 1.0), up=(0.0, -1.0, 0.0)
+            )
 
-    @update_legend
+    @update_viewer(legend=True, bounds=True)
     def add(self, x, name=None, center=True, clear=False, **kwargs):
         """Add object to canvas.
 
         This function is a general entry point for adding objects to the canvas.
         It will look at the type of the input and try to find an appropriate
         function to convert the input to visuals.
 
@@ -619,113 +660,150 @@
                 self.add(xx, center=False, clear=False, name=name, **kwargs)
             if center:
                 self.center_camera()
             return
 
         converter = get_converter(x, raise_missing=False)
         if converter is None:
-            raise NotImplementedError(f'No converter found for {x} ({type(x)})')
+            raise NotImplementedError(f"No converter found for {x} ({type(x)})")
 
         # Check if we have to provide a color
-        if 'color' not in kwargs and 'color' in inspect.signature(converter).parameters:
-            kwargs['color'] = tuple(self._next_color().rgba)
+        if "color" not in kwargs and "color" in inspect.signature(converter).parameters:
+            kwargs["color"] = tuple(self._next_color().rgba)
 
         visuals = utils.make_iterable(converter(x, **kwargs))
 
         for v in visuals:
             # If we have a name, assign it to the visual
             if name is not None:
                 v._object_id = name
             # If not we either use existing ID or generate a new one
             else:
                 # Give visuals an _object_id if they don't already have one
-                if not hasattr(v, '_object_id'):
-                    new_id = self._next_label('Object')
+                if not hasattr(v, "_object_id"):
+                    new_id = self._next_label("Object")
                     for v2 in visuals:
                         v._object_id = new_id
                 elif not isinstance(v._object_id, str):
                     v._object_id = str(v._object_id)
 
             self.scene.add(v)
 
         if center:
             self.center_camera()
 
-    @update_legend
-    def add_mesh(self, mesh, name=None, color=None, center=True):
+    @update_viewer(legend=True, bounds=True)
+    def _add_to_scene(self, visual, center=True):
+        """Add visual to scene.
+
+        This is just a convenient collection point for us to trigger a bunch of updates in one go,
+        """
+        self.scene.add(visual)
+
+        if center:
+            self.center_camera()
+
+    def add_mesh(self, mesh, name=None, color=None, alpha=None, center=True):
         """Add mesh to canvas.
 
         Parameters
         ----------
         mesh :      Mesh-like
                     Mesh to plot.
         name :      str, optional
                     Name for the visual.
         color :     str | tuple, optional
-                    Color to use for plotting. Can be the name of
-                    a colormap or a single color.
+                    Color to use for plotting. If multiple colors,
+                    must be a list of colors with the same length as
+                    the number of faces or vertices.
+        alpha :     float, optional
+                    Opacity value [0-1]. If provided, will override
+                    the alpha channel of the color.
         center :    bool, optional
                     If True, re-center camera to all objects on canvas.
 
         """
         if not utils.is_mesh_like(mesh):
-            raise TypeError(f'Expected mesh-like object, got {type(mesh)}')
+            raise TypeError(f"Expected mesh-like object, got {type(mesh)}")
         if color is None:
             color = self._next_color()
         if name is None:
-            name = self._next_label('Mesh')
+            name = self._next_label("Mesh")
         elif not isinstance(name, str):
             name = str(name)
 
-        visual = mesh2gfx(mesh, color=color)
+        visual = mesh2gfx(mesh, color=color, alpha=alpha)
         visual._object_id = name if name else uuid.uuid4()
-        self.scene.add(visual)
 
-        if center:
-            self.center_camera()
+        self._add_to_scene(visual, center)
 
-    @update_legend
-    def add_points(self, points, name=None, color=None, size=2, center=True):
+    def add_points(
+        self,
+        points,
+        name=None,
+        color=None,
+        marker=None,
+        size=2,
+        size_space="screen",
+        center=True,
+    ):
         """Add points plot to canvas.
 
         Parameters
         ----------
         points :    (N, 3) array
                     Points to plot.
         name :      str, optional
                     Name for the visual.
         color :     str | tuple, optional
                     Color to use for plotting. Can be the name of
                     a colormap or a single color.
+        marker :    str, optional
+                    Marker to use for plotting. By default (None), will
+                    use a point. Other options include e.g. "circle", "ring"
+                    or "diamond". See `pygfx.MarkerShape` for the definitive
+                    list of options. Please note that you may have to
+                    increase the size of the marker to see some of the shapes.
         size :      int | float
-                    Marker size.
+                    Marker size. Can
+        size_space : "screen" | "world" | "model", optional
+                    Units to use for the marker size. "screen" (default)
+                    will keep the line width constant on the screen, while
+                    "world" and "model" will keep it constant in world and
+                    model coordinates, respectively.
         center :    bool, optional
                     If True, re-center camera to all objects on canvas.
 
         """
         if not isinstance(points, np.ndarray):
-            raise TypeError(f'Expected numpy array, got {type(points)}')
+            raise TypeError(f"Expected numpy array, got {type(points)}")
         if points.ndim != 2 or points.shape[1] != 3:
-            raise ValueError(f'Expected (N, 3) array, got {points.shape}')
+            raise ValueError(f"Expected (N, 3) array, got {points.shape}")
         if color is None:
             color = self._next_color()
         if name is None:
-            name = self._next_label('Scatter')
+            name = self._next_label("Scatter")
         elif not isinstance(name, str):
             name = str(name)
 
-        visual = points2gfx(points, color=color, size=size)
+        visual = points2gfx(points, color=color, size=size, size_space=size_space, marker=marker)
         visual._object_id = name if name else uuid.uuid4()
-        self.scene.add(visual)
 
-        if center:
-            self.center_camera()
+        self._add_to_scene(visual, center)
 
-    @update_legend
-    def add_lines(self, lines, name=None, color=None, linewidth=1, center=True):
+    def add_lines(
+        self,
+        lines,
+        name=None,
+        color=None,
+        linewidth=1,
+        linewidth_space="screen",
+        linestyle="solid",
+        center=True,
+    ):
         """Add lines to canvas.
 
         Parameters
         ----------
         lines :     list of (N, 3) arrays | (N, 3) array
                     Lines to plot. If a list of arrays, each array
                     represents a separate line. If a single array,
@@ -734,127 +812,168 @@
         name :      str, optional
                     Name for the visual.
         color :     str | tuple, optional
                     Color to use for plotting. Can be a single color
                     or one for every point in the line(s).
         linewidth : float, optional
                     Line width.
+        linewidth_space : "screen" | "world" | "model", optional
+                    Units to use for the line width. "screen" (default)
+                    will keep the line width constant on the screen, while
+                    "world" and "model" will keep it constant in world and
+                    model coordinates, respectively.
+        linestyle : "solid" | "dashed" | "dotted" | "dashdot" | tuple, optional
+                    Line style to use. If a tuple, must define the on/off
+                    sequence.
         center :    bool, optional
                     If True, re-center camera to all objects on canvas.
 
         """
         # TODO:
         # - allow providing a tuple of (positions, edges) for lines
 
         if isinstance(lines, np.ndarray):
             if lines.ndim != 2 or lines.shape[1] != 3:
-                raise ValueError(f'Expected (N, 3) array, got {lines.shape}')
+                raise ValueError(f"Expected (N, 3) array, got {lines.shape}")
         elif isinstance(lines, list):
             if not all([l.ndim == 2 and l.shape[1] == 3 for l in lines]):
-                raise ValueError('Expected list of (N, 3) arrays.')
+                raise ValueError("Expected list of (N, 3) arrays.")
         else:
-            raise TypeError(f'Expected numpy array or list, got {type(lines)}')
+            raise TypeError(f"Expected numpy array or list, got {type(lines)}")
 
         if color is None:
             color = self._next_color()
         if name is None:
-            name = self._next_label('Lines')
+            name = self._next_label("Lines")
         elif not isinstance(name, str):
             name = str(name)
 
-        visual = lines2gfx(lines, linewidth=linewidth, color=color)
+        visual = lines2gfx(
+            lines,
+            linewidth=linewidth,
+            linewidth_space=linewidth_space,
+            color=color,
+            dash_pattern=linestyle,
+        )
         visual._object_id = name if name else uuid.uuid4()
-        self.scene.add(visual)
+        self._add_to_scene(visual, center)
 
-        if center:
-            self.center_camera()
-
-    @update_legend
-    def add_volume(self, volume, dims, name=None, color=None, offset=(0, 0, 0), cmin=None, cmax='auto', center=True):
+    def add_volume(
+        self,
+        volume,
+        dims,
+        name=None,
+        color=None,
+        offset=(0, 0, 0),
+        clim="data",
+        interpolation="linear",
+        hide_zero=True,
+        center=True,
+    ):
         """Add image volume to canvas.
 
         Parameters
         ----------
         volume :    (N, M, K) array
                     Volume to plot.
         dims :      tuple
                     Scale factors for the volume.
         name :      str, optional
                     Name for the visual.
-        color :     tuple, optional
-                    Color to use for plotting. Can be the name of
-                    a colormap or a single color.
+        color :     color | list of colors | pygfx.Texture, optional
+                    Colormap to render the volume. This can be:
+                      - name of a colormap (e.g. "viridis" or "magma")
+                      - a single color (name, hex, rgb, rgba)
+                      - a list of colors
+                      - a 1D pygfx.Texture
+                    Note that single colors typically don't look good and
+                    it's better to define at least two colors. For example,
+                    instead of "red" use ["red", "yellow"]. If `None` will
+                    use one of the built-in pygfx colormaps.
         offset :    tuple, optional
-                    Offset for the volume.
-        cmin/cmax : float | "auto", optional
-                    Min/max values for the colormap. If "auto", will
-                    use the min/max of the volume. If `None` will determine
-                    the min/max based on the data type of `volume`.
+                    (x, y, z) offset for the volume. If None, will use (0, 0, 0).
+        clim :      "data" | "datatype" | tuple, optional
+                    The contrast limits to scale the data values with.
+                      - "data" (default) will use the min/max of the data
+                      - "datatype" will use (0, theoretical max of data type)
+                        for integer data, e.g. (0, 255) for int8 and uint8,
+                        and (0, 1) for float data assuming the data has been
+                        normalized
+                      - tuple of min/max values or combination of "data" and
+                        "datatype" strings
+        interpolation : "linear" | "nearest"
+                    Interpolation to use when rendering the volume. "linear"
+                    (default) looks better but is slower.
+        hide_zero : bool
+                    If True, will hide voxels with lowest value according to `cmin`.
         center :    bool, optional
                     If True, re-center camera to all objects on canvas.
 
         """
         if not isinstance(volume, np.ndarray):
-            raise TypeError(f'Expected numpy array, got {type(volume)}')
+            raise TypeError(f"Expected numpy array, got {type(volume)}")
         if volume.ndim != 3:
-            raise ValueError(f'Expected 3D array, got {volume.ndim}')
-        if color is None:
-            color = self._next_color()
+            raise ValueError(f"Expected 3D array, got {volume.ndim}")
         if name is None:
-            name = self._next_label('Volume')
+            name = self._next_label("Volume")
         elif not isinstance(name, str):
             name = str(name)
 
-        visual = volume2gfx(volume, dims=dims, offset=offset, color=color, cmin=cmin, cmax=cmax)
+        visual = volume2gfx(
+            volume,
+            dims=dims,
+            offset=offset,
+            color=color,
+            clim=clim,
+            interpolation=interpolation,
+            hide_zero=hide_zero,
+        )
         visual._object_id = name if name else uuid.uuid4()
-        self.scene.add(visual)
-
-        if center:
-            self.center_camera()
+        self._add_to_scene(visual, center)
 
     def close(self):
         """Close the viewer."""
         # Skip if this is headless mode
-        if getattr(config, 'HEADLESS', False):
+        if getattr(config, "HEADLESS", False):
             return
 
         # Clear first to free all visuals
         self.clear()
 
         # Remove from config if this is the primary viewer
-        if self == getattr(config, 'PRIMARY_VIEWER', None):
+        if self == getattr(config, "PRIMARY_VIEWER", None):
             del config.PRIMARY_VIEWER
 
         # Close if not already closed
         if not self.canvas.is_closed():
             self.canvas.close()
 
-        if hasattr(self, '_controls'):
+        if hasattr(self, "_controls"):
             self._controls.close()
 
         # Close the Jupyter widget
-        if hasattr(self, 'widget') and not getattr(self.widget, '_is_closed', False):
+        if hasattr(self, "widget") and not getattr(self.widget, "_is_closed", False):
             self.widget.close(close_viewer=False)
 
     def hide_objects(self, obj):
         """Hide given object(s).
 
         Parameters
         ----------
         obj :   str | list
                 Object(s) to hide.
 
         """
-        objects = self.objects   # grab once to speed things up
+        objects = self.objects  # grab once to speed things up
         for ob in utils.make_iterable(obj):
             if ob not in objects:
                 logger.warning(f'Object "{ob}" not found on canvas.')
                 continue
             for v in objects[ob]:
-                if getattr(v, '_pinned', False):
+                if getattr(v, "_pinned", False):
                     continue
                 if v.visible:
                     v.visible = False
 
     def hide_selected(self):
         """Hide currently selected object(s)."""
         self.hide_neurons(self.selected)
@@ -872,18 +991,18 @@
         if obj is not None:
             ids = utils.make_iterable(obj)
         else:
             ids = list(objects.keys())
 
         for ob in ids:
             if ob not in objects:
-                logger.warning(f'Object {ob} not found on canvas.')
+                logger.warning(f"Object {ob} not found on canvas.")
                 continue
             for v in objects[ob]:
-                if getattr(v, '_pinned', False):
+                if getattr(v, "_pinned", False):
                     continue
                 if not v.visible:
                     v.visible = True
 
     def pin_objects(self, obj):
         """Pin given object(s).
 
@@ -893,15 +1012,15 @@
 
         """
         obj = utils.make_iterable(obj)
         objects = self.objects  # grab only once to speed things up
 
         for ob in obj:
             if ob not in objects:
-                logger.warning(f'Object {ob} not found on canvas.')
+                logger.warning(f"Object {ob} not found on canvas.")
                 continue
             for v in objects[ob]:
                 v._pinned = True
 
     def unpin_objects(self, obj=None):
         """Unpin given object(s).
 
@@ -912,22 +1031,22 @@
         if not isinstance(obj, type(None)):
             obj = utils.make_iterable(obj)
         else:
             obj = objects
 
         for ob in obj:
             if ob not in objects:
-                logger.warning(f'Object {ob} not found on canvas.')
+                logger.warning(f"Object {ob} not found on canvas.")
                 continue
             for v in objects[ob]:
                 v.unfreeze()
                 v._pinned = False
                 v.freeze()
 
-    @update_legend
+    @update_viewer(legend=True, bounds=False)
     def set_colors(self, c):
         """Set object color.
 
         Parameters
         ----------
         c :      tuple | dict
                  RGB color(s) to apply. Values must be 0-1. Accepted:
@@ -942,27 +1061,27 @@
             cmap = c
         else:
             raise TypeError(f'Unable to use colors of type "{type(c)}"')
 
         for n in objects:
             if n in cmap:
                 for v in objects[n]:
-                    if getattr(v, '_pinned', False):
+                    if getattr(v, "_pinned", False):
                         continue
-                    if not hasattr(v, 'material'):
+                    if not hasattr(v, "material"):
                         continue
                     # Note: there is currently a bug where removing or adding an alpha
                     # channel from a color will break the rendering pipeline
                     if len(v.material.color) == 4:
                         new_c = gfx.Color(cmap[n]).rgba
                     else:
                         new_c = gfx.Color(cmap[n]).rgb
                     v.material.color = gfx.Color(new_c)
 
-    def colorize(self, palette='seaborn:tab10', objects=None, randomize=True):
+    def colorize(self, palette="seaborn:tab10", objects=None, randomize=True):
         """Colorize objects using a color palette.
 
         Parameters
         ----------
         palette :   str | cmap Colormap
                     Name of the `cmap` palette to use. See
                     https://cmap-docs.readthedocs.io/en/latest/catalog/#colormaps-by-category
@@ -1000,19 +1119,17 @@
         """
         self._background.set_colors(gfx.Color(c).rgba)
 
     def _toggle_fps(self):
         """Switch FPS measurement on and off."""
         self._show_fps = not self._show_fps
 
-    def screenshot(self,
-                   filename='screenshot.png',
-                   size=None,
-                   pixel_ratio=None,
-                   alpha=True):
+    def screenshot(
+        self, filename="screenshot.png", size=None, pixel_ratio=None, alpha=True
+    ):
         """Save a screenshot of the canvas.
 
         Parameters
         ----------
         filename :      str, optional
                         Filename to save to. If ``None``, will return image array.
                         Note that this will always save a PNG file, no matter
@@ -1026,17 +1143,19 @@
                         on offscreen canvases.
         alpha :         bool, optional
                         If True, will export transparent background.
 
         """
         im = self._screenshot(alpha=alpha, size=size, pixel_ratio=pixel_ratio)
         if filename:
-            if not filename.endswith('.png'):
-                filename += '.png'
-            png.from_array(im.reshape(im.shape[0], im.shape[1] * im.shape[2]), mode='RGBA').save(filename)
+            if not filename.endswith(".png"):
+                filename += ".png"
+            png.from_array(
+                im.reshape(im.shape[0], im.shape[1] * im.shape[2]), mode="RGBA"
+            ).save(filename)
         else:
             return im
 
     def _screenshot(self, alpha=True, size=None, pixel_ratio=None):
         """Return image array for screenshot."""
         if alpha:
             op = self._background.opacity
@@ -1072,15 +1191,21 @@
 
         Parameters
         ----------
         view :      XY | XZ | YZ
                     View to set.
 
         """
-        if view == 'XY':
-            self.camera.show_object(self.scene, view_dir=(0., 0., 1.), up=(0., -1., 0.))
-        elif view == 'XZ':
-            self.camera.show_object(self.scene, scale=1, view_dir=(0., 1., 0.), up=(0., 0., 1.))
-        elif view == 'YZ':
-            self.camera.show_object(self.scene, scale=1, view_dir=(-1., 0., 0.), up=(0., -1., 0.))
+        if view == "XY":
+            self.camera.show_object(
+                self.scene, view_dir=(0.0, 0.0, 1.0), up=(0.0, -1.0, 0.0)
+            )
+        elif view == "XZ":
+            self.camera.show_object(
+                self.scene, scale=1, view_dir=(0.0, 1.0, 0.0), up=(0.0, 0.0, 1.0)
+            )
+        elif view == "YZ":
+            self.camera.show_object(
+                self.scene, scale=1, view_dir=(-1.0, 0.0, 0.0), up=(0.0, -1.0, 0.0)
+            )
         else:
-            raise TypeError(f'Unable to set view from {type(view)}')
+            raise TypeError(f"Unable to set view from {type(view)}")
```

### Comparing `octarine3d-0.1.1/octarine/visuals.py` & `octarine3d-0.1.2/octarine/visuals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+import cmap
 
 import pygfx as gfx
 import numpy as np
 import trimesh as tm
 
 from . import config, utils
 
@@ -50,24 +51,34 @@
 
 def parse_mesh_color(mesh, color, alpha=None):
     """Parse color for mesh plotting."""
     mat_color_kwargs = dict()
     obj_color_kwargs = dict()
     if isinstance(color, np.ndarray) and color.ndim == 2:
         if alpha is not None:
+            if color.shape[1] == 3:
+                color = np.hstack((color, np.ones((color.shape[0], 1))))
+            elif color.shape[1] != 4:
+                raise ValueError("Expected colors to have 3 or 4 channels.")
             color[:, -1] = alpha
 
+        # Make sure the color is what pygfx expects
+        if color.dtype in (np.float64, ):
+            color = color.astype(np.float32, copy=False)
+
         if len(color) == len(mesh.vertices):
             obj_color_kwargs = dict(colors=color)
             mat_color_kwargs = dict(color_mode="vertex")
         elif len(color) == len(mesh.faces):
             obj_color_kwargs = dict(colors=color)
             mat_color_kwargs = dict(color_mode="face")
         else:
-            mat_color_kwargs["color"] = color
+            raise ValueError(
+                "Expected colors to have the same length as the number of vertices or faces."
+            )
     else:
         if alpha is not None:
             color = gfx.Color(color).rgba
             color = (color[0], color[1], color[2], alpha)
 
         mat_color_kwargs["color"] = color
 
@@ -90,69 +101,130 @@
     # rgb, not rgba. So we need to remove the alpha channel.
     colormap_data = colormap_data[:, :3]
 
     # Convert to vispy cmap
     return gfx.Texture(colormap_data, dim=1)
 
 
-def volume2gfx(vol, dims, color, offset=(0, 0, 0), cmin=None, cmax=None, **kwargs):
+def volume2gfx(
+    vol,
+    dims,
+    color,
+    offset=(0, 0, 0),
+    clim="auto",
+    interpolation="linear",
+    hide_zero=True,
+):
     """Convert volume (i.e. 3d arrays) to pygfx visual.
 
     Parameters
     ----------
     vol :           np.ndarray
                     3D array representing the volume.
     dims :          tuple
                     Dimensions of the volume along the (x, y, z) axes.
-    color :         str | tuple
-                    CURRENTLY NOT USED.
+    color :         color | list of colors | pygfx.Texture, optional
+                    Colormap to render the volume. This can be:
+                      - name of a colormap (e.g. "viridis" or "magma")
+                      - a single color (name, hex, rgb, rgba)
+                      - a list of colors
+                      - a 1D pygfx.Texture
+                    Note that single colors typically don't look good and
+                    it's better to define at least two colors. For example,
+                    instead of "red" use ["red", "yellow"]. If `None` will
+                    use one of the built-in pygfx colormaps.
+    offset :        tuple, optional
+                    Offset to apply to the volume.
+    clim :          "data" | "datatype" | tuple, optional
+                    The contrast limits to scale the data values with.
+                      - "data" (default) will use the min/max of the data
+                      - "datatype" will use (0, theoretical max of data type)
+                        for integer data, e.g. (0, 255) for int8 and uint8,
+                        and (0, 1) for float data assuming the data has been
+                        normalized
+                      - tuple of min/max values or combination of "data" and
+                        "datatype" strings
+    interpolation : str, optional
+                    Interpolation method to use. Either "linear" or "nearest".
+    hide_zero :     bool, optional
+                    If True, will set the alpha for the lowest value to 0.
+
+    Returns
+    -------
+    vis :           gfx.Volume
+                    Pygfx visual representing the volume.
 
     """
     # TODOs:
-    # - add support for custom color maps (see cmap's to_pygfx method)
     # - add support for other Volume materials (e.g. gfx.VolumeMipMaterial)
 
     assert isinstance(vol, np.ndarray), "Expected 3D numpy array."
     assert vol.ndim == 3, "Expected 3D numpy array."
     assert isinstance(dims, (tuple, list, np.ndarray, int, float))
     if isinstance(dims, (int, float)):
         dims = [dims] * 3
     assert len(dims) == 3, "Expected dimensions as tuple of length 3."
 
     # Similar to vispy, pygfx seems to expect zyx coordinate space
     grid = vol.T
 
-    # Avoid boolean matrices here
-    if grid.dtype == bool:
-        grid = grid.astype(int)
-    elif grid.dtype.str.contains('>u') or grid.dtype.str.contains('<u'):
-        grid = grid.astype(np.uint32)
-    elif grid.dtype.str.contains('>f') or grid.dtype.str.contains('<f'):
-        grid = grid.astype(np.float32)
+    # Convert to data type that pygfx can handle:
+    # Convert non-native byte order to native; e.g. >u4 -> u4 = uint64
+    if grid.dtype.byteorder in (">", "<"):
+        grid = grid.astype(grid.dtype.str.replace(grid.dtype.byteorder, ""))
+    # Convert boolean matrices to uint16; I tried uint4 but that renders as
+    # uniform volume and uint8 looks fuzzy
+    elif grid.dtype == bool:
+        grid = grid.astype(np.uint16)
 
     # Find the potential min/max value of the volume
-    if cmax is None:
-        cmax = np.iinfo(grid.dtype).max
-    elif cmax == "auto":
-        cmax = grid.max()
+    if isinstance(clim, str) and clim == "datatype":
+        cmin = cmax = "datatype"
+    elif isinstance(clim, str) and clim == "data":
+        cmin = cmax = "data"
+    else:
+        cmin, cmax = clim
 
-    if cmin is None:
+    if cmin == "datatype":
         cmin = 0
-    elif cmin == "auto":
+    elif cmin == "data":
         cmin = grid.min()
 
+    if cmax == "datatype":
+        # If float, assume that the data is normalized
+        if grid.dtype.kind == "f":
+            cmax = 1
+        # Otherwise, use the maximum value of the data type
+        else:
+            cmax = np.iinfo(grid.dtype).max
+    elif cmax == "data":
+        cmax = grid.max()
+
     # Initialize texture
     tex = gfx.Texture(grid, dim=3)
 
+    # Initialize colormap (and make copy of the data to avoid issues
+    # with the original colormap data being modified)
+    cmap = to_colormap(color, hide_zero=hide_zero)
+
     # Initialize the volume
     vis = gfx.Volume(
         gfx.Geometry(grid=tex),
-        gfx.VolumeRayMaterial(clim=(0, cmax), map=gfx.cm.cividis),
+        gfx.VolumeMipMaterial(
+            clim=(cmin, cmax),
+            map=cmap,
+            interpolation=interpolation,
+            map_interpolation=interpolation,
+        ),
     )
 
+    # To trigger an update of the colormap data later:
+    # vis.material.data[:, 1] = 0
+    # vis.material.map.update_range((0, 0, 0), vis.material.map.size)
+
     # Set scales and offset
     (
         vis.local.scale_x,
         vis.local.scale_y,
         vis.local.scale_z,
     ) = dims
     (vis.local.x, vis.local.y, vis.local.z) = offset
@@ -160,32 +232,79 @@
     # Add custom attributes
     vis._object_type = "volume"
     vis._object_id = uuid.uuid4()
 
     return vis
 
 
-def points2gfx(points, color, size=2):
+def to_colormap(x, hide_zero):
+    """Convert `x` to a gfx.Texture that can be used for Volumes."""
+    # If this is a texture
+    if x is None:
+        tex = gfx.cm.cividis
+    elif isinstance(x, gfx.Texture):
+        if x.dim != 1:
+            raise ValueError("Expected 1D texture.")
+        tex = x
+    elif isinstance(x, str) and hasattr(gfx.cm, x):
+        tex = getattr(gfx.cm, x)
+    elif isinstance(x, gfx.Color):
+        # cmap needs a list of colors (even if len == 1)
+        tex = cmap.Colormap([x.rgba]).to_pygfx()
+    elif isinstance(x, cmap.Colormap):
+        tex = x.to_pygfx()
+    elif isinstance(x, (dict, list)):
+        # cmap can interpret dict and list of colors
+        tex = cmap.Colormap(x).to_pygfx()
+    else:
+        # Last ditch effort: see if cmap can handle it
+        tex = cmap.Colormap([x]).to_pygfx()
+
+    if hide_zero:
+        # Add an alpha column if needed
+        if tex.data.shape[1] == 3:
+            colors = np.hstack(
+                (tex.data, np.ones((tex.data.shape[0], 1))), dtype=tex.data.dtype
+            )
+            tex = gfx.Texture(colors, dim=1)
+        # Otherwise make a copy to avoid modifying the original data
+        else:
+            tex = gfx.Texture(tex.data.copy(), dim=1)
+
+        # Set alpha channel for first color to 0
+        tex.data[0, 3] = 0
+
+    return tex
+
+
+def points2gfx(points, color, size=2, marker=None, size_space="screen"):
     """Convert points to pygfx visuals.
 
     Parameters
     ----------
     points :        (N, 3) array
                     Points to plot.
     color :         tuple | array
                     Color to use for plotting. If multiple colors,
                     must be a list of colors with the same length as
                     the number of points.
     size :          int, optional
                     Marker size.
+    marker :        str, optional
+                    See gfx.MarkerShape for available markers.
+    size_space :    "screen" | "world" | "model", optional
+                    Units to use for the marker size. "screen" (default)
+                    will keep the line width constant on the screen, while
+                    "world" and "model" will keep it constant in world and
+                    model coordinates, respectively.
 
     Returns
     -------
-    list
-                    Contains pygfx visuals for points.
+    vis :           gfx.Points
+                    Pygfx visual for points.
 
     """
     # TODOs:
     # - add support for per-vertex sizes and colors
     assert isinstance(points, np.ndarray), "Expected numpy array."
     assert points.ndim == 2, "Expected 2D numpy array."
     assert points.shape[1] == 3, "Expected (N, 3) array."
@@ -200,51 +319,104 @@
     material_kwargs = {}
     if utils.is_iterable(size):
         if len(size) != len(points):
             raise ValueError(
                 "Expected `size` to be a single value or "
                 "an array of the same length as `points`."
             )
-        geometry_kwargs['sizes'] = np.asarray(size).astype(np.float32, copy=False)
-        material_kwargs['vertex_sizes'] = True
+        geometry_kwargs["sizes"] = np.asarray(size).astype(np.float32, copy=False)
+        material_kwargs["size_mode"] = 'vertex'
     else:
-        material_kwargs['size'] = size
+        material_kwargs["size"] = size
 
-    vis = gfx.Points(
-        gfx.Geometry(positions=points, **geometry_kwargs),
-        gfx.PointsMaterial(color=color, **material_kwargs),
-    )
+    if marker is None:
+        material = gfx.PointsMaterial(
+            color=color, size_space=size_space, **material_kwargs
+        )
+    else:
+        material = gfx.PointsMarkerMaterial(
+            color=color, marker=marker, size_space=size_space, **material_kwargs
+        )
+
+    vis = gfx.Points(gfx.Geometry(positions=points, **geometry_kwargs), material)
 
     # Add custom attributes
     vis._object_type = "points"
     vis._object_id = uuid.uuid4()
 
     return vis
 
 
-def lines2gfx(lines, color, linewidth=1):
-    """Convert lines into pygfx visuals."""
+def lines2gfx(lines, color, linewidth=1, linewidth_space="screen", dash_pattern=None):
+    """Convert lines into pygfx visuals.
+
+    Parameters
+    ----------
+    lines :     list of (N, 3) arrays | (N, 3) array
+                Lines to plot. If a list of arrays, each array
+                represents a separate line. If a single array,
+                each row represents a point in the line. You can
+                introduce breaks in the line by inserting NaNs.
+    color :     str | tuple, optional
+                Color to use for plotting. Can be a single color
+                or one for every point in the line(s).
+    linewidth : float, optional
+                Line width.
+    linewidth_space : "screen" | "world" | "model", optional
+                Units to use for the line width. "screen" (default)
+                will keep the line width constant on the screen, while
+                "world" and "model" will keep it constant in world and
+                model coordinates, respectively.
+    dash_pattern : "solid" | "dashed" | "dotted" | "dashdot" | tuple, optional
+                Line style to use. If a tuple, must define the on/off
+                sequence.
+
+    Returns
+    -------
+    vis :           gfx.Line
+                    Pygfx visuals for lines.
+
+    """
     if isinstance(lines, np.ndarray):
         assert lines.ndim == 2
         assert lines.shape[1] == 3
         assert len(lines) > 1
     elif isinstance(lines, list):
         assert all([isinstance(l, np.ndarray) for l in lines])
         assert all([l.ndim == 2 for l in lines])
         assert all([l.shape[1] == 3 for l in lines])
         assert all([len(l) > 1 for l in lines])
 
         # Convert to the (N, 3) format
         if len(lines) == 1:
             lines = lines[0]
         else:
-            lines = np.insert(np.vstack(lines), np.cumsum([len(l) for l in lines[:-1]]), np.nan, axis=0)
+            lines = np.insert(
+                np.vstack(lines),
+                np.cumsum([len(l) for l in lines[:-1]]),
+                np.nan,
+                axis=0,
+            )
     else:
         raise TypeError("Expected numpy array or list of numpy arrays.")
 
+    if dash_pattern is None:
+        dash_pattern = ()  # pygfx expects an empty tuple for solid lines
+    elif isinstance(dash_pattern, str):
+        if dash_pattern == "solid":
+            dash_pattern = ()
+        elif dash_pattern == "dashed":
+            dash_pattern = (5, 2)
+        elif dash_pattern == "dotted":
+            dash_pattern = (1, 2)
+        elif dash_pattern == "dashdot":
+            dash_pattern = (5, 2, 1, 2)
+        else:
+            raise ValueError(f"Unknown dash pattern: {dash_pattern}")
+
     geometry_kwargs = {}
     material_kwargs = {}
 
     # Parse color(s)
     if isinstance(color, np.ndarray) and color.ndim == 2:
         # If colors are provided for each node we have to make sure
         # that we also include `None` for the breaks in the segments
@@ -254,26 +426,29 @@
             if len(color) == n_points:
                 breaks = np.where(np.isnan(lines[:, 0]))[0]
                 for b in breaks:
                     color = np.insert(color, b, np.nan, axis=0)
             else:
                 raise ValueError(f"Got {len(color)} colors for {n_points} points.")
         color = color.astype(np.float32, copy=False)
-        geometry_kwargs['colors'] = color
-        material_kwargs['color_mode'] = 'vertex'
+        geometry_kwargs["colors"] = color
+        material_kwargs["color_mode"] = "vertex"
     else:
         if isinstance(color, np.ndarray):
             color = color.astype(np.float32, copy=False)
-        material_kwargs['color'] = color
+        material_kwargs["color"] = color
 
     vis = gfx.Line(
-        gfx.Geometry(positions=lines.astype(np.float32, copy=False),
-                     **geometry_kwargs),
-        gfx.LineMaterial(thickness=linewidth,
-                         **material_kwargs),
+        gfx.Geometry(positions=lines.astype(np.float32, copy=False), **geometry_kwargs),
+        gfx.LineMaterial(
+            thickness=linewidth,
+            thickness_space=linewidth_space,
+            dash_pattern=dash_pattern,
+            **material_kwargs,
+        ),
     )
 
     # Add custom attributes
     vis._object_type = "lines"
     vis._object_id = uuid.uuid4()
 
     return vis
@@ -303,19 +478,18 @@
             [0, 1]
         )  # uv.y = 1 - uv.y
         kwargs["texcoords"] = np.ascontiguousarray(wgpu_uv, dtype="f4")
     elif mesh.visual.kind == "vertex":
         kwargs["colors"] = np.ascontiguousarray(mesh.visual.vertex_colors, dtype="f4")
 
     # Generate the geometry
-    vis = gfx.Mesh(gfx.Geometry(**kwargs),
-                   gfx.MeshBasicMaterial())
+    vis = gfx.Mesh(gfx.Geometry(**kwargs), gfx.MeshPhongMaterial())
 
     # If we have a material (including a texture)
-    if hasattr(mesh.visual, 'material') and use_material:
+    if hasattr(mesh.visual, "material") and use_material:
         material = mesh.visual.material
         # The material can be a PBRMaterial or a SimpleMaterial
         # pygfx' helper method only supports PBRMaterials
         if isinstance(material, tm.visual.material.PBRMaterial):
             vis.material = gfx.material_from_trimesh(material)
         elif isinstance(material, tm.visual.material.SimpleMaterial):
             vis.material = simple_material_from_trimesh(material)
@@ -334,22 +508,22 @@
     Returns
     -------
     converted : Material
         The converted material.
 
     """
     if not isinstance(material, tm.visual.material.SimpleMaterial):
-         raise NotImplementedError()
+        raise NotImplementedError()
 
     gfx_material = gfx.MeshPhongMaterial(color=material.ambient / 255)
 
     gfx_material.shininess = material.glossiness
     gfx_material.specular = gfx.Color(*(material.specular / 255))
 
-    if hasattr(material, 'image'):
+    if hasattr(material, "image"):
         gfx_material.map = texture_from_pillow_image(material.image)
 
     gfx_material.side = "FRONT"
     return gfx_material
 
 
 def texture_from_pillow_image(image, dim=2, **kwargs):
@@ -371,42 +545,47 @@
     Returns
     -------
     image_texture : Texture
         A texture object representing the given image.
 
     """
     # If this is a palette image, convert it to RGBA
-    if getattr(image, 'mode', None) == 'P':
-        image = image.convert('RGBA')
+    if getattr(image, "mode", None) == "P":
+        image = image.convert("RGBA")
 
     m = memoryview(image.tobytes())
 
     im_channels = len(image.getbands())
     buffer_shape = image.size + (im_channels,)
 
     m = m.cast(m.format, shape=buffer_shape)
     return gfx.Texture(m, dim=dim, **kwargs)
 
+
 # Monkey-patch the pygfx texture_from_pillow_image function
 gfx.materials._compat.texture_from_pillow_image = texture_from_pillow_image
 
 
 def scene2gfx(scene):
     """Convert trimesh Scene to pygfx visuals."""
-    assert isinstance(scene, tm.scene.scene.Scene), f"Expected trimesh scene, got {type(scene)}."
+    assert isinstance(
+        scene, tm.scene.scene.Scene
+    ), f"Expected trimesh scene, got {type(scene)}."
 
     # Get all the geometry names
     gfx_geometries = {}
     visuals = []
     for node_name in scene.graph.nodes_geometry:
         transform, geometry_name = scene.graph[node_name]
 
         if geometry_name not in gfx_geometries:
             gfx_geometries[geometry_name] = trimesh2gfx(scene.geometry[geometry_name])
 
-        vis = gfx.Mesh(gfx_geometries[geometry_name].geometry,
-                       gfx_geometries[geometry_name].material)
+        vis = gfx.Mesh(
+            gfx_geometries[geometry_name].geometry,
+            gfx_geometries[geometry_name].material,
+        )
         vis.local.matrix = transform
 
         visuals.append(vis)
 
     return visuals
```

### Comparing `octarine3d-0.1.1/setup.py` & `octarine3d-0.1.2/setup.py`

 * *Files identical despite different names*

