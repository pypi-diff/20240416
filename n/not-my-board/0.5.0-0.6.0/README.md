# Comparing `tmp/not_my_board-0.5.0.tar.gz` & `tmp/not_my_board-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_my_board-0.5.0.tar", last modified: Thu Feb  8 23:21:08 2024, max compression
+gzip compressed data, was "not_my_board-0.6.0.tar", last modified: Tue Apr 16 12:50:35 2024, max compression
```

## Comparing `not_my_board-0.5.0.tar` & `not_my_board-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,60 @@
--rw-r--r--   0        0        0     1999 2024-02-08 18:12:34.000000 not_my_board-0.5.0/.github/workflows/on-push.yml
--rw-r--r--   0        0        0       47 2024-02-08 18:12:34.000000 not_my_board-0.5.0/.gitignore
--rw-r--r--   0        0        0      301 2024-02-08 18:12:34.000000 not_my_board-0.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1097 2024-02-08 18:12:34.000000 not_my_board-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      280 2024-02-08 18:12:34.000000 not_my_board-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-08 23:21:08.735911 not_my_board-0.5.0/VERSION
--rw-r--r--   0        0        0      928 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/conf.py
--rw-r--r--   0        0        0     3547 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/explanation/overview.md
--rw-r--r--   0        0        0     1184 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/explanation/sensitive-usb-devices.md
--rw-r--r--   0        0        0       53 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/googlef248cffc234a230d.html
--rw-r--r--   0        0        0     3117 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/how-to-guides/usb-export.md
--rw-r--r--   0        0        0     1462 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/how-to-guides/usb-import.md
--rw-r--r--   0        0        0     2107 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/index.md
--rw-r--r--   0        0        0      419 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/installation.md
--rw-r--r--   0        0        0     2669 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/reference/cli.md
--rw-r--r--   0        0        0     2464 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/reference/export-description.md
--rw-r--r--   0        0        0     2819 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/reference/import-description.md
--rw-r--r--   0        0        0     2399 2024-02-08 18:12:34.000000 not_my_board-0.5.0/doc/tutorials/sharing-http-server.md
--rw-r--r--   0        0        0     1027 2024-02-08 18:12:34.000000 not_my_board-0.5.0/meson.build
--rw-r--r--   0        0        0       26 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/__about__.py.in
--rw-r--r--   0        0        0       27 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/__init__.py
--rw-r--r--   0        0        0       87 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/__main__.py
--rw-r--r--   0        0        0    14335 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_agent.py
--rw-r--r--   0        0        0     3678 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_client.py
--rw-r--r--   0        0        0     8252 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_export.py
--rw-r--r--   0        0        0     2932 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_http.py
--rw-r--r--   0        0        0     6657 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_hub.py
--rw-r--r--   0        0        0     8467 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_jsonrpc.py
--rw-r--r--   0        0        0     1123 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_models.py
--rw-r--r--   0        0        0    17079 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_usbip.py
--rw-r--r--   0        0        0      357 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_util/__init__.py
--rw-r--r--   0        0        0     4890 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_util/_asyncio.py
--rw-r--r--   0        0        0     3954 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_util/_matching.py
--rw-r--r--   0        0        0      428 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/_util/_misc.py
--rw-r--r--   0        0        0     6078 2024-02-08 18:12:34.000000 not_my_board-0.5.0/not_my_board/cli/__init__.py
--rw-r--r--   0        0        0     2812 2024-02-08 18:12:34.000000 not_my_board-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1680 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/_vmctl/alpine-chroot-install.sh
--rw-r--r--   0        0        0     2188 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/_vmctl/configure-vm.sh
--rw-r--r--   0        0        0      100 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/_vmctl/known_hosts
--rw-r--r--   0        0        0      411 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/_vmctl/ssh_host_ed25519_key
--rw-r--r--   0        0        0      103 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/_vmctl/ssh_host_ed25519_key.pub
--rwxr-xr-x   0        0        0      927 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/get_version
--rwxr-xr-x   0        0        0    10511 2024-02-08 18:12:34.000000 not_my_board-0.5.0/scripts/vmctl
--rw-r--r--   0        0        0        0 2024-02-08 18:12:34.000000 not_my_board-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      233 2024-02-08 18:12:34.000000 not_my_board-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      111 2024-02-08 18:12:34.000000 not_my_board-0.5.0/tests/qemu-usb-place.toml
--rw-r--r--   0        0        0       76 2024-02-08 18:12:34.000000 not_my_board-0.5.0/tests/qemu-usb.toml
--rw-r--r--   0        0        0     7746 2024-02-08 18:12:34.000000 not_my_board-0.5.0/tests/test_hub.py
--rw-r--r--   0        0        0     8252 2024-02-08 18:12:34.000000 not_my_board-0.5.0/tests/test_usbip.py
--rw-r--r--   0        0        0     3493 2024-02-08 23:21:08.817894 not_my_board-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2563 2024-04-16 12:29:26.000000 not_my_board-0.6.0/.github/workflows/on-push.yml
+-rw-r--r--   0        0        0       73 2024-04-16 12:29:26.000000 not_my_board-0.6.0/.gitignore
+-rw-r--r--   0        0        0      301 2024-04-16 12:29:26.000000 not_my_board-0.6.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1097 2024-04-16 12:29:26.000000 not_my_board-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      280 2024-04-16 12:29:26.000000 not_my_board-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 12:50:34.948108 not_my_board-0.6.0/VERSION
+-rw-r--r--   0        0        0      149 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/_static/css/custom.css
+-rw-r--r--   0        0        0     1039 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/conf.py
+-rw-r--r--   0        0        0     3547 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/explanation/overview.md
+-rw-r--r--   0        0        0     1184 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/explanation/sensitive-usb-devices.md
+-rw-r--r--   0        0        0       53 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/googlef248cffc234a230d.html
+-rw-r--r--   0        0        0     2742 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/how-to-guides/deploy-hub.md
+-rw-r--r--   0        0        0      951 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/how-to-guides/set-up-agent.md
+-rw-r--r--   0        0        0     1478 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/how-to-guides/set-up-exporter.md
+-rw-r--r--   0        0        0     3051 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/how-to-guides/usb-export.md
+-rw-r--r--   0        0        0      545 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/how-to-guides/usb-import.md
+-rw-r--r--   0        0        0     2189 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/index.md
+-rw-r--r--   0        0        0      419 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/installation.md
+-rw-r--r--   0        0        0     3032 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/reference/cli.md
+-rw-r--r--   0        0        0     2464 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/reference/export-description.md
+-rw-r--r--   0        0        0     2819 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/reference/import-description.md
+-rw-r--r--   0        0        0     2409 2024-04-16 12:29:26.000000 not_my_board-0.6.0/doc/tutorials/sharing-http-server.md
+-rw-r--r--   0        0        0     1142 2024-04-16 12:29:26.000000 not_my_board-0.6.0/meson.build
+-rw-r--r--   0        0        0       26 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/__about__.py.in
+-rw-r--r--   0        0        0       27 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/__main__.py
+-rw-r--r--   0        0        0    13699 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_agent.py
+-rw-r--r--   0        0        0     3836 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_client.py
+-rw-r--r--   0        0        0     7909 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_export.py
+-rw-r--r--   0        0        0    14397 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_http.py
+-rw-r--r--   0        0        0     6740 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_hub.py
+-rw-r--r--   0        0        0      129 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0    11377 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_jsonrpc/_protocol.py
+-rw-r--r--   0        0        0      828 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_jsonrpc/_websocket.py
+-rw-r--r--   0        0        0     1123 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_models.py
+-rw-r--r--   0        0        0    17024 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_usbip.py
+-rw-r--r--   0        0        0      476 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_util/__init__.py
+-rw-r--r--   0        0        0     6013 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_util/_asyncio.py
+-rw-r--r--   0        0        0     3954 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/_util/_matching.py
+-rw-r--r--   0        0        0     6395 2024-04-16 12:29:26.000000 not_my_board-0.6.0/not_my_board/cli/__init__.py
+-rw-r--r--   0        0        0     2859 2024-04-16 12:29:26.000000 not_my_board-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1660 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/_vmctl/alpine-chroot-install.sh
+-rw-r--r--   0        0        0     2408 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/_vmctl/configure-vm.sh
+-rw-r--r--   0        0        0      100 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/_vmctl/known_hosts
+-rw-r--r--   0        0        0      411 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/_vmctl/ssh_host_ed25519_key
+-rw-r--r--   0        0        0      103 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/_vmctl/ssh_host_ed25519_key.pub
+-rwxr-xr-x   0        0        0      927 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/get_version
+-rwxr-xr-x   0        0        0    10470 2024-04-16 12:29:26.000000 not_my_board-0.6.0/scripts/vmctl
+-rw-r--r--   0        0        0        0 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      111 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/qemu-usb-place.toml
+-rw-r--r--   0        0        0       76 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/qemu-usb.toml
+-rw-r--r--   0        0        0    13193 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/test_agent.py
+-rw-r--r--   0        0        0     5817 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/test_http.py
+-rw-r--r--   0        0        0     7739 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/test_hub.py
+-rw-r--r--   0        0        0    13362 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/test_jsonrpc.py
+-rw-r--r--   0        0        0     3382 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/test_usbip.py
+-rw-r--r--   0        0        0       55 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/tinyproxy.conf
+-rw-r--r--   0        0        0     4123 2024-04-16 12:29:26.000000 not_my_board-0.6.0/tests/util.py
+-rw-r--r--   0        0        0     3548 2024-04-16 12:50:35.056565 not_my_board-0.6.0/PKG-INFO
```

### Comparing `not_my_board-0.5.0/.github/workflows/on-push.yml` & `not_my_board-0.6.0/.github/workflows/on-push.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,79 @@
 name: on-push
 
 on: [push]
 
 jobs:
