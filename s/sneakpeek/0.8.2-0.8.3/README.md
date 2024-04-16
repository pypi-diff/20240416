# Comparing `tmp/sneakpeek-0.8.2.tar.gz` & `tmp/sneakpeek-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneakpeek-0.8.2.tar", max compression
+gzip compressed data, was "sneakpeek-0.8.3.tar", max compression
```

## Comparing `sneakpeek-0.8.2.tar` & `sneakpeek-0.8.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-06-22 08:34:03.000000 sneakpeek-0.8.2/LICENSE
--rw-r--r--   0        0        0     9150 2023-07-05 11:03:50.000000 sneakpeek-0.8.2/README.md
--rw-r--r--   0        0        0     1582 2023-07-05 13:23:45.000000 sneakpeek-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       56 2023-07-05 13:23:51.000000 sneakpeek-0.8.2/sneakpeek/__init__.py
--rw-r--r--   0        0        0     1245 2023-06-23 02:05:57.000000 sneakpeek-0.8.2/sneakpeek/console.py
--rw-r--r--   0        0        0      458 2023-06-23 01:43:18.000000 sneakpeek-0.8.2/sneakpeek/server.py
--rw-r--r--   0        0        0     4978 2023-07-05 11:34:49.000000 sneakpeek-0.8.2/sneakpeek/sneakpeek.py
--rw-r--r--   0        0        0    10861 1970-01-01 00:00:00.000000 sneakpeek-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-16 13:11:38.798221 sneakpeek-0.8.3/LICENSE
+-rw-r--r--   0        0        0     8064 2024-04-16 13:11:38.798221 sneakpeek-0.8.3/README.md
+-rw-r--r--   0        0        0     1659 2024-04-16 13:38:03.500435 sneakpeek-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-16 13:11:38.799221 sneakpeek-0.8.3/sneakpeek/__init__.py
+-rw-r--r--   0        0        0     1245 2024-04-16 13:11:38.800221 sneakpeek-0.8.3/sneakpeek/console.py
+-rw-r--r--   0        0        0      458 2024-04-16 13:11:38.800221 sneakpeek-0.8.3/sneakpeek/server.py
+-rw-r--r--   0        0        0     5725 2024-04-16 13:38:03.500435 sneakpeek-0.8.3/sneakpeek/sneakpeek.py
+-rw-r--r--   0        0        0     9820 1970-01-01 00:00:00.000000 sneakpeek-0.8.3/PKG-INFO
```

### Comparing `sneakpeek-0.8.2/LICENSE` & `sneakpeek-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sneakpeek-0.8.2/README.md` & `sneakpeek-0.8.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```
 
 
 ## Usage as a Python Module
 
 ### From a URL
 
-```py
+```sh
 >>> import sneakpeek
 >>> from pprint import pprint
 
 >>> link = sneakpeek.SneakPeek("https://www.youtube.com/watch?v=dQw4w9WgXcQ")
 >>> link.fetch()
 >>> link.is_valid()
 True
@@ -204,43 +204,27 @@
 poetry run pytest
 ```
 
 - Tested Websites
   - [x] [YouTube](https://youtube.com)
   - [x] [GitHub](https://github.com)
   - [x] [LinkedIN](https://linkedin.com)
+  - [x] [Reddit](https://reddit.com)
   - [x] [StackOverflow](https://stackoverflow.com)
   - [x] [Business Insider](https://www.businessinsider.in)
   - [x] [HackerNews](https://news.ycombinator.com/)
+  - [x] [Twitter](https://twitter.com)
 
 
 ## TODO
 
-- [ ] handle images ending in jpg / png etc
-  - [ ] the image could be this itself or a snap of the top part of the image
-  - [ ] the text can be AI generated or text detected in image
-  - [ ] https://i.ibb.co/ZLp46Kx/Screenshot-20230623-133028-Gmail.jpg
-- [ ] [Twitter](https://twitter.com) use v@ API with tweepy and have fallback as what is current
-- [ ] write a custom parser for [Reddit](https://reddit.com)
-- [ ] switch CLI to [typer](https://github.com/tiangolo/typer)
 - [ ] [Instagram](https://instagram.com) (using [instagram-scraper](https://github.com/arc298/instagram-scraper))
-- [ ] [Techcrunch](https://techcrunch.com/2023/06/23/pillow-discontinue/)
 - [ ] [Facebook](https://facebook.com)
+- [ ] https://joinfishbowl.com/post_v3ibj1p63t
 - [ ] CI/CD for publishing to PyPi
-- [ ] [Google](https://google.com) should show Google's image atleast
-- [ ] [LinkedIn](https://linkedin.com)
-- [ ] [HackerNews](https://news.ycombinator.com/) via API
-- [ ] safe image handling for sites like - https://techpays.eu/countries/germany
-- [ ] test cases
-  - [ ] test website without image
-  - [ ] test website without description
-  - [ ] test google should return custom Google image
-  - [ ] https://www.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
-  - [ ] https://edition.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
-  - [ ] https://www.levels.fyi/comp.html?track=Software+Engineer&showAll=true
 
 
 ## Contribution
 
 Have better suggestions to optimize the server image? Found some typos? Need special handling for a new website? Found a bug? Go ahead and create an [Issue](https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind welcome!
 
 Want to work on a TODO? Its always a good idea to talk about what are going to do before you actually start it, so frustration can be avoided.
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 sneakpeek)](https://hub.docker.com/r/codingcoffee/sneakpeek) [![Docker Image
 Size (tag)](https://img.shields.io/docker/image-size/codingcoffee/sneakpeek/
 latest)](https://hub.docker.com/r/codingcoffee/sneakpeek) ## What is supported
 - Any page which supports [Open Graph Protocol](https://ogp.me) (which most
 sane websites do) - Special handling for sites like - [Twitter](https://
 twitter.com) (requires a twitter [API key](https://developer.twitter.com/)) ##
 Installation Run the following to install ```sh pip install sneakpeek ``` ##
-Usage as a Python Module ### From a URL ```py >>> import sneakpeek >>> from
+Usage as a Python Module ### From a URL ```sh >>> import sneakpeek >>> from
 pprint import pprint >>> link = sneakpeek.SneakPeek("https://www.youtube.com/
 watch?v=dQw4w9WgXcQ") >>> link.fetch() >>> link.is_valid() True >>> pprint
 (link) {'description': 'The official video for âNever Gonna Give You Upâ by
 Rick ' 'AstleyTaken from the album âWhenever You Need Somebodyâ â '
 'deluxe 2CD and digital deluxe out 6th May ...', 'domain': 'www.youtube.com',
 'image': 'https://i.ytimg.com/vi/dQw4w9WgXcQ/maxresdefault.jpg', 'image:
 height': '720', 'image:width': '1280', 'scrape': False, 'site_name': 'YouTube',
@@ -79,38 +79,24 @@
 [here](https://developer.twitter.com/) - Create an app - Add the following
 variables as ENV vars ``` TWITTER_CONSUMER_KEY="sample"
 TWITTER_CONSUMER_SECRET="sample" TWITTER_ACCESS_TOKEN="sample"
 TWITTER_ACCESS_TOKEN_SECRET="sample" ``` ## Development ``` pip install -
 U poetry git clone https://github.com/codingcoffee/sneakpeek cd sneakpeek
 poetry install ``` ## Running Tests ```sh poetry run pytest ``` - Tested
 Websites - [x] [YouTube](https://youtube.com) - [x] [GitHub](https://
-github.com) - [x] [LinkedIN](https://linkedin.com) - [x] [StackOverflow](https:
-//stackoverflow.com) - [x] [Business Insider](https://www.businessinsider.in) -
-[x] [HackerNews](https://news.ycombinator.com/) ## TODO - [ ] handle images
-ending in jpg / png etc - [ ] the image could be this itself or a snap of the
-top part of the image - [ ] the text can be AI generated or text detected in
-image - [ ] https://i.ibb.co/ZLp46Kx/Screenshot-20230623-133028-Gmail.jpg - [ ]
-[Twitter](https://twitter.com) use v@ API with tweepy and have fallback as what
-is current - [ ] write a custom parser for [Reddit](https://reddit.com) - [ ]
-switch CLI to [typer](https://github.com/tiangolo/typer) - [ ] [Instagram]
-(https://instagram.com) (using [instagram-scraper](https://github.com/arc298/
-instagram-scraper)) - [ ] [Techcrunch](https://techcrunch.com/2023/06/23/
-pillow-discontinue/) - [ ] [Facebook](https://facebook.com) - [ ] CI/CD for
-publishing to PyPi - [ ] [Google](https://google.com) should show Google's
-image atleast - [ ] [LinkedIn](https://linkedin.com) - [ ] [HackerNews](https:/
-/news.ycombinator.com/) via API - [ ] safe image handling for sites like -
-https://techpays.eu/countries/germany - [ ] test cases - [ ] test website
-without image - [ ] test website without description - [ ] test google should
-return custom Google image - [ ] https://www.cnn.com/2022/07/07/tech/tech-
-layoffs-workers-silicon-valley/index.html - [ ] https://edition.cnn.com/2022/
-07/07/tech/tech-layoffs-workers-silicon-valley/index.html - [ ] https://
-www.levels.fyi/comp.html?track=Software+Engineer&showAll=true ## Contribution
-Have better suggestions to optimize the server image? Found some typos? Need
-special handling for a new website? Found a bug? Go ahead and create an [Issue]
-(https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind
-welcome! Want to work on a TODO? Its always a good idea to talk about what are
-going to do before you actually start it, so frustration can be avoided. Some
-rules for coding: - Use the code style the project uses - For each feature,
-make a seperate branch, so it can be reviewed separately - Use commits with a
-good description, so everyone can see what you did ## License The code in this
-repository has been released under the [MIT License](https://opensource.org/
-licenses/MIT)
+github.com) - [x] [LinkedIN](https://linkedin.com) - [x] [Reddit](https://
+reddit.com) - [x] [StackOverflow](https://stackoverflow.com) - [x] [Business
+Insider](https://www.businessinsider.in) - [x] [HackerNews](https://
+news.ycombinator.com/) - [x] [Twitter](https://twitter.com) ## TODO - [ ]
+[Instagram](https://instagram.com) (using [instagram-scraper](https://
+github.com/arc298/instagram-scraper)) - [ ] [Facebook](https://facebook.com) -
+[ ] https://joinfishbowl.com/post_v3ibj1p63t - [ ] CI/CD for publishing to PyPi
+## Contribution Have better suggestions to optimize the server image? Found
+some typos? Need special handling for a new website? Found a bug? Go ahead and
+create an [Issue](https://github.com/codingcoffee/sneakpeek/issues)!
+Contributions of any kind welcome! Want to work on a TODO? Its always a good
+idea to talk about what are going to do before you actually start it, so
+frustration can be avoided. Some rules for coding: - Use the code style the
+project uses - For each feature, make a seperate branch, so it can be reviewed
+separately - Use commits with a good description, so everyone can see what you
+did ## License The code in this repository has been released under the [MIT
+License](https://opensource.org/licenses/MIT)
```

### Comparing `sneakpeek-0.8.2/pyproject.toml` & `sneakpeek-0.8.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sneakpeek"
-version = "0.8.2"
+version = "0.8.3"
 description = "A python module to generate link previews."
 license = "MIT"
 authors = ["Ameya Shenoy <shenoy.ameya@gmail.com>"]
 maintainers = ["Ameya Shenoy <shenoy.ameya@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/codingcoffee/sneakpeek"
 repository = "https://github.com/codingcoffee/sneakpeek"
@@ -24,27 +24,31 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 validators = "^0.20.0"
 beautifulsoup4 = "^4.11.1"
 fastapi = "^0.79.0"
 click = "^8.1.3"
 uvicorn = "^0.18.2"
 rich = "^12.5.1"
 tweepy = "^4.10.0"
 loguru = "^0.7.0"
+yt-dlp = "^2024.4.9"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
+[tool.poetry.group.dev.dependencies]
+bpython = "^0.24"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 sneakpeek = 'sneakpeek.console:cli'
```

### Comparing `sneakpeek-0.8.2/sneakpeek/console.py` & `sneakpeek-0.8.3/sneakpeek/console.py`

 * *Files identical despite different names*

### Comparing `sneakpeek-0.8.2/sneakpeek/sneakpeek.py` & `sneakpeek-0.8.3/sneakpeek/sneakpeek.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 import re
 import urllib.request
 from urllib.parse import urlparse
 
 # third-party imports
 import validators
+import yt_dlp as ydl
 from bs4 import BeautifulSoup
 from loguru import logger
 
 
 class SneakPeek(dict):
     """ """
 
@@ -48,14 +49,28 @@
 
     def __getattr__(self, name):
         return self[name]
 
     def is_valid_url(self, url=None):
         return validators.url(url)
 
+    def fetch_and_parse_youtube(self):
+        ydl_opts = {
+            "quiet": True,
+        }
+        with ydl.YoutubeDL(ydl_opts) as ydl_youtube:
+            try:
+                info_dict = ydl_youtube.extract_info(self.url, download=False)
+                self.title = info_dict.get("title")
+                self.description = info_dict.get("description")
+                self.title = info_dict.get("title")
+                self.image = info_dict.get("thumbnail")
+            except ydl.utils.DownloadError:
+                return
+
     def fetch_and_parse_twitter(self):
         if not isinstance(self.url, str):
             return
         if "status" in self.url:
             # tweet_id = int(self.url.split("status/")[-1].split("?")[0])
             username = self.url.split("/")[3]
             self.title = f"{username} on Twitter"
@@ -68,20 +83,27 @@
             self.description = "Social Network Company"
         else:
             username = self.url.strip("/").split("/")[-1]
             self.title = f"{username} on Twitter"
             self.type = "profile"
             self.description = ""
 
-        self.image = "https://upload.wikimedia.org/wikipedia/commons/6/6f/Logo_of_Twitter.svg"
+        self.image = "https://upload.wikimedia.org/wikipedia/commons/5/57/X_logo_2023_%28white%29.png"
 
     def fetch(self):
         """ """
-        if self.domain in ["twitter.com", "mobile.twitter.com", "www.twitter.com"]:
+        if self.domain in [
+            "twitter.com",
+            "mobile.twitter.com",
+            "www.twitter.com",
+            "x.com",
+        ]:
             return self.fetch_and_parse_twitter()
+        if self.domain in ["youtube.com", "www.youtube.com"]:
+            return self.fetch_and_parse_youtube()
         if not isinstance(self.url, str):
             return
         # TODO: use random user agent for every request - https://github.com/Luqman-Ud-Din/random_user_agent
         req = urllib.request.Request(self.url, headers={"User-Agent": "Mozilla/5.0"})
         try:
             with urllib.request.urlopen(req) as raw:
                 html = raw.read()
```

### Comparing `sneakpeek-0.8.2/PKG-INFO` & `sneakpeek-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: sneakpeek
-Version: 0.8.2
+Version: 0.8.3
 Summary: A python module to generate link previews.
 Home-page: https://github.com/codingcoffee/sneakpeek
 License: MIT
 Keywords: open-graph-protocol,ogp,twitter,twitter-cards,python,schema,link-preview
 Author: Ameya Shenoy
 Author-email: shenoy.ameya@gmail.com
 Maintainer: Ameya Shenoy
 Maintainer-email: shenoy.ameya@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fastapi (>=0.79.0,<0.80.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: tweepy (>=4.10.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.18.2,<0.19.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: yt-dlp (>=2024.4.9,<2025.0.0)
 Project-URL: Documentation, https://github.com/codingcoffee/sneakpeek
 Project-URL: Repository, https://github.com/codingcoffee/sneakpeek
 Description-Content-Type: text/markdown
 
 
 <div align="center">
   <h1>
@@ -70,15 +71,15 @@
 ```
 
 
 ## Usage as a Python Module
 
 ### From a URL
 
-```py
+```sh
 >>> import sneakpeek
 >>> from pprint import pprint
 
 >>> link = sneakpeek.SneakPeek("https://www.youtube.com/watch?v=dQw4w9WgXcQ")
 >>> link.fetch()
 >>> link.is_valid()
 True
@@ -244,43 +245,27 @@
 poetry run pytest
 ```
 
 - Tested Websites
   - [x] [YouTube](https://youtube.com)
   - [x] [GitHub](https://github.com)
   - [x] [LinkedIN](https://linkedin.com)
+  - [x] [Reddit](https://reddit.com)
   - [x] [StackOverflow](https://stackoverflow.com)
   - [x] [Business Insider](https://www.businessinsider.in)
   - [x] [HackerNews](https://news.ycombinator.com/)
+  - [x] [Twitter](https://twitter.com)
 
 
 ## TODO
 
-- [ ] handle images ending in jpg / png etc
-  - [ ] the image could be this itself or a snap of the top part of the image
-  - [ ] the text can be AI generated or text detected in image
-  - [ ] https://i.ibb.co/ZLp46Kx/Screenshot-20230623-133028-Gmail.jpg
-- [ ] [Twitter](https://twitter.com) use v@ API with tweepy and have fallback as what is current
-- [ ] write a custom parser for [Reddit](https://reddit.com)
-- [ ] switch CLI to [typer](https://github.com/tiangolo/typer)
 - [ ] [Instagram](https://instagram.com) (using [instagram-scraper](https://github.com/arc298/instagram-scraper))
-- [ ] [Techcrunch](https://techcrunch.com/2023/06/23/pillow-discontinue/)
 - [ ] [Facebook](https://facebook.com)
+- [ ] https://joinfishbowl.com/post_v3ibj1p63t
 - [ ] CI/CD for publishing to PyPi
-- [ ] [Google](https://google.com) should show Google's image atleast
-- [ ] [LinkedIn](https://linkedin.com)
-- [ ] [HackerNews](https://news.ycombinator.com/) via API
-- [ ] safe image handling for sites like - https://techpays.eu/countries/germany
-- [ ] test cases
-  - [ ] test website without image
-  - [ ] test website without description
-  - [ ] test google should return custom Google image
-  - [ ] https://www.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
-  - [ ] https://edition.cnn.com/2022/07/07/tech/tech-layoffs-workers-silicon-valley/index.html
-  - [ ] https://www.levels.fyi/comp.html?track=Software+Engineer&showAll=true
 
 
 ## Contribution
 
 Have better suggestions to optimize the server image? Found some typos? Need special handling for a new website? Found a bug? Go ahead and create an [Issue](https://github.com/codingcoffee/sneakpeek/issues)! Contributions of any kind welcome!
 
 Want to work on a TODO? Its always a good idea to talk about what are going to do before you actually start it, so frustration can be avoided.
```

