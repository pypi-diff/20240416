# Comparing `tmp/TkEasyGUI-0.2.43.tar.gz` & `tmp/tkeasygui-0.2.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TkEasyGUI-0.2.43.tar", last modified: Thu Apr  4 13:09:38 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.44.tar", last modified: Mon Apr 15 03:38:14 2024, max compression
```

## Comparing `TkEasyGUI-0.2.43.tar` & `tkeasygui-0.2.44.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-04 13:09:38.248565 TkEasyGUI-0.2.43/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 TkEasyGUI-0.2.43/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     4996 2024-04-04 13:09:38.248268 TkEasyGUI-0.2.43/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     2567 2024-04-03 00:43:13.000000 TkEasyGUI-0.2.43/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-04 13:09:38.246442 TkEasyGUI-0.2.43/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      285 2024-03-25 13:03:18.000000 TkEasyGUI-0.2.43/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    16604 2024-04-02 14:45:10.000000 TkEasyGUI-0.2.43/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-04 13:09:36.000000 TkEasyGUI-0.2.43/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    98926 2024-04-03 23:59:06.000000 TkEasyGUI-0.2.43/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-04 13:09:38.247879 TkEasyGUI-0.2.43/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     4996 2024-04-04 13:09:38.000000 TkEasyGUI-0.2.43/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      281 2024-04-04 13:09:38.000000 TkEasyGUI-0.2.43/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-04 13:09:38.000000 TkEasyGUI-0.2.43/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        7 2024-04-04 13:09:38.000000 TkEasyGUI-0.2.43/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-04 13:09:38.000000 TkEasyGUI-0.2.43/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1331 2024-04-04 13:09:27.000000 TkEasyGUI-0.2.43/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-04 13:09:38.248637 TkEasyGUI-0.2.43/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-15 03:38:14.129075 tkeasygui-0.2.44/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.44/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-15 03:38:14.128792 tkeasygui-0.2.44/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2975 2024-04-15 03:34:58.000000 tkeasygui-0.2.44/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-15 03:38:14.126428 tkeasygui-0.2.44/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      329 2024-04-14 07:30:36.000000 tkeasygui-0.2.44/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    16604 2024-04-02 14:45:10.000000 tkeasygui-0.2.44/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      188 2024-04-14 12:33:36.000000 tkeasygui-0.2.44/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-15 03:38:11.000000 tkeasygui-0.2.44/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   107539 2024-04-15 03:24:03.000000 tkeasygui-0.2.44/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-15 03:38:14.128459 tkeasygui-0.2.44/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     5429 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      300 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-15 03:38:14.000000 tkeasygui-0.2.44/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1346 2024-04-15 03:37:59.000000 tkeasygui-0.2.44/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-15 03:38:14.129151 tkeasygui-0.2.44/setup.cfg
```

### Comparing `TkEasyGUI-0.2.43/LICENSE` & `tkeasygui-0.2.44/LICENSE`

 * *Files identical despite different names*

### Comparing `TkEasyGUI-0.2.43/PKG-INFO` & `tkeasygui-0.2.44/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.43
+Version: 0.2.44
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -41,14 +41,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
+Requires-Dist: pyperclip
 
 # TkEasyGUI
 
 `TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
 In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
 Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
@@ -81,33 +82,46 @@
 
 ## How to use
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
+# define layout
+layout = [[eg.Text("Hello, World!")],
+          [eg.Button("Exit")]]
+# create a window
+with eg.Window("test", layout) as window:
+    # event loop
+    for event, values in window.event_iter():
+        if event == "Exit":
+            eg.popup("Thank you.")
+            break
+```
+
+You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
-# Create window
-layout = [
-    [eg.Text("Hello, World!")],
-    [eg.Button("OK")]
-]
-window = eg.Window("Hello", layout=layout)
-
-# Event loop
-while window.is_alive():
-    # get event
+```py
+import TkEasyGUI as eg
+# define layout
+layout = [[eg.Text("Hello, World!")],
+          [eg.Button("Exit")]]
+# create a window
+window = eg.Window("test", layout)
+# event loop
+while True:
     event, values = window.read()
-    # check event
-    if event == "OK":
-        eg.popup("Pushed OK Button")
+    if event in ["Exit", eg.WINDOW_CLOSED]:
+        eg.popup("Thank you.")
         break
+# close window
 window.close()
 ```
 
