# Comparing `tmp/musicscan-0.1.2.tar.gz` & `tmp/musicscan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicscan-0.1.2.tar", last modified: Sun Apr  7 12:49:33 2024, max compression
+gzip compressed data, was "musicscan-0.1.3.tar", last modified: Tue Apr 16 10:44:27 2024, max compression
```

## Comparing `musicscan-0.1.2.tar` & `musicscan-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.428525 musicscan-0.1.2/
--rw-r--r--   0 chrisj     (102) other        (1)     1071 2024-02-17 16:38:18.000000 musicscan-0.1.2/LICENSE
--rw-r--r--   0 chrisj     (102) other        (1)     6224 2024-04-07 12:49:33.428434 musicscan-0.1.2/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)     5168 2024-04-06 20:54:31.000000 musicscan-0.1.2/README.md
--rw-r--r--   0 chrisj     (102) other        (1)     1194 2024-04-07 12:47:49.000000 musicscan-0.1.2/pyproject.toml
--rw-r--r--   0 chrisj     (102) other        (1)      150 2024-04-07 12:49:33.429117 musicscan-0.1.2/setup.cfg
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.415646 musicscan-0.1.2/src/
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.418407 musicscan-0.1.2/src/musicscan/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:52.000000 musicscan-0.1.2/src/musicscan/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.423748 musicscan-0.1.2/src/musicscan/data/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:59.000000 musicscan-0.1.2/src/musicscan/data/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5803 2024-04-03 01:25:41.000000 musicscan-0.1.2/src/musicscan/data/analyzer.py
--rw-r--r--   0 chrisj     (102) other        (1)     2199 2024-04-03 01:26:18.000000 musicscan-0.1.2/src/musicscan/data/artist.py
--rw-r--r--   0 chrisj     (102) other        (1)     5019 2024-04-03 01:41:03.000000 musicscan-0.1.2/src/musicscan/data/cd.py
--rw-r--r--   0 chrisj     (102) other        (1)     3541 2024-04-06 21:04:19.000000 musicscan-0.1.2/src/musicscan/data/flags.py
--rw-r--r--   0 chrisj     (102) other        (1)     4082 2024-04-03 01:26:06.000000 musicscan-0.1.2/src/musicscan/data/library.py
--rw-r--r--   0 chrisj     (102) other        (1)     2973 2024-04-03 01:26:55.000000 musicscan-0.1.2/src/musicscan/data/stringtools.py
--rw-r--r--   0 chrisj     (102) other        (1)     4124 2024-04-03 01:25:53.000000 musicscan-0.1.2/src/musicscan/data/titletools.py
--rw-r--r--   0 chrisj     (102) other        (1)     4084 2024-04-06 21:23:16.000000 musicscan-0.1.2/src/musicscan/data/track.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.425250 musicscan-0.1.2/src/musicscan/fileops/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:02.000000 musicscan-0.1.2/src/musicscan/fileops/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1370 2024-04-03 01:27:53.000000 musicscan-0.1.2/src/musicscan/fileops/filenames.py
--rw-r--r--   0 chrisj     (102) other        (1)     3316 2024-04-03 01:27:23.000000 musicscan-0.1.2/src/musicscan/fileops/scanner.py
--rw-r--r--   0 chrisj     (102) other        (1)     5556 2024-04-04 03:19:55.000000 musicscan-0.1.2/src/musicscan/fileops/xmlwriter.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.426014 musicscan-0.1.2/src/musicscan/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:05.000000 musicscan-0.1.2/src/musicscan/generic/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2485 2024-02-25 01:18:01.000000 musicscan-0.1.2/src/musicscan/generic/stats.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.426774 musicscan-0.1.2/src/musicscan/tools/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:09.000000 musicscan-0.1.2/src/musicscan/tools/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     6103 2024-04-07 12:41:49.000000 musicscan-0.1.2/src/musicscan/tools/id3scan.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.427606 musicscan-0.1.2/src/musicscan/xml/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-04-03 01:29:17.000000 musicscan-0.1.2/src/musicscan/xml/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)    12012 2024-04-06 21:20:18.000000 musicscan-0.1.2/src/musicscan/xml/builder.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.428011 musicscan-0.1.2/src/musicscan.egg-info/
--rw-r--r--   0 chrisj     (102) other        (1)     6224 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)      845 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/SOURCES.txt
--rw-r--r--   0 chrisj     (102) other        (1)        1 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/dependency_links.txt
--rw-r--r--   0 chrisj     (102) other        (1)        8 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/requires.txt
--rw-r--r--   0 chrisj     (102) other        (1)       10 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/top_level.txt
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.448145 musicscan-0.1.3/
+-rw-r--r--   0 chrisj     (102) other        (1)     1071 2024-02-17 16:38:18.000000 musicscan-0.1.3/LICENSE
+-rw-r--r--   0 chrisj     (102) other        (1)     6224 2024-04-16 10:44:27.448052 musicscan-0.1.3/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)     5168 2024-04-07 13:08:05.000000 musicscan-0.1.3/README.md
+-rw-r--r--   0 chrisj     (102) other        (1)     1194 2024-04-09 02:25:16.000000 musicscan-0.1.3/pyproject.toml
+-rw-r--r--   0 chrisj     (102) other        (1)      150 2024-04-16 10:44:27.448724 musicscan-0.1.3/setup.cfg
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.435001 musicscan-0.1.3/src/
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.437850 musicscan-0.1.3/src/musicscan/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:52.000000 musicscan-0.1.3/src/musicscan/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.443244 musicscan-0.1.3/src/musicscan/data/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:59.000000 musicscan-0.1.3/src/musicscan/data/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6475 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/data/analyzer.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2199 2024-04-03 01:26:18.000000 musicscan-0.1.3/src/musicscan/data/artist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5705 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/data/cd.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3787 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/data/flags.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4082 2024-04-03 01:26:06.000000 musicscan-0.1.3/src/musicscan/data/library.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3012 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/data/stringtools.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4124 2024-04-03 01:25:53.000000 musicscan-0.1.3/src/musicscan/data/titletools.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4260 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/data/track.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.444821 musicscan-0.1.3/src/musicscan/fileops/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:02.000000 musicscan-0.1.3/src/musicscan/fileops/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1370 2024-04-03 01:27:53.000000 musicscan-0.1.3/src/musicscan/fileops/filenames.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3316 2024-04-03 01:27:23.000000 musicscan-0.1.3/src/musicscan/fileops/scanner.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5600 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/fileops/xmlwriter.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.445616 musicscan-0.1.3/src/musicscan/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:05.000000 musicscan-0.1.3/src/musicscan/generic/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2485 2024-02-25 01:18:01.000000 musicscan-0.1.3/src/musicscan/generic/stats.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.446399 musicscan-0.1.3/src/musicscan/tools/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:09.000000 musicscan-0.1.3/src/musicscan/tools/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6103 2024-04-16 10:39:02.000000 musicscan-0.1.3/src/musicscan/tools/id3scan.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.447201 musicscan-0.1.3/src/musicscan/xml/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-04-03 01:29:17.000000 musicscan-0.1.3/src/musicscan/xml/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)    12323 2024-04-16 10:41:56.000000 musicscan-0.1.3/src/musicscan/xml/builder.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-16 10:44:27.447626 musicscan-0.1.3/src/musicscan.egg-info/
+-rw-r--r--   0 chrisj     (102) other        (1)     6224 2024-04-16 10:44:27.000000 musicscan-0.1.3/src/musicscan.egg-info/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)      845 2024-04-16 10:44:27.000000 musicscan-0.1.3/src/musicscan.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        1 2024-04-16 10:44:27.000000 musicscan-0.1.3/src/musicscan.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        8 2024-04-16 10:44:27.000000 musicscan-0.1.3/src/musicscan.egg-info/requires.txt
+-rw-r--r--   0 chrisj     (102) other        (1)       10 2024-04-16 10:44:27.000000 musicscan-0.1.3/src/musicscan.egg-info/top_level.txt
```

### Comparing `musicscan-0.1.2/LICENSE` & `musicscan-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/PKG-INFO` & `musicscan-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicscan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for converting music metadata to XML
 Author-email: Chris J <cjcodeproj@fastmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/cjcodeproj/musicscan
 Project-URL: bug tracker, https://github.com/cjcodeproj/musicscan/issues
 Project-URL: repository, https://github.com/cjcodeproj/musicscan
 Project-URL: changelog, https://github.com/cjcodeproj/musicscan/blob/main/CHANGELOG.md