+  docs:
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python
+      uses: actions/setup-python@v3
+      with:
+        python-version: 3.12
+    - name: Install dependencies
+      run: |
+        pip install .[docs]
+    - name: Build Sphinx documentation
+      run: sphinx-build -n -W --keep-going doc doc/_build
   static_checks:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
-        python-version: 3.11
+        python-version: 3.12
     - name: Install dependencies
       run: |
         pip install .[test]
     - name: Lint with Pylint
       run: pylint --score=n not_my_board tests
     - name: Check format with Black
       run: black --check --quiet not_my_board tests doc
     - name: Check import statement order with isort
       run: isort --check not_my_board tests
     - name: Check spelling
       run: git ls-files -z | xargs -0 -- codespell
   test:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python
+    - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
-        python-version: 3.11
+        python-version: ${{ matrix.python-version }}
     - name: Create test VM image
       run: sudo ./scripts/vmctl makeimg
     - name: Install dependencies
       run: |
         sudo apt-get update
-        sudo apt-get install qemu-system
+        sudo apt-get install \
+          qemu-system \
+          openssl \
+          tinyproxy \
+          ;
         pip install .[test]
     - name: Allow kvm usage
       run: |
         sudo chmod o+rw /dev/kvm || :
     - name: Run tests
       run: pytest -s
   release:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
-        python-version: 3.11
+        python-version: 3.12
     - name: Install dependencies
       run: |
         # python3-build is broken on 22.04:
         # https://bugs.launchpad.net/ubuntu/+source/python-build/+bug/1992108
         # install everything from pip instead
         pip install build twine
     - name: Build dist packages
```

### Comparing `not_my_board-0.5.0/LICENSE.txt` & `not_my_board-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/doc/conf.py` & `not_my_board-0.6.0/doc/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 html_theme = "furo"
 html_title = f"{project} Documentation"
 
 myst_enable_extensions = [
     "deflist",
+    "colon_fence",
 ]
 
 # exclude prompts and output from copies
 copybutton_exclude = ".linenos, .gp, .go"
 
 # add search console verification
 html_extra_path = ["googlef248cffc234a230d.html"]
+
+# add custom CSS
+html_static_path = ["_static"]
+html_css_files = [
+    "css/custom.css",
+]
```

### Comparing `not_my_board-0.5.0/doc/explanation/overview.md` & `not_my_board-0.6.0/doc/explanation/overview.md`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/doc/explanation/sensitive-usb-devices.md` & `not_my_board-0.6.0/doc/explanation/sensitive-usb-devices.md`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/doc/how-to-guides/usb-export.md` & `not_my_board-0.6.0/doc/how-to-guides/usb-export.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 This guide shows you how to make USB devices available in the board farm.
 
 ## Device Manager Integration
 
 `not-my-board` exports not only the currently plugged in USB device, but every
 USB device, that appears on a specific USB port. For that to work,
 `not-my-board` needs support from the device manager to get notified when a new
-device appears and to load the `usbip-host` driver instead of the default
-driver.
+device appears.
 
 ### Integration with `udev`
 
 Most popular Linux distributions use `udev` as a device manager. To integrate
 `not-my-board` create a new rules file:
 
 ```{code-block}
```

### Comparing `not_my_board-0.5.0/doc/index.md` & `not_my_board-0.6.0/doc/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 tutorials/sharing-http-server
 ```
 
 ```{toctree}
 :caption: How-to Guides
 :hidden:
 
+how-to-guides/deploy-hub
+how-to-guides/set-up-exporter
+how-to-guides/set-up-agent
 how-to-guides/usb-export
 how-to-guides/usb-import
 ```
 
 ```{toctree}
 :caption: Reference
 :hidden:
```

### Comparing `not_my_board-0.5.0/doc/reference/cli.md` & `not_my_board-0.6.0/doc/reference/cli.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 # CLI Interface
 
 Here's a description of all the commands and options `not-my-board` supports.
 
 ## Commands
 
-**`hub`** [**`-h`**|**`--help`**]
+**`hub`** \[**`-h`**|**`--help`**\]
 : Start the board farm *Hub*. There should be only one hub in the entire
   network.
 
-**`export`** [**`-h`**|**`--help`**] *hub_url* *export_description*
+**`export`** \[**`-h`**|**`--help`**\] \[**`--cacert`** *cacert*\] *hub_url* *export_description*
 : Make connected boards and equipment available in the board farm.
 
-**`agent`** [**`-h`**|**`--help`**] *hub_url*
+**`agent`** \[**`-h`**|**`--help`**\] \[**`--cacert`**\] *hub_url*
 : Start an *Agent*.
 
-**`reserve`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] [**`-n`**|**`--with-name`** *name*] *import_description*
+**`reserve`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] \[**`-n`**|**`--with-name`** *name*\] *import_description*
 : Reserve a *Place*.
 
-**`return`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] *name*
+**`return`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] *name*
 : Return a reserved *Place*.
 
-**`attach`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] [**`-k`**|**`--keep-others`**] *name*|*import_description*
+**`attach`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] \[**`-k`**|**`--keep-others`**\] *name*|*import_description*
 : Attach a reserved *Place*. As a convenience this will also implicitly reserve
   the *Place*, if it's not reserved, yet.
 
-**`detach`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] [**`-k`**|**`--keep`**] *name*
+**`detach`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] \[**`-k`**|**`--keep`**\] *name*
 : Detach an attached *Place*. By default this will also return the reservation:
   Use {option}`--keep <not-my-board --keep>` to keep the reservation.
 
-**`list`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] [**`-n`**|**`--no-header`**]
+**`list`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] \[**`-n`**|**`--no-header`**\]
 : List reserved *Places*.
 
-**`status`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] [**`-n`**|**`--no-header`**]
+**`status`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] \[**`-n`**|**`--no-header`**\]
 : Show status of attached places and its interfaces.
 
-**`uevent`** [**`-h`**|**`--help`**] [**`-v`**|**`--verbose`**] *devpath*
+**`uevent`** \[**`-h`**|**`--help`**\] \[**`-v`**|**`--verbose`**\] *devpath*
 : Handle Kernel uevent for USB devices. This should be called by the device
   manager, e.g. *udev*(7).
 
 ## Options
 
 ```{program} not-my-board
 ```
 
 ```{option} -h, --help
 Show help message and exit.
 ```
 
+```{option} --cacert cacert
+Load additional CA certificates to trust when using TLS. *cacert* is a path to a
+file of concatenated CA certificates in PEM format. Can be used multiple times
+to load more than one file. System default CA certificates are always trusted.
+```
+
 ```{option} hub_url
 HTTP or HTTPS URL of the *Hub*.
 ```
 
 ```{option} export_description
 Path to an export description file.
 ```
```

### Comparing `not_my_board-0.5.0/doc/reference/export-description.md` & `not_my_board-0.6.0/doc/reference/export-description.md`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/doc/reference/import-description.md` & `not_my_board-0.6.0/doc/reference/import-description.md`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/doc/tutorials/sharing-http-server.md` & `not_my_board-0.6.0/doc/tutorials/sharing-http-server.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 Before you can reserve and attach the exported place you need to start a
 background process, that handles the communication with the board farm: the
 agent. This usually runs on a different host than the exporter, but as mentioned
 before, you run everything on a single host. Start the agent, leave it running
 and continue in a new terminal window.
 ```console
-$ not-my-board agent http://localhost:2092
+$ sudo not-my-board agent http://localhost:2092
 ```
 
 Now create a file with the import description. It says "I want a place, which
 has one part. This part has at least the tag `tutorial-http-server` and a TCP
 interface named `http`. Bind that interface to localhost, port `8081`."
 ```{code-block} toml
 :caption: tutorial-tcp.toml
@@ -57,15 +57,15 @@
 compatible = [ "tutorial-http-server" ]
 tcp.http = { local_port = 8081 }
 ```
 
 Use that import description to reserve and attach the place, that you previously
 exported.
 ```console
-$ not-my-board attach ./tutorial-tcp.toml
+$ sudo not-my-board attach ./tutorial-tcp.toml
 ```
 
 Now the exported HTTP server is available through the board farm. Notice that
 the real HTTP server is listening on port `8080` and the agent exposes the
 imported HTTP server on port `8081`:
 ```console
 $ curl http://localhost:8081/hello
```

### Comparing `not_my_board-0.5.0/meson.build` & `not_my_board-0.6.0/meson.build`

 * *Files 9% similar despite different names*

