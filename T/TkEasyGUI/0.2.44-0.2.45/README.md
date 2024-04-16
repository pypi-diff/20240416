# Comparing `tmp/tkeasygui-0.2.44.tar.gz` & `tmp/tkeasygui-0.2.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.44.tar", last modified: Mon Apr 15 03:38:14 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.45.tar", last modified: Tue Apr 16 00:08:49 2024, max compression
```

## Comparing `tkeasygui-0.2.44.tar` & `tkeasygui-0.2.45.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-15 03:38:14.129075 tkeasygui-0.2.44/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.44/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-15 03:38:14.128792 tkeasygui-0.2.44/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     2975 2024-04-15 03:34:58.000000 tkeasygui-0.2.44/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-15 03:38:14.126428 tkeasygui-0.2.44/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.44/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    16604 2024-04-02 14:45:10.000000 tkeasygui-0.2.44/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      188 2024-04-14 12:33:36.000000 tkeasygui-0.2.44/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-15 03:38:11.000000 tkeasygui-0.2.44/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   107539 2024-04-15 03:24:03.000000 tkeasygui-0.2.44/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-15 03:38:14.128459 tkeasygui-0.2.44/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1346 2024-04-15 03:37:59.000000 tkeasygui-0.2.44/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-15 03:38:14.129151 tkeasygui-0.2.44/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 00:08:49.133697 tkeasygui-0.2.45/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.45/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-16 00:08:49.133415 tkeasygui-0.2.45/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2975 2024-04-15 03:34:58.000000 tkeasygui-0.2.45/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 00:08:49.132094 tkeasygui-0.2.45/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.45/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    16604 2024-04-02 14:45:10.000000 tkeasygui-0.2.45/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      188 2024-04-14 12:33:36.000000 tkeasygui-0.2.45/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-16 00:08:47.000000 tkeasygui-0.2.45/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   108336 2024-04-15 23:41:53.000000 tkeasygui-0.2.45/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-16 00:08:49.133135 tkeasygui-0.2.45/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-16 00:08:49.000000 tkeasygui-0.2.45/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1346 2024-04-16 00:08:41.000000 tkeasygui-0.2.45/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-16 00:08:49.133753 tkeasygui-0.2.45/setup.cfg
```

### Comparing `tkeasygui-0.2.44/LICENSE` & `tkeasygui-0.2.45/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.44/PKG-INFO` & `tkeasygui-0.2.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.44
+Version: 0.2.45
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.44/README.md` & `tkeasygui-0.2.45/README.md`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.44/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.45/TkEasyGUI/dialogs.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.44/TkEasyGUI/widgets.py` & `tkeasygui-0.2.45/TkEasyGUI/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
 WINDOW_TIMEOUT: str = "-TIMEOUT-"
 TIMEOUT_KEY: str = WINDOW_TIMEOUT
+WINDOW_KEY_EVENT: str = "-WINDOW_KEY_EVENT-"
 LISTBOX_SELECT_MODE_MULTIPLE: str = "multiple"
 LISTBOX_SELECT_MODE_BROWSE: str = "browse"
 LISTBOX_SELECT_MODE_EXTENDED: str = "extended"
 LISTBOX_SELECT_MODE_SINGLE: str = "single"
 TABLE_SELECT_MODE_NONE: str = tk.NONE
 TABLE_SELECT_MODE_BROWSE: str = tk.BROWSE
 TABLE_SELECT_MODE_EXTENDED: str = tk.EXTENDED
@@ -190,14 +191,16 @@
                 resizable:bool=False,
                 font:FontType|None=None,
                 modal: bool=False, 
                 keep_on_top:bool=False, # keep on top
                 no_titlebar: bool=False, # hide titlebar
                 grab_anywhere: bool=False, # can move window by dragging anywhere
                 alpha_channel: float=1.0,
+                enable_key_events: bool=False, # enable keyboard events
+                return_keyboard_events: bool=False, # enable keyboard events (for compatibility)
                 **kw) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = _get_active_window()
         if active_win is None:
             active_win = get_root_window()
@@ -222,14 +225,16 @@
         self._grab_anywhere: bool = grab_anywhere
         self._grab_flag: bool = False
         self._start_x: int|None = None
         self._start_y: int|None = None
         self._mouse_x: int|None = None
         self._mouse_y: int|None = None
         self.alpha_channel: float = alpha_channel
+        self.enable_key_events: bool = enable_key_events
+        self.return_keyboard_events: bool = return_keyboard_events
         # Frame
         self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         if size is not None:
             self.window.geometry(f"{size[0]}x{size[1]}")
@@ -243,14 +248,22 @@
             self.window.attributes("-topmost", True)
         if no_titlebar:
             self.hide_titlebar(True)
         if grab_anywhere:
             self.set_grab_anywhere(True)
         if alpha_channel < 1.0:
             self.set_alpha_channel(alpha_channel)
+        # bind events
+        if self.enable_key_events:
+            self.window.bind("<Key>", lambda e: self._event_handler(
+                WINDOW_KEY_EVENT,
+                {"event": e, "key": e.keysym, "event_type": "key"}))
+        if self.return_keyboard_events: # for compatibility with PySimpleGUI
+            self.window.bind("<Key>", lambda e: self._event_handler(
+                e.keysym if len(e.keysym) == 1 else f"{e.keysym}:{e.keycode}", {}))
         # check modal
         if modal:
             # check position
             parent = active_win
             if parent is not None:
                 self.window.geometry(f"+{parent.winfo_x()+20}+{parent.winfo_y()+20}")
             # set modal action
```

### Comparing `tkeasygui-0.2.44/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.45/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.44
+Version: 0.2.45
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
```

### Comparing `tkeasygui-0.2.44/pyproject.toml` & `tkeasygui-0.2.45/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.44"
+version = "0.2.45"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.8"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