```

### Comparing `musicscan-0.1.2/README.md` & `musicscan-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/pyproject.toml` & `musicscan-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "musicscan"
-version = "0.1.2"
+version = "0.1.3"
 description = "Package for converting music metadata to XML"
 readme = "README.md"
 requires-python = ">3.8"
 dependencies = [
   "tinytag"
 ]
```

### Comparing `musicscan-0.1.2/src/musicscan/__init__.py` & `musicscan-0.1.3/src/musicscan/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/data/__init__.py` & `musicscan-0.1.3/src/musicscan/data/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/data/analyzer.py` & `musicscan-0.1.3/src/musicscan/data/analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,26 +36,46 @@
     add flags when appropriate.
     '''
 
     def main_test(self, in_album):
         '''
         Main album testing routine.
         '''
+        self.check_album_values(in_album)
         self.test_album_title(in_album)
         self.test_album_artist(in_album)
         self.test_soundtrack(in_album)
         self.test_score(in_album)
         for dsc in sorted(in_album.discs):
             for trk in sorted(in_album.discs[dsc].tracks,
                               key=lambda x: x.track_no):
+                self.check_track_values(trk)
                 self.test_album_track_chrs(trk)
                 self.test_album_track_featured(trk)
                 self.test_album_track_live(trk)
                 self.test_album_track_blank(trk)
 
+    def check_album_values(self, in_album):
+        '''
+        If album values are missing, put in placeholder
+        values.
+        '''
+        if not in_album.title:
+            in_album.title = 'PLACEHOLDER ALBUM TITLE'
+            in_album.flags.add_flag(FlagCodes.m_album_title)
+
+    def check_track_values(self, in_track):
+        '''
+        If track values are missing, put in placeholder
+        values.
+        '''
+        if not in_track.artist:
+            in_track.artist = 'PLACEHOLDER TRACK ARTIST'
+            in_track.flags.add_flag(FlagCodes.m_track_artist)
+
     def test_album_title(self, in_album):
         '''
         Test album title for keywords that may indicate
         a compilation of some kind.
         '''
         greatest_p = re.compile(r'Greatest', re.IGNORECASE)
         hits_p = re.compile(r'\s+Hit', re.IGNORECASE)
@@ -80,15 +100,15 @@
     def test_score(self, in_album):
         '''
         Test album title for keywords that may indicate
         a score album.
         '''
         score_p = re.compile(r'\s+Score\s+', re.IGNORECASE)
         if score_p.search(in_album.title):
-            in_album.flags.add(FlagCodes.p_score)
+            in_album.flags.add_flag(FlagCodes.p_score)
 
     def test_album_artist(self, in_album):
         '''
         Test the name of the artist for indicators
         the band may be a group.
         '''
         and_p = re.compile(r'\s+and\s+', re.IGNORECASE)
```

### Comparing `musicscan-0.1.2/src/musicscan/data/artist.py` & `musicscan-0.1.3/src/musicscan/data/artist.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/data/cd.py` & `musicscan-0.1.3/src/musicscan/data/cd.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 '''
 Data objects for music.
 '''
 
 # pylint: disable=too-many-instance-attributes
 
-from musicscan.data.flags import Flags
+from musicscan.data.flags import Flags, FlagCodes
 from musicscan.data.titletools import ShortTitleIndex, ShortTitle
 from musicscan.data.track import Track
 from musicscan.data.stringtools import build_complete_filename
 
 
 class Album():
     '''