```diff
@@ -10,30 +10,35 @@
 py.install_sources(
   'not_my_board/__init__.py',
   'not_my_board/__main__.py',
   'not_my_board/_agent.py',
   'not_my_board/_client.py',
   'not_my_board/_export.py',
   'not_my_board/_http.py',
-  'not_my_board/_jsonrpc.py',
   'not_my_board/_models.py',
   'not_my_board/_hub.py',
   'not_my_board/_usbip.py',
   subdir: 'not_my_board',
 )
 
 py.install_sources(
   'not_my_board/_util/__init__.py',
   'not_my_board/_util/_asyncio.py',
   'not_my_board/_util/_matching.py',
-  'not_my_board/_util/_misc.py',
   subdir: 'not_my_board/_util',
 )
 
 py.install_sources(
+  'not_my_board/_jsonrpc/__init__.py',
+  'not_my_board/_jsonrpc/_protocol.py',
+  'not_my_board/_jsonrpc/_websocket.py',
+  subdir: 'not_my_board/_jsonrpc',
+)
+
+py.install_sources(
   'not_my_board/cli/__init__.py',
   subdir: 'not_my_board/cli',
 )
 
 configure_file(
   input: 'not_my_board/__about__.py.in',
   output: '__about__.py',
```

### Comparing `not_my_board-0.5.0/not_my_board/_agent.py` & `not_my_board-0.6.0/not_my_board/_agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,194 +1,284 @@
 #!/usr/bin/env python3
 
 import asyncio
 import contextlib
+import functools
 import ipaddress
 import logging
 import os
 import pathlib
+import shutil
 import traceback
 import urllib.parse
-
-import websockets
+import weakref
+from dataclasses import dataclass, field
+from typing import List, Tuple
 
 import not_my_board._http as http
 import not_my_board._jsonrpc as jsonrpc
 import not_my_board._models as models
 import not_my_board._usbip as usbip
 import not_my_board._util as util
 
 logger = logging.getLogger(__name__)
+USBIP_REMOTE = ("usb.not-my-board.localhost", 3240)
+Address = Tuple[str, int]
 
 
-async def agent(hub_url):
-    async with Agent(hub_url) as a:
-        await a.serve_forever()
+async def agent(hub_url, ca_files):
+    io = _AgentIO(hub_url, http.Client(ca_files))
+    async with Agent(hub_url, io) as agent_:
+        await agent_.serve_forever()
 
 
-class Agent:
-    def __init__(self, hub_url):
+class _AgentIO:
+    def __init__(self, hub_url, http_client):
         self._hub_url = hub_url
-        self._reserved_places = {}
-        self._pending = set()
-        url = urllib.parse.urlsplit(hub_url)
-        ws_scheme = "ws" if url.scheme == "http" else "wss"
-        self._ws_uri = f"{ws_scheme}://{url.netloc}/ws-agent"
-        self._hub_host = url.netloc.split(":")[0]
+        self._http = http_client
 
-    async def __aenter__(self):
-        runtime_dir = pathlib.Path(os.environ["XDG_RUNTIME_DIR"])
+    @contextlib.asynccontextmanager
+    async def hub_rpc(self):
+        auth = "Bearer dummy-token-1"
+        url = f"{self._hub_url}/ws-agent"
+        async with jsonrpc.WebsocketChannel(url, self._http, auth=auth) as rpc:
+            yield rpc
 
-        async with contextlib.AsyncExitStack() as stack:
-            headers = {"Authorization": "Bearer dummy-token-1"}
-            ws = await stack.enter_async_context(
-                websockets.connect(self._ws_uri, extra_headers=headers)
-            )
+    @contextlib.asynccontextmanager
+    async def unix_server(self, api_obj):
+        socket_path = pathlib.Path("/run") / "not-my-board-agent.sock"
 
-            async def receive_iter():
-                try:
-                    while True:
-                        yield await ws.recv()
-                except websockets.ConnectionClosedOK:
-                    pass
+        connection_handler = functools.partial(self._handle_unix_client, api_obj)
+        async with util.UnixServer(connection_handler, socket_path) as unix_server:
+            os.chmod(socket_path, 0o660)
+            try:
+                shutil.chown(socket_path, group="not-my-board")
+            except Exception as e:
+                logger.warning(
+                    'Failed to change group on agent socket "%s": %s', socket_path, e
+                )
 
-            self._hub_proxy = jsonrpc.Proxy(ws.send, receive_iter())
+            yield unix_server
 
-            stack.push_async_callback(self._cleanup)
+    @staticmethod
+    async def _handle_unix_client(api_obj, reader, writer):
+        async def send(data):
+            writer.write(data + b"\n")
+            await writer.drain()
 
-            self._unix_server = await stack.enter_async_context(
-                util.UnixServer(self._handle_client, runtime_dir / "not-my-board.sock")
-            )
+        channel = jsonrpc.Channel(send, reader, api_obj)
+        await channel.communicate_forever()
 
-            self._stack = stack.pop_all()
-            await self._stack.__aenter__()
-            return self
+    async def get_places(self):
+        response = await self._http.get_json(f"{self._hub_url}/api/v1/places")
+        return [models.Place(**p) for p in response["places"]]
+
+    @staticmethod
+    async def usbip_refresh_status():
+        await usbip.refresh_vhci_status()
+
+    @staticmethod
+    def usbip_is_attached(vhci_port):
+        return usbip.is_attached(vhci_port)
 
-    async def __aexit__(self, exc_type, exc, tb):
-        await self._stack.__aexit__(exc_type, exc, tb)
+    async def usbip_attach(self, proxy, target, port_num, usbid):
+        tunnel = self._http.open_tunnel(*proxy, *target)
+        async with tunnel as (reader, writer, trailing_data):
+            if trailing_data:
+                raise ProtocolError("USB/IP implementation cannot handle trailing data")
+            return await usbip.attach(reader, writer, usbid, port_num)
 
-    async def _cleanup(self):
-        for _, place in self._reserved_places.items():
-            if place.is_attached:
-                await place.detach()
+    @staticmethod
+    def usbip_detach(vhci_port):
+        usbip.detach(vhci_port)
 