+
 ## Samples
 
 We have prepared a selection of samples to demonstrate simple usage. Please check them out.
 
 - [samples](https://github.com/kujirahand/tkeasygui-python/tree/main/tests).
 
 ## Documents
```

### Comparing `TkEasyGUI-0.2.43/README.md` & `tkeasygui-0.2.44/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,33 +33,46 @@
 
 ## How to use
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
+# define layout
+layout = [[eg.Text("Hello, World!")],
+          [eg.Button("Exit")]]
+# create a window
+with eg.Window("test", layout) as window:
+    # event loop
+    for event, values in window.event_iter():
+        if event == "Exit":
+            eg.popup("Thank you.")
+            break
+```
+
+You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
-# Create window
-layout = [
-    [eg.Text("Hello, World!")],
-    [eg.Button("OK")]
-]
-window = eg.Window("Hello", layout=layout)
-
-# Event loop
-while window.is_alive():
-    # get event
+```py
+import TkEasyGUI as eg
+# define layout
+layout = [[eg.Text("Hello, World!")],
+          [eg.Button("Exit")]]
+# create a window
+window = eg.Window("test", layout)
+# event loop
+while True:
     event, values = window.read()
-    # check event
-    if event == "OK":
-        eg.popup("Pushed OK Button")
+    if event in ["Exit", eg.WINDOW_CLOSED]:
+        eg.popup("Thank you.")
         break
+# close window
 window.close()
 ```
 
+
 ## Samples
 
 We have prepared a selection of samples to demonstrate simple usage. Please check them out.
 
 - [samples](https://github.com/kujirahand/tkeasygui-python/tree/main/tests).
 
 ## Documents
```

### Comparing `TkEasyGUI-0.2.43/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.44/TkEasyGUI/dialogs.py`

 * *Files identical despite different names*

### Comparing `TkEasyGUI-0.2.43/TkEasyGUI/widgets.py` & `tkeasygui-0.2.44/TkEasyGUI/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 """
 import io
 import os
 import platform
 import sys
 import tkinter as tk
 import tkinter.font as tkfont
+from tkinter import scrolledtext
 from datetime import datetime
 from queue import Queue
 from tkinter import ttk
-from typing import Any, Literal, TypeAlias, Union
-
+from typing import Any, Literal, TypeAlias, Union, Generator
 from PIL import Image as PILImage
 from PIL import ImageTk
 
-import TkEasyGUI as eg
+from . import utils
+from . import dialogs
 
 #------------------------------------------------------------------------------
 # Const
 #------------------------------------------------------------------------------
 WINDOW_CLOSED: str = "WINDOW_CLOSED"
 WIN_CLOSED: str = "WINDOW_CLOSED"
 WINDOW_TIMEOUT: str = "-TIMEOUT-"
@@ -93,14 +94,24 @@
         set_theme("aqua")
     elif is_win():
         # set_theme("winnative")
         set_theme("vista")
     else:
         set_theme("clam")
 
+def convert_color_rgb16(color_name: str) -> tuple[int, int, int]:
+    """Convert color to RGB, return (r, g, b) tuple. range=0-65535"""
+    root = get_root_window()
+    return root.winfo_rgb(color_name)
+
+def convert_color_html(color_name: str) -> str:
+    """Convert RGB color(16bit tuple) to HTML color name."""
+    r, g, b = convert_color_rgb16(color_name)
+    return f"#{r//256:02x}{g//256:02x}{b//256:02x}"
+
 #------------------------------------------------------------------------------
 # Widget wrapper
 #------------------------------------------------------------------------------
 class TkEasyError(Exception):
     def __init__(self, message="TkEasyError"):
         self.message = message
         super().__init__(self.message)
@@ -250,14 +261,22 @@
         else:
             if isinstance(self.window, tk.Tk):
                 self.window.eval('tk::PlaceWindow . center')
         # push window
         if not modal:
             _window_push(self)
     
+    def __enter__(self):
+        """Initialize resource"""
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Finalize resource"""
+        self.close()
+    
     def register_event_hooks(self, hooks: dict[str, list[callable]]) -> None:
         """
         [Window.register_event_hooks] Register event hooks. (append events)
         **Example**
         ```
         window.register_event_hooks({
             "-input-": [
@@ -352,15 +371,14 @@
                 # pady
                 if elem.pady is not None:
                     row_prop["pady"] = elem.pady
             # add row
             frame_row.pack(**row_prop)
         # end of create
         if self.need_focus_widget is not None:
-            # print("focus_set", self.need_focus_widget)
             self.need_focus_widget.focus_set()
 
     def move_to_center(self) -> None:
         """Move the window to the center of the screen."""
         if isinstance(self.window, tk.Tk):
             self.window.eval('tk::PlaceWindow . center')
 
@@ -407,14 +425,32 @@
         if key in self._event_hooks:
             flag_stop = self._dispatch_event_hooks(key, values)
             if flag_stop:
                 key = f"{key}-stopped" # change event name
                 values = self.get_values() # collect values again
         return (key, values)
     
+    def event_iter(self, timeout: int|None=None, timeout_key: str=TIMEOUT_KEY) -> Any:
+        """
+        Return generator with event and values
+        **Example**
+        ```py
+        import TkEasyGUI as eg
+        # create a window
+        with eg.Window("test", layout=[[eg.Button("Hello")]]) as window:
+            # event loop
+            for event, values in window.event_iter():
+                if event == "Hello":
+                    eg.popup("Hello, World!")
+        ```
+       """
+        while self.is_alive():
+            event, values = self.read(timeout=timeout, timeout_key=timeout_key)
+            yield (event, values)
+    
     def _dispatch_event_hooks(self, key: str, values: dict[str, Any]) -> bool:
         """Dispatch event hooks."""
         # execute _event_hooks
         flag_stop = False
         if key in self._event_hooks:
             for handle in self._event_hooks[key]:
                 result = handle(key, values)
@@ -594,16 +630,14 @@
         """Start move window"""
         self._grab_flag = True
         loc = self.window.geometry().split("+")
         self._start_x = int(loc[1])
         self._start_y = int(loc[2])
         self._mouse_x = self.window.winfo_x() + event.x
         self._mouse_y = self.window.winfo_y() + event.y
-        # print(f"_start_xy={self._start_x}x{self._start_y}")
-        # print(f"_mouse_xy={self._mouse_x}x{self._mouse_y}")
     
     def _stop_move_window(self, event: tk.Event) -> None:
         """Stop move window"""
         self._grab_flag = False
     
     def bind(self, element: "Element", event_name: str, handle_name: str, propagate: bool=True, event_mode: EventMode = "user") -> None:
         """[Window.bind] Bind element event and handler"""
@@ -792,15 +826,14 @@
         if self.padx is not None:
             props["padx"] = self.padx
         if self.pady is not None:
             props["pady"] = self.pady
         # anchor
         if self.anchor is not None:
             props["anchor"] = self.anchor
-        # print("pack.props=", self.key, props)
         return props
 
     def convert_props(self, props: dict[str, Any]) -> dict[str, Any]:
         result = {}
         # copy
         for key, val in props.items():
             result[key] = val
@@ -938,15 +971,14 @@
             self.props[k] = v
         kw = self.convert_props(kw)
         try:
             if (self.widget is not None)and(len(kw) > 0):
                 self.widget.configure(**kw)
         except Exception as e:
             print(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}", file=sys.stderr)
-            # raise TkEasyError(f"TkEasyGUI.Element.widget_update.Error: key='{self.key}', try to update {kw}, {e}")
 
     def get_prev_widget(self, target_key: str|None=None) -> tk.Widget:
         """Get the previous widget."""
         # check target_key
         target: tk.Widget = None
         if target_key:
             if target_key in self.window.key_elements:
@@ -1209,23 +1241,21 @@
             state=state,
             command=lambda : self.disptach_event({EG_SWAP_EVENT_NAME: key}))
 
     def _create_menu(self, parent: tk.Menu, items: list[list[str|list[Any]]], level:int = 0) -> None:
         i = 0
         while i < len(items):
             item = items[i]
-            # print(f"{'-' * level}[{i}].{item}")
             if isinstance(item, int) or isinstance(item, float):
                 item = str(item)
             if isinstance(item, str):
                 # check next item
                 next_item = items[i+1] if i+1 < len(items) else None
                 if (next_item is None) or (not isinstance(next_item, list)):
                     self._add_command(parent, item)
-                    # print(f"{'-' * level} add_command label={item}")
                     i += 1
                     continue
                 else: # if isinstance(next_item, list):
                     # submenu
                     submenu = tk.Menu(parent, tearoff=False)
                     parent.add_cascade(label=item, menu=submenu)
                     self._create_menu(submenu, next_item, level+1)
@@ -1413,15 +1443,14 @@
         if len(args) >= 1:
             self.set_value(args[0])
         if len(args) >= 2:
             self.set_text(args[1])
         if "text" in kw:
             self.set_text(kw.pop("text"))
         if "value" in kw:
-            print("set_value", kw)
             self.set_value(kw.pop("value"))
         self.widget_update(**kw)
 
 class Radio(Element):
     """Checkbox element."""
     def __init__(
                 self, text: str="",
@@ -1547,17 +1576,19 @@
                 "<FocusOut>": "focusout",
                 "<Button-1>": "click",
                 "<Button-3>": "right_click"
             }, "system")
     
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """create Input widget"""
+        # check props
+        if "height" in self.props:
+            self.props.pop("height") # no property
         # set default text
         self.text_var = tk.StringVar(value=self.default_text)
-        print(self.text_var.get())
         # create
         self.widget = ttk.Entry(
             parent,
             textvariable=self.text_var,
             style=self.style_name,
             **self.props)
         # set readonly
@@ -1570,25 +1601,41 @@
         return self.widget
 
     def get(self) -> Any:
         """Get the value of the widget."""
         return self.get_text()
     
     def set_text(self, text: str) -> None:
+        """set text"""
         if self.widget is None:
             return
         # change text
         self.widget.config(textvariable=self.text_var)
         self.text_var.set(text)
         #  OR
         #   self.delete(0, "end")
         #   self.insert(0, text)
 
     def get_text(self) -> str:
+        """get text"""
         return self.text_var.get()
+    
+    def get_selected_text(self) -> str:
+        """get selected text"""
+        if self.widget is None:
+            return ""
+        try:
+            return self.widget.selection_get()
+        except Exception as e:
+            return ""
+
+    def copy_selected_text(self) -> None:
+        """Copy selected text"""
+        text = self.get_selected_text()
+        utils.set_clipboard(text)
 
     def set_readonly(self, readonly: bool) -> None:
         """set readonly"""
         self.readonly = readonly
         state = "readonly" if self.readonly else "normal"
         self.widget_update(state=state)
 
@@ -1605,14 +1652,108 @@
                 self.set_readonly(False)
                 self.set_text(text)
                 self.set_readonly(True)
             else:
                 self.set_text(text)
         # update others
         self.widget_update(**kw)
+    
+    def select_all(self) -> None:
+        """select_all"""
+        if self.widget is None:
+            return
+        input: tk.Entry = self.widget
+        input.select_range(0, "end")
+        input.icursor("end")
+    
+    def copy(self) -> str:
+        """copy to clipboard"""
+        if self.widget is None:
+            return
+        text = self.get_selected_text()
+        utils.set_clipboard(text)
+        return text
+
+    def cut(self) -> str:
+        """cut to clipboard"""
+        if self.widget is None:
+            return
+        self.copy()
+        return self.delete_selected()
+    
+    def delete_selected(self) -> str:
+        """delete selected text"""
+        if self.widget is None:
+            return
+        try:
+            text = self.get_selected_text()
+            self.widget.delete(tk.SEL_FIRST, tk.SEL_LAST)
+        except Exception as _:
+            return ""
+        return text
+
+    def paste(self):
+        """paste from clipboard"""
+        if self.widget is None:
+            return
+        # delete selected
+        self.delete_selected()
+        # insert
+        text = utils.get_clipboard()
+        input: tk.Entry = self.widget
+        current_cursor_position = input.index(tk.INSERT)
+        input.insert(current_cursor_position, text)
+    
+    def get_selection_pos(self) -> tuple[int, int]:
+        """get selection positions"""
+        try:
+            entry: tk.Entry = self.widget
+            start_pos = entry.index(tk.SEL_FIRST)
+            end_pos = entry.index(tk.SEL_LAST)
+            return start_pos, end_pos
+        except Exception as _:
+            cur = self.get_cursor_pos()
+            return [cur, cur]
+    
+    def get_cursor_pos(self) -> int:
+        """get cursor position"""
+        cursor_pos = self.widget.index(tk.INSERT)
+        return cursor_pos
+
+    def set_cursor_pos(self, index: int) -> None:
+        """set cursor position"""
+        self.widget.icursor(index)
+ 
+    def get_selection_start(self) -> int:
+        """get selection start"""
+        try:
+            entry: tk.Entry = self.widget
+            start_pos = entry.index(tk.SEL_FIRST)
+            return start_pos
+        except Exception as _:
+            return self.get_cursor_pos()
+
+    def get_selection_length(self) -> tuple[int, int]:
+        """get selection length"""
+        try:
+            entry: tk.Entry = self.widget
+            start_pos = entry.index(tk.SEL_FIRST)
+            end_pos = entry.index(tk.SEL_LAST)
+            return end_pos - start_pos
+        except Exception as _:
+            return 0
+    
+    def set_selection_start(self, sel_start: int, sel_length: int=0) -> None:
+        """set selection start and length"""
+        try:
+            entry: tk.Entry = self.widget
+            sel_end = sel_start + sel_length
+            entry.selection_range(sel_start, sel_end)
+        except Exception as _:
+            pass
 
 class InputText(Input):
     """InputText element. (alias of Input)"""
     pass
 
 class Multiline(Element):
     """Multiline text input element."""
@@ -1665,42 +1806,75 @@
                 "<FocusIn>": "focusin",
                 "<FocusOut>": "focusout",
                 "<Button-1>": "click",
                 "<Button-3>": "right_click"
             }, "system")
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
-        # frame
-        self.widget_frame = widget_frame = ttk.Frame(parent)
+        """Create a Multiline widget."""
         # text
         text = self.props.pop("text", "")
-        self.widget = tk.Text(widget_frame, **self.props)
+        # create
+        self.widget = scrolledtext.ScrolledText(parent, **self.props)
+        # set text
         self.widget.insert("1.0", text)
         # readonly
         if self.readonly:
             self.set_readonly(self.readonly)
-        # scrollbar
-        self.scrollbar = ttk.Scrollbar(widget_frame, orient="vertical", command=self.widget.yview)
-        self.widget.configure(yscrollcommand=self.scrollbar.set)
-        # pack to frame
-        self.scrollbar.pack(side="right", fill="y")
-        self.widget.pack(side="right", fill="both", expand=True)
-        return self.widget_frame
+        return self.widget
 
     def get(self) -> Any:
         """Get the value of the widget."""
         if self.widget is None:
             return ""
         return self.get_text()
     
     def get_text(self) -> str:
+        """Get the text of the widget."""
         if self.widget is None:
             return ""
         text = self.widget.get("1.0", "end -1c") # get all text
         return text
+    
+    def get_selected_text(self) -> str:
+        """Get the selected text."""
+        if self.widget is None:
+            return ""
+        try:
+            text = self.widget.selection_get()
+        except Exception as e:
+            text = ""
+        return text
+    
+    def copy(self) -> str:
+        """Copy the selected text."""
+        if self.widget is None:
+            return
+        text = self.get_selected_text()
+        utils.set_clipboard(text)
+        return text
+    
+    def paste(self) -> None:
+        """Paste the text."""
+        if self.widget is None:
+            return
+        text = utils.get_clipboard()
+        self.widget.insert(tk.INSERT, text)
+        self.widget.tag_remove(tk.SEL, '1.0', tk.END) 
+        self.widget.see(tk.INSERT)
+
+    def cut(self) -> str:
+        """Cut the selected text."""
+        if self.widget is None:
+            return
+        text = ""
+        if self.widget.tag_ranges(tk.SEL):
+            text = self.copy()
+            self.widget.delete(tk.SEL_FIRST, tk.SEL_LAST)
+        return text
 
     def update(self, text: str|None = None, readonly: bool|None = None, **kw) -> None:
         """Update the widget."""
         if text is not None:
             self.set_text(text)
         if readonly is not None:
             self.set_readonly(readonly)
@@ -1720,29 +1894,139 @@
             self.widget_update(state=tk.NORMAL)
         self.props["text"] = text
         self.widget.delete("1.0", "end") # clear text
         self.widget.insert("1.0", text) # set text
         if self.readonly:
             self.widget_update(state=tk.DISABLED)
     
+    def get_selection_pos(self) -> tuple[str, str]:
+        """Get selection position, returns (start_pos, end_pos)."""
+        if self.widget is None:
+            return ("", "")
+        try:
+            sel_start, sel_end = self.widget.tag_ranges("sel")
+            return (sel_start, sel_end)
+        except Exception as _:
+            pos = self.get_cursor_pos()
+            return (pos, pos)
+
+    def set_selection_pos(self, start_pos: str, end_pos: str) -> None:
+        """Set selection position."""
+        if self.widget is None:
+            return
+        try:
+            text: tk.Text = self.widget
+            text.tag_remove('sel', "1.0", "end")
+            text.tag_add('sel', start_pos, end_pos)
+        except Exception as _:
+            self.set_cursor_pos(start_pos)
+
+    def pos_to_index(self, pos: str) -> str:
+        """Convert position to index."""
+        row, col = pos.split(".")
+        row, col = int(row), int(col)
+        text = self.get_text()
+        retcode = "\r\n" if "\r\n" in text else "\n"
+        retcode_len = len(retcode)
+        start = 0
+        for i, line in enumerate(text.split("\n")):
+            if (row - 1) == i:
+                start += col
+                break
+            start += len(line) + retcode_len
+        return start
+
+    def index_to_pos(self, index: int) -> str:
+        """Convert index to postion."""
+        text = self.get_text()
+        retcode = "\r\n" if "\r\n" in text else "\n"
+        retcode_len = len(retcode)
+        row = 1
+        col = 0
+        start = 0
+        for line_no, line in enumerate(text.split("\n")):
+            line_start = start
+            line_end = line_start + len(line) + retcode_len
+            start = line_end
+            if index < line_end:
+                row = line_no + 1
+                col = index - line_start
+                break
+        return f"{row}.{col}"
+
+    def get_cursor_pos(self) -> str:
+        """Get Cursor position. liek `3.0` row=3, col=0"""
+        if self.widget is None:
+            return 0
+        try:
+            cur = self.widget.index("insert")
+        except Exception as _:
+            cur = ""
+        return cur
+
+    def set_cursor_pos(self, pos: str) -> None:
+        """Set cursor position. (like `3.0`, row=3, col=0)"""
+        if self.widget is None:
+            return
+        self.widget.mark_set(tk.INSERT, pos)
+
+    def get_selection_start(self) -> int:
+        """get selection start"""
+        if self.widget is None:
+            return 0
+        try:
+            sel_start, _ = self.widget.tag_ranges("sel")
+            return self.pos_to_index(sel_start)
+        except Exception as _:
+            pos = self.get_cursor_pos()
+            return self.pos_to_index(pos)
+        
+    def set_selection_start(self, index: int, sel_length: int=0) -> None:
+        """set selection start"""
+        pos1 = self.index_to_pos(index)
+        pos2 = self.index_to_pos(index + sel_length)
+        if sel_length > 0:
+            self.set_selection_pos(pos1, pos2)
+        else:
+            self.set_cursor_pos(pos1)
+
+    def get_selection_length(self) -> int:
+        """get selection length"""
+        if self.widget is None:
+            return 0
+        try:
+            text = self.get_selected_text()
+            return len(text)
+        except Exception as _:
+            return 0
+
+    def select_all(self) -> None:
+        """select all text"""
+        if self.widget is None:
+            return
+        text: tk.Text = self.widget
+        text.tag_add(tk.SEL, "1.0", tk.END)
+        text.mark_set(tk.INSERT, '1.0')
+        self.widget.see(tk.INSERT)
+        print("@select_all")
+
     def print(self, text: str, text_color: str|None=None, background_color: str|None=None, end:str="\n") -> None:
         """Print text."""
         text += end
         if self.widget is None:
             return
         tags: list[str] = []
         if text_color is not None:
             tag = generate_element_style_key("--multiline-text_color")
             self.widget.tag_config(tag, foreground=text_color)
             tags.append(tag)
         if background_color is not None:
             tag = generate_element_style_key("--multiline-background_color")
             self.widget.tag_config(tag, background=background_color)
             tags.append(tag)
-        print(tags)
         self.widget.insert("end", text, tags)
 
 class Textarea(Multiline):
     """Textarea element. (alias of Multiline)"""
     pass
 
 class Output(Multiline):
@@ -2403,15 +2687,15 @@
 
     def show_dialog(self, *args) -> str|None:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # get initial directory
         init_dir = self._get_initial_directory()
         # popup
-        result = eg.popup_get_file(
+        result = dialogs.popup_get_file(
             title=self.title,
             initial_folder=init_dir,
             save_as=self.save_as,
             file_types=self.file_types,
             multiple_files=self.multiple_files,
         )
         if isinstance(result, list) or isinstance(result, tuple):
@@ -2498,15 +2782,15 @@
         self.default_path = default_path
         self.props["text"] = button_text
     
     def show_dialog(self, *args) -> str|None:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # popup
-        result = eg.popup_get_folder(
+        result = dialogs.popup_get_folder(
             title=self.title,
             default_path=self.default_path,
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
         return result
 
@@ -2529,15 +2813,15 @@
         self.default_color = default_color
         self.props["text"] = button_text
     
     def show_dialog(self, *args) -> str|None:
         """Show file dialog"""
         target: tk.Widget = self.get_prev_widget(self.target_key)
         # popup
-        result = eg.popup_color(
+        result = dialogs.popup_color(
             title=self.title,
             default_color=self.default_color,
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
         return result
```

### Comparing `TkEasyGUI-0.2.43/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.44/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.43
+Version: 0.2.44
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -41,14 +41,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Pillow
+Requires-Dist: pyperclip
 
 # TkEasyGUI
 
 `TkEasyGUI` is a Python library that allows for the easy and simple creation of GUI applications.
 In the event model, it is compatible with the well-known GUI library `PySimpleGUI`.
 
 Python's standard UI library `Tkinter`, is often considered to have a high barrier to entry and to be difficult to use. By using this library, you can create GUI applications easily and intuitively.
@@ -81,33 +82,46 @@
 
 ## How to use
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
+# define layout
+layout = [[eg.Text("Hello, World!")],
+          [eg.Button("Exit")]]
+# create a window
+with eg.Window("test", layout) as window:
+    # event loop
+    for event, values in window.event_iter():
+        if event == "Exit":
+            eg.popup("Thank you.")
+            break
+```
+
+You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
-# Create window
-layout = [
-    [eg.Text("Hello, World!")],
-    [eg.Button("OK")]
-]
-window = eg.Window("Hello", layout=layout)
-
-# Event loop
-while window.is_alive():
-    # get event
+```py
+import TkEasyGUI as eg
+# define layout
+layout = [[eg.Text("Hello, World!")],
+          [eg.Button("Exit")]]
+# create a window
+window = eg.Window("test", layout)
+# event loop
+while True:
     event, values = window.read()
-    # check event
-    if event == "OK":
-        eg.popup("Pushed OK Button")
+    if event in ["Exit", eg.WINDOW_CLOSED]:
+        eg.popup("Thank you.")
         break
+# close window
 window.close()
 ```
 
+
 ## Samples
 
 We have prepared a selection of samples to demonstrate simple usage. Please check them out.
 
 - [samples](https://github.com/kujirahand/tkeasygui-python/tree/main/tests).
 
 ## Documents
```

### Comparing `TkEasyGUI-0.2.43/pyproject.toml` & `tkeasygui-0.2.44/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.43"
+version = "0.2.44"
 dependencies = [
   "Pillow",
+  "pyperclip",
 ]
 requires-python = ">=3.8"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
 ]
 maintainers = [
  { name="kujirahand", email="web@kujirahand.com" },
```