@@ -41,14 +41,15 @@
     disc containing one or more tracks.
     '''
     def __init__(self, in_artist, in_album_title):
         self.title = in_album_title
         self.artist = in_artist
         self.title_index = ShortTitleIndex()
         self.discs = {}
+        self._first_disc = None
         self.flags = Flags()
         self.track_count = 0
 
     def import_tag(self, in_tag):
         '''
         Import an ID3 tag into the album, creating
         a Disc object if necessary.
@@ -90,33 +91,41 @@
         '''
         return build_complete_filename(self, in_suffix)
 
     def first_track(self):
         '''
         Return the very first track of the album.
         '''
-        return self.discs[1].tracks[0]
+        # return self.discs[1].tracks[0]
+        return self._first_disc.first_track()
 
     def tracks_in_order(self):
         '''
         Return all tracks from all discs on the album.
         '''
         all_tracks = []
         for dsc in sorted(self.discs):
             for trk in sorted(self.discs[dsc].tracks,
                               key=lambda x: x.track_no):
                 all_tracks.append(trk)
         return all_tracks
 
     def finalize(self):
         '''
-        Finalize each object by setting up the short titles
-        for each track.
+        Finalize each object with several cleanup routines.
+
+        1. Identify which disc is the first.
+        2. Set up the short titles for every track.
+
         '''
-        for dsc in sorted(self.discs):
+        # Identify first disc
+        sort_d = sorted(self.discs)
+        self._first_disc = self.discs[sort_d[0]]
+        # Process all short titles
+        for dsc in sort_d:
             self.discs[dsc].finalize()
 
     def __str__(self):
         return f"{self.title} ({len(self.discs)})"
 
 
 class Disc():
@@ -124,29 +133,41 @@
     Class representing a single physical compact disc.
     '''
     def __init__(self, in_number, in_album):
         self.disc_no = in_number
         self.album = in_album
         self.tracks = []
         self.raw = []