-    # TODO: hide from JSON-RPC interface
-    async def serve_forever(self):
-        await util.run_concurrently(
-            self._unix_server.serve_forever(), self._hub_proxy.io_loop()
+    async def port_forward(self, ready_event, proxy, target, local_port):
+        localhost = "127.0.0.1"
+        connection_handler = functools.partial(
+            self._handle_port_forward_client, proxy, target
         )
+        async with util.Server(connection_handler, localhost, local_port) as server:
+            ready_event.set()
+            await server.serve_forever()
 
-    async def _handle_client(self, reader, writer):
-        async def send(data):
-            writer.write(data + b"\n")
-            await writer.drain()
+    async def _handle_port_forward_client(self, proxy, target, client_r, client_w):
+        async with self._http.open_tunnel(*proxy, *target) as (
+            remote_r,
+            remote_w,
+            trailing_data,
+        ):
+            client_w.write(trailing_data)
+            await client_w.drain()
+            await util.relay_streams(client_r, client_w, remote_r, remote_w)
 
-        socket_server = jsonrpc.Server(send, reader, self)
-        await socket_server.serve_forever()
 
-    async def reserve(self, name, import_description_file):
-        if name in self._reserved_places:
-            raise RuntimeError(f'A place named "{name}" is already reserved')
+class Agent(util.ContextStack):
+    def __init__(self, hub_url, io):
+        url = urllib.parse.urlsplit(hub_url)
+        self._hub_host = url.netloc.split(":")[0]
+        self._io = io
+        self._locks = weakref.WeakValueDictionary()
+        self._reservations = {}
+
+    async def _context_stack(self, stack):
+        self._hub = await stack.enter_async_context(self._io.hub_rpc())
+        stack.push_async_callback(self._cleanup)
+        self._unix_server = await stack.enter_async_context(self._io.unix_server(self))
 
-        if name in self._pending:
-            raise RuntimeError(f'A place named "{name}" is currently being reserved')
+    async def serve_forever(self):
+        await self._unix_server.serve_forever()
 
-        self._pending.add(name)
-        try:
-            import_description_content = util.toml_loads(
-                pathlib.Path(import_description_file).read_text()
-            )
-            import_description = models.ImportDesc(
-                name=name, **import_description_content
-            )
+    async def _cleanup(self):
+        coros = [t.close() for r in self._reservations.values() for t in r.tunnels]
 
-            response = await http.get_json(f"{self._hub_url}/api/v1/places")
-            places = [models.Place(**p) for p in response["places"]]
+        await util.run_concurrently(*coros)
 
-            candidates = self._filter_places(import_description, places)
-            candidate_ids = list(candidates)
-            if not candidate_ids:
+    async def reserve(self, import_description):
+        import_description = models.ImportDesc(**import_description)
+        name = import_description.name
+
+        async with self._name_lock(name):
+            if name in self._reservations:
+                raise RuntimeError(f'A place named "{name}" is already reserved')
+
+            places = await self._io.get_places()
+
+            candidates = _filter_places(import_description, places)
+            if not candidates:
                 raise RuntimeError("No matching place found")
 
-            place_id = await self._hub_proxy.reserve(candidate_ids)
+            candidate_ids = list(candidates)
+            place_id = await self._hub.reserve(candidate_ids)
 
-            assert name not in self._reserved_places
-            self._reserved_places[name] = candidates[place_id]
-        finally:
-            self._pending.remove(name)
+            tunnels = [
+                desc.tunnel_cls(desc, self._hub_host, self._io)
+                for desc in candidates[place_id]
+            ]
+            self._reservations[name] = _Reservation(place_id, tunnels)
 
     async def return_reservation(self, name, force=False):
-        async with self._reserved_place(name) as reserved_place:
-            if reserved_place.is_attached:
+        async with self._reservation(name) as reservation:
+            if reservation.is_attached:
                 if force:
-                    await reserved_place.detach()
+                    await self._detach_reservation(reservation)
                 else:
                     raise RuntimeError(f'Place "{name}" is still attached')
-            await self._hub_proxy.return_reservation(reserved_place.id)
-            del self._reserved_places[name]
+            await self._hub.return_reservation(reservation.place_id)
+            del self._reservations[name]
 
     async def attach(self, name):
-        async with self._reserved_place(name) as reserved_place:
-            await reserved_place.attach()
+        async with self._reservation(name) as reservation:
+            if reservation.is_attached:
+                raise RuntimeError(f'Place "{name}" is already attached')
+
+            coros = [t.open() for t in reservation.tunnels]
+
+            async with util.on_error(self._detach_reservation, reservation):
+                await util.run_concurrently(*coros)
+                reservation.is_attached = True
 
     async def detach(self, name):
-        async with self._reserved_place(name) as reserved_place:
-            await reserved_place.detach()
+        async with self._reservation(name) as reservation:
+            if not reservation.is_attached:
+                raise RuntimeError(f'Place "{name}" is not attached')
+
+            await self._detach_reservation(reservation)
+
+    async def _detach_reservation(self, reservation):
+        coros = [t.close() for t in reservation.tunnels]
+        await util.run_concurrently(*coros)
+        reservation.is_attached = False
 
     @contextlib.asynccontextmanager
-    async def _reserved_place(self, name):
-        def check_reserved():
-            if name not in self._reserved_places:
-                raise RuntimeError(f'A place named "{name}" is not reserved')
+    async def _name_lock(self, name):
+        if name not in self._locks:
+            lock = asyncio.Lock()
+            self._locks[name] = lock
+        else:
+            lock = self._locks[name]
 
-        check_reserved()
-        reserved_place = self._reserved_places[name]
-        async with reserved_place.lock:
-            # after waiting for the lock the place might have been returned, so
-            # check again
-            check_reserved()
-            yield reserved_place
+        async with lock:
+            yield
+
+    @contextlib.asynccontextmanager
+    async def _reservation(self, name):
+        async with self._name_lock(name):
+            if name not in self._reservations:
+                raise RuntimeError(f'A place named "{name}" is not reserved')
+            yield self._reservations[name]
 
     async def list(self):
         return [
-            {"place": name, "attached": place.is_attached}
-            for name, place in self._reserved_places.items()
+            {"place": name, "attached": reservation.is_attached}
+            for name, reservation in self._reservations.items()
         ]
 
     async def status(self):
-        usbip.refresh_vhci_status()
+        await self._io.usbip_refresh_status()
+
         return [
-            {"place": name, **status}
-            for name, place in self._reserved_places.items()
-            for status in place.status
+            {
+                "place": tunnel.place_name,
+                "part": tunnel.part_name,
+                "interface": tunnel.iface_name,
+                "type": tunnel.type_name,
+                "attached": tunnel.is_attached(),
+            }
+            for name, reservation in self._reservations.items()
+            for tunnel in reservation.tunnels
         ]
 
-    def _filter_places(self, import_description, places):
-        reserved_places = {}
 
-        imported_part_sets = [
-            (name, _part_to_set(imported_part))
-            for name, imported_part in import_description.parts.items()
-        ]
+def _filter_places(import_description, places):
+    candidates = {}
 
-        for place in places:
-            matching = _find_matching(imported_part_sets, place)
-            if matching:
-                real_host = self._real_host(place.host)
-                reserved_places[place.id] = ReservedPlace(
-                    import_description, place, real_host, matching
-                )
+    imported_part_sets = [
+        (name, _part_to_set(imported_part))
+        for name, imported_part in import_description.parts.items()
+    ]
+
+    for place in places:
+        matching = _find_matching(imported_part_sets, place)
+        if matching:
+            candidates[place.id] = _create_tunnel_descriptions(
+                import_description, place, matching
+            )
 
-        return reserved_places
+    return candidates
 
-    def _real_host(self, host):
-        if ipaddress.ip_address(host).is_loopback:
-            logger.info("Replacing %s with %s", host, self._hub_host)
-            return self._hub_host
-        return host
+
+# pylint: disable=too-many-locals
+def _create_tunnel_descriptions(import_description, place, matching):
+    place_name = import_description.name
+    proxy = (place.host, place.port)
+    tunnel_descs = set()
+
+    for part_name, place_part_idx in matching:
+        imported_part = import_description.parts[part_name]
+        place_part = place.parts[place_part_idx]
+
+        for iface_name, usb_import_description in imported_part.usb.items():
+            usbid = place_part.usb[iface_name].usbid
+            port_num = usb_import_description.port_num
+            tunnel_desc = _UsbTunnelDesc(
+                place_name, part_name, iface_name, proxy, usbid, port_num
+            )
+            tunnel_descs.add(tunnel_desc)
+
+        for iface_name, tcp_import_description in imported_part.tcp.items():
+            host = place_part.tcp[iface_name].host
+            port = place_part.tcp[iface_name].port
+            remote = (host, port)
+            local_port = tcp_import_description.local_port
+            tunnel_desc = _TcpTunnelDesc(
+                place_name, part_name, iface_name, proxy, remote, local_port
+            )
+            tunnel_descs.add(tunnel_desc)
+
+    return tunnel_descs
 
 
 def _find_matching(imported_part_sets, place):
     match_graph = {}
     for name, imported_part_set in imported_part_sets:
         match_graph[name] = []
         for place_part_idx, place_part in enumerate(place.parts):
@@ -218,230 +308,120 @@
     return (
         {f"compatible:{c}" for c in part.compatible}
         | {f"usb:{k}" for k in part.usb}
         | {f"tcp:{k}" for k in part.tcp}
     )
 
 
-class ReservedPlace:
-    def __init__(self, import_description, place, real_host, matching):
-        self._import_description = import_description
-        self._place = place
-        self._tunnels = []
-        self._stack = None
-        self.lock = asyncio.Lock()
-        proxy = real_host, place.port
-
-        for name, place_part_idx in matching:
-            imported_part = import_description.parts[name]
-            place_part = place.parts[place_part_idx]
-
-            for usb_name, usb_import_description in imported_part.usb.items():
-                self._tunnels.append(
-                    UsbTunnel(
-                        part_name=name,
-                        iface_name=usb_name,
-                        proxy=proxy,
-                        usbid=place_part.usb[usb_name].usbid,
-                        port_num=usb_import_description.port_num,
-                    )
-                )
+class _Tunnel:
+    _ready_timeout = 5
 
-            for tcp_name, tcp_import_description in imported_part.tcp.items():
-                self._tunnels.append(
-                    TcpTunnel(
-                        part_name=name,
-                        iface_name=tcp_name,
-                        proxy=proxy,
-                        remote=(
-                            place_part.tcp[tcp_name].host,
-                            place_part.tcp[tcp_name].port,
-                        ),
-                        local_port=tcp_import_description.local_port,
-                    )
-                )
+    def __init__(self, desc, hub_host, io):
+        self._desc = desc
+        self._io = io
+        self._task = None
+        self._ready_event = asyncio.Event()
 
-    async def attach(self):
-        if self._stack is not None:
-            raise RuntimeError(
-                'Place "{self._import_description.name}" is already attached'
-            )
+        host = self.proxy[0]
+        if ipaddress.ip_address(host).is_loopback:
+            host = hub_host
+        self._proxy = (host, self.proxy[1])
 
-        async with contextlib.AsyncExitStack() as stack:
-            for tunnel in self._tunnels:
-                await stack.enter_async_context(tunnel)
-            self._stack = stack.pop_all()
-
-    async def detach(self):
-        if self._stack is None:
-            raise RuntimeError(
-                'Place "{self._import_description.name}" is not attached'
-            )
+    def __getattr__(self, attr):
+        return getattr(self._desc, attr)
 
-        try:
-            await self._stack.aclose()
-        finally:
-            self._stack = None
+    async def open(self):
+        if not self._task:
+            logger.debug("%s: Opening %s tunnel", self.name, self.type_name)
+            self._ready_event.clear()
+            self._task = asyncio.create_task(self._task_func())
+            self._task.add_done_callback(self._task_done_callback)
 
-    @property
-    def id(self):
-        return self._place.id
+        try:
+            await asyncio.wait_for(self._ready_event.wait(), self._ready_timeout)
+        except asyncio.TimeoutError:
+            logger.warning("%s: Opening %s tunnel timed out", self.name, self.type_name)
+
+    def _task_done_callback(self, _):
+        self._task = None
+
+    async def close(self):
+        if self._task:
+            await util.cancel_tasks([self._task])
 
-    @property
     def is_attached(self):
-        return self._stack is not None
+        return bool(self._task and self._ready_event.is_set())
 
-    @property
-    def status(self):
-        return [
-            {
-                "part": t.part_name,
-                "interface": t.iface_name,
-                "type": t.type_name,
-                "attached": t.attached,
-            }
-            for t in self._tunnels
-        ]
 
+class _UsbTunnel(_Tunnel):
+    _vhci_port = None
 
-class UsbTunnel:
-    _target = "usb.not-my-board.localhost", 3240
-    _ready_timeout = 5
-
-    def __init__(self, part_name, iface_name, proxy, usbid, port_num):
-        self._part_name = part_name
-        self._iface_name = iface_name
-        self._name = f"{part_name}.{iface_name}"
-        self._proxy = proxy
-        self._usbid = usbid
-        self._port_num = port_num
-        self._vhci_port = None
-
-    async def __aenter__(self):
-        async with contextlib.AsyncExitStack() as stack:
-            ready_event = asyncio.Event()
-            await stack.enter_async_context(
-                util.background_task(self._tunnel_task(ready_event))
-            )
-            logger.debug("%s: Attaching USB device", self._name)
-
-            try:
-                await asyncio.wait_for(ready_event.wait(), self._ready_timeout)
-            except asyncio.TimeoutError:
-                logger.warning("%s: Attaching USB device timed out", self._name)
-
-            self._stack = stack.pop_all()
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self._stack.__aexit__(exc_type, exc, tb)
+    async def close(self):
+        await super().close()
+        if self._vhci_port is not None:
+            self._io.usbip_detach(self._vhci_port)
 
-    async def _tunnel_task(self, ready_event):
+    async def _task_func(self):
         retry_timeout = 1
-        try:
-            while True:
-                try:
-                    await self._attach()
-                    ready_event.set()
-                    retry_timeout = 1
-                except Exception:
-                    traceback.print_exc()
-                    await asyncio.sleep(retry_timeout)
-                    retry_timeout = min(2 * retry_timeout, 30)
-        finally:
-            if self._vhci_port is not None:
-                usbip.detach(self._vhci_port)
-            logger.debug("%s: USB device detached", self._name)
-
-    async def _attach(self):
-        tunnel = http.open_tunnel(*self._proxy, *self._target)
-        async with tunnel as (reader, writer, trailing_data):
-            if trailing_data:
-                raise ProtocolError("USB/IP implementation cannot handle trailing data")
-            self._vhci_port = await usbip.attach(
-                reader, writer, self._usbid, self._port_num
-            )
-        logger.debug("%s: USB device attached", self._name)
-
-    @property
-    def part_name(self):
-        return self._part_name
+        while True:
+            try:
+                self._vhci_port = await self._io.usbip_attach(
+                    self._proxy, USBIP_REMOTE, self.port_num, self.usbid
+                )
+                logger.debug("%s: USB device attached", self.name)
+                self._ready_event.set()
+                retry_timeout = 1
+            except Exception:
+                traceback.print_exc()
+                await asyncio.sleep(retry_timeout)
+                retry_timeout = min(2 * retry_timeout, 30)
 
-    @property
-    def iface_name(self):
-        return self._iface_name
+    def is_attached(self):
+        if self._vhci_port is None:
+            return False
+        return self._io.usbip_is_attached(self._vhci_port)
 
-    @property
-    def type_name(self):
-        return "USB"
 
-    @property
-    def attached(self):
-        return (
-            usbip.is_attached(self._vhci_port) if self._vhci_port is not None else False
+class _TcpTunnel(_Tunnel):
+    async def _task_func(self):
+        await self._io.port_forward(
+            self._ready_event, self._proxy, self.remote, self.local_port
         )
 
 
-class TcpTunnel:
-    def __init__(self, part_name, iface_name, proxy, remote, local_port):
-        self._part_name = part_name
-        self._iface_name = iface_name
-        self._name = f"{part_name}.{iface_name}"
-        self._proxy = proxy
-        self._remote = remote
-        self._local_port = local_port
-        self._is_attached = False
-
-    async def __aenter__(self):
-        async with contextlib.AsyncExitStack() as stack:
-            ready_event = asyncio.Event()
-            await stack.enter_async_context(
-                util.background_task(self._tunnel_task(ready_event))
-            )
-            await ready_event.wait()
-            self._is_attached = True
-            self._stack = stack.pop_all()
-        return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self._stack.__aexit__(exc_type, exc, tb)
-        self._is_attached = False
-
-    async def _tunnel_task(self, ready_event):
-        localhost = "127.0.0.1"
-        async with util.Server(
-            self._handle_client, localhost, self._local_port
-        ) as server:
-            ready_event.set()
-            await server.serve_forever()
-
-    async def _handle_client(self, client_r, client_w):
-        logger.debug("%s: Opening tunnel", self._name)
-        async with http.open_tunnel(*self._proxy, *self._remote) as (
-            remote_r,
-            remote_w,
-            trailing_data,
-        ):
-            logger.debug("%s: Tunnel created, relaying data", self._name)
-            client_w.write(trailing_data)
-            await client_w.drain()
-            await util.relay_streams(client_r, client_w, remote_r, remote_w)
-
-    @property
-    def part_name(self):
-        return self._part_name
-
-    @property
-    def iface_name(self):
-        return self._iface_name
-
-    @property
-    def type_name(self):
-        return "TCP"
-
-    @property
-    def attached(self):
-        return self._is_attached
+@dataclass(frozen=True)
+class _TunnelDesc:
+    place_name: str
+    part_name: str
+    iface_name: str
+    proxy: Address
+
+    @property
+    def name(self):
+        return f"{self.place_name}.{self.part_name}.{self.iface_name}"
+
+
+@dataclass(frozen=True)
+class _UsbTunnelDesc(_TunnelDesc):
+    usbid: str
+    port_num: int
+    type_name: str = field(default="USB", init=False)
+    tunnel_cls: type = field(default=_UsbTunnel, init=False)
+
+
+@dataclass(frozen=True)
+class _TcpTunnelDesc(_TunnelDesc):
+    remote: Address
+    local_port: int
+    type_name: str = field(default="TCP", init=False)
+    tunnel_cls: type = field(default=_TcpTunnel, init=False)
+
+
+@dataclass
+class _Reservation:
+    place_id: int
+    is_attached: bool = field(default=False, init=False)
+    tunnels: List[_Tunnel]
 
 
 class ProtocolError(Exception):
     pass
```

### Comparing `not_my_board-0.5.0/not_my_board/_client.py` & `not_my_board-0.6.0/not_my_board/_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,65 +3,65 @@
 import asyncio
 import contextlib
 import os
 import pathlib
 import sys
 
 import not_my_board._jsonrpc as jsonrpc
+import not_my_board._models as models
+import not_my_board._util as util
 
 
 async def reserve(import_description, with_name=None):
-    import_description_file = _find_import_description(import_description)
-    reservation_name = import_description_file.stem if not with_name else with_name
+    found_import_desc = _find_import_description(import_description, with_name)
 
-    async with agent_proxy() as proxy:
-        await proxy.reserve(reservation_name, import_description_file.as_posix())
+    async with agent_channel() as agent:
+        await agent.reserve(found_import_desc.dict())
 
 
 async def return_reservation(name):
-    async with agent_proxy() as proxy:
-        await proxy.return_reservation(name)
+    async with agent_channel() as agent:
+        await agent.return_reservation(name)
 
 
 async def attach(name, keep_others=False):
-    async with agent_proxy() as proxy:
-        reserved_names = {e["place"] for e in await proxy.list()}
+    async with agent_channel() as agent:
+        reserved_names = {e["place"] for e in await agent.list()}
         if name in reserved_names:
-            await proxy.attach(name)
+            await agent.attach(name)
 
             others = reserved_names - {name}
             if not keep_others and others:
                 for other in others:
-                    await proxy.return_reservation(name=other, force=True)
+                    await agent.return_reservation(name=other, force=True)
         else:
-            import_description_file = _find_import_description(name)
-            reservation_name = import_description_file.stem
-            await proxy.reserve(reservation_name, import_description_file.as_posix())
-            await proxy.attach(reservation_name)
+            found_import_desc = _find_import_description(name)
+            await agent.reserve(found_import_desc.dict())
+            await agent.attach(found_import_desc.name)
 
             if not keep_others and reserved_names:
                 for other in reserved_names:
-                    await proxy.return_reservation(name=other, force=True)
+                    await agent.return_reservation(name=other, force=True)
 
 
 async def detach(name, keep=False):
-    async with agent_proxy() as proxy:
-        await proxy.detach(name)
+    async with agent_channel() as agent:
+        await agent.detach(name)
         if not keep:
-            await proxy.return_reservation(name)
+            await agent.return_reservation(name)
 
 
 async def list_():
-    async with agent_proxy() as proxy:
-        return await proxy.list()
+    async with agent_channel() as agent:
+        return await agent.list()
 
 
 async def status():
-    async with agent_proxy() as proxy:
-        return await proxy.status()
+    async with agent_channel() as agent:
+        return await agent.status()
 
 
 async def uevent(devpath):
     # devpath has a leading "/", so joining with the / operator doesn't
     # work
     sysfs_path = pathlib.Path("/sys" + devpath)
     devname = sysfs_path.name
@@ -72,15 +72,15 @@
             f.write(b".")
     else:
         print(f"Loading default driver: {devname}", file=sys.stderr)
         probe_path = pathlib.Path("/sys/bus/usb/drivers_probe")
         probe_path.write_text(devname)
 
 
-def _find_import_description(name):
+def _find_import_description(name, with_name=None):
     if "/" in name:
         import_description_file = pathlib.Path(name)
     else:
         path = pathlib.Path()
         home = pathlib.Path.home()
 
         while path != home:
@@ -97,23 +97,27 @@
             config_home = pathlib.Path(
                 os.environ.get("XDG_CONFIG_HOME", home / ".config")
             )
             import_description_file = config_home / "not-my-board" / f"{name}.toml"
             if not import_description_file.is_file():
                 raise ValueError(f"No import description file exists for name {name}")
 
-    return import_description_file
+    reservation_name = import_description_file.stem if not with_name else with_name
+    import_description_content = util.toml_loads(import_description_file.read_text())
+    import_description = models.ImportDesc(
+        name=reservation_name, **import_description_content
+    )
+
+    return import_description
 
 
 @contextlib.asynccontextmanager
-async def agent_proxy():
-    runtime_dir = pathlib.Path(os.environ["XDG_RUNTIME_DIR"])
-    reader, writer = await asyncio.open_unix_connection(
-        runtime_dir / "not-my-board.sock"
-    )
+async def agent_channel():
+    socket_path = pathlib.Path("/run") / "not-my-board-agent.sock"
+    reader, writer = await asyncio.open_unix_connection(socket_path)
 
     async def send(data):
         writer.write(data + b"\n")
         await writer.drain()
 
-    async with jsonrpc.Proxy(send, reader) as proxy:
-        yield proxy
+    async with jsonrpc.Channel(send, reader) as channel:
+        yield channel
```

### Comparing `not_my_board-0.5.0/not_my_board/_export.py` & `not_my_board-0.6.0/not_my_board/_export.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 #!/usr/bin/env python3
 
 import asyncio
-import contextlib
 import datetime
 import email.utils
 import ipaddress
 import logging
 
 import h11
-import websockets
 
+import not_my_board._http as http
 import not_my_board._jsonrpc as jsonrpc
 import not_my_board._models as models
 import not_my_board._usbip as usbip
 import not_my_board._util as util
 
 logger = logging.getLogger(__name__)
 
 
-async def export(hub_url, place):
-    async with Exporter(hub_url, place) as exporter:
+async def export(hub_url, place, ca_files):
+    http_client = http.Client(ca_files)
+    async with Exporter(hub_url, place, http_client) as exporter:
         await exporter.serve_forever()
 
 
-class Exporter:
-    def __init__(self, hub_url, export_desc_path):
+class Exporter(util.ContextStack):
+    def __init__(self, hub_url, export_desc_path, http_client):
         self._hub_url = hub_url
         self._ip_to_tasks_map = {}
         export_desc_content = export_desc_path.read_text()
         self._place = models.ExportDesc(**util.toml_loads(export_desc_content))
+        self._http = http_client
 
         tcp_targets = {
             f"{tcp.host}:{tcp.port}".encode()
             for part in self._place.parts
             for _, tcp in part.tcp.items()
         }
         self._usb_target = {b"usb.not-my-board.localhost:3240"}
@@ -40,49 +41,37 @@
 
         self._usbip_devices = [
             usbip.UsbIpDevice(usb.usbid)
             for part in self._place.parts
             for _, usb in part.usb.items()
         ]
 
-    async def __aenter__(self):
-        async with contextlib.AsyncExitStack() as stack:
-            self._usbip_server = await stack.enter_async_context(
-                usbip.UsbIpServer(self._usbip_devices)
-            )
-
-            self._http_server = await stack.enter_async_context(
-                util.Server(self._handle_client, port=self._place.port)
-            )
+    async def _context_stack(self, stack):
+        self._usbip_server = await stack.enter_async_context(
+            usbip.UsbIpServer(self._usbip_devices)
+        )
 
-            url = f"{self._hub_url}/ws-exporter"
-            auth = "Bearer dummy-token-1"
-            self._ws = await stack.enter_async_context(util.ws_connect(url, auth))
-            self._ws_server = jsonrpc.Server(self._ws.send, self._receive_iter(), self)
-
-            self._stack = stack.pop_all()
-            await self._stack.__aenter__()
-            return self
+        self._http_server = await stack.enter_async_context(
+            util.Server(self._handle_client, port=self._place.port)
+        )
 
-    async def __aexit__(self, exc_type, exc, tb):
-        await self._stack.__aexit__(exc_type, exc, tb)
+        url = f"{self._hub_url}/ws-exporter"
+        auth = "Bearer dummy-token-1"
+        self._ws_server = await stack.enter_async_context(
+            jsonrpc.WebsocketChannel(
+                url, self._http, start=False, auth=auth, api_obj=self
+            )
+        )
 
-    # TODO: hide from JSON-RPC interface
+    @jsonrpc.hidden
     async def serve_forever(self):
         await util.run_concurrently(
-            self._http_server.serve_forever(), self._ws_server.serve_forever()
+            self._http_server.serve_forever(), self._ws_server.communicate_forever()
         )
 
-    async def _receive_iter(self):
-        try:
-            while True:
-                yield await self._ws.recv()
-        except websockets.ConnectionClosedOK:
-            pass
-
     async def get_place(self):
         return self._place.dict()
 
     async def set_allowed_ips(self, ips):
         new_ips = set(map(ipaddress.ip_address, ips))
         old_ips = set(self._ip_to_tasks_map)
```

### Comparing `not_my_board-0.5.0/not_my_board/_hub.py` & `not_my_board-0.6.0/not_my_board/_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,22 +39,22 @@
             return await _hub.get_places()
     return 404, {}, "Page not found"
 
 
 async def _handle_agent(ws):
     await _authorize_ws(ws)
     client_ip = ws.scope["client"][0]
-    server = jsonrpc.Server(ws.send, ws.receive_iter())
+    server = jsonrpc.Channel(ws.send, ws.receive_iter())
     await _hub.agent_communicate(client_ip, server)
 
 
 async def _handle_exporter(ws):
     await _authorize_ws(ws)
     client_ip = ws.scope["client"][0]
-    exporter = jsonrpc.Proxy(ws.send, ws.receive_iter())
+    exporter = jsonrpc.Channel(ws.send, ws.receive_iter())
     await _hub.exporter_communicate(client_ip, exporter)
 
 
 async def _authorize_ws(ws):
     try:
         auth = ws.headers["authorization"]
         scheme, token = auth.split(" ", 1)
@@ -76,29 +76,32 @@
     _available = set()
     _wait_queue = []
     _reservations = {}
 
     def __init__(self):
         self._id_generator = itertools.count(start=1)
 
+    @jsonrpc.hidden
     async def get_places(self):
         return {"places": [p.dict() for p in self._places.values()]}
 
+    @jsonrpc.hidden
     async def agent_communicate(self, client_ip, rpc):
         client_ip_var.set(client_ip)
         async with self._register_agent():
             rpc.set_api_object(self)
-            await rpc.serve_forever()
+            await rpc.communicate_forever()
 
+    @jsonrpc.hidden
     async def exporter_communicate(self, client_ip, rpc):
         client_ip_var.set(client_ip)
-        async with util.background_task(rpc.io_loop()) as io_loop:
+        async with util.background_task(rpc.communicate_forever()) as com_task:
             export_desc = await rpc.get_place()
             with self._register_place(export_desc, rpc, client_ip):
-                await io_loop
+                await com_task
 
     @contextlib.contextmanager
     def _register_place(self, export_desc, rpc, client_ip):
         id_ = next(self._id_generator)
         place = models.Place(id=id_, host=_unmap_ip(client_ip), **export_desc)
 
         try:
```

### Comparing `not_my_board-0.5.0/not_my_board/_models.py` & `not_my_board-0.6.0/not_my_board/_models.py`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/not_my_board/_usbip.py` & `not_my_board-0.6.0/not_my_board/_usbip.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,32 +19,22 @@
     from typing import Annotated
 
 
 logger = logging.getLogger(__name__)
 _vhci_status_attached = {}
 
 
-class UsbIpServer:
+class UsbIpServer(util.ContextStack):
     def __init__(self, devices):
         self._devices = {d.busid: d for d in devices}
 
-    async def __aenter__(self):
-        async with contextlib.AsyncExitStack() as stack:
-            for _, device in self._devices.items():
-                stack.callback(device.restore_default_usb_driver)
-                await stack.enter_async_context(
-                    util.background_task(_refresh_task(device))
-                )
-
-            self._stack = stack.pop_all()
-            await self._stack.__aenter__()
-            return self
-
-    async def __aexit__(self, exc_type, exc, tb):
-        await self._stack.__aexit__(exc_type, exc, tb)
+    async def _context_stack(self, stack):
+        for _, device in self._devices.items():
+            stack.callback(device.restore_default_usb_driver)
+            await stack.enter_async_context(util.background_task(_refresh_task(device)))
 
     async def handle_client(self, reader, writer):
         sock = writer.transport.get_extra_info("socket")
         _enable_keep_alive(sock)
 
         request = await ImportRequest.from_reader(reader)
         logger.debug("Received: %s", request)
@@ -91,46 +81,41 @@
 
 
 class _SysfsFileHex(_SysfsFileInt):
     def __init__(self, default=None):
         super().__init__(16, default)
 
 
-class UsbIpDevice:
+class UsbIpDevice(util.ContextStack):
     def __init__(self, busid):
         self._busid = busid
         self._sysfs_path = pathlib.Path("/sys/bus/usb/devices/") / busid
         self._lock = asyncio.Lock()
         self._refresh_event = asyncio.Event()
         self._is_exported = False
 
     def refresh(self):
         self._refresh_event.set()
 
-    async def __aenter__(self):
+    async def _context_stack(self, stack):
         async with contextlib.AsyncExitStack() as stack:
             await stack.enter_async_context(self._lock)
             await self.available()
+            stack.callback(self.stop_export)
 
-            self._stack = stack.pop_all()
-            await self._stack.__aenter__()
-            return self
-
-    async def __aexit__(self, exc_type, exc, tb):
+    def stop_export(self):
         if self._is_exported:
             try:
                 (self._sysfs_path / "usbip_sockfd").write_text("-1\n")
             except (OSError, FileNotFoundError):
                 # client might have disconnected or device disappeared
                 pass
             except Exception as e:
                 logger.warning("Error while stopping export: %s", e)
 
-        await self._stack.__aexit__(exc_type, exc, tb)
-
     async def available(self):
         while True:
             await self._ensure_usbip_host_driver()
 
             if self._is_available():
                 break
 
@@ -233,14 +218,16 @@
     proc = await asyncio.create_subprocess_exec(*args, **kwargs)
     await proc.communicate()
     if proc.returncode:
         raise RuntimeError(f"{args!r} exited with {proc.returncode}")
 
 
 async def attach(reader, writer, busid, port_num):
+    await _ensure_vhci_hcd_driver_available()
+
     sock = writer.transport.get_extra_info("socket")
     # Client waits 2 seconds longer before sending keep alive probes, otherwise
     # both sides start sending at the same time.
     _enable_keep_alive(sock, extra_idle_sec=2)
 
     request = ImportRequest(busid.encode())
     logger.debug("Sending: %s", request)
@@ -312,15 +299,17 @@
     try:
         detach_path.write_text(f"{vhci_port}")
     except OSError:
         # not attached anymore
         pass
 
 
-def refresh_vhci_status():
+async def refresh_vhci_status():
+    await _ensure_vhci_hcd_driver_available()
+
     def status_paths():
         vhci_path = pathlib.Path("/sys/devices/platform/vhci_hcd.0")
         # the first status path doesn't have a suffix
         status_path = vhci_path / "status"
         count = itertools.count(1)
 
         while status_path.exists():
@@ -342,14 +331,21 @@
                 _vhci_status_attached[port] = status == status_attached
 
 
 def is_attached(port):
     return _vhci_status_attached[port]
 
 
+async def _ensure_vhci_hcd_driver_available():
+    vhci_hcd_path = pathlib.Path("/sys/devices/platform/vhci_hcd.0")
+    if not vhci_hcd_path.exists():
+        logger.info("Loading vhci-hcd Kernel module")
+        await _exec("modprobe", "vhci-hcd")
+
+
 def _enable_keep_alive(sock, extra_idle_sec=0):
     # enable TCP keep alive
     sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
 
     # Drop connections faster than the 2 hour default: Send first probe after 5
     # (+extra_idle_sec) seconds, then every 5 seconds. After 3 unanswered
     # probes the connection is closed.
@@ -491,15 +487,15 @@
         tmp_path.replace(pipe_path)
 
         async with _open_read_pipe(pipe_path, "r+b", buffering=0) as pipe:
             while True:
                 await pipe.read(4096)
                 device.refresh()
     finally:
-        tmp_path.unlink()
+        pipe_path.unlink()
 
 
 @contextlib.asynccontextmanager
 async def _open_read_pipe(*args, **kwargs):
     with open(*args, **kwargs) as pipe:
         loop = asyncio.get_running_loop()
         reader = asyncio.StreamReader(loop=loop)
```

### Comparing `not_my_board-0.5.0/not_my_board/_util/_asyncio.py` & `not_my_board-0.6.0/not_my_board/_util/_asyncio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import contextlib
+import fcntl
 import signal
 import traceback
 
 _RELAY_BUFFER_SIZE = 64 * 1024  # 64 KiB
 
 
 def run(coro, debug=False):
@@ -169,7 +170,42 @@
 class UnixServer(Server):
     """Same as `Server`, but for `asyncio.start_unix_server()`"""
 
     async def _start(self):
         return await asyncio.start_unix_server(
             self._on_connect, *self._args, **self._kwargs
         )
+
+
+class ContextStack:
+    """Mix-in class to simplify implementing a context manager
+
+    Child classes can implement the _context_stack() function, instead of
+    __aenter__() and __aexit__(). _context_stack() is called when entering the
+    context. It needs to to build up an AsyncExitStack(), that is passed as an
+    argument, which is then cleaned up when exiting the context.
+    """
+
+    async def _context_stack(self, stack):
+        raise NotImplementedError()
+
+    async def __aenter__(self):
+        async with contextlib.AsyncExitStack() as stack:
+            await self._context_stack(stack)
+            self._stack = stack.pop_all()
+            await self._stack.__aenter__()
+            return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self._stack.__aexit__(exc_type, exc, tb)
+
+
+@contextlib.asynccontextmanager
+async def flock(f):
+    """File lock as a context manager"""
+
+    loop = asyncio.get_running_loop()
+    try:
+        await loop.run_in_executor(None, fcntl.flock, f.fileno(), fcntl.LOCK_EX)
+        yield
+    finally:
+        fcntl.flock(f, fcntl.LOCK_UN)
```

### Comparing `not_my_board-0.5.0/not_my_board/_util/_matching.py` & `not_my_board-0.6.0/not_my_board/_util/_matching.py`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/not_my_board/cli/__init__.py` & `not_my_board-0.6.0/not_my_board/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,28 +36,38 @@
         return subparser
 
     def add_verbose_arg(subparser):
         subparser.add_argument(
             "-v", "--verbose", action="store_true", help="Enable debug logs"
         )
 
+    def add_cacert_arg(subparser):
+        subparser.add_argument(
+            "--cacert",
+            type=pathlib.Path,
+            action="append",
+            help="path to CA certificates, which should be trusted",
+        )
+
     subparser = add_subcommand("hub", help="start the board farm hub")
     subparser.set_defaults(verbose=True)
 
     subparser = add_subcommand(
         "export", help="make connected boards available in the board farm"
     )
     subparser.set_defaults(verbose=True)
+    add_cacert_arg(subparser)
     subparser.add_argument("hub_url", help="http(s) URL of the hub")
     subparser.add_argument(
         "export_description", type=pathlib.Path, help="path to a export description"
     )
 
     subparser = add_subcommand("agent", help="start an agent")
     subparser.set_defaults(verbose=True)
+    add_cacert_arg(subparser)
     subparser.add_argument("hub_url", help="http(s) URL of the hub")
 
     subparser = add_subcommand("reserve", help="reserve a place")
     add_verbose_arg(subparser)
     subparser.add_argument("-n", "--with-name", help="reserve under a different name")
     subparser.add_argument(
         "import_description", help="name or full path of an import description"
@@ -134,19 +144,19 @@
 
 
 def _hub_command(_):
     hub()
 
 
 async def _export_command(args):
-    await export(args.hub_url, args.export_description)
+    await export(args.hub_url, args.export_description, args.cacert)
 
 
 async def _agent_command(args):
-    await agent(args.hub_url)
+    await agent(args.hub_url, args.cacert)
 
 
 async def _reserve_command(args):
     await client.reserve(args.import_description, args.with_name)
 
 
 async def _return_command(args):
```

### Comparing `not_my_board-0.5.0/pyproject.toml` & `not_my_board-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: Software Development :: Testing",
 ]
 dependencies = [
     "asgineer",
+    "async-timeout; python_version < '3.11'",
     "h11",
     "pydantic ~= 1.10",
     "tomli; python_version < '3.11'",
     "typing_extensions; python_version < '3.9'",
     "uvicorn",
     "websockets",
 ]
```

### Comparing `not_my_board-0.5.0/scripts/_vmctl/alpine-chroot-install.sh` & `not_my_board-0.6.0/scripts/_vmctl/alpine-chroot-install.sh`

 * *Files 7% similar despite different names*

```diff
@@ -20,20 +20,19 @@
 iface eth0 inet dhcp
 EOF
 
 setup-timezone -z UTC
 
 setup-user -au admin
 echo "permit nopass :wheel" >> /etc/doas.d/doas.conf
-addgroup -S vhci
-addgroup admin vhci
+addgroup -S not-my-board
+addgroup admin not-my-board
 
 # configure sshd
 sed -e 's/#\(PermitEmptyPasswords\) no/\1 yes/' \
-    -e 's/#\(UsePAM\) no/\1 yes/' \
     -i /etc/ssh/sshd_config
 cat >> /etc/conf.d/sshd << EOF
 sshd_disable_keygen="yes"
 EOF
 
 # disable gettys
 sed -i 's/tty\d::.*getty.*/#\0/' /etc/inittab
```

### Comparing `not_my_board-0.5.0/scripts/_vmctl/configure-vm.sh` & `not_my_board-0.6.0/scripts/_vmctl/configure-vm.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/bin/sh
 
+ip_hub=192.168.200.1
+ip_exporter=192.168.200.2
+ip_client=192.168.200.3
+
 main() {
     vm="${1:?}"
     PS4=">>> "
     set -ex
 
     case "$vm" in
     hub)
@@ -14,47 +18,70 @@
         setup_network_exporter
         install_project
         reconfigure_device_manager
         ;;
     client)
         setup_network_client
         install_project
