# Comparing `tmp/spotidex-0.0.7.tar.gz` & `tmp/spotidex-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotidex-0.0.7.tar", max compression
+gzip compressed data, was "spotidex-1.0.0.tar", max compression
```

## Comparing `spotidex-0.0.7.tar` & `spotidex-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      552 2024-04-13 17:30:43.922225 spotidex-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      499 2024-04-06 09:42:27.400268 spotidex-0.0.7/README.md
--rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-0.0.7/spotidex/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-0.0.7/spotidex/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-0.0.7/spotidex/cli/app_screens/__init__.py
--rw-r--r--   0        0        0     6908 2024-04-12 11:27:13.657978 spotidex-0.0.7/spotidex/cli/app_screens/DownloadInterface.py
--rw-r--r--   0        0        0     4674 2024-04-12 12:43:31.490186 spotidex-0.0.7/spotidex/cli/app_screens/MainMenuInterface.py
--rw-r--r--   0        0        0     5719 2024-04-13 12:46:07.764636 spotidex-0.0.7/spotidex/cli/app_screens/SearchInterface.py
--rw-r--r--   0        0        0     4053 2024-04-13 05:48:36.635880 spotidex-0.0.7/spotidex/cli/app_screens/SelectDownloadInterface.py
--rw-r--r--   0        0        0     2450 2024-04-13 05:23:06.441432 spotidex-0.0.7/spotidex/cli/app_screens/SettingsInterface.py
--rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-0.0.7/spotidex/cli/custom_widgets/__init__.py
--rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
--rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
--rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
--rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
--rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
--rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
--rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
--rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
--rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
--rw-r--r--   0        0        0     4510 2024-04-10 14:45:36.699352 spotidex-0.0.7/spotidex/cli/custom_widgets/AppInterface.py
--rw-r--r--   0        0        0     1467 2024-04-10 18:25:15.239179 spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadPathSelector.py
--rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadQualitySelection.py
--rw-r--r--   0        0        0     1854 2024-04-12 10:43:16.844163 spotidex-0.0.7/spotidex/cli/custom_widgets/MetadataCheckBox.py
--rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-0.0.7/spotidex/cli/popup_screens/__init__.py
--rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
--rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
--rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
--rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
--rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
--rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
--rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
--rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
--rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
--rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
--rw-r--r--   0        0        0     4303 2024-04-13 05:59:34.299624 spotidex-0.0.7/spotidex/cli/popup_screens/DownloadPathPopup.py
--rw-r--r--   0        0        0     1135 2024-04-10 14:45:53.954177 spotidex-0.0.7/spotidex/cli/popup_screens/ExitScreenPopup.py
--rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-0.0.7/spotidex/cli/popup_screens/GoBackSettingsPopup.py
--rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-0.0.7/spotidex/cli/popup_screens/NetworkErrorPopup.py
--rw-r--r--   0        0        0      700 2024-04-10 18:25:42.766710 spotidex-0.0.7/spotidex/cli/SpotidexApp.py
--rw-r--r--   0        0        0     4619 2024-04-13 17:10:46.966551 spotidex-0.0.7/spotidex/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-0.0.7/spotidex/src/__init__.py
--rw-r--r--   0        0        0     5841 2024-04-13 16:54:40.790363 spotidex-0.0.7/spotidex/src/content.py
--rw-r--r--   0        0        0     6847 2024-04-13 17:27:05.680218 spotidex-0.0.7/spotidex/src/download.py
--rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-0.0.7/spotidex/src/static.py
--rw-r--r--   0        0        0     5057 2024-04-13 16:42:59.190419 spotidex-0.0.7/spotidex/src/utils.py
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 spotidex-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      725 2024-04-16 06:38:36.612704 spotidex-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1793 2024-04-16 06:32:25.340903 spotidex-1.0.0/README.md
+-rw-r--r--   0        0        0      121 2024-04-07 04:09:46.405092 spotidex-1.0.0/spotidex/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:04:49.449417 spotidex-1.0.0/spotidex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 10:54:48.391174 spotidex-1.0.0/spotidex/cli/app_screens/__init__.py
+-rw-r--r--   0        0        0     6921 2024-04-15 17:51:44.234430 spotidex-1.0.0/spotidex/cli/app_screens/DownloadInterface.py
+-rw-r--r--   0        0        0     4674 2024-04-12 12:43:31.490186 spotidex-1.0.0/spotidex/cli/app_screens/MainMenuInterface.py
+-rw-r--r--   0        0        0     5777 2024-04-15 18:55:16.254811 spotidex-1.0.0/spotidex/cli/app_screens/SearchInterface.py
+-rw-r--r--   0        0        0     4053 2024-04-13 05:48:36.635880 spotidex-1.0.0/spotidex/cli/app_screens/SelectDownloadInterface.py
+-rw-r--r--   0        0        0     2450 2024-04-13 05:23:06.441432 spotidex-1.0.0/spotidex/cli/app_screens/SettingsInterface.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:37.274535 spotidex-1.0.0/spotidex/cli/custom_widgets/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-06 10:24:05.804875 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     6639 2024-04-05 01:25:43.428330 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc
+-rw-r--r--   0        0        0     7051 2024-04-06 08:37:17.715706 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc
+-rw-r--r--   0        0        0     2802 2024-03-26 10:59:06.959928 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc
+-rw-r--r--   0        0        0     2858 2024-03-26 11:49:33.182036 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc
+-rw-r--r--   0        0        0     2705 2024-04-06 10:40:56.495563 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc
+-rw-r--r--   0        0        0     2862 2024-04-05 02:11:28.490517 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc
+-rw-r--r--   0        0        0     1814 2024-03-25 11:56:24.969323 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc
+-rw-r--r--   0        0        0     2925 2024-03-26 10:27:17.221884 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc
+-rw-r--r--   0        0        0     2930 2024-04-05 02:11:28.487946 spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc
+-rw-r--r--   0        0        0     4510 2024-04-10 14:45:36.699352 spotidex-1.0.0/spotidex/cli/custom_widgets/AppInterface.py
+-rw-r--r--   0        0        0     1467 2024-04-10 18:25:15.239179 spotidex-1.0.0/spotidex/cli/custom_widgets/DownloadPathSelector.py
+-rw-r--r--   0        0        0     1694 2024-03-26 11:07:37.915285 spotidex-1.0.0/spotidex/cli/custom_widgets/DownloadQualitySelection.py
+-rw-r--r--   0        0        0     1854 2024-04-12 10:43:16.844163 spotidex-1.0.0/spotidex/cli/custom_widgets/MetadataCheckBox.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:19:46.325307 spotidex-1.0.0/spotidex/cli/popup_screens/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-06 10:24:05.820610 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4015 2024-03-26 09:26:02.229660 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     4011 2024-04-05 02:11:28.481442 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6492 2024-04-06 09:29:03.384757 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1821 2024-04-03 13:36:39.691516 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     1825 2024-04-05 02:11:04.033205 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     1920 2024-03-26 16:25:44.077331 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc
+-rw-r--r--   0        0        0     1923 2024-04-05 02:11:04.033205 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     2116 2024-04-03 13:47:52.935756 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc
+-rw-r--r--   0        0        0     2113 2024-04-05 02:11:28.455505 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc
+-rw-r--r--   0        0        0     6594 2024-03-27 01:20:52.848095 spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc
+-rw-r--r--   0        0        0     4620 2024-04-15 03:47:02.055547 spotidex-1.0.0/spotidex/cli/popup_screens/DownloadPathPopup.py
+-rw-r--r--   0        0        0     1135 2024-04-10 14:45:53.954177 spotidex-1.0.0/spotidex/cli/popup_screens/ExitScreenPopup.py
+-rw-r--r--   0        0        0     1210 2024-03-26 12:20:40.784194 spotidex-1.0.0/spotidex/cli/popup_screens/GoBackSettingsPopup.py
+-rw-r--r--   0        0        0     1398 2024-04-09 17:09:41.333135 spotidex-1.0.0/spotidex/cli/popup_screens/NetworkErrorPopup.py
+-rw-r--r--   0        0        0      700 2024-04-10 18:25:42.766710 spotidex-1.0.0/spotidex/cli/SpotidexApp.py
+-rw-r--r--   0        0        0     3850 2024-04-15 03:36:55.336129 spotidex-1.0.0/spotidex/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 10:22:02.968074 spotidex-1.0.0/spotidex/src/__init__.py
+-rw-r--r--   0        0        0     5841 2024-04-13 16:54:40.790363 spotidex-1.0.0/spotidex/src/content.py
+-rw-r--r--   0        0        0     7175 2024-04-15 17:43:34.567580 spotidex-1.0.0/spotidex/src/download.py
+-rw-r--r--   0        0        0     1049 2023-12-06 02:16:07.479525 spotidex-1.0.0/spotidex/src/static.py
+-rw-r--r--   0        0        0     5307 2024-04-15 06:30:05.113213 spotidex-1.0.0/spotidex/src/utils.py
+-rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 spotidex-1.0.0/PKG-INFO
```

### Comparing `spotidex-0.0.7/pyproject.toml` & `spotidex-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "spotidex"
-version = "0.0.7"
+version = "1.0.0"
 description = "Spotify Downloader TUI"
 authors = ["Libin Lalu <libinlalu000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/libin-codes/spotidex.git"
+homepage = "https://github.com/libin-codes/spotidex"
+keywords = ["spotify", "downloader", "spotidex", "music"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 mutagen = "1.47.0"
 requests = "2.31.0"
 rich = "13.7.1"
 spotipy = "2.23.0"
```

### Comparing `spotidex-0.0.7/spotidex/cli/app_screens/DownloadInterface.py` & `spotidex-1.0.0/spotidex/cli/app_screens/DownloadInterface.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def compose(self):
         yield AppInterface(
             Horizontal(RichLog(id="music-info"), id="info-container"),
             Horizontal(
                 Label("PROGRESS", id="progress"),
                 Horizontal(
-                    Static("DOWNLOADING : ", id="stat"), ProgressBar(id="bar"), id="bc"
+                    Static("DOWNLOADING : ", id="stat"), ProgressBar(id="progress-bar"), id="bc"
                 ),
                 id="progress-bar-container",
             ),
             id="download-interface",
         )
 
     def on_mount(self):
@@ -138,22 +138,22 @@
         text_log.write(table)
         self.app.query_one("#back-button").label = "GO HOME"
         self.app.query_one("#back-button").disabled = True
         self.app.query_one("#exit-button").disabled = True
         self.download_music()
 
     def progress_hook(self, percent):
-        if self.app.query_one("ProgressBar").percentage != 0.0:
-            self.app.query_one("ProgressBar").update(total=100)
-        self.app.query_one("ProgressBar",ProgressBar).update(progress=float(percent))
+        if self.query_one("#progress-bar",ProgressBar).total == None:
+            self.query_one("#progress-bar").update(total=100)
+        self.app.query_one("#progress-bar",ProgressBar).update(progress=float(percent))
 
     def on_worker_state_changed(self, event) -> None:
         def eval(value):
             if value == "retry":
-                self.app.query_one("ProgressBar",ProgressBar).update(progress=0, total=None)
+                self.query_one("#progress-bar",ProgressBar).update(progress=0, total=None)
                 self.download_music()
 
         if str(event.state) == "WorkerState.CANCELLED":
             self.app.push_screen(NetworkErrorScreen(), eval)
 
     @work(thread=True, exclusive=True)
     def download_music(self):
```

### Comparing `spotidex-0.0.7/spotidex/cli/app_screens/MainMenuInterface.py` & `spotidex-1.0.0/spotidex/cli/app_screens/MainMenuInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/app_screens/SearchInterface.py` & `spotidex-1.0.0/spotidex/cli/app_screens/SearchInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 }
 """
 
 
 class Search(Screen):
     DEFAULT_CSS = CSS
     BINDINGS = [
-        Binding("tab", "paste_link", "PASTE SPOTIFY LINK",priority=True),
-        Binding("delete", "clear_input", "CLEAR INPUT",priority=True)
+        Binding("tab", "paste_link", "PASTE SPOTIFY LINK", priority=True),
+        Binding("delete", "clear_input", "CLEAR INPUT", priority=True),
     ]
 
     def compose(self):
         yield AppInterface(
             Horizontal(
                 Input(
                     id="search-input",
@@ -67,30 +67,32 @@
                 Button("SEARCH", "success", id="search-button", disabled=True),
             ),
             Label(app_description, id="app-description", shrink=True),
             id="search-interface",
         )
 
     def action_paste_link(self):
-        if self.query_one("#search-input", Input).value =="":
+        if self.query_one("#search-input", Input).value == "":
             self.query_one("#search-input", Input).value = pyperclip.paste()
         self.query_one("#search-input", Input).focus()
-    
+
     def action_clear_input(self):
         self.query_one("#search-input", Input).value = ""
 
-
     @work(exclusive=True, thread=True)
     def get_link_info(self):
         self.app.query_one("LoadingIndicator").styles.background = "#1c1c1c"
         try:
             self.app.link_details = get_link_details(self.app.spotify_link)
-            if int(self.app.link_details[0]['TOTAL TRACKS']) > 100:
+            if (
+                "track" not in self.app.spotify_link
+                and int(self.app.link_details[0]["TOTAL TRACKS"]) > 100
+            ):
                 raise SpotidexError("Maxlimit")
-                
+
         except Exception as spotidex_error:
             if spotidex_error.message == "NetworkError":
                 self.app.notify(
                     "Please check you internet connection and try again",
                     title="Network Error",
                     severity="error",
                 )
@@ -103,15 +105,15 @@
             elif spotidex_error.message == "Maxlimit":
                 self.query_one("#search-input").value = ""
                 self.app.notify(
                     "The total track of playlist/album has exceeded the maximum limit which is 100",
                     title="MAX LIMIT REACHED",
                     severity="error",
                 )
-                
+
             get_current_worker().cancel()
         self.app.query_one("#interface").loading = False
         self.app.query_one("#exit-button").disabled = False
         self.app.query_one("#interface").styles.padding = (2, 3, 0, 3)
 
     def on_worker_state_changed(self, event: Worker.StateChanged) -> None:
         if str(event.state) == "WorkerState.CANCELLED":
```

### Comparing `spotidex-0.0.7/spotidex/cli/app_screens/SelectDownloadInterface.py` & `spotidex-1.0.0/spotidex/cli/app_screens/SelectDownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/app_screens/SettingsInterface.py` & `spotidex-1.0.0/spotidex/cli/app_screens/SettingsInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/app_interface.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/AppInterface.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/download_path_selector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/download_quality_selection.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/DownloadPathSelector.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/DownloadQualitySelection.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/header.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/metadata_checkbox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/custom_widgets/__pycache__/MetadataCheckBox.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/AppInterface.py` & `spotidex-1.0.0/spotidex/cli/custom_widgets/AppInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadPathSelector.py` & `spotidex-1.0.0/spotidex/cli/custom_widgets/DownloadPathSelector.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/DownloadQualitySelection.py` & `spotidex-1.0.0/spotidex/cli/custom_widgets/DownloadQualitySelection.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/custom_widgets/MetadataCheckBox.py` & `spotidex-1.0.0/spotidex/cli/custom_widgets/MetadataCheckBox.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/create_folder_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/CreateFolderPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/DownloadPathPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/exit_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/ExitScreenPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/go_back_settings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/GoBackSettingsPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/network_error_screen.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/NetworkErrorPopup.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc` & `spotidex-1.0.0/spotidex/cli/popup_screens/__pycache__/select_download_path.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/DownloadPathPopup.py` & `spotidex-1.0.0/spotidex/cli/popup_screens/DownloadPathPopup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from textual.containers import Container
 
 from spotidex.cli.utils import (
     shorten_path,
     Path,
     get_data_drive_path,
     get_downloads_folder,
+    os,
+    can_create_directory,
 )
 
 CSS = """
 DownloadPathScreen{
   
     align:center middle;
 
@@ -129,31 +131,38 @@
             self.FilteredDirectoryTree(self.current_path, id="filteredtree")
         )
         self.app.query_one("#download-path-log").clear().write(
             shorten_path(self.current_path, 60)
         )
 
     def on_directory_tree_directory_selected(self, path):
-        if self.current_path != str(get_downloads_folder()):
-            self.current_path = str(path.path)
+        self.current_path = str(path.path)
         self.refresh_tree()
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "download-path-back-button":
-            if self.current_path == str(get_downloads_folder()):
-                self.current_path = str(Path(get_data_drive_path()))
-            else:
+            if os.name == "nt":
                 self.current_path = str(
                     Path("\\".join(self.current_path.split("\\")[:-1]) + "\\")
                 )
+            else:
+                self.current_path = str(
+                    Path("/".join(self.current_path.split("/")[:-1]) + "/")
+                )
             self.refresh_tree()
 
         elif event.button.id == "download-path-reset-button":
             self.current_path = str(Path.cwd())
             self.refresh_tree()
 
         elif event.button.id == "downloads-folder-button":
             self.current_path = str(get_downloads_folder())
             self.refresh_tree()
 
         elif event.button.id == "download-path-confirm-button":
-            self.dismiss(self.current_path)
+            if can_create_directory(self.current_path):
+                self.dismiss(self.current_path)
+            else:
+                self.app.notify(
+                    "Cannot access the given path, please run the terminal as administrator or use other path",
+                    title="PERMISSION DENIED",severity="warning"
+                )
```

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/ExitScreenPopup.py` & `spotidex-1.0.0/spotidex/cli/popup_screens/ExitScreenPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/GoBackSettingsPopup.py` & `spotidex-1.0.0/spotidex/cli/popup_screens/GoBackSettingsPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/popup_screens/NetworkErrorPopup.py` & `spotidex-1.0.0/spotidex/cli/popup_screens/NetworkErrorPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/SpotidexApp.py` & `spotidex-1.0.0/spotidex/cli/SpotidexApp.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/cli/utils.py` & `spotidex-1.0.0/spotidex/cli/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,21 +61,21 @@
                 for track in album_details["track_details"]
             },
         )
 
 
 def shorten_path(path: str, length):
     while len(path) > length:
-        path_parts = path.split("\\")
+        path_parts = path.split("\\") if os.name == "nt" else path.split("/")
         if "..." in path_parts:
             path_parts.pop(2)
         else:
             path_parts.pop(1)
             path_parts.insert(1, "...")
-        path = "\\".join(path_parts)
+        path = "\\".join(path_parts) if os.name == "nt" else "/".join(path_parts)
     return path
 
 
 def create_download_path(path, folder_name):
     folder_path = Path(path, folder_name)
     folder_path.mkdir(parents=True, exist_ok=True)
 
@@ -87,62 +87,32 @@
     if ("spotify" in value)
     and (any(keyword in value for keyword in ["track", "playlist", "album"]))
     else False
 )
 
 
 def get_data_drive_path():
-    if os.name == "nt":  # Windows
-        system_drive = (
-            os.environ["SYSTEMDRIVE"] if "SYSTEMDRIVE" in os.environ else "C:"
-        )
-        drives = [
-            "A",
-            "B",
-            "C",
-            "D",
-            "E",
-            "F",
-            "G",
-            "H",
-            "I",
-            "J",
-            "K",
-            "L",
-            "M",
-            "N",
-            "O",
-            "P",
-            "Q",
-            "R",
-            "S",
-            "T",
-            "U",
-            "V",
-            "W",
-            "X",
-            "Y",
-            "Z",
-        ]
-        available_drives = [
-            drive + ":\\"
-            for drive in drives
-            if os.path.exists(drive + ":\\") and drive + ":" != system_drive
-        ]
-        return available_drives[0] if available_drives else None
-    else:  # Unix-like systems
-        # Filter out root directory ('/') from mounted drives
-        mounted_drives = [root for root, dirs, files in os.walk("/") if dirs or files]
-        return mounted_drives[0] if mounted_drives else None
-
+    if os.name != "nt":
+        return "/"
+    drives = [chr(_) for _ in list(range(ord("A"),ord("Z")+1))]
+    drives.remove("C")
+    available_drives = [
+        drive + ":\\"
+        for drive in drives
+        if os.path.exists(drive + ":\\")
+    ]
+    return available_drives[0] if available_drives else None
 
 def get_downloads_folder():
-    # Get the user's home directory
     home_dir = os.path.expanduser("~")
-
-    # Operating system specific logic to get the Downloads folder
-    if os.name == "posix":  # Unix-like OS (Linux, macOS)
-        downloads_folder = os.path.join(home_dir, "Downloads")
-    elif os.name == "nt":  # Windows
-        downloads_folder = os.path.join(home_dir, "Downloads")
+    downloads_folder = os.path.join(home_dir, "Downloads")
 
     return downloads_folder
+
+def can_create_directory(path):
+    try:
+        os.mkdir(os.path.join(path,"temp826328ljij"))
+        shutil.rmtree(os.path.join(path,"temp826328ljij"))
+        return True
+    
+    except PermissionError:
+        return False
```

### Comparing `spotidex-0.0.7/spotidex/src/content.py` & `spotidex-1.0.0/spotidex/src/content.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/src/download.py` & `spotidex-1.0.0/spotidex/src/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from requests import ConnectionError,ReadTimeout
 from spotidex.src.content import SpotifyContent
 
 
 class SpotifyDownloader:
     def __init__(self) -> None:
         self.spotidex_path = get_spotidex_data_directory()
+        delete_temp_folders()
         self.ffmpeg_path = get_ffmpeg()
         self.total_tracks = None
         self.sp = spotipy.Spotify(
             client_credentials_manager=
                 SpotifyClientCredentials(
                     client_id,
                     client_secret,
@@ -39,18 +40,21 @@
         with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
             if make_folder:
                 folder_name = get_valid_name(download_path, folder_name)
                 temp_path = Path(temp_folder).joinpath(folder_name)
             else:
                 temp_path = Path(temp_folder)
 
-            done, not_done = pool_download(
+            done, un_done = pool_download(
                 self, list(set(links)), custom_hook, temp_path, quality, metadata
             )
-            if len(not_done) != 0:
+            try:
+                for done_result in done:done_result.result()
+                for undone_result in un_done:undone_result.result()
+            except Exception:
                 raise SpotidexError("NetworkError")
             progress_hook(self, {"status": "downloaded"}, custom_hook)
             for file_path in Path(temp_folder).iterdir():
                 shutil.move(str(file_path), str(download_path))
             progress_hook(self, {"status": "transfered"}, custom_hook)
         
 
@@ -72,15 +76,15 @@
         track_artist = ",".join([artist["name"] for artist in data["artists"]])
         query = data["name"]+f" song by {track_artist} official lyrics "
         file_name = get_valid_name(download_path,data["name"]+".mp3")
     
         with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
             options = {
                 "format": "bestaudio/best",
-                "outtmpl": str(download_path)+'\\'+file_name,
+                "outtmpl": os.path.join(str(download_path),file_name),
                 "quiet": True,
                 "noprogress": True,
                 "progress": "false",
                 "ffmpeg_location": str(self.ffmpeg_path),
                 "postprocessors": [
                     {
                         "key": "FFmpegExtractAudio",
@@ -90,21 +94,24 @@
                 ],
                 "retries": 20,
                 "progress_hooks": [lambda d: progress_hook(self, d, custom_hook)]
                 if custom_hook != None
                 else [],
             }
                 
-            if self.total_tracks == None:
-                options['outtmpl'] = str(Path(temp_folder))+'\\'+file_name
-            ydl = yt_dlp.YoutubeDL(options)
-            yt_video_result = ydl.extract_info(f"ytsearch:{query}", download=False)
-            first_yt_video_link = yt_video_result["entries"][0]["webpage_url"]
-            yt_video_download = ydl.extract_info(first_yt_video_link, download=True)
-            downloaded_path = ydl.prepare_filename(yt_video_download)
+            try:
+                if self.total_tracks == None:
+                    options['outtmpl'] = os.path.join(str(Path(temp_folder)),file_name)
+                ydl = yt_dlp.YoutubeDL(options)
+                yt_video_result = ydl.extract_info(f"ytsearch:{query}", download=False)
+                first_yt_video_link = yt_video_result["entries"][0]["webpage_url"]
+                yt_video_download = ydl.extract_info(first_yt_video_link, download=True)
+                downloaded_path = ydl.prepare_filename(yt_video_download)
+            except Exception:
+                raise SpotidexError("NetworkError")
 
             if metadata:
                 add_metadata(data, Path(downloaded_path + ".mp3").resolve())
 
             if self.total_tracks == None:
                 progress_hook(self, {"status": "downloaded"}, custom_hook)
                 for file_path in Path(temp_folder).iterdir():
@@ -156,15 +163,15 @@
             track_links = [track["link"] for track in album_data['track_details']]
         except SpotifyException:
             raise SpotidexError("InvalidSpotifyLink")
         except (ConnectionError,ReadTimeout):
             raise SpotidexError("NetworkError")
         
         
-        folder_name = get_valid_name(download_path,album_data['name'])
+        folder_name = get_valid_name(download_path,album_data['album_name'])
         
         self._download_with_temp_directory(
                 track_links,
                 folder_name,
                 custom_hook,
                 download_path,
                 quality,
```

### Comparing `spotidex-0.0.7/spotidex/src/static.py` & `spotidex-1.0.0/spotidex/src/static.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.7/spotidex/src/utils.py` & `spotidex-1.0.0/spotidex/src/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, re, stat, platform, requests, subprocess
+import os, re, stat, platform, requests, subprocess ,shutil
 from mutagen.id3 import ID3, APIC, TPE1, TIT2, TALB
 import concurrent.futures
 from pathlib import Path
 from rich.progress import Progress, SpinnerColumn
 
 from spotidex.src.static import FFMPEG_URLS
 
@@ -150,7 +150,14 @@
         name, i = (
             (name.replace(".mp3", "") + f" ({i})" + add_mp3, i + 1)
             if i == 1
             else (name.replace('.mp3',"")[::-1].split("(",1)[-1][::-1] + f"({i})" + add_mp3, i + 1)
         )
 
     return name.replace(".mp3", "")
+
+def delete_temp_folders():
+    directory = get_spotidex_data_directory()
+    for item in os.listdir(directory):
+        item_path = os.path.join(directory, item)
+        if os.path.isdir(item_path):
+            shutil.rmtree(item_path)
```