+        self._first_track = None
 
     def import_tag(self, in_tag, in_album):
         '''
         Import data from an ID3 tag into the disc object.
         '''
         self.raw.append(in_tag)
         trk = Track(in_tag)
         trk.set_album_object(in_album)
         self.tracks.append(trk)
 
+    def first_track(self):
+        '''
+        Return the first track of the disc.
+        '''
+        return self._first_track
+
     def finalize(self):
         '''
         Update data after all import operations are done.
         '''
-        for trk in sorted(self.tracks):
+        sort_t = sorted(self.tracks, key=lambda x: x.track_no)
+        self._first_track = sort_t[0]
+        for trk in sort_t:
+            if not trk.title:
+                trk.title = 'PLACEHOLDER TITLE'
+                trk.flags.add_flag(FlagCodes.m_title)
             trk.short_title = ShortTitle(trk.title, self.album.title_index)
 
     def report(self):
         '''
         Generate a simple report on the disc object.
         '''
         print(f"Disc: {self.disc_no}")
```

### Comparing `musicscan-0.1.2/src/musicscan/data/flags.py` & `musicscan-0.1.3/src/musicscan/data/flags.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     l_group = 20
     p_feat_artist = 30
     p_live = 31
     p_demo = 32
     p_blank_track = 40
     p_genre_country_folk = 50
     m_year = 60
+    m_title = 61
+    m_album_title = 62
+    m_track_artist = 63
 
     @classmethod
     def to_str(cls, in_code):
         '''
         Convert a flag value to a usable string.
         '''
         matrix = {FlagCodes.p_greatest: 'possible_greatest_hits',
@@ -92,11 +95,14 @@
                   FlagCodes.l_group: 'likely_group_artist',
                   FlagCodes.p_feat_artist: 'possible_featured_artist',
                   FlagCodes.p_live: 'possible_live_performance',
                   FlagCodes.p_demo: 'possible_demo_performance',
                   FlagCodes.p_blank_track: 'possible_blank_track',
                   FlagCodes.p_genre_country_folk:
                   'country_and_folk_genre_is_too_vague',
-                  FlagCodes.m_year: 'missing_copyright_year'}
+                  FlagCodes.m_year: 'missing_copyright_year',
+                  FlagCodes.m_title: 'missing_title',
+                  FlagCodes.m_album_title: 'missing_album_title',
+                  FlagCodes.m_track_artist: 'missing_artist'}
         if in_code in matrix:
             return matrix[in_code]
         return ''
```

### Comparing `musicscan-0.1.2/src/musicscan/data/library.py` & `musicscan-0.1.3/src/musicscan/data/library.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/data/stringtools.py` & `musicscan-0.1.3/src/musicscan/data/stringtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,18 @@
 
 
 def sanitize_for_xml(in_string):
     '''
     Fix a string so it is suitable to go into
     XML output.
     '''
-    out = in_string.replace('&', '&amp;') \
-        .replace('<', '&lt;').replace('>', '&gt;')
+    out = ''
+    if in_string:
+        out = in_string.replace('&', '&amp;') \
+            .replace('<', '&lt;').replace('>', '&gt;')
     return out
 
 
 def transform_ampersand(in_value):
     '''
     Simple function to transform an ampersand.
     '''
