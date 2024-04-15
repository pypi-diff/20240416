# Comparing `tmp/stickersbot-3.0.0.tar.gz` & `tmp/stickersbot-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stickersbot-3.0.0.tar", last modified: Tue Feb  6 04:09:22 2024, max compression
+gzip compressed data, was "stickersbot-4.0.0.tar", last modified: Mon Apr 15 23:17:44 2024, max compression
```

## Comparing `stickersbot-3.0.0.tar` & `stickersbot-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 04:09:22.391116 stickersbot-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 04:09:22.387116 stickersbot-3.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-06 04:09:04.000000 stickersbot-3.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 04:09:22.387116 stickersbot-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-06 04:09:04.000000 stickersbot-3.0.0/.github/workflows/python-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 04:09:04.000000 stickersbot-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-02-06 04:09:04.000000 stickersbot-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21888 2024-02-06 04:09:22.391116 stickersbot-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-06 04:09:04.000000 stickersbot-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-02-06 04:09:04.000000 stickersbot-3.0.0/avatar.png
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-06 04:09:04.000000 stickersbot-3.0.0/pylama.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-06 04:09:04.000000 stickersbot-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 04:09:22.391116 stickersbot-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 04:09:22.391116 stickersbot-3.0.0/stickersbot/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-06 04:09:04.000000 stickersbot-3.0.0/stickersbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 04:09:04.000000 stickersbot-3.0.0/stickersbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-02-06 04:09:04.000000 stickersbot-3.0.0/stickersbot/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-02-06 04:09:04.000000 stickersbot-3.0.0/stickersbot/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-06 04:09:04.000000 stickersbot-3.0.0/stickersbot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 04:09:22.391116 stickersbot-3.0.0/stickersbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21888 2024-02-06 04:09:22.000000 stickersbot-3.0.0/stickersbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-06 04:09:22.000000 stickersbot-3.0.0/stickersbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 04:09:22.000000 stickersbot-3.0.0/stickersbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 04:09:22.000000 stickersbot-3.0.0/stickersbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-06 04:09:22.000000 stickersbot-3.0.0/stickersbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 04:09:22.000000 stickersbot-3.0.0/stickersbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:17:44.800376 stickersbot-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:17:44.796376 stickersbot-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-15 23:17:34.000000 stickersbot-4.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:17:44.800376 stickersbot-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-15 23:17:34.000000 stickersbot-4.0.0/.github/workflows/python-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 23:17:34.000000 stickersbot-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-15 23:17:34.000000 stickersbot-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-15 23:17:44.800376 stickersbot-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-15 23:17:34.000000 stickersbot-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-15 23:17:34.000000 stickersbot-4.0.0/avatar.png
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 23:17:34.000000 stickersbot-4.0.0/pylama.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-15 23:17:34.000000 stickersbot-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:17:44.800376 stickersbot-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:17:44.800376 stickersbot-4.0.0/stickersbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-15 23:17:34.000000 stickersbot-4.0.0/stickersbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 23:17:34.000000 stickersbot-4.0.0/stickersbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-15 23:17:34.000000 stickersbot-4.0.0/stickersbot/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-15 23:17:34.000000 stickersbot-4.0.0/stickersbot/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-15 23:17:34.000000 stickersbot-4.0.0/stickersbot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:17:44.800376 stickersbot-4.0.0/stickersbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-15 23:17:44.000000 stickersbot-4.0.0/stickersbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-15 23:17:44.000000 stickersbot-4.0.0/stickersbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:17:44.000000 stickersbot-4.0.0/stickersbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 23:17:44.000000 stickersbot-4.0.0/stickersbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-15 23:17:44.000000 stickersbot-4.0.0/stickersbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 23:17:44.000000 stickersbot-4.0.0/stickersbot.egg-info/top_level.txt
```

### Comparing `stickersbot-3.0.0/.github/workflows/python-ci.yml` & `stickersbot-4.0.0/.github/workflows/python-ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.8', '3.11']
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install '.[dev]'
-    - name: Check code with black
-      run: |
-        black --check .
-    - name: Lint code
-      run: |
-        pylama
-    - name: Test with pytest
-      run: |
-        #pytest
+      - uses: actions/checkout@v2
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install '.[dev]'
+      - name: Check code with black
+        run: |
+          black --check .
+      - name: Lint code
+        run: |
+          pylama
+      - name: Test with pytest
+        run: |
+          #pytest
 
   deploy:
     needs: test
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - uses: actions/setup-python@v2
```

### Comparing `stickersbot-3.0.0/LICENSE` & `stickersbot-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stickersbot-3.0.0/README.md` & `stickersbot-4.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 ## Installation and configuration
 
 ```sh
 pip install stickersbot
 ```
 
