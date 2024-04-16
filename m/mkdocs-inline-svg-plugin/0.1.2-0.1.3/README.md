# Comparing `tmp/mkdocs_inline_svg_plugin-0.1.2.tar.gz` & `tmp/mkdocs_inline_svg_plugin-0.1.3.tar.gz`

## Comparing `mkdocs_inline_svg_plugin-0.1.2.tar` & `mkdocs_inline_svg_plugin-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/mkdocs.yml
--rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/docs/index.md
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/docs/css/extra.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/src/inline_svg/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/src/inline_svg/config.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/src/inline_svg/plugin.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/src/inline_svg/util.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/README.md
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/mkdocs.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-publish-test.yml
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/docs/index.md
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/docs/css/extra.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/__version__.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/config.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/plugin.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/util.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 mkdocs_inline_svg_plugin-0.1.3/PKG-INFO
```

### Comparing `mkdocs_inline_svg_plugin-0.1.2/mkdocs.yml` & `mkdocs_inline_svg_plugin-0.1.3/mkdocs.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 # extra_css:
 #   - css/extra.css
 
 plugins:
   - kroki:
       # ServerURL: http://127.0.0.1:9000
       FencePrefix: ''
-      HttpMethod: 'POST'
-      DownloadImages: true
+      # HttpMethod: 'POST'
+      # DownloadImages: false
   - inline-svg:
-      AltName: Kroki
-      # PatchStyle: true
+      alt_name: Kroki
+      include_assets: true
+      # patch_style: true
```

### Comparing `mkdocs_inline_svg_plugin-0.1.2/docs/index.md` & `mkdocs_inline_svg_plugin-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.2/docs/css/extra.css` & `mkdocs_inline_svg_plugin-0.1.3/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.2/src/inline_svg/plugin.py` & `mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-from mkdocs.plugins import BasePlugin
-from mkdocs.config.config_options import Type
+import re
+
 from bs4 import BeautifulSoup
+from mkdocs.plugins import BasePlugin as MkDocsBasePlugin
 
-from inline_svg.config import Config
+from inline_svg.config import InlineSvgConfig
 from inline_svg.util import (
-    info,
-    debug,
     get_svg_data,
     get_svg_tag,
     include_assets,
+    log,
 )
-import re
-from tempfile import TemporaryDirectory
 
-WILDCARD = "*"
-
-
-class InlineSvgPlugin(BasePlugin):
-    config_scheme = (
-        ("AltName", Type(str, default=WILDCARD)),
-        ("IncludeAssets", Type(bool, default=False)),
-        ("AssetDir", Type(str, default="assets/")),
-        ("PatchStyle", Type(bool, default=False)),
-    )
 
+class InlineSvgPlugin(MkDocsBasePlugin[InlineSvgConfig]):
     def on_config(self, config, **_kwargs):
-        info(f"Configuring: {self.config}")
-        self._config = Config(
-            alt_name=self.config["AltName"],
-            include_assets=self.config["IncludeAssets"],
-            asset_dir=self.config["AssetDir"],
-            patch_style=self.config["PatchStyle"],
-            site_url=config.get("site_url", "/"),
-            site_dir=config["site_dir"],
-            temp_dir=TemporaryDirectory(),
-        )
+        self.config.site_url = config.get("site_url", "/")
+        self.config.site_dir = config["site_dir"]
+        log.debug(f"Config: {self.config}")
+
         return config
 
-    def on_page_content(self, html, page, config, files, **_kwargs):
+    def on_page_content(self, html: str, *, files, **_kwargs):
+        log.debug("on_page_content")
         soup = BeautifulSoup(html, "html.parser")
 
-        for img_tag in soup.find_all("img", {"src": re.compile(r"\.svg$")}):
-            if self._config.alt_name != WILDCARD and img_tag["alt"] != self._config.alt_name:
+        for img_tag in soup.find_all("img", {"src": re.compile(r"(/svg/)|(\.svg$)")}):
+            if self.config.image_should_be_ignored(img_tag["alt"]):
                 continue
