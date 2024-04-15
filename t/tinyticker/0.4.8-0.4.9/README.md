# Comparing `tmp/tinyticker-0.4.8.tar.gz` & `tmp/tinyticker-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.4.8.tar", max compression
+gzip compressed data, was "tinyticker-0.4.9.tar", max compression
```

## Comparing `tinyticker-0.4.8.tar` & `tinyticker-0.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-02-28 19:52:22.065387 tinyticker-0.4.8/LICENSE
--rw-r--r--   0        0        0     3863 2024-02-28 19:52:22.065387 tinyticker-0.4.8/README.md
--rw-r--r--   0        0        0      869 2024-02-28 19:52:22.065387 tinyticker-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      207 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/__init__.py
--rw-r--r--   0        0        0     5101 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/__main__.py
--rw-r--r--   0        0        0     1435 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/config.py
--rw-r--r--   0        0        0     9202 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/paths.py
--rw-r--r--   0        0        0    15317 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/ticker.py
--rw-r--r--   0        0        0     3155 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/utils.py
--rw-r--r--   0        0        0      318 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0      907 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     8353 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    11878 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14564 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10440 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     5824 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6616 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5679 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     3148 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/epdconfig.py
--rw-r--r--   0        0        0     1285 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2547 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6520 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/web/app.py
--rw-r--r--   0        0        0     2566 2024-02-28 19:52:22.069387 tinyticker-0.4.8/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    10283 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0      787 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1275 2024-02-28 19:52:22.073387 tinyticker-0.4.8/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 tinyticker-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-27 23:36:51.638880 tinyticker-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3863 2024-03-27 23:36:51.638880 tinyticker-0.4.9/README.md
+-rw-r--r--   0        0        0      869 2024-03-27 23:36:51.638880 tinyticker-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5101 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/__main__.py
+-rw-r--r--   0        0        0     1731 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/config.py
+-rw-r--r--   0        0        0     9202 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/paths.py
+-rw-r--r--   0        0        0    15408 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/ticker.py
+-rw-r--r--   0        0        0     3155 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/utils.py
+-rw-r--r--   0        0        0      318 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1060 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     8353 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    11878 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14564 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10440 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     5824 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6616 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5679 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     3148 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/epdconfig.py
+-rw-r--r--   0        0        0     1285 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2547 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6826 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2566 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-03-27 23:36:51.642880 tinyticker-0.4.9/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    10616 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0      787 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1275 2024-03-27 23:36:51.646880 tinyticker-0.4.9/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 tinyticker-0.4.9/PKG-INFO
```

### Comparing `tinyticker-0.4.8/LICENSE` & `tinyticker-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/README.md` & `tinyticker-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/pyproject.toml` & `tinyticker-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.4.8"
+version = "0.4.9"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.4.8/tinyticker/__main__.py` & `tinyticker-0.4.9/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/config.py` & `tinyticker-0.4.9/tinyticker/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,16 +19,23 @@
     wait_time: Optional[int] = None
     plot_type: str = "candle"
     mav: Optional[int] = None
     volume: bool = False
 
 
 @dc.dataclass
+class SequenceConfig:
+    skip_outdated: bool = True
+    skip_empty: bool = True
+
+
+@dc.dataclass
 class TinytickerConfig:
     tickers: List[TickerConfig] = dc.field(default_factory=lambda: [TickerConfig()])
+    sequence: SequenceConfig = dc.field(default_factory=lambda: SequenceConfig())
     epd_model: str = "EPD_v3"
     api_key: Optional[str] = None
     flip: bool = False
 
     @classmethod
     def from_file(cls, file: Path) -> "TinytickerConfig":
         with file.open("r") as fp:
@@ -40,14 +47,17 @@
 
     @classmethod
     def from_json(cls, json_: Union[str, bytes, bytearray]) -> "TinytickerConfig":
         data = json.loads(json_)
         data["tickers"] = [
             TickerConfig(**ticker_data) for ticker_data in data["tickers"]
         ]
