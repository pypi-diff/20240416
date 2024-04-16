# Comparing `tmp/how_is_the_weather-0.1.0.tar.gz` & `tmp/how_is_the_weather-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "how_is_the_weather-0.1.0.tar", max compression
+gzip compressed data, was "how_is_the_weather-0.2.0.tar", max compression
```

## Comparing `how_is_the_weather-0.1.0.tar` & `how_is_the_weather-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-16 18:06:51.371516 how_is_the_weather-0.1.0/LICENSE
--rw-r--r--   0        0        0      876 2024-04-16 18:12:19.609384 how_is_the_weather-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 14:44:15.551347 how_is_the_weather-0.1.0/src/how_is_the_weather/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-16 14:52:42.116669 how_is_the_weather-0.1.0/src/how_is_the_weather/weather.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 how_is_the_weather-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/LICENSE
+-rw-r--r--   0        0        0      910 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/README.md
+-rw-r--r--   0        0        0      897 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/src/how_is_the_weather/__init__.py
+-rw-r--r--   0        0        0     1016 2024-04-16 18:26:28.954656 how_is_the_weather-0.2.0/src/how_is_the_weather/weather.py
+-rw-r--r--   0        0        0     1555 1970-01-01 00:00:00.000000 how_is_the_weather-0.2.0/PKG-INFO
```

### Comparing `how_is_the_weather-0.1.0/LICENSE` & `how_is_the_weather-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `how_is_the_weather-0.1.0/pyproject.toml` & `how_is_the_weather-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "how_is_the_weather"
-version = "0.1.0"
+version = "0.2.0"
 authors = [{ name = "Jim Jimbo", email = "jim377893@gmail.com" }]
 description = "A simple tool to describe weather conditions."
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -13,18 +13,19 @@
 dependencies = ["requests"]
 
 [project.scripts]
 how-is-the-weather = "how_is_the_weather.weather:main"
 
 [tool.poetry]
 name = "how-is-the-weather"
-version = "0.1.0"
+version = "0.2.0"
 description = "A simple tool to describe weather conditions"
 authors = ["Jim Jimbo <jim377893@gmail.com>"]
 license = "MIT"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
```

### Comparing `how_is_the_weather-0.1.0/src/how_is_the_weather/weather.py` & `how_is_the_weather-0.2.0/src/how_is_the_weather/weather.py`

 * *Files identical despite different names*