-            debug(f'inlining {img_tag} -> {img_tag["src"]}')
 
-            svg_data = get_svg_data(img_tag["src"], files, self._config)
+            log.debug(f'inlining {img_tag} -> {img_tag["src"]}')
+            svg_data = get_svg_data(img_tag["src"], files, self.config)
             if svg_data:
-                svg_tag = get_svg_tag(svg_data, self._config)
-                if self._config.include_assets:
-                    svg_tag = include_assets(svg_tag, files, self._config)
+                svg_tag = get_svg_tag(svg_data, self.config)
+                if self.config.include_assets:
+                    svg_tag = include_assets(svg_tag, files, self.config)
                 img_tag.replace_with(svg_tag)
 
         return str(soup)
```

### Comparing `mkdocs_inline_svg_plugin-0.1.2/src/inline_svg/util.py` & `mkdocs_inline_svg_plugin-0.1.3/src/inline_svg/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-from typing import Optional
-from bs4 import BeautifulSoup
-from functools import partial
-from mkdocs.plugins import log
-from mkdocs.structure.files import File, Files
-import requests
-import re
+from __future__ import annotations
+
 import os
-from inline_svg import __version__
-from inline_svg.config import Config
+import re
+from typing import TYPE_CHECKING
 
+import requests
+from bs4 import BeautifulSoup
+from mkdocs.plugins import get_plugin_logger
+from mkdocs.structure.files import (
+    File as MkDocsFile,
+)
+from mkdocs.structure.files import (
+    Files as MkDocsFiles,
+)
 
-PACKAGE_NAME = __package__.upper()
+from inline_svg.__version__ import __version__
 
-info = partial(log.info, f"[{PACKAGE_NAME}] %s")
-debug = partial(log.debug, f"[{PACKAGE_NAME}] %s")
-error = partial(log.error, f"[{PACKAGE_NAME}] %s")
+if TYPE_CHECKING:
+    from inline_svg.config import InlineSvgConfig
+
+
+log = get_plugin_logger(__name__)
 
 tag_blocklist = "script"
 user_agent_string = f"{__package__}/{__version__}"
+REQUESTS_TIMEOUT = 10
 
 
 def _sanitize_svg(svg_soup):
     for tag in svg_soup.findAll():
         if tag.name.lower() in tag_blocklist:
             tag.extract()
             continue
@@ -57,108 +64,112 @@
     "#fdf6e3": "var(--nomnoml-yellow2)",
 }
 
 
 def _patch_style(svg_soup):
     for element in svg_soup.findAll(["polygon", "ellipse", "rect", "line", "path", "text", "g"]):
         if "fill" in element.attrs:
-            element.attrs["fill"] = (
-                color_mappings.get(element.attrs["fill"]) or element.attrs["fill"]
-            )
+            element.attrs["fill"] = color_mappings.get(element.attrs["fill"]) or element.attrs["fill"]
         if "stroke" in element.attrs:
-            element.attrs["stroke"] = (
-                color_mappings.get(element.attrs["stroke"]) or element.attrs["stroke"]
-            )
+            element.attrs["stroke"] = color_mappings.get(element.attrs["stroke"]) or element.attrs["stroke"]
 
         if "style" in element.attrs:
             for color, replacement in color_mappings.items():
                 element.attrs["style"] = element.attrs["style"].replace(color, replacement)
 
         if element.name == "text" and "fill" not in element.attrs:
             element.attrs["fill"] = "var(--md-default-fg-color)"
 
 
-def _get_local_file_from_url(url: str, files: Files, config: Config) -> Optional[File]:
-    debug(f"url.removeprefix(config.site_url: {url}, {config.site_url}")
+def _get_local_file_from_url(url: str, files: MkDocsFiles, config: InlineSvgConfig) -> MkDocsFile | None:
     return files.get_file_from_path(url.removeprefix(config.site_url))
 
 
-def get_svg_data(url: str, files: Files, config: Config) -> str:
+def get_svg_data(url: str, files: MkDocsFiles, config: InlineSvgConfig) -> str | None:
     static_file = _get_local_file_from_url(url, files, config)