-        load_vhci_hcd
         ;;
     *)
         echo "error: invalid VM: $vm"
         exit 1
     esac
 }
 
 setup_network_hub() {
     ip link add name br0 type bridge
     ip link set eth1 up
     ip link set dev eth1 master br0
     ip link set eth2 up
     ip link set dev eth2 master br0
 
-    ip addr add 192.168.200.1/24 dev br0
+    ip addr add "$ip_hub/24" dev br0
     ip link set br0 up
+
+    cat >> /etc/hosts << EOF
+127.0.0.1 hub.local
+$ip_exporter exporter.local
+$ip_client client.local
+EOF
 }
 
 setup_network_exporter() {
-    ip addr add 192.168.200.2/24 dev eth1
+    ip addr add "$ip_exporter/24" dev eth1
     ip link set eth1 up
+
+    cat >> /etc/hosts << EOF
+$ip_hub hub.local
+127.0.0.1 exporter.local
+$ip_client client.local
+EOF
 }
 
 setup_network_client() {
-    ip addr add 192.168.200.3/24 dev eth1
+    ip addr add "$ip_client/24" dev eth1
     ip link set eth1 up
+
+    cat >> /etc/hosts << EOF
+$ip_hub hub.local
+$ip_exporter exporter.local
+127.0.0.1 client.local
+EOF
 }
 
 install_project() {
     mount_project_source
 
-    pip install --no-index --find-links ./src/scripts/_vmctl/img/pip-cache --no-build-isolation --config-settings=builddir="$PWD/build" --editable ./src/
+    pip install \
+        --break-system-packages \
+        --no-index \
+        --find-links ./src/scripts/_vmctl/img/pip-cache \
+        --no-build-isolation \
+        --config-settings=builddir="$PWD/build" \
+        --editable ./src/
     chown -R admin:admin build
 }
 
 mount_project_source() {
     # meson-python needs to write in the source directory while installing
     # the package. To not modify the actual source directory, mount it with
     # a writable overlay.
@@ -77,16 +104,8 @@
 
     echo > /dev/mdev.seq
     echo > /dev/mdev.log
 
     /etc/init.d/mdev restart
 }
 