```

### Comparing `musicscan-0.1.2/src/musicscan/data/titletools.py` & `musicscan-0.1.3/src/musicscan/data/titletools.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/data/track.py` & `musicscan-0.1.3/src/musicscan/data/track.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,52 +40,58 @@
     '''
     def __init__(self, in_tag):
         self.title = ''
         self.artist = ''
         self.album = ''
         self.album_o = None
         self.track_no = 0
+        self.track_total = 0
+        self.disc_no = 0
+        self.disc_total = 0
         self.bpm = 0
         self.short_title = ''
         self.album_artist = ''
         self.composer = ''
         self.year = '0000'
         self.flags = Flags()
         self.indices = []
         self._process(in_tag)
 
     def _process(self, in_tag):
         self.title = in_tag.title
         self.genre = in_tag.genre
         self.artist = in_tag.artist
-        self.track_no = int(in_tag.track)
-        self.track_total = int(in_tag.track_total)
-        if not in_tag.disc:
-            self.disc_no = 1
-        else:
-            self.disc_no = int(in_tag.disc)
-        if not in_tag.disc_total:
-            self.disc_total = 1
-        else:
-            self.disc_total = int(in_tag.disc_total)
+        self._process_integer_values(in_tag)
         self.album = in_tag.album
         if in_tag.albumartist:
             self.album_artist = in_tag.albumartist
         if in_tag.composer:
             self.composer = in_tag.composer
-        # self.disc_count = int(in_tag.disc_total)
         self.duration_r = in_tag.duration
         self.duration_f = self.duration_r * 100 / int(100)
         self.duration_t = timedelta(seconds=float(self.duration_f))
         self.duration_s = Track._make_iso_interval(self.duration_t)
         if in_tag.year:
             self.year = sanitize_year(in_tag.year)
         else:
             self.flags.add_flag(FlagCodes.m_year)
 
+    def _process_integer_values(self, in_tag):
+        '''
+        Process integer values and make sure they are valid.
+        '''
+        if in_tag.track:
+            self.track_no = int(in_tag.track)
+        if in_tag.track_total:
+            self.track_total = int(in_tag.track_total)
+        if in_tag.disc:
+            self.disc_no = int(in_tag.disc)
+        if in_tag.disc_total:
+            self.disc_total = int(in_tag.disc_total)
+
     def set_album_object(self, in_album_object):
         '''
         The album object is a reference back to the object that
         contains the track.
         '''
         self.album_o = in_album_object
```

### Comparing `musicscan-0.1.2/src/musicscan/fileops/__init__.py` & `musicscan-0.1.3/src/musicscan/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/fileops/filenames.py` & `musicscan-0.1.3/src/musicscan/fileops/filenames.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/fileops/scanner.py` & `musicscan-0.1.3/src/musicscan/fileops/scanner.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/fileops/xmlwriter.py` & `musicscan-0.1.3/src/musicscan/fileops/xmlwriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             self.write_single_xml(in_album)
 
     def write_single_xml(self, in_album):
         '''
         Write all the XML data in a single file.
         '''
         complete = self._path + '/' + in_album.filename('audiocd')
-        audiocd = CompleteCompactDiscXML()
+        audiocd = CompleteCompactDiscXML(self._debug)
         if not os.path.isfile(complete) or self._overwrite:
             with open(complete, mode='w', encoding='utf-8') as f_handle:
                 f_handle.write(audiocd.build(in_album))
                 f_handle.close()
                 self.files_written += 1
 
     def write_split_xml(self, in_album):
@@ -124,26 +124,26 @@
         self.write_split_xml_album(in_album)
 
     def write_split_xml_audiocd(self, in_album):
         '''
         Write the XML data pertaining to the audio CD.
         '''
         complete = self._path + '/' + in_album.filename('audiocd')
-        audiocd = SplitCompactDiscXML()
+        audiocd = SplitCompactDiscXML(self._debug)
         if not os.path.isfile(complete) or self._overwrite:
             with open(complete, mode='w', encoding='utf-8') as f_handle:
                 f_handle.write(audiocd.build(in_album))
                 f_handle.close()
                 self.files_written += 1
 
     def write_split_xml_index(self, in_album):
         '''
         Write the XML data pertaining to the CD index.
         '''
-        index = Index()
+        index = Index(self._debug)
         for dsc in sorted(in_album.discs):
             dsc_o = in_album.discs[dsc]
             f_str = f"cd{dsc_o.disc_no:02}-index"
             complete = self._path + '/' + in_album.filename(f_str)
             if not os.path.isfile(complete) or self._overwrite:
                 with open(complete, mode='w', encoding='utf-8') as f_handle:
                     f_handle.write(index.build_index_per_cd(dsc_o, True))
@@ -151,13 +151,13 @@
                     self.files_written += 1
 
     def write_split_xml_album(self, in_album):
         '''
         Write out the XML data pertaining to the album contents.
         '''
         complete = self._path + '/' + in_album.filename('album')
-        album = Album()
+        album = Album(self._debug)
         if not os.path.isfile(complete) or self._overwrite:
             with open(complete, mode='w', encoding='utf-8') as f_handle:
                 f_handle.write(album.build_standalone_album(in_album))
                 f_handle.close()
                 self.files_written += 1
```

### Comparing `musicscan-0.1.2/src/musicscan/generic/__init__.py` & `musicscan-0.1.3/src/musicscan/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/generic/stats.py` & `musicscan-0.1.3/src/musicscan/generic/stats.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/tools/__init__.py` & `musicscan-0.1.3/src/musicscan/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/tools/id3scan.py` & `musicscan-0.1.3/src/musicscan/tools/id3scan.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/xml/__init__.py` & `musicscan-0.1.3/src/musicscan/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1.2/src/musicscan/xml/builder.py` & `musicscan-0.1.3/src/musicscan/xml/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,20 @@
         return "".join(chunks)
 
     def build_index_per_cd(self, in_cd, in_namespace=False):
         '''
         Build an index structure for a single CD.
         '''
         ns_str = ''
+        timestamp = datetime.datetime.now()
         if in_namespace:
             ns_str = " xmlns='http://vectortron.com/xml/media/media'"
         output = f"  <cdIndex ref='cd{in_cd.disc_no:02}'{ns_str}>\n"
-        for trk in sorted(in_cd.tracks):
+        output += f"  <!-- created by id3scan ({timestamp}) -->\n"
+        for trk in sorted(in_cd.tracks, key=lambda x: x.track_no):
             output += self.add_track_xml(trk)
         output += "  </cdIndex>\n"
         return output
 
     def build_xi_refs_from_album(self, in_album):
         '''
         Output all of the xi:include references in the index.