+    log.debug("_get_local_file_from_url(url, files, config): %s", static_file)
     if static_file:
         with open(static_file.abs_src_path) as file:
             svg_data = file.read()
         files.remove(static_file)
         return svg_data
-    else:
-        return requests.get(url, headers={"User-Agent": user_agent_string})
+
+    response = requests.get(url, headers={"User-Agent": user_agent_string}, timeout=REQUESTS_TIMEOUT)
+    if not response.ok:
+        log.error("Could not download [%s: %s %s]", url, response.status_code, response.reason)
+        return None
+
+    return response.text
 
 
-def include_assets(svg_soup, files: Files, config: Config):
+def include_assets(svg_soup, files: MkDocsFiles, config: InlineSvgConfig):
     url_regex = r'url\(["\']([^"\']+)["\']\)'
 
     def _css_url(url: str) -> str:
         return f'url("{url}")'
 
     def _download_asset(match: re.Match) -> str:
         url = match.groups("url")[0]
         if _get_local_file_from_url(url, files, config):
+            log.debug("asset not remote: %s, leaving as it is", url)
             return _css_url(url)
 
         file_name = url.split("/")[-1]
         file_src = os.path.join(config.temp_dir.name, file_name)
         file_path = os.path.join(config.site_url, config.asset_dir, file_name)
         if os.path.exists(file_src):
+            log.debug("asset already present: %s -> using present %s", url, file_path)
             return _css_url(file_path)
 
-        response = requests.get(url, headers={"User-Agent": user_agent_string})
+        response = requests.get(url, headers={"User-Agent": user_agent_string}, timeout=REQUESTS_TIMEOUT)
         if not response.ok:
-            error(f"Could not download [{url}: {response.status_code} {response.reason}]")
+            log.error("Could not download [%s]: %s %s], skipping", url, response.status_code, response.reason)
             return _css_url(url)
 
         asset_data = response.content
         with open(file_src, "xb") as file:
             file.write(asset_data)
 
         files.append(
-            File(
+            MkDocsFile(
                 path=file_name,
                 src_dir=config.temp_dir.name,
                 dest_dir=os.path.join(config.site_dir, config.asset_dir),
                 use_directory_urls=False,
             )
         )
+        log.debug("include asset: %s -> %s", url, file_path)
         return _css_url(file_path)
 
     for tag in svg_soup.find_all("style"):
         tag.string = re.sub(url_regex, _download_asset, tag.string)
 
     return svg_soup
 
 
-def get_svg_tag(svg_data, config: Config):
+def get_svg_tag(svg_data, config: InlineSvgConfig):
     svg_soup = BeautifulSoup(svg_data, "html.parser")
 
     # suppress upscaling of smaller images
     if "width" in svg_soup.svg.attrs:
         max_width = svg_soup.svg.attrs["width"]
         svg_soup.svg.attrs["style"] = f"max-width: {max_width}"
 
     # set the viewbox if not present
     if "viewbox" not in svg_soup.svg.attrs:
         if ("height" in svg_soup.svg.attrs) and ("width" in svg_soup.svg.attrs):
             height = "".join(filter(str.isdigit, svg_soup.svg.attrs["height"]))
             width = "".join(filter(str.isdigit, svg_soup.svg.attrs["width"]))
             svg_soup.svg.attrs["viewbox"] = f"0 0 {width} {height}"
         else:
-            error("SVG does not contain viewbox or height and width.")
+            log.error("SVG does not contain viewbox or height and width.")
 
     # remove unnecessary attrs
     svg_soup.svg.attrs = {
-        k: v for k, v in svg_soup.svg.attrs.items() if k in ["version", "viewbox", "style"]
+        k: v for k, v in svg_soup.svg.attrs.items() if k in ["version", "viewbox", "style", "width", "height"]
     }
 
     svg_soup.svg.attrs["id"] = __package__
     _sanitize_svg(svg_soup)
 
     if config.patch_style:
         _patch_style(svg_soup)
```

### Comparing `mkdocs_inline_svg_plugin-0.1.2/.gitignore` & `mkdocs_inline_svg_plugin-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.2/LICENSE.txt` & `mkdocs_inline_svg_plugin-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_inline_svg_plugin-0.1.2/README.md` & `mkdocs_inline_svg_plugin-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 ```yaml
 plugins:
   - kroki:
       FencePrefix: ''
       HttpMethod: 'POST'
       DownloadImages: true
   - inline-svg:
-      AltName: Kroki
+      alt_name: Kroki
 ```
 
 ### Configuration
 
 | Config value | What for |
 |---|---|
-| `AltName` | default: `*`, that does not check the `img` `alt` property |
-| `IncludeAssets` | default: `False`, looks for `url(..)`, downloads the contents to `AssetDir` and replaces the url |
-| `AssetDir` | default: `assets/` |
-| `PatchStyle` | default: `False`, this feature is **EXPERIMENTAL** and not yet finished, needs an additional CSS |
+| `alt_name` | default: `*`, that does not check the `img` `alt` property |
+| `include_assets` | default: `False`, looks for `url(..)`, downloads the contents to `asset_dir` and replaces the url |
+| `asset_dir` | default: `assets/` |
+| `patch_style` | default: `False`, this feature is **EXPERIMENTAL** and not yet finished, needs an additional CSS |
 
 ## Test
 
 Serve documentation:
 ```sh
 hatch run docs:serve
-```
+```
```

### Comparing `mkdocs_inline_svg_plugin-0.1.2/pyproject.toml` & `mkdocs_inline_svg_plugin-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,118 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mkdocs-inline-svg-plugin"
+version = "0.1.3"
 description = 'MkDocs plugin for inlining svg-href img tags'
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = ["MkDocs"]
 authors = [
   { name = "Oni Boni", email = "oniboni@mailbox.org" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-	"mkdocs >= 1.4.2",
-	"requests >= 2.31.0",
-	"beautifulsoup4 >= 4.12.0",
+	"mkdocs ~= 1.5.0",
+	"requests ~= 2.31.0",
+	"beautifulsoup4 ~= 4.12.0",
 ]
-dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/oniboni/mkdocs-inline-svg-plugin#readme"
 Issues = "https://github.com/oniboni/mkdocs-inline-svg-plugin/issues"
 Source = "https://github.com/oniboni/mkdocs-inline-svg-plugin"
 
 [project.entry-points."mkdocs.plugins"]
 inline-svg = "inline_svg.plugin:InlineSvgPlugin"
 
-[tool.hatch.version]
-path = "src/inline_svg/__init__.py"
-
 [tool.hatch.build.targets.wheel]
 packages = ["src/inline_svg"]
 
 [tool.hatch.envs.default]
 dependencies = [
+  "coverage[toml]>=6.5",
   "pytest",
-  "pytest-cov",
+  "pip-audit",
 ]
 [tool.hatch.envs.default.scripts]
-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=inline_svg --cov=tests {args}"
-no-cov = "cov --no-cov {args}"
+test = "pytest {args:tests}"
+test-cov = "coverage run -m pytest {args:tests}"
+cov-report = [
+  "- coverage combine",
+  "coverage report",
+]
+cov = [
+  "test-cov",
+  "cov-report",
+]
+audit = "pip-audit"
 
 [tool.hatch.envs.docs]
 dependencies = [
   "mkdocs-material",
 	"mkdocs-kroki-plugin"
 ]
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
-serve = "mkdocs serve --dev-addr localhost:8000 -vv"
+serve = "mkdocs serve -vv"
 
 [tool.hatch.envs.dev]
 dependencies = [
   "pre-commit",
-  "ruff",
-  "black",
   "commitizen",
-  "pip-audit",
-]
-post-install-commands = [
-  "pre-commit install --hook-type commit-msg --hook-type pre-push"
 ]
 [tool.hatch.envs.dev.scripts]
-audit = "pip-audit"
-lint = "ruff check src/"
-format = "black src/"
-commit = "cz commit"
-
-
-[tool.ruff]
-line-length = 99
-target-version = "py310"
-
-[tool.black]
-line-length = 99
-target-version = ['py310']
-
-# TODO: find a way testing mkdocs plugins
-# [[tool.hatch.envs.test.matrix]]
-# python = ["39", "310", "311"]
+install-pre-commit-hooks = "pre-commit install --hook-type commit-msg --hook-type pre-push"
+commit = ["install-pre-commit-hooks","cz commit"]
+
+
+# TODO: find a way testing mkdocs plugin
+# [[tool.hatch.envs.all.matrix]]
+# python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
+
+# [tool.hatch.envs.types]
+# dependencies = [
+#   "mypy>=1.0.0",
+# ]
+# [tool.hatch.envs.types.scripts]
+# check = "mypy --install-types --non-interactive {args:src/inline_svg tests}"
 
 # [tool.coverage.run]
+# source_pkgs = ["inline_svg", "tests"]
 # branch = true
 # parallel = true
+# omit = [
+#   "src/inline_svg/__about__.py",
+# ]
+
+# [tool.coverage.paths]
+# inline_svg = ["src/inline_svg", "*/inline_svg/src/inline_svg"]
+# tests = ["tests", "*/inline_svg/tests"]
 
 # [tool.coverage.report]
 # exclude_lines = [
 #   "no cov",
 #   "if __name__ == .__main__.:",
 #   "if TYPE_CHECKING:",
 # ]
+
+[tool.commitizen]
+version = "0.1.3"
+tag_format = "v$version"
+version_files = [
+  "pyproject.toml:version",
+  "src/inline_svg/__init__.py",
+]
```

### Comparing `mkdocs_inline_svg_plugin-0.1.2/PKG-INFO` & `mkdocs_inline_svg_plugin-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mkdocs-inline-svg-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: MkDocs plugin for inlining svg-href img tags
 Project-URL: Documentation, https://github.com/oniboni/mkdocs-inline-svg-plugin#readme
 Project-URL: Issues, https://github.com/oniboni/mkdocs-inline-svg-plugin/issues
 Project-URL: Source, https://github.com/oniboni/mkdocs-inline-svg-plugin
 Author-email: Oni Boni <oniboni@mailbox.org>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: MkDocs
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
-Requires-Dist: beautifulsoup4>=4.12.0
-Requires-Dist: mkdocs>=1.4.2
-Requires-Dist: requests>=2.31.0
+Requires-Python: >=3.8
+Requires-Dist: beautifulsoup4~=4.12.0
+Requires-Dist: mkdocs~=1.5.0
+Requires-Dist: requests~=2.31.0
 Description-Content-Type: text/markdown
 
 > **NOTE:** this project is still WIP!
 
 # mkdocs-inline-svg-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-inline-svg-plugin.svg)](https://pypi.org/project/mkdocs-inline-svg-plugin)
@@ -54,25 +56,25 @@
 ```yaml
 plugins:
   - kroki:
       FencePrefix: ''
       HttpMethod: 'POST'
       DownloadImages: true
   - inline-svg:
-      AltName: Kroki
+      alt_name: Kroki
 ```
 
 ### Configuration
 
 | Config value | What for |
 |---|---|
-| `AltName` | default: `*`, that does not check the `img` `alt` property |
-| `IncludeAssets` | default: `False`, looks for `url(..)`, downloads the contents to `AssetDir` and replaces the url |
-| `AssetDir` | default: `assets/` |
-| `PatchStyle` | default: `False`, this feature is **EXPERIMENTAL** and not yet finished, needs an additional CSS |
+| `alt_name` | default: `*`, that does not check the `img` `alt` property |
+| `include_assets` | default: `False`, looks for `url(..)`, downloads the contents to `asset_dir` and replaces the url |
+| `asset_dir` | default: `assets/` |
+| `patch_style` | default: `False`, this feature is **EXPERIMENTAL** and not yet finished, needs an additional CSS |
 
 ## Test
 
 Serve documentation:
 ```sh
 hatch run docs:serve
-```
+```
```