-load_vhci_hcd() {
-    modprobe vhci-hcd
-    for file_name in attach detach; do
-        chgrp vhci "/sys/devices/platform/vhci_hcd.0/$file_name"
-        chmod g+w "/sys/devices/platform/vhci_hcd.0/$file_name"
-    done
-}
-
 main "$@"
```

### Comparing `not_my_board-0.5.0/scripts/get_version` & `not_my_board-0.6.0/scripts/get_version`

 * *Files identical despite different names*

### Comparing `not_my_board-0.5.0/scripts/vmctl` & `not_my_board-0.6.0/scripts/vmctl`

 * *Files 2% similar despite different names*

```diff
@@ -79,19 +79,19 @@
         "$mnt/sys" \
         "$mnt/etc/apk" \
         "$mnt/mnt" \
         "$work/boot" \
         "$disk_mnt" \
         ;
 
-    ALPINE_RELEASE="v3.18"
-    download_alpine_package apk-tools-static 2.14.0-r2 \
-        c8465a56bac138677d3fb025f7e13a30d18210ef327880673314ad63d59c1977
+    ALPINE_RELEASE="v3.19"
+    download_alpine_package apk-tools-static 2.14.3-r1 \
+        13028afe91f3f8a64927844ea69e0d8f11ba96197a74e3efa199f3f1b3351a15
     download_alpine_package alpine-keys 2.4-r1 \