@@ -232,15 +234,17 @@
         output += self.build_album_body(in_album)
         return output
 
     def build_album_body(self, in_album):
         '''
         Write out the main body of the album element.
         '''
+        timestamp = datetime.datetime.now()
         output = "  <album xmlns='http://vectortron.com/xml/media/audio'>\n"
+        output += f" <!-- created by id3scan ({timestamp}) -->\n"
         output += f"   <title>{in_album.title}</title>\n"
         output += in_album.flags.to_xml_comment()
         output += self.build_chunk_catalog(in_album)
         output += self.build_chunk_classification(in_album)
         output += self.build_chunk_elements(in_album)
         output += "  </album>\n"
         return output
@@ -286,15 +290,16 @@
         '''
         Output the element element and all
         child content elements.
         '''
         output = " <elements>\n"
         song = SongElementXML(self.debug)
         for dsc in sorted(in_album.discs):
-            for trk in in_album.discs[dsc].tracks:
+            for trk in sorted(in_album.discs[dsc].tracks,
+                              key=lambda x: x.track_no):
                 output += song.build(trk)
         output += " </elements>\n"
         return output
 
 
 class SongElementXML():
     '''
```

### Comparing `musicscan-0.1.2/src/musicscan.egg-info/PKG-INFO` & `musicscan-0.1.3/src/musicscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musicscan
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for converting music metadata to XML
 Author-email: Chris J <cjcodeproj@fastmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/cjcodeproj/musicscan
 Project-URL: bug tracker, https://github.com/cjcodeproj/musicscan/issues
 Project-URL: repository, https://github.com/cjcodeproj/musicscan
 Project-URL: changelog, https://github.com/cjcodeproj/musicscan/blob/main/CHANGELOG.md
```

### Comparing `musicscan-0.1.2/src/musicscan.egg-info/SOURCES.txt` & `musicscan-0.1.3/src/musicscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