+        data["sequence"] = SequenceConfig(
+            **data.get("sequence", dc.asdict(SequenceConfig()))
+        )
         return cls(**data)
 
     def to_json(self) -> str:
         return json.dumps(self.to_dict())
 
     def to_dict(self) -> dict:
         return dc.asdict(self)
```

### Comparing `tinyticker-0.4.8/tinyticker/display.py` & `tinyticker-0.4.9/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/ticker.py` & `tinyticker-0.4.9/tinyticker/ticker.py`

 * *Files 3% similar despite different names*

```diff
@@ -336,22 +336,19 @@
                 str(self.wait_time),
             ]
         )
 
 
 class Sequence:
     @classmethod
-    def from_tinyticker_config(
-        cls, tt_config: TinytickerConfig, **kwargs
-    ) -> "Sequence":
+    def from_tinyticker_config(cls, tt_config: TinytickerConfig) -> "Sequence":
         """Create a `Sequence` from a `TinytickerConfig`.
 
         Args:
             tt_config: `TinytickerConfig` from which to create the `Sequence`.
-            **kwargs: Paseed to the `Sequence.__init__` method.
 
         Returns:
             The `Sequence` instance.
         """
         return Sequence(
             [
                 Ticker(
@@ -363,31 +360,31 @@
                     wait_time=ticker.wait_time,
                     plot_type=ticker.plot_type,
                     mav=ticker.mav,
                     volume=ticker.volume,
                 )
                 for ticker in tt_config.tickers
             ],
-            **kwargs,
+            skip_empty=tt_config.sequence.skip_empty,
+            skip_outdated=tt_config.sequence.skip_outdated,
         )
 
     def __init__(
         self,
         tickers: List[Ticker],
         skip_empty: bool = True,
         skip_outdated: bool = True,
     ):
         """Runs multiple `Ticker` instances in sequence.
 
         Args:
             tickers: list of `Ticker` instances.
-            skip_empty: if the response doesn't contain any data, move on to the
-                next ticker.
-            skip_outdated: if the last candle of the response is too old, move on to the
-                next ticker. This typically happens when the stock market closes.
+            skip_empty: if the response doesn't contain any data, move on to the next ticker.
+            skip_outdated: if the last candle of the response is too old, move on to the next
+                ticker. This typically happens when the stock market closes.
         """
         if len(tickers) == 0:
             raise ValueError("No tickers provided.")
         self.tickers = tickers
         self.skip_empty = skip_empty
         self.skip_outdated = skip_outdated
 
@@ -432,8 +429,11 @@
                         LOGGER.debug(f"{ticker} response outdated, skipping.")
                         continue
                 all_skipped = False
                 yield (ticker, response)
                 time.sleep(ticker.wait_time)
 
     def __str__(self):
-        return "Sequence: \n" + "\n".join([ticker.__str__() for ticker in self.tickers])
+        return (
+            f"Sequence(skip_outdated={self.skip_outdated}, skip_empty={self.skip_empty}): \n"
+            + "\n".join([ticker.__str__() for ticker in self.tickers])
+        )
```

### Comparing `tinyticker-0.4.8/tinyticker/utils.py` & `tinyticker-0.4.9/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/epdconfig.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/epdconfig.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/waveshare_lib/models.py` & `tinyticker-0.4.9/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/__main__.py` & `tinyticker-0.4.9/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/app.py` & `tinyticker-0.4.9/tinyticker/web/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from socket import timeout
 from typing import Optional
 from urllib.error import HTTPError, URLError
 
 from flask import Flask, abort, redirect, render_template, request, send_from_directory
 
 from .. import __version__
-from ..config import PLOT_TYPES, TickerConfig, TinytickerConfig
+from ..config import PLOT_TYPES, SequenceConfig, TickerConfig, TinytickerConfig
 from ..paths import CONFIG_FILE, LOG_DIR
 from ..ticker import INTERVAL_LOOKBACKS, INTERVAL_TIMEDELTAS, SYMBOL_TYPES
 from ..utils import check_for_update
 from ..waveshare_lib.models import MODELS
 from .command import COMMANDS, reboot, refresh
 
 LOGGER = logging.getLogger(__name__)