-        880983a4ba0e6403db432e7b2687af976e023567ab11d1428c758351011263e9
+        125e1ab758948ba6c597919d1c3b36e2e842f7a5be68d828ff5a1dceded41ebb
 
     apk() {
         "$work/apk-tools-static/sbin/apk.static" \
             --keys-dir="$work/alpine-keys/etc/apk/keys" \
             "$@"
     }
 
@@ -117,23 +117,19 @@
         --initdb \
         --no-progress \
         alpine-base \
         alpine-conf \
         doas \
         "linux-$kernel_variant" \
         linux-firmware-none \
-        linux-pam \
         openssh \
-        openssh-server-pam \
-        pam-rundir \
         py3-meson-python \
         py3-pip \
         python3 \
         tzdata \
-        util-linux-login \
         ;
 
     chroot "$mnt" /usr/bin/env - \
         PATH=/sbin:/usr/sbin:/bin:/usr/bin \
         HOME=/root \
         /bin/sh < "$vmctldir/alpine-chroot-install.sh"
 
@@ -343,26 +339,29 @@
     wait_for_sshd "$vm"
     ssh_vm "$vm" "doas sh -s $vm" < "$vmctldir/configure-vm.sh" >&2
 }
 
 wait_for_sshd() {
     vm="$1"
     i=0
-    while [ "$i" -lt 30 ]; do
+    while [ "$i" -lt 70 ]; do
         if ssh_vm "$vm" true 2>/dev/null; then
-            break
+            return
         fi
         i=$((i + 1))
         if [ -e /dev/kvm ]; then
             sleep 0.1
         else
             # without kvm, booting the VM takes quite a bit longer
             sleep 5
         fi
     done
+
+    echo "error: VM doesn't respond" >&2
+    return 1
 }
 
 ssh() {
     if [ "$#" -lt 1 ]; then
         usage_error "the following argument is required: vm"
     fi
```

### Comparing `not_my_board-0.5.0/tests/test_hub.py` & `not_my_board-0.6.0/tests/test_hub.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     assert places["places"] == []
 
 
 class FakeExporter:
     def __init__(self, register_event):
         self._register_event = register_event
 
-    async def io_loop(self):
+    async def communicate_forever(self):
         # wait forever
         await asyncio.Event().wait()
 
     async def get_place(self):
         self._register_event.set()
         return {
             "port": 1234,
@@ -59,51 +59,51 @@
 # pylint: disable=redefined-outer-name
 @contextlib.asynccontextmanager
 async def register_exporter(hub, ip=DEFAULT_EXPORTER_IP):
     register_event = asyncio.Event()
     fake_exporter = FakeExporter(register_event)
     coro = hub.exporter_communicate(ip, fake_exporter)
     async with util.background_task(coro) as exporter_task:
-        async with asyncio.timeout(2):
+        async with util.timeout(2):
             await register_event.wait()
         yield fake_exporter, exporter_task
 
 
 async def test_register_exporter(hub):
     async with register_exporter(hub):
         places = await hub.get_places()
         assert len(places["places"]) == 1
 
     places = await hub.get_places()
     assert len(places["places"]) == 0
 
 
 def fake_rpc_pair():
-    proxy_to_server = asyncio.Queue()
-    server_to_proxy = asyncio.Queue()
+    rpc1_to_rpc2 = asyncio.Queue()
+    rpc2_to_rpc1 = asyncio.Queue()
 
     async def receive_iter(queue):
         while True:
             data = await queue.get()
             yield data
             queue.task_done()
 
-    server = jsonrpc.Server(server_to_proxy.put, receive_iter(proxy_to_server))
-    proxy = jsonrpc.Proxy(proxy_to_server.put, receive_iter(server_to_proxy))
-    return server, proxy
+    rpc1 = jsonrpc.Channel(rpc1_to_rpc2.put, receive_iter(rpc2_to_rpc1))
+    rpc2 = jsonrpc.Channel(rpc2_to_rpc1.put, receive_iter(rpc1_to_rpc2))
+    return rpc1, rpc2
 
 
 # pylint: disable=redefined-outer-name
 @contextlib.asynccontextmanager
 async def register_agent(hub, ip=DEFAULT_AGENT_IP):
-    server, proxy = fake_rpc_pair()
-    coro = hub.agent_communicate(ip, server)
+    rpc1, rpc2 = fake_rpc_pair()
+    coro = hub.agent_communicate(ip, rpc2)
     async with util.background_task(coro):
-        async with util.background_task(proxy.io_loop()):
-            yield proxy
+        async with util.background_task(rpc1.communicate_forever()):
+            yield rpc1
 
 
 async def test_reserve_place(hub):
     async with register_exporter(hub) as (exporter, _):
         async with register_agent(hub) as agent:
             places = await hub.get_places()
             candidate_ids = [places["places"][0]["id"]]
```

### Comparing `not_my_board-0.5.0/PKG-INFO` & `not_my_board-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-my-board
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tool to setup, manage and use a board farm 
 Keywords: board-farm embedded testing
 Author-Email: Simon Holesch <simon@holesch.de>
 License: MIT License
         
         Copyright (c) 2022-present Simon Holesch <simon@holesch.de>
         
@@ -27,26 +27,27 @@
         SOFTWARE.
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Testing
 Project-URL: Documentation, http://not-my-board.readthedocs.io
 Project-URL: Issues, https://github.com/holesch/not-my-board/issues
 Project-URL: Source, https://github.com/holesch/not-my-board
 Requires-Python: >=3.7
 Requires-Dist: asgineer
+Requires-Dist: async-timeout; python_version < "3.11"
 Requires-Dist: h11
 Requires-Dist: pydantic~=1.10
 Requires-Dist: tomli; python_version < "3.11"
 Requires-Dist: typing_extensions; python_version < "3.9"
 Requires-Dist: uvicorn
 Requires-Dist: websockets
 Requires-Dist: black; extra == "test"
```