+**IMPORTANT:** You might need first to install `libwebp` library in your system
+(For Debian/Ubuntu it's libwebp-dev package)
+
 Configure the bot:
 
 ```sh
 stickersbot init bot@example.com PASSWORD
 ```
 
 Start the bot:
@@ -26,12 +29,13 @@
 
 Run `stickersbot --help` to see all available options.
 
 ## Usage
 
 To get sticker packs, browse https://signalstickers.com/ and copy the URL of the pack you want (the link in the "+ Add to Signal" button, an URL starting with ``https://signal.art/addstickers``) and send the pack URL to the bot in private, the bot will send you a zip with the sticker pack.
 
-To create an sticker from a normal image send the image to the bot and it will send you back the image as sticker.
+To create an sticker from a normal image send the image to the bot and it will remove the background
+and send you back the image as sticker.
 
 Send any text to the bot to search packs matching the given text.
 
 Send an emoji to the bot to get a random sticker associated with that emoji.
```

### Comparing `stickersbot-3.0.0/avatar.png` & `stickersbot-4.0.0/avatar.png`

 * *Files identical despite different names*

### Comparing `stickersbot-3.0.0/pyproject.toml` & `stickersbot-4.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 
 [project]
 name = "stickersbot"
 description = "Sticker packs for all your Delta Chat needs"
 dynamic = ["version"]
 readme = "README.md"
 requires-python = ">=3.8"
-license = {file = "LICENSE"}
 keywords = ["deltachat", "bot"]
 authors = [
   {name = "adbenitez", email = "adb@merlinux.eu"},
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 ]
 dependencies = [
-    "deltabot-cli>=3.0.0,<4.0",
+    "deltabot-cli>=6.0.0,<7.0",
     "signalstickers-client>=3.1.0",
     "emoji>=1.6.1",
     "cachelib>=0.7.0",
     "requests>=2.26.0",
+    "pillow>=10.3.0",
+    "rembg>=2.0.56",
 ]
 
 [project.optional-dependencies]
 dev = [
   "black",
   "mypy",
   "isort",
```

### Comparing `stickersbot-3.0.0/stickersbot/hooks.py` & `stickersbot-4.0.0/stickersbot/hooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,147 +1,184 @@
 """Event Hooks"""
 
 import os
 from argparse import Namespace
+from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from cachelib import FileSystemCache
-from deltabot_cli import (
-    AttrDict,
+from deltabot_cli import BotCli
+from deltachat2 import (
     Bot,
-    BotCli,
     ChatType,
+    CoreEvent,
     EventType,
+    Message,
+    MsgData,
+    NewMsgEvent,
     events,
-    is_not_known_command,
 )
 from emoji import emoji_count
+from PIL import Image
+from rembg import remove
 
 from .signal import SignalStickers
 from .util import sizeof_fmt, upload
 
-DEF_MAX_PACK_SIZE = "15"
-DEF_CLOUDS = "https://ttm.sh/ https://envs.sh/ https://x0.at/ https://0x0.st/"
 signal = SignalStickers()
 cli = BotCli("stickersbot")
 
 
 @cli.on_init
 def on_init(bot: Bot, _args: Namespace) -> None:
     for accid in bot.rpc.get_all_account_ids():
         if not bot.rpc.get_config(accid, "displayname"):
             bot.rpc.set_config(accid, "displayname", "StickersBot")
             status = "I am a Delta Chat bot, send me /help for more info"
             bot.rpc.set_config(accid, "selfstatus", status)
-            bot.rpc.set_config(accid, "delete_server_after", "1")
+            bot.rpc.set_config(accid, "delete_device_after", str(60 * 60 * 24))
 
 
 @cli.on_start
 def on_start(_bot: Bot, args: Namespace) -> None:
     path = os.path.join(args.config_dir, "cache")
     if not os.path.exists(path):
         os.makedirs(path)
     signal.cache = FileSystemCache(
         path, threshold=5000, default_timeout=60 * 60 * 24 * 60
     )
 
 
 @cli.on(events.RawEvent)
-def log_event(bot: Bot, accid: int, event: AttrDict) -> None:
+def log_event(bot: Bot, accid: int, event: CoreEvent) -> None:
     if event.kind == EventType.INFO:
-        bot.logger.info(event.msg)
+        bot.logger.debug(event.msg)
     elif event.kind == EventType.WARNING:
         bot.logger.warning(event.msg)
     elif event.kind == EventType.ERROR:
         bot.logger.error(event.msg)
+    elif event.kind == EventType.MSG_DELIVERED:
+        bot.rpc.delete_messages(accid, [event.msg_id])
     elif event.kind == EventType.SECUREJOIN_INVITER_PROGRESS:
         if event.progress == 1000:
-            bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
-            chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
-            send_help(bot, accid, chatid)
+            if not bot.rpc.get_contact(accid, event.contact_id).is_bot:
+                bot.logger.debug("QR scanned by contact id=%s", event.contact_id)
+                chatid = bot.rpc.create_chat_by_contact_id(accid, event.contact_id)
+                send_help(bot, accid, chatid)
 
 
-@cli.on(events.NewMessage(is_info=False, func=is_not_known_command))
-def on_message(bot: Bot, accid: int, event: AttrDict) -> None:
+@cli.on(events.NewMessage(is_info=False))
+def on_message(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    if bot.has_command(event.command):
+        return
     msg = event.msg
     chat = bot.rpc.get_basic_chat_info(accid, msg.chat_id)
     if chat.chat_type != ChatType.SINGLE:
         return
 
     bot.rpc.markseen_msgs(accid, [msg.id])
 
-    if msg.file_mime and msg.file_mime.startswith("image/"):
-        bot.rpc.send_sticker(accid, msg.chat_id, msg.file)
+    if msg.file_mime and msg.file_mime.lower().startswith("image/"):
+        if msg.file_mime.lower().split("/")[-1] in ("png", "jpg", "jpeg"):
+            with TemporaryDirectory() as tmp_dir:
+                path = extract_sticker(bot, msg.file, tmp_dir)
+                bot.rpc.send_sticker(accid, msg.chat_id, path)
+        else:
+            bot.rpc.send_sticker(accid, msg.chat_id, msg.file)
     elif signal.is_pack(msg.text):
         process_signal_pack(bot, accid, msg)
     elif emoji_count(msg.text):
         pack_url, sticker = signal.get_random_sticker(msg.text)
         if pack_url:
             with TemporaryDirectory() as tmp_dir:
                 filename = os.path.join(tmp_dir, f"{msg.text}.webp")
                 with open(filename, mode="wb") as attachment:
                     attachment.write(sticker)
                 msg_id = bot.rpc.send_sticker(accid, msg.chat_id, filename)
                 bot.rpc.send_msg(
-                    accid, msg.chat_id, {"text": pack_url, "quotedMessageId": msg_id}
+                    accid, msg.chat_id, MsgData(text=pack_url, quoted_message_id=msg_id)
                 )
         else:
             text = f"❌ No sticker found for: {msg.text!r}"
-            bot.rpc.send_msg(accid, msg.chat_id, {"text": text})
+            bot.rpc.send_msg(accid, msg.chat_id, MsgData(text=text))
     elif msg.text:
         selfaddr = bot.rpc.get_config(accid, "configured_addr")
         html = signal.search_html(selfaddr, msg.text)
         if html:
             text = f"Results for: {msg.text!r}"
-            bot.rpc.send_msg(accid, msg.chat_id, {"text": text, "html": html})
+            bot.rpc.send_msg(accid, msg.chat_id, MsgData(text=text, html=html))
         else:
             text = f"❌ No results for: {msg.text!r}"
-            bot.rpc.send_msg(accid, msg.chat_id, {"text": text})
+            bot.rpc.send_msg(accid, msg.chat_id, MsgData(text=text))
 
 
 @cli.on(events.NewMessage(command="/help"))
-def _help(bot: Bot, accid: int, event: AttrDict) -> None:
+def _help(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     send_help(bot, accid, event.msg.chat_id)
 
 
 @cli.on(events.NewMessage(command="/info"))
-def _info(bot: Bot, accid: int, event: AttrDict) -> None:
+def _info(bot: Bot, accid: int, event: NewMsgEvent) -> None:
     msg = event.msg
     if signal.is_pack(event.payload):
         text, cover = signal.get_pack_metadata(event.payload)
         with TemporaryDirectory() as tmp_dir:
             filename = os.path.join(tmp_dir, "cover.webp")
             with open(filename, mode="wb") as attachment:
                 attachment.write(cover)
-            reply = {"text": text, "file": filename, "quotedMessageId": msg.id}
+            reply = MsgData(text=text, file=filename, quoted_message_id=msg.id)
             bot.rpc.send_msg(accid, msg.chat_id, reply)
     else:
-        reply = {"text": "❌ Unknow pack URL", "quotedMessageId": msg.id}
+        reply = MsgData(text="❌ Unknow pack URL", quoted_message_id=msg.id)
         bot.rpc.send_msg(accid, msg.chat_id, reply)
 
 
-def process_signal_pack(bot: Bot, accid: int, msg: AttrDict) -> None:
+@cli.on(events.NewMessage)
+def delete_msgs(bot: Bot, accid: int, event: NewMsgEvent) -> None:
+    """NOTE: This hook must be added at the end so it is not executed before other commands and hooks"""
+    bot.rpc.delete_messages(accid, [event.msg.id])
+
+
+def process_signal_pack(bot: Bot, accid: int, msg: Message) -> None:
     title, path = signal.download_pack(bot.account.get_blobdir(), msg.text)
     size = os.stat(path).st_size
     if size > 1024**2 * 15:
         url = upload(bot.logger, path)
         if url:
             text = f"Name: {title}\nSize: {sizeof_fmt(size)}\nDownload: {url}"
         else:
             text = f"❌ Pack too big ({sizeof_fmt(size)})"
-        bot.rpc.send_msg(accid, msg.chat_id, {"text": text, "quotedMessageId": msg.id})
+        reply = MsgData(text=text, quoted_message_id=msg.id)
+        bot.rpc.send_msg(accid, msg.chat_id, reply)
     else:
-        bot.rpc.send_msg(accid, msg.chat_id, {"file": path, "quotedMessageId": msg.id})
+        reply = MsgData(file=path, quoted_message_id=msg.id)
+        bot.rpc.send_msg(accid, msg.chat_id, reply)
     os.remove(path)
 
 
 def send_help(bot: Bot, accid: int, chatid: int) -> None:
     lines = [
-        "Send me an image and I will convert it to a Delta Chat sticker for you.\n",
+        "Send me an image and I will remove the background and convert it to a Delta Chat sticker"
+        " for you.\n",
         "Send me an emoji to get an sticker representing that emoji.\n",
         "Send me a text to search for sticker packs matching that text.\n",
-        "Also, you can send me an URL of a Signal sticker pack, and I will send you the pack, for example, something that looks like:",
-        "sgnl://addstickers/?pack_id=59d338...&pack_key=56af35..." "",
+        "Also, you can send me an URL of a Signal sticker pack, and I will send you the pack,"
+        " for example, something that looks like:",
+        "sgnl://addstickers/?pack_id=59d338...&pack_key=56af35...",
+        "",
         "**Available commands**",
-        "/info URL - Get more information about the sticker pack with given URL, example: /info sgnl://addstickers/?pack_id=59d338...&pack_key=56af35...",
+        "/info URL - Get more information about the sticker pack with given URL, example:"
+        " /info sgnl://addstickers/?pack_id=59d338...&pack_key=56af35...",
     ]
-    bot.rpc.send_msg(accid, chatid, {"text": "\n".join(lines)})
+    bot.rpc.send_msg(accid, chatid, MsgData(text="\n".join(lines)))
+
+
+def extract_sticker(bot: Bot, filename: str, outdir: str) -> str:
+    img = remove(Image.open(filename))
+    path = Path(outdir, "sticker.webp")
+    try:
+        img.save(path)
+    except Exception as ex:  # noqa: W0718
+        bot.logger.exception(ex)
+        path = Path(outdir, "sticker.png")
+        img.save(path)
+    return str(path)
```

### Comparing `stickersbot-3.0.0/stickersbot/signal.py` & `stickersbot-4.0.0/stickersbot/signal.py`

 * *Files identical despite different names*

### Comparing `stickersbot-3.0.0/stickersbot/util.py` & `stickersbot-4.0.0/stickersbot/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 def upload(logger: Logger, path: str) -> str:
     urls = ["https://ttm.sh/", "https://envs.sh/", "https://x0.at/", "https://0x0.st/"]
     random.shuffle(urls)
     for url in urls:
         try:
             with open(path, "rb") as file:
                 with session.post(url, files={"file": file}) as resp:
-                    if 200 <= resp.status_code <= 300:
+                    if 200 <= resp.status_code <= 300 and resp.text.strip():
                         return resp.text.strip()
         except Exception as ex:  # noqa
             logger.exception(ex)
     return ""
```