@@ -105,23 +105,30 @@
         tickers["plot_type"] = request.args.getlist("plot_type")
         tickers["interval"] = request.args.getlist("interval")
         tickers["lookback"] = request.args.getlist("lookback", type=no_empty_int)
         tickers["wait_time"] = request.args.getlist("wait_time", type=no_empty_int)
         tickers["mav"] = request.args.getlist("mav", type=no_empty_int)
         tickers["volume"] = request.args.getlist("volume", type=str_to_bool)
 
+        sequence = SequenceConfig(
+            skip_outdated=request.args.get("skip_outdated", False, type=bool),
+            # Note: currently not toggleable from the web app
+            skip_empty=request.args.get("skip_empty", True, type=bool),
+        )
+
         # invert the ticker dict of list to list of dict and create ticker list
         tickers = [
             TickerConfig(**dict(zip(tickers, t))) for t in zip(*tickers.values())
         ]
         tt_config = TinytickerConfig(
             api_key=request.args.get("api_key", type=no_empty_str),
             flip=request.args.get("flip", default=False, type=bool),
             epd_model=request.args.get("epd_model", "EPD_v3"),
             tickers=tickers,
+            sequence=sequence,
         )
         LOGGER.debug(tt_config)
         tt_config.to_file(config_file)
         refresh()
         return redirect("/", code=302)
 
     @app.route("/command")
```

### Comparing `tinyticker-0.4.8/tinyticker/web/command.py` & `tinyticker-0.4.9/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.4.9/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.4.9/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.4.9/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.4.9/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/index.html` & `tinyticker-0.4.9/tinyticker/web/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -131,14 +131,15 @@
                 {%- endfor %}
                   <div class="uk-card uk-card-primary uk-flex-none uk-margin-right uk-padding-small uk-button uk-border-rounded uk-animation-fade" onclick="add_ticker()">
                     <span uk-icon="plus"></span>
                   </div>
                 </div>
               </div>
               <div class="uk-width-1-1 uk-margin">
+                <label class="uk-form-label" for="skip_outdated" uk-tooltip="Typically happens when the market is closed."><input class="uk-checkbox uk-margin-small-right" type="checkbox" id="skip_outdated" name="skip_outdated" {% if sequence.skip_outdated | default(True) %}checked{% endif %}>Skip tickers with oudated data</label>
                 <button type="submit" value="submit" class="uk-button uk-button-primary uk-width-expand">Apply</button>
               </div>
             </div>
           </form>
         </div>
         <div class="uk-width-large uk-margin">
           <div class="uk-width-1-1">
```

#### html2text {}

```diff
@@ -45,11 +45,12 @@
 none %} [mav                 ]{%- else %} [{{ticker.mav}}      ]{%- endif %}
 Show trade volume {% if ticker.volume | default(False) %} {% else %} {% endif
 %}
 % if ticker.volume | default(False) %}checked{% endif %}
 onclick="this.previousElementSibling.value=1-
 this.previousElementSibling.value">
 {%- endfor %}
-Apply
+% if sequence.skip_outdated | default(True) %}checked{% endif %}>Skip tickers
+with oudated data Apply
 Command
 {% for command, desc in commands | items %} {{command.title()}} {% endfor %}
 TinyTicker v{{version}} - _T_i_n_y_T_i_c_k_e_r - _L_o_g_ _f_i_l_e_s
```

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/js/index.js` & `tinyticker-0.4.9/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.4.9/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.4.9/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/tinyticker/web/templates/logfiles.html` & `tinyticker-0.4.9/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.4.8/PKG-INFO` & `tinyticker-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.4.8
+Version: 0.4.9
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.8,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.4.8 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.4.9 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

