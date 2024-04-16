# Comparing `tmp/DragonPyEmulator-0.9.1.tar.gz` & `tmp/dragonpyemulator-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DragonPyEmulator-0.9.1.tar", last modified: Fri Nov  3 07:13:19 2023, max compression
+gzip compressed data, was "dragonpyemulator-0.9.2.tar", last modified: Tue Apr 16 15:15:03 2024, max compression
```

## Comparing `DragonPyEmulator-0.9.1.tar` & `dragonpyemulator-0.9.2.tar`

### file list

```diff
@@ -1,255 +1,262 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.1/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.1/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1934 2023-11-03 07:03:25.000000 DragonPyEmulator-0.9.1/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      123 2023-11-03 06:59:12.000000 DragonPyEmulator-0.9.1/.gitignore
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/lib/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/site-packages/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-11-03 06:52:19.000000 DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/lib/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/site-packages/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-11-03 06:51:37.000000 DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/bleach/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/bleach/_vendor/
--rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-08-05 19:46:50.000000 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/bleach/_vendor/vendor_install.sh
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 19:46:49.000000 DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/activate.sh
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib/python3.11/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib/python3.11/site-packages/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib/python3.11/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib/python3.11/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/.venv/lib/python3.11/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-11-03 06:47:17.000000 DragonPyEmulator-0.9.1/.venv/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib64/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib64/python3.11/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib64/python3.11/site-packages/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib64/python3.11/site-packages/virtualenv/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/.venv/lib64/python3.11/site-packages/virtualenv/activation/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/.venv/lib64/python3.11/site-packages/virtualenv/activation/bash/
--rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-11-03 06:47:17.000000 DragonPyEmulator-0.9.1/.venv/lib64/python3.11/site-packages/virtualenv/activation/bash/activate.sh
--rw-rw-r--   0 jens      (1000) users      (100)      937 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/AUTHORS
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/BASIC examples/
--rwxrwxr-x   0 jens      (1000) users      (100)     2623 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/DumpBasicProgram.bas
--rw-rw-r--   0 jens      (1000) users      (100)      717 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/ListVariables.bas
--rw-rw-r--   0 jens      (1000) users      (100)       90 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/display_all_chars.bas
--rw-rw-r--   0 jens      (1000) users      (100)       69 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/display_all_chars_loop.bas
--rw-rw-r--   0 jens      (1000) users      (100)     1448 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/hex_view01.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     4237 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/hustle.c10.bas
--rw-rw-r--   0 jens      (1000) users      (100)      494 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/mandelbrot1.bas
--rw-rw-r--   0 jens      (1000) users      (100)      707 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/mandelbrot2.bas
--rwxrwxr-x   0 jens      (1000) users      (100)       44 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/print_all_chars.bas
--rwxrwxr-x   0 jens      (1000) users      (100)       58 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/print_all_chars_loop.bas
--rwxrwxr-x   0 jens      (1000) users      (100)      105 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC examples/print_timer.bas
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/BASIC games/
--rwxrwxr-x   0 jens      (1000) users      (100)     6239 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC games/INVADER.bas
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.981755 DragonPyEmulator-0.9.1/BASIC tools/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/BASIC tools/FloatingPoint/
--rwxrwxr-x   0 jens      (1000) users      (100)     1601 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/FloatingPoint/test_FPA0.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1878 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/FloatingPoint/test_FPA0_02.bas
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/BASIC tools/HexViewer/
--rw-rw-r--   0 jens      (1000) users      (100)      231 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/HexViewer/README.creole
--rw-rw-r--   0 jens      (1000) users      (100)     1205 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/HexViewer/hex_view01.bas
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/BASIC tools/InputOutput/
--rwxrwxr-x   0 jens      (1000) users      (100)     1220 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/InputOutput/keyboard.bas
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.989755 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/
--rwxrwxr-x   0 jens      (1000) users      (100)     7660 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/README.creole
--rwxrwxr-x   0 jens      (1000) users      (100)     1779 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1936 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_ADDA.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1872 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_DEC.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1872 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_INC.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1938 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_LSL.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1908 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_NEGA.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1935 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_SUBA.bas
--rwxrwxr-x   0 jens      (1000) users      (100)     1791 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_TST.bas
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/
--rw-r--r--   0 jens      (1000) users      (100)    89338 2023-11-03 07:13:17.000000 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     5934 2023-11-03 07:13:18.000000 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-11-03 07:13:17.000000 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-11-03 07:13:17.000000 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      232 2023-11-03 07:13:17.000000 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)       27 2023-11-03 07:13:17.000000 DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)    35121 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/LICENSE
--rw-rw-r--   0 jens      (1000) users      (100)      296 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/MANIFEST.in
--rw-r--r--   0 jens      (1000) users      (100)    89338 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/PKG-INFO
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/PyDC/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/PyDC/PyDC/
--rw-rw-r--   0 jens      (1000) users      (100)    26714 2023-03-07 15:38:05.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/CassetteObjects.py
--rw-rw-r--   0 jens      (1000) users      (100)     2999 2023-03-07 15:37:28.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3590 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/base_cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     3698 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/basic_tokens.py
--rwxrwxr-x   0 jens      (1000) users      (100)    11975 2023-03-07 15:38:27.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/bitstream_handler.py
--rw-rw-r--   0 jens      (1000) users      (100)     4858 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/configs.py
--rwxrwxr-x   0 jens      (1000) users      (100)    11290 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/tests.py
--rwxrwxr-x   0 jens      (1000) users      (100)    21278 2023-03-07 15:40:41.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/utils.py
--rw-rw-r--   0 jens      (1000) users      (100)    23319 2023-03-07 15:37:50.000000 DragonPyEmulator-0.9.1/PyDC/PyDC/wave2bitstream.py
--rwxrwxr-x   0 jens      (1000) users      (100)     5031 2023-03-07 17:23:27.000000 DragonPyEmulator-0.9.1/PyDC/PyDC_cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     5166 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/README.creole
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/PyDC/test_files/
--rwxrwxr-x   0 jens      (1000) users      (100)   225708 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/test_files/HelloWorld1 origin.wav
--rwxrwxr-x   0 jens      (1000) users      (100)    82204 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/test_files/HelloWorld1 xroar.wav
--rwxrwxr-x   0 jens      (1000) users      (100)       54 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/test_files/HelloWorld1.bas
--rwxrwxr-x   0 jens      (1000) users      (100)   264236 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/test_files/LineNumber Test 01.wav
--rwxrwxr-x   0 jens      (1000) users      (100)   401452 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/test_files/LineNumber Test 02.wav
--rwxrwxr-x   0 jens      (1000) users      (100)      128 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/PyDC/test_files/LineNumberTest.bas
--rw-rw-r--   0 jens      (1000) users      (100)    88020 2023-11-03 07:05:07.000000 DragonPyEmulator-0.9.1/README.md
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/basic_editor/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    11100 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/editor.py
--rw-rw-r--   0 jens      (1000) users      (100)      611 2023-03-07 14:53:57.000000 DragonPyEmulator-0.9.1/basic_editor/editor_base.py
--rw-rw-r--   0 jens      (1000) users      (100)     5817 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/highlighting.py
--rw-rw-r--   0 jens      (1000) users      (100)     3610 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/scrolled_text.py
--rw-rw-r--   0 jens      (1000) users      (100)      981 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/status_bar.py
--rw-rw-r--   0 jens      (1000) users      (100)      584 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/tkinter_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     4296 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/basic_editor/token_window.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3045 2023-11-03 06:58:41.000000 DragonPyEmulator-0.9.1/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3045 2023-11-03 06:58:41.000000 DragonPyEmulator-0.9.1/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/CoCo/
--rw-rw-r--   0 jens      (1000) users      (100)      918 2023-03-07 14:18:17.000000 DragonPyEmulator-0.9.1/dragonpy/CoCo/CoCo2b_rom.py
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/CoCo/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3796 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/CoCo/config.py
--rw-rw-r--   0 jens      (1000) users      (100)      684 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/CoCo/machine.py
--rw-rw-r--   0 jens      (1000) users      (100)     1828 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/CoCo/mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)     1771 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/CoCo/periphery_coco.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/Dragon32/
--rw-rw-r--   0 jens      (1000) users      (100)     1086 2023-03-07 06:59:50.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/Dragon32_rom.py
--rw-rw-r--   0 jens      (1000) users      (100)    17337 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/MC6821_PIA.py
--rw-rw-r--   0 jens      (1000) users      (100)     4015 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/MC6847.py
--rw-rw-r--   0 jens      (1000) users      (100)     8435 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/MC6883_SAM.py
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      975 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/cassette.py
--rw-rw-r--   0 jens      (1000) users      (100)     5287 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/config.py
--rw-rw-r--   0 jens      (1000) users      (100)     7255 2023-03-06 19:37:02.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/dragon_charmap.py
--rw-rw-r--   0 jens      (1000) users      (100)    30337 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/dragon_font.py
--rw-rw-r--   0 jens      (1000) users      (100)    10791 2023-03-06 19:37:02.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/gui_config.py
--rwxrwxr-x   0 jens      (1000) users      (100)    11074 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/keyboard_map.py
--rw-rw-r--   0 jens      (1000) users      (100)      791 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/machine.py
--rw-rw-r--   0 jens      (1000) users      (100)    46500 2023-03-06 19:35:33.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)     5407 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/periphery_dragon.py
--rw-rw-r--   0 jens      (1000) users      (100)     1517 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon32/speaker.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/Dragon64/
--rwxrwxr-x   0 jens      (1000) users      (100)     2755 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/6809dasm_comments.py
--rw-rw-r--   0 jens      (1000) users      (100)   138378 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/Dragon 64 in 32 mode.txt
--rw-rw-r--   0 jens      (1000) users      (100)     1555 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/Dragon64_rom.py
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2105 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/config.py
--rw-rw-r--   0 jens      (1000) users      (100)      765 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/create_mem_info.py
--rwxrwxr-x   0 jens      (1000) users      (100)   158695 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/dasm_asm_d64_rom.sh
--rw-rw-r--   0 jens      (1000) users      (100)      708 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/machine.py
--rw-rw-r--   0 jens      (1000) users      (100)   193693 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Dragon64/mem_info.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/
--rw-rw-r--   0 jens      (1000) users      (100)     1876 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/Multicomp6809_rom.py
--rwxrwxr-x   0 jens      (1000) users      (100)      761 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/README.creole
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2017 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/config.py
--rw-rw-r--   0 jens      (1000) users      (100)      443 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/gui.py
--rw-rw-r--   0 jens      (1000) users      (100)      773 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/machine.py
--rw-rw-r--   0 jens      (1000) users      (100)     2759 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/periphery_Multicomp6809.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/Simple6809/
--rwxrwxr-x   0 jens      (1000) users      (100)      232 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/Grant's 6809 computer.URL
--rwxrwxr-x   0 jens      (1000) users      (100)      554 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/README.creole
--rw-rw-r--   0 jens      (1000) users      (100)     2003 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/Simple6809_rom.py
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/__init__.py
--rwxrwxr-x   0 jens      (1000) users      (100)     1547 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/asm_lst2py_unittest.py
--rw-rw-r--   0 jens      (1000) users      (100)     2490 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/config.py
--rw-rw-r--   0 jens      (1000) users      (100)      741 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/machine.py
--rwxrwxr-x   0 jens      (1000) users      (100)      923 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/make_mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)   233609 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)     3281 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/periphery_simple6809.py
--rw-rw-r--   0 jens      (1000) users      (100)     2365 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/Simple6809/reformat_rom.py
--rw-rw-r--   0 jens      (1000) users      (100)     1470 2023-11-03 07:01:25.000000 DragonPyEmulator-0.9.1/dragonpy/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.1/dragonpy/__main__.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 19:20:05.000000 DragonPyEmulator-0.9.1/dragonpy/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     5990 2023-11-03 07:07:50.000000 DragonPyEmulator-0.9.1/dragonpy/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7856 2023-11-03 07:05:03.000000 DragonPyEmulator-0.9.1/dragonpy/cli/dev.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/components/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/components/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    13109 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/components/memory.py
--rw-rw-r--   0 jens      (1000) users      (100)     9857 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/components/periphery.py
--rw-rw-r--   0 jens      (1000) users      (100)     6073 2023-03-07 07:18:07.000000 DragonPyEmulator-0.9.1/dragonpy/components/rom.py
--rw-rw-r--   0 jens      (1000) users      (100)      942 2023-11-03 07:01:25.000000 DragonPyEmulator-0.9.1/dragonpy/constants.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.993755 DragonPyEmulator-0.9.1/dragonpy/core/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/core/__init__.py
--rwxrwxr-x   0 jens      (1000) users      (100)     1988 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/core/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)     3735 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/core/configs.py
--rwxrwxr-x   0 jens      (1000) users      (100)    16429 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/core/gui.py
--rw-rw-r--   0 jens      (1000) users      (100)     7715 2023-11-03 06:50:57.000000 DragonPyEmulator-0.9.1/dragonpy/core/gui_starter.py
--rw-rw-r--   0 jens      (1000) users      (100)     6447 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/core/machine.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/dragonpy/sbc09/
--rw-rw-r--   0 jens      (1000) users      (100)     2167 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/README.creole
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1676 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/config.py
--rw-rw-r--   0 jens      (1000) users      (100)     5818 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/create_trace.py
--rw-rw-r--   0 jens      (1000) users      (100)      439 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/gui.py
--rw-rw-r--   0 jens      (1000) users      (100)      687 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/machine.py
--rwxrwxr-x   0 jens      (1000) users      (100)   142429 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/make_mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)    28291 2023-03-06 19:35:23.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)     4174 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/periphery.py
--rwxrwxr-x   0 jens      (1000) users      (100)    29929 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/sbc09.creole
--rw-rw-r--   0 jens      (1000) users      (100)      712 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/sbc09_rom.py
--rw-rw-r--   0 jens      (1000) users      (100)    32768 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/sbc09/v09.rom
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/dragonpy/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      150 2023-08-05 18:21:05.000000 DragonPyEmulator-0.9.1/dragonpy/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1324 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/tests/project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     3209 2023-11-03 06:55:37.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_BASIC_Dragon32.py
--rw-rw-r--   0 jens      (1000) users      (100)    25042 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_BASIC_simple09.py
--rw-rw-r--   0 jens      (1000) users      (100)    15796 2023-03-07 16:21:59.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_base.py
--rw-rw-r--   0 jens      (1000) users      (100)      749 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_config.py
--rw-rw-r--   0 jens      (1000) users      (100)      280 2023-11-03 07:01:25.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2558 2023-08-05 18:21:05.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2148 2023-08-05 19:45:06.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)      776 2023-11-03 06:51:16.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_readme_history.py
--rw-rw-r--   0 jens      (1000) users      (100)     1601 2023-03-07 16:22:09.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_rom_download.py
--rw-rw-r--   0 jens      (1000) users      (100)     6708 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/tests/test_sbc09.py
--rw-rw-r--   0 jens      (1000) users      (100)      402 2023-03-07 15:36:28.000000 DragonPyEmulator-0.9.1/dragonpy/tests/utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/dragonpy/utils/
--rw-rw-r--   0 jens      (1000) users      (100)     4104 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/BASIC09_floating_point.py
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3214 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/bits.py
--rw-rw-r--   0 jens      (1000) users      (100)     1271 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/disable_logging.py
--rwxrwxr-x   0 jens      (1000) users      (100)     2321 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/hex2bin.py
--rw-rw-r--   0 jens      (1000) users      (100)     2341 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/humanize.py
--rwxrwxr-x   0 jens      (1000) users      (100)    17555 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/pager.py
--rw-rw-r--   0 jens      (1000) users      (100)     2107 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/simple_debugger.py
--rwxrwxr-x   0 jens      (1000) users      (100)     5553 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/utils/srecord_utils.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/dragonpy/vectrex/
--rwxrwxr-x   0 jens      (1000) users      (100)    10241 2023-03-06 19:37:43.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/MOS6522.py
--rw-rw-r--   0 jens      (1000) users      (100)     8192 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/SYSTEM.IMG
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1746 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/config.py
--rw-rw-r--   0 jens      (1000) users      (100)      750 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/machine.py
--rw-rw-r--   0 jens      (1000) users      (100)     2429 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/mem_info.py
--rw-rw-r--   0 jens      (1000) users      (100)     1725 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/periphery.py
--rw-rw-r--   0 jens      (1000) users      (100)      367 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/vectrex_gui.py
--rw-rw-r--   0 jens      (1000) users      (100)      717 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/dragonpy/vectrex/vectrex_rom.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/misc/
--rw-rw-r--   0 jens      (1000) users      (100)    11745 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/misc/README.creole
--rwxrwxr-x   0 jens      (1000) users      (100)     5407 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/misc/add_info_in_trace.py
--rwxrwxr-x   0 jens      (1000) users      (100)    10558 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/misc/filter_xroar_trace.py
--rw-rw-r--   0 jens      (1000) users      (100)     2196 2023-03-06 18:48:22.000000 DragonPyEmulator-0.9.1/misc/xroar_gdb_tests.py
--rw-rw-r--   0 jens      (1000) users      (100)     5055 2023-11-03 07:01:06.000000 DragonPyEmulator-0.9.1/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    55752 2023-11-03 07:01:10.000000 DragonPyEmulator-0.9.1/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)    31733 2023-11-03 07:01:10.000000 DragonPyEmulator-0.9.1/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-11-03 07:13:18.997755 DragonPyEmulator-0.9.1/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/
+-rw-rw-r--   0 jens      (1000) users      (100)      310 2024-01-04 17:10:16.000000 dragonpyemulator-0.9.2/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-03-06 19:20:05.000000 dragonpyemulator-0.9.2/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1938 2024-04-16 14:35:03.000000 dragonpyemulator-0.9.2/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      131 2024-04-16 14:35:03.000000 dragonpyemulator-0.9.2/.gitignore
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2024-04-16 15:03:58.000000 dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2024-04-16 15:03:37.000000 dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/bleach/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/bleach/_vendor/
+-rwxrwxr-x   0 jens      (1000) users      (100)      453 2023-08-05 19:46:50.000000 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/bleach/_vendor/vendor_install.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2023-08-05 19:46:49.000000 dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib/python3.11/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib/python3.11/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib/python3.11/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/.venv/lib/python3.11/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2024-04-16 15:09:37.000000 dragonpyemulator-0.9.2/.venv/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib64/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib64/python3.11/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib64/python3.11/site-packages/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib64/python3.11/site-packages/virtualenv/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/.venv/lib64/python3.11/site-packages/virtualenv/activation/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/.venv/lib64/python3.11/site-packages/virtualenv/activation/bash/
+-rw-rw-r--   0 jens      (1000) users      (100)     2264 2024-04-16 15:09:37.000000 dragonpyemulator-0.9.2/.venv/lib64/python3.11/site-packages/virtualenv/activation/bash/activate.sh
+-rw-rw-r--   0 jens      (1000) users      (100)      937 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/AUTHORS
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/BASIC examples/
+-rwxrwxr-x   0 jens      (1000) users      (100)     2623 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/DumpBasicProgram.bas
+-rw-rw-r--   0 jens      (1000) users      (100)      717 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/ListVariables.bas
+-rw-rw-r--   0 jens      (1000) users      (100)       90 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/display_all_chars.bas
+-rw-rw-r--   0 jens      (1000) users      (100)       69 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/display_all_chars_loop.bas
+-rw-rw-r--   0 jens      (1000) users      (100)     1448 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/hex_view01.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     4237 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/hustle.c10.bas
+-rw-rw-r--   0 jens      (1000) users      (100)      494 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/mandelbrot1.bas
+-rw-rw-r--   0 jens      (1000) users      (100)      707 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/mandelbrot2.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)       44 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/print_all_chars.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)       58 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/print_all_chars_loop.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)      105 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC examples/print_timer.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/BASIC games/
+-rwxrwxr-x   0 jens      (1000) users      (100)     6239 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC games/INVADER.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.571957 dragonpyemulator-0.9.2/BASIC tools/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/BASIC tools/FloatingPoint/
+-rwxrwxr-x   0 jens      (1000) users      (100)     1601 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/FloatingPoint/test_FPA0.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1878 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/FloatingPoint/test_FPA0_02.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/BASIC tools/HexViewer/
+-rw-rw-r--   0 jens      (1000) users      (100)      231 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/HexViewer/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)     1205 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/HexViewer/hex_view01.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/BASIC tools/InputOutput/
+-rwxrwxr-x   0 jens      (1000) users      (100)     1220 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/InputOutput/keyboard.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/
+-rwxrwxr-x   0 jens      (1000) users      (100)     7660 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/README.creole
+-rwxrwxr-x   0 jens      (1000) users      (100)     1779 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1936 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_ADDA.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1872 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_DEC.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1872 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_INC.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1938 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_LSL.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1908 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_NEGA.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1935 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_SUBA.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)     1791 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_TST.bas
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/
+-rw-r--r--   0 jens      (1000) users      (100)    89931 2024-04-16 15:15:01.000000 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     6129 2024-04-16 15:15:03.000000 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2024-04-16 15:15:01.000000 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2024-04-16 15:15:01.000000 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      280 2024-04-16 15:15:01.000000 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       27 2024-04-16 15:15:01.000000 dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    35121 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/LICENSE
+-rw-rw-r--   0 jens      (1000) users      (100)      296 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/MANIFEST.in
+-rw-r--r--   0 jens      (1000) users      (100)    89931 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/PKG-INFO
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/PyDC/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/PyDC/PyDC/
+-rw-rw-r--   0 jens      (1000) users      (100)    26714 2023-03-07 15:38:05.000000 dragonpyemulator-0.9.2/PyDC/PyDC/CassetteObjects.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2999 2023-03-07 15:37:28.000000 dragonpyemulator-0.9.2/PyDC/PyDC/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3590 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/PyDC/base_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3698 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/PyDC/basic_tokens.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    11975 2023-03-07 15:38:27.000000 dragonpyemulator-0.9.2/PyDC/PyDC/bitstream_handler.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4858 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/PyDC/configs.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    11290 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/PyDC/tests.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    21283 2024-01-04 17:10:16.000000 dragonpyemulator-0.9.2/PyDC/PyDC/utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)    23319 2023-03-07 15:37:50.000000 dragonpyemulator-0.9.2/PyDC/PyDC/wave2bitstream.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     5031 2023-03-07 17:23:27.000000 dragonpyemulator-0.9.2/PyDC/PyDC_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5166 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/README.creole
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/PyDC/test_files/
+-rwxrwxr-x   0 jens      (1000) users      (100)   225708 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/test_files/HelloWorld1 origin.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)    82204 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/test_files/HelloWorld1 xroar.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)       54 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/test_files/HelloWorld1.bas
+-rwxrwxr-x   0 jens      (1000) users      (100)   264236 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/test_files/LineNumber Test 01.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)   401452 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/test_files/LineNumber Test 02.wav
+-rwxrwxr-x   0 jens      (1000) users      (100)      128 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/PyDC/test_files/LineNumberTest.bas
+-rw-rw-r--   0 jens      (1000) users      (100)    88444 2024-04-16 15:12:28.000000 dragonpyemulator-0.9.2/README.md
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.579957 dragonpyemulator-0.9.2/basic_editor/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    11100 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/editor.py
+-rw-rw-r--   0 jens      (1000) users      (100)      611 2023-03-07 14:53:57.000000 dragonpyemulator-0.9.2/basic_editor/editor_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5817 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/highlighting.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3610 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/scrolled_text.py
+-rw-rw-r--   0 jens      (1000) users      (100)      981 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/status_bar.py
+-rw-rw-r--   0 jens      (1000) users      (100)      584 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/tkinter_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4296 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/basic_editor/token_window.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3080 2024-04-16 14:33:11.000000 dragonpyemulator-0.9.2/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3080 2024-04-16 14:33:11.000000 dragonpyemulator-0.9.2/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/CoCo/
+-rw-rw-r--   0 jens      (1000) users      (100)      918 2023-03-07 14:18:17.000000 dragonpyemulator-0.9.2/dragonpy/CoCo/CoCo2b_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/CoCo/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3796 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/CoCo/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      684 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/CoCo/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1829 2024-01-04 17:10:16.000000 dragonpyemulator-0.9.2/dragonpy/CoCo/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1771 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/CoCo/periphery_coco.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/Dragon32/
+-rw-rw-r--   0 jens      (1000) users      (100)     1086 2023-03-07 06:59:50.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/Dragon32_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)    17337 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/MC6821_PIA.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4015 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/MC6847.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8435 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/MC6883_SAM.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      975 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/cassette.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5287 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7247 2024-01-04 17:10:16.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/dragon_charmap.py
+-rw-rw-r--   0 jens      (1000) users      (100)    30337 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/dragon_font.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10791 2023-03-06 19:37:02.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/gui_config.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    11074 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/keyboard_map.py
+-rw-rw-r--   0 jens      (1000) users      (100)      791 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)    46500 2023-03-06 19:35:33.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5407 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/periphery_dragon.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1517 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon32/speaker.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/Dragon64/
+-rwxrwxr-x   0 jens      (1000) users      (100)     2756 2024-01-04 17:10:16.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/6809dasm_comments.py
+-rw-rw-r--   0 jens      (1000) users      (100)   138378 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/Dragon 64 in 32 mode.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     1555 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/Dragon64_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2105 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      765 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/create_mem_info.py
+-rwxrwxr-x   0 jens      (1000) users      (100)   158695 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/dasm_asm_d64_rom.sh
+-rw-rw-r--   0 jens      (1000) users      (100)      708 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)   193697 2024-01-04 17:10:16.000000 dragonpyemulator-0.9.2/dragonpy/Dragon64/mem_info.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/
+-rw-rw-r--   0 jens      (1000) users      (100)     1876 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/Multicomp6809_rom.py
+-rwxrwxr-x   0 jens      (1000) users      (100)      761 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2017 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      443 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)      773 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2759 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Multicomp6809/periphery_Multicomp6809.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/Simple6809/
+-rwxrwxr-x   0 jens      (1000) users      (100)      232 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/Grant's 6809 computer.URL
+-rwxrwxr-x   0 jens      (1000) users      (100)      554 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)     2003 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/Simple6809_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/__init__.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     1547 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/asm_lst2py_unittest.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2490 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      741 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/machine.py
+-rwxrwxr-x   0 jens      (1000) users      (100)      923 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/make_mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)   233609 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3281 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/periphery_simple6809.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2365 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/Simple6809/reformat_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1470 2024-04-16 15:06:57.000000 dragonpyemulator-0.9.2/dragonpy/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      154 2024-04-16 14:33:11.000000 dragonpyemulator-0.9.2/dragonpy/__main__.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/cli_app/
+-rw-rw-r--   0 jens      (1000) users      (100)     1918 2024-04-16 14:50:30.000000 dragonpyemulator-0.9.2/dragonpy/cli_app/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      335 2024-04-16 14:50:16.000000 dragonpyemulator-0.9.2/dragonpy/cli_app/debug.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2074 2024-04-16 14:52:41.000000 dragonpyemulator-0.9.2/dragonpy/cli_app/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1610 2024-04-16 14:47:47.000000 dragonpyemulator-0.9.2/dragonpy/cli_app/roms.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/cli_dev/
+-rw-rw-r--   0 jens      (1000) users      (100)     2130 2024-04-16 15:00:59.000000 dragonpyemulator-0.9.2/dragonpy/cli_dev/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      961 2024-04-16 15:00:59.000000 dragonpyemulator-0.9.2/dragonpy/cli_dev/code_style.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2347 2024-04-16 15:14:02.000000 dragonpyemulator-0.9.2/dragonpy/cli_dev/packaging.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1513 2024-04-16 15:00:59.000000 dragonpyemulator-0.9.2/dragonpy/cli_dev/testing.py
+-rw-rw-r--   0 jens      (1000) users      (100)      799 2024-04-16 14:43:28.000000 dragonpyemulator-0.9.2/dragonpy/cli_dev/update_readme_history.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/components/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/components/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    13109 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/components/memory.py
+-rw-rw-r--   0 jens      (1000) users      (100)     9857 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/components/periphery.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6073 2023-03-07 07:18:07.000000 dragonpyemulator-0.9.2/dragonpy/components/rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1031 2024-04-16 14:35:03.000000 dragonpyemulator-0.9.2/dragonpy/constants.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/core/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/core/__init__.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     1988 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/core/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3735 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/core/configs.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    16432 2024-02-09 14:57:10.000000 dragonpyemulator-0.9.2/dragonpy/core/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7715 2023-11-03 06:50:57.000000 dragonpyemulator-0.9.2/dragonpy/core/gui_starter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6447 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/core/machine.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.583957 dragonpyemulator-0.9.2/dragonpy/sbc09/
+-rw-rw-r--   0 jens      (1000) users      (100)     2167 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/README.creole
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1676 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5818 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/create_trace.py
+-rw-rw-r--   0 jens      (1000) users      (100)      439 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)      687 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/machine.py
+-rwxrwxr-x   0 jens      (1000) users      (100)   142429 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/make_mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)    28291 2023-03-06 19:35:23.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4174 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/periphery.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    29929 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/sbc09.creole
+-rw-rw-r--   0 jens      (1000) users      (100)      712 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/sbc09_rom.py
+-rw-rw-r--   0 jens      (1000) users      (100)    32768 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/sbc09/v09.rom
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/dragonpy/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)     1249 2024-04-16 14:35:03.000000 dragonpyemulator-0.9.2/dragonpy/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1324 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/tests/project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3209 2023-11-03 06:55:37.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_BASIC_Dragon32.py
+-rw-rw-r--   0 jens      (1000) users      (100)    25042 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_BASIC_simple09.py
+-rw-rw-r--   0 jens      (1000) users      (100)    15796 2023-03-07 16:21:59.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_base.py
+-rw-rw-r--   0 jens      (1000) users      (100)      749 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      280 2024-04-16 14:35:03.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1446 2024-04-16 15:00:59.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2172 2024-04-16 15:01:50.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)      772 2024-04-16 15:02:19.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_readme_history.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1601 2023-03-07 16:22:09.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_rom_download.py
+-rw-rw-r--   0 jens      (1000) users      (100)     6708 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/tests/test_sbc09.py
+-rw-rw-r--   0 jens      (1000) users      (100)      402 2023-03-07 15:36:28.000000 dragonpyemulator-0.9.2/dragonpy/tests/utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/dragonpy/utils/
+-rw-rw-r--   0 jens      (1000) users      (100)     4104 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/BASIC09_floating_point.py
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3214 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/bits.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1271 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/disable_logging.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     2321 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/hex2bin.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2341 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/humanize.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    17555 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/pager.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2121 2024-02-09 14:57:10.000000 dragonpyemulator-0.9.2/dragonpy/utils/simple_debugger.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     5553 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/utils/srecord_utils.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/dragonpy/vectrex/
+-rwxrwxr-x   0 jens      (1000) users      (100)    10241 2023-03-06 19:37:43.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/MOS6522.py
+-rw-rw-r--   0 jens      (1000) users      (100)     8192 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/SYSTEM.IMG
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1746 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/config.py
+-rw-rw-r--   0 jens      (1000) users      (100)      750 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/machine.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2429 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/mem_info.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1725 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/periphery.py
+-rw-rw-r--   0 jens      (1000) users      (100)      367 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/vectrex_gui.py
+-rw-rw-r--   0 jens      (1000) users      (100)      717 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/dragonpy/vectrex/vectrex_rom.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/misc/
+-rw-rw-r--   0 jens      (1000) users      (100)    11745 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/misc/README.creole
+-rwxrwxr-x   0 jens      (1000) users      (100)     5407 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/misc/add_info_in_trace.py
+-rwxrwxr-x   0 jens      (1000) users      (100)    10558 2023-03-06 18:48:22.000000 dragonpyemulator-0.9.2/misc/filter_xroar_trace.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2210 2024-02-09 14:57:10.000000 dragonpyemulator-0.9.2/misc/xroar_gdb_tests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5355 2024-04-16 15:00:31.000000 dragonpyemulator-0.9.2/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    67628 2024-04-16 14:57:40.000000 dragonpyemulator-0.9.2/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)    33290 2024-04-16 14:57:18.000000 dragonpyemulator-0.9.2/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2024-04-16 15:15:03.587957 dragonpyemulator-0.9.2/setup.cfg
```

### Comparing `DragonPyEmulator-0.9.1/.github/workflows/tests.yml` & `dragonpyemulator-0.9.2/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,32 +13,29 @@
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.12", "3.11", "3.10", "3.9"]
-    env:
-      PYTHONUNBUFFERED: 1
-      PYTHONWARNINGS: always
     steps:
     - name: Checkout
       run: |
         echo $GITHUB_REF $GITHUB_SHA
         git clone https://github.com/$GITHUB_REPOSITORY.git .
         git fetch origin $GITHUB_SHA:temporary-ci-branch
         git checkout $GITHUB_SHA || (git fetch && git checkout $GITHUB_SHA)
 
     - name: 'Set up Python ${{ matrix.python-version }}'
       uses: actions/setup-python@v4
       # https://github.com/marketplace/actions/setup-python
       with:
         python-version: '${{ matrix.python-version }}'
         cache: 'pip' # caching pip dependencies
-        cache-dependency-path: '**/requirements.dev.txt'
+        cache-dependency-path: '**/requirements.*.txt'
 
     - name: Cache ROMs
       id: cache-roms
       uses: actions/cache@v3
       # https://github.com/marketplace/actions/cache
       with:
         path: roms
@@ -67,14 +64,17 @@
         ./cli.py download-roms
 
     - name: 'Safety'
       run: |
         ./dev-cli.py safety
 
     - name: 'Run tests with Python v${{ matrix.python-version }}'
+      env:
+        PYTHONUNBUFFERED: 1
+        PYTHONWARNINGS: always
       run: |
         ./dev-cli.py coverage
 
     - name: 'Upload coverage report'
       uses: codecov/codecov-action@v3
       # https://github.com/marketplace/actions/codecov
       with:
```

### Comparing `DragonPyEmulator-0.9.1/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh` & `dragonpyemulator-0.9.2/.tox/py310/lib/python3.10/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh` & `dragonpyemulator-0.9.2/.tox/py311/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/activate.sh` & `dragonpyemulator-0.9.2/.tox/py39/lib/python3.9/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/.venv/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh` & `dragonpyemulator-0.9.2/.venv/lib/python3.11/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/.venv/lib64/python3.11/site-packages/virtualenv/activation/bash/activate.sh` & `dragonpyemulator-0.9.2/.venv/lib64/python3.11/site-packages/virtualenv/activation/bash/activate.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/AUTHORS` & `dragonpyemulator-0.9.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC examples/DumpBasicProgram.bas` & `dragonpyemulator-0.9.2/BASIC examples/DumpBasicProgram.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC examples/ListVariables.bas` & `dragonpyemulator-0.9.2/BASIC examples/ListVariables.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC examples/hex_view01.bas` & `dragonpyemulator-0.9.2/BASIC examples/hex_view01.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC examples/hustle.c10.bas` & `dragonpyemulator-0.9.2/BASIC examples/hustle.c10.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC examples/mandelbrot2.bas` & `dragonpyemulator-0.9.2/BASIC examples/mandelbrot2.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC games/INVADER.bas` & `dragonpyemulator-0.9.2/BASIC games/INVADER.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/FloatingPoint/test_FPA0.bas` & `dragonpyemulator-0.9.2/BASIC tools/FloatingPoint/test_FPA0.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/FloatingPoint/test_FPA0_02.bas` & `dragonpyemulator-0.9.2/BASIC tools/FloatingPoint/test_FPA0_02.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/HexViewer/hex_view01.bas` & `dragonpyemulator-0.9.2/BASIC tools/HexViewer/hex_view01.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/InputOutput/keyboard.bas` & `dragonpyemulator-0.9.2/BASIC tools/InputOutput/keyboard.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/README.creole` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_ADDA.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_ADDA.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_DEC.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_DEC.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_INC.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_INC.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_LSL.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_LSL.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_NEGA.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_NEGA.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_SUBA.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_SUBA.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/BASIC tools/TestCC_Registers/testCC_TST.bas` & `dragonpyemulator-0.9.2/BASIC tools/TestCC_Registers/testCC_TST.bas`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/PKG-INFO` & `dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: DragonPyEmulator
-Version: 0.9.1
+Version: 0.9.2
 Summary: Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python...
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/DragonPy
 Project-URL: Source, https://github.com/jedie/DragonPy
 Keywords: Emulator,6809,Dragon,CoCo,Vectrex,tkinter,pypy
-Requires-Python: <4,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: MC6809
 Requires-Dist: dragonlib
 Requires-Dist: cli-base-utilities
 Requires-Dist: manageprojects
 Requires-Dist: pygments
 Requires-Dist: bx_py_utils
 Requires-Dist: click
 Requires-Dist: rich-click
 Requires-Dist: rich
 Provides-Extra: dev
+Requires-Dist: manageprojects; extra == "dev"
+Requires-Dist: urllib3; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: pyupgrade; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-bugbear; extra == "dev"
 Requires-Dist: pyflakes; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Requires-Dist: EditorConfig; extra == "dev"
 Requires-Dist: safety; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: twine; extra == "dev"
+Requires-Dist: typeguard; extra == "dev"
 Requires-Dist: darker[color,flynt,isort]; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 
 ## Dragon/CoCO emulator written in Python
 
 DragonPy is a Open source (GPL v3 or later) emulator for the old (1981) homecomputer `Dragon 32` and `Tandy TRS-80 Color Computer` (CoCo)...
 
@@ -140,39 +144,38 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ download-roms              Download/Test only ROM files                                          │
-│ editor                     Run only the BASIC editor                                             │
-│ gui                        Start the DragonPy tkinter starter GUI                                │
-│ log-list                   List all exiting loggers and exit.                                    │
-│ run                        Run a machine emulation                                               │
-│ version                    Print version and exit                                                │
+│ download-roms       Download/Test only ROM files                                                 │
+│ editor              Run only the BASIC editor                                                    │
+│ gui                 <<< **start this** - Start the DragonPy tkinter starter GUI                  │
+│ log-list            List all exiting loggers and exit.                                           │
+│ run                 Run a machine emulation                                                      │
+│ version             Print version and exit                                                       │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 The output of `./cli.py run --help` looks like:
 
 [comment]: <> (✂✂✂ auto generated run help start ✂✂✂)
 ```
 Usage: ./cli.py run [OPTIONS]
 
  Run a machine emulation
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --verbosity           [1|10|20|30|40|50|99|100]            1:hardcode DEBUG ;), 10:DEBUG,        │
-│                                                            20:INFO, 30:WARNING, 40:ERROR,        │
-│                                                            50:CRITICAL/FATAL, 99:nearly all off, │
-│                                                            100:all off                           │
-│                                                            [default: 100]                        │
+│ --verbosity           INTEGER RANGE [0<=x<=3]              Verbosity level; Accepts integer      │
+│                                                            value e.g.: "--verbose 2" or can be   │
+│                                                            count e.g.: "-vv"                     │
+│                                                            [default: 0; 0<=x<=3]                 │
 │ --trace/--no-trace                                         Create trace lines                    │
 │                                                            [default: no-trace]                   │
 │ --max-ops             INTEGER                              If given: Stop CPU after given cycles │
 │                                                            else: run forever                     │
 │ --machine             [CoCo2b|Dragon32|Dragon64|Multicomp  Used machine configuration            │
 │                       6809|Simple6809|Vectrex|sbc09]       [default: Dragon32]                   │
 │ --help                                                     Show this message and exit.           │
@@ -215,23 +218,24 @@
 Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
-│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
+│ coverage                    Run tests and show coverage report.                                  │
+│ fix-code-style              Fix code style of all cli_base source code files via darker          │
+│ install                     Run pip-sync and install 'cli_base' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ publish                     Build and upload this project to PyPi                                │
 │ safety                      Run safety check against current requirements files                  │
 │ test                        Run unittests                                                        │
 │ tox                         Run tox                                                              │
 │ update                      Update "requirements*.txt" dependencies files                        │
+│ update-readme-history       Update project history base on git commits/tags in README.md         │
 │ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
 
@@ -499,14 +503,22 @@
 * Create release
 
 
 ## History
 
 [comment]: <> (✂✂✂ auto generated history start ✂✂✂)
 
+* [v0.9.2](https://github.com/jedie/DragonPy/compare/v0.9.1...v0.9.2)
+  * 2024-04-16 - Bugfix packaging
+  * 2024-04-16 - Update requirements and apply manageproject updates
+  * 2024-02-09 - Update requirements
+  * 2024-01-16 - Update requirements + fix code style
+  * 2023-12-17 - Fix code style and typos
+  * 2023-12-17 - Don't slow down tests because of mass DEBUG log output
+  * 2023-12-17 - Apply manageprojects updates
 * [v0.9.1](https://github.com/jedie/DragonPy/compare/v0.9.0...v0.9.1)
   * 2023-11-03 - Fix CI
   * 2023-11-03 - Apply manageprojects updates
   * 2023-11-03 - fix test_tokens_in_string()
   * 2023-11-03 - Auto generate README history
   * 2023-11-03 - Use https://github.com/jedie/cli-base-utilities
   * 2023-11-02 - Bump pip from 23.2.1 to 23.3
@@ -540,14 +552,17 @@
   * 2022-01-30 - update utils.py
   * 2022-01-30 - fix format
   * 2022-01-30 - fix meta config stuff
   * 2022-01-30 - Refacotor "download_roms" from old CLI into a dev-shell command
   * 2022-01-30 - remove nose test from CLI
   * 2022-01-30 - Use dev-shell
   * 2022-01-30 - Cache pip+roms
+
+<details><summary>Expand older history entries ...</summary>
+
 * [v0.7.0](https://github.com/jedie/DragonPy/compare/v0.6.0...v0.7.0)
   * 2020-10-01 - update README
   * 2020-10-01 - Update windows tk work-a-round: https://github.com/pypa/virtualenv/issues/93
   * 2020-10-01 - update vectrex
   * 2020-10-01 - Bugfix "--max_ops" cli options
   * 2020-10-01 - Update ROM download URLs for CoCo2b, Multicomp6809 and Simple6809
   * 2020-10-01 - Update Dragon 32/64 ROM download urls
@@ -562,17 +577,14 @@
   * 2020-02-10 - Update pythonapp.yml
   * 2020-02-10 - apply pyupgrate + code style
   * 2020-02-10 - apply code style
   * 2020-02-10 - fixup! remove bootstrap files
   * 2020-02-10 - run 2to3 and make minimal updates to get the tests running and pass
   * 2020-02-10 - remove bootstrap files
   * 2020-02-10 - WIP: modernize project setup
-
-<details><summary>Expand older history entries ...</summary>
-
 * [v0.6.0](https://github.com/jedie/DragonPy/compare/v0.5.3...v0.6.0)
   * 2018-06-19 - Fix "No module named 'nose'" on normal PyPi installation
   * 2018-06-19 - +build.log
   * 2018-06-19 - https://pypi.python.org/pypi/ -> https://pypi.org/project/
   * 2018-06-19 - +python-creole
   * 2018-06-19 - +twine
   * 2018-06-19 - update setup.py publish code
```

### Comparing `DragonPyEmulator-0.9.1/DragonPyEmulator.egg-info/SOURCES.txt` & `dragonpyemulator-0.9.2/DragonPyEmulator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,23 @@
 dragonpy/Simple6809/asm_lst2py_unittest.py
 dragonpy/Simple6809/config.py
 dragonpy/Simple6809/machine.py
 dragonpy/Simple6809/make_mem_info.py
 dragonpy/Simple6809/mem_info.py
 dragonpy/Simple6809/periphery_simple6809.py
 dragonpy/Simple6809/reformat_rom.py
-dragonpy/cli/__init__.py
-dragonpy/cli/cli_app.py
-dragonpy/cli/dev.py
+dragonpy/cli_app/__init__.py
+dragonpy/cli_app/debug.py
+dragonpy/cli_app/gui.py
+dragonpy/cli_app/roms.py
+dragonpy/cli_dev/__init__.py
+dragonpy/cli_dev/code_style.py
+dragonpy/cli_dev/packaging.py
+dragonpy/cli_dev/testing.py
+dragonpy/cli_dev/update_readme_history.py
 dragonpy/components/__init__.py
 dragonpy/components/memory.py
 dragonpy/components/periphery.py
 dragonpy/components/rom.py
 dragonpy/core/__init__.py
 dragonpy/core/cli.py
 dragonpy/core/configs.py
```

### Comparing `DragonPyEmulator-0.9.1/LICENSE` & `dragonpyemulator-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PKG-INFO` & `dragonpyemulator-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: DragonPyEmulator
-Version: 0.9.1
+Version: 0.9.2
 Summary: Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python...
 Author-email: Jens Diemer <git@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/DragonPy
 Project-URL: Source, https://github.com/jedie/DragonPy
 Keywords: Emulator,6809,Dragon,CoCo,Vectrex,tkinter,pypy
-Requires-Python: <4,>=3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: MC6809
 Requires-Dist: dragonlib
 Requires-Dist: cli-base-utilities
 Requires-Dist: manageprojects
 Requires-Dist: pygments
 Requires-Dist: bx_py_utils
 Requires-Dist: click
 Requires-Dist: rich-click
 Requires-Dist: rich
 Provides-Extra: dev
+Requires-Dist: manageprojects; extra == "dev"
+Requires-Dist: urllib3; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: autopep8; extra == "dev"
 Requires-Dist: pyupgrade; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-bugbear; extra == "dev"
 Requires-Dist: pyflakes; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Requires-Dist: EditorConfig; extra == "dev"
 Requires-Dist: safety; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: twine; extra == "dev"
+Requires-Dist: typeguard; extra == "dev"
 Requires-Dist: darker[color,flynt,isort]; extra == "dev"
 Requires-Dist: tomli; extra == "dev"
 
 ## Dragon/CoCO emulator written in Python
 
 DragonPy is a Open source (GPL v3 or later) emulator for the old (1981) homecomputer `Dragon 32` and `Tandy TRS-80 Color Computer` (CoCo)...
 
@@ -140,39 +144,38 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ download-roms              Download/Test only ROM files                                          │
-│ editor                     Run only the BASIC editor                                             │
-│ gui                        Start the DragonPy tkinter starter GUI                                │
-│ log-list                   List all exiting loggers and exit.                                    │
-│ run                        Run a machine emulation                                               │
-│ version                    Print version and exit                                                │
+│ download-roms       Download/Test only ROM files                                                 │
+│ editor              Run only the BASIC editor                                                    │
+│ gui                 <<< **start this** - Start the DragonPy tkinter starter GUI                  │
+│ log-list            List all exiting loggers and exit.                                           │
+│ run                 Run a machine emulation                                                      │
+│ version             Print version and exit                                                       │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 The output of `./cli.py run --help` looks like:
 
 [comment]: <> (✂✂✂ auto generated run help start ✂✂✂)
 ```
 Usage: ./cli.py run [OPTIONS]
 
  Run a machine emulation
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --verbosity           [1|10|20|30|40|50|99|100]            1:hardcode DEBUG ;), 10:DEBUG,        │
-│                                                            20:INFO, 30:WARNING, 40:ERROR,        │
-│                                                            50:CRITICAL/FATAL, 99:nearly all off, │
-│                                                            100:all off                           │
-│                                                            [default: 100]                        │
+│ --verbosity           INTEGER RANGE [0<=x<=3]              Verbosity level; Accepts integer      │
+│                                                            value e.g.: "--verbose 2" or can be   │
+│                                                            count e.g.: "-vv"                     │
+│                                                            [default: 0; 0<=x<=3]                 │
 │ --trace/--no-trace                                         Create trace lines                    │
 │                                                            [default: no-trace]                   │
 │ --max-ops             INTEGER                              If given: Stop CPU after given cycles │
 │                                                            else: run forever                     │
 │ --machine             [CoCo2b|Dragon32|Dragon64|Multicomp  Used machine configuration            │
 │                       6809|Simple6809|Vectrex|sbc09]       [default: Dragon32]                   │
 │ --help                                                     Show this message and exit.           │
@@ -215,23 +218,24 @@
 Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
-│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
+│ coverage                    Run tests and show coverage report.                                  │
+│ fix-code-style              Fix code style of all cli_base source code files via darker          │
+│ install                     Run pip-sync and install 'cli_base' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ publish                     Build and upload this project to PyPi                                │
 │ safety                      Run safety check against current requirements files                  │
 │ test                        Run unittests                                                        │
 │ tox                         Run tox                                                              │
 │ update                      Update "requirements*.txt" dependencies files                        │
+│ update-readme-history       Update project history base on git commits/tags in README.md         │
 │ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
 
@@ -499,14 +503,22 @@
 * Create release
 
 
 ## History
 
 [comment]: <> (✂✂✂ auto generated history start ✂✂✂)
 
+* [v0.9.2](https://github.com/jedie/DragonPy/compare/v0.9.1...v0.9.2)
+  * 2024-04-16 - Bugfix packaging
+  * 2024-04-16 - Update requirements and apply manageproject updates
+  * 2024-02-09 - Update requirements
+  * 2024-01-16 - Update requirements + fix code style
+  * 2023-12-17 - Fix code style and typos
+  * 2023-12-17 - Don't slow down tests because of mass DEBUG log output
+  * 2023-12-17 - Apply manageprojects updates
 * [v0.9.1](https://github.com/jedie/DragonPy/compare/v0.9.0...v0.9.1)
   * 2023-11-03 - Fix CI
   * 2023-11-03 - Apply manageprojects updates
   * 2023-11-03 - fix test_tokens_in_string()
   * 2023-11-03 - Auto generate README history
   * 2023-11-03 - Use https://github.com/jedie/cli-base-utilities
   * 2023-11-02 - Bump pip from 23.2.1 to 23.3
@@ -540,14 +552,17 @@
   * 2022-01-30 - update utils.py
   * 2022-01-30 - fix format
   * 2022-01-30 - fix meta config stuff
   * 2022-01-30 - Refacotor "download_roms" from old CLI into a dev-shell command
   * 2022-01-30 - remove nose test from CLI
   * 2022-01-30 - Use dev-shell
   * 2022-01-30 - Cache pip+roms
+
+<details><summary>Expand older history entries ...</summary>
+
 * [v0.7.0](https://github.com/jedie/DragonPy/compare/v0.6.0...v0.7.0)
   * 2020-10-01 - update README
   * 2020-10-01 - Update windows tk work-a-round: https://github.com/pypa/virtualenv/issues/93
   * 2020-10-01 - update vectrex
   * 2020-10-01 - Bugfix "--max_ops" cli options
   * 2020-10-01 - Update ROM download URLs for CoCo2b, Multicomp6809 and Simple6809
   * 2020-10-01 - Update Dragon 32/64 ROM download urls
@@ -562,17 +577,14 @@
   * 2020-02-10 - Update pythonapp.yml
   * 2020-02-10 - apply pyupgrate + code style
   * 2020-02-10 - apply code style
   * 2020-02-10 - fixup! remove bootstrap files
   * 2020-02-10 - run 2to3 and make minimal updates to get the tests running and pass
   * 2020-02-10 - remove bootstrap files
   * 2020-02-10 - WIP: modernize project setup
-
-<details><summary>Expand older history entries ...</summary>
-
 * [v0.6.0](https://github.com/jedie/DragonPy/compare/v0.5.3...v0.6.0)
   * 2018-06-19 - Fix "No module named 'nose'" on normal PyPi installation
   * 2018-06-19 - +build.log
   * 2018-06-19 - https://pypi.python.org/pypi/ -> https://pypi.org/project/
   * 2018-06-19 - +python-creole
   * 2018-06-19 - +twine
   * 2018-06-19 - update setup.py publish code
```

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/CassetteObjects.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/CassetteObjects.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/__init__.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/__init__.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/base_cli.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/base_cli.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/basic_tokens.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/basic_tokens.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/bitstream_handler.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/bitstream_handler.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/configs.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/configs.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/tests.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/tests.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/utils.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,20 +64,20 @@
     if t < 1:
         return f"{round(t * 1000, 1):.1f} ms"
     if t < 60:
         return f"{round(t, 1):.1f} sec"
     if t < 60 * 60:
         return f"{round(t / 60, 1):.1f} min"
 
-    for seconds, name in chunks:
+    for seconds, _name in chunks:
         count = t / seconds
         if count >= 1:
             count = round(count, 1)
             break
-    return f"{count:.1f} {name}"
+    return f"{count:.1f} {_name}"
 
 
 class ProcessInfo:
     """
     >>> p = ProcessInfo(100)
     >>> p.update(1)[0]
     99
@@ -154,15 +154,15 @@
             values = []
     if values:
         yield list(values)
 
 
 def iter_window(g, window_size):
     """
-    interate over 'g' bit-by-bit and yield a window with the given 'window_size' width.
+    iterate over 'g' bit-by-bit and yield a window with the given 'window_size' width.
 
     >>> for v in iter_window([1,2,3,4], window_size=2): v
     [1, 2]
     [2, 3]
     [3, 4]
     >>> for v in iter_window([1,2,3,4,5], window_size=3): v
     [1, 2, 3]
@@ -256,20 +256,20 @@
 def count_the_same(iterable, sentinel):
     """
     >>> count_the_same([0x55,0x55,0x55,0x55,0x3C,"foo","bar"],0x55)
     (4, 60)
     >>> 0x3C == 60
     True
     """
-    count = 0
+    _count = 0
     x = None
-    for count, x in enumerate(iterable):
+    for _count, x in enumerate(iterable):
         if x != sentinel:
             break
-    return count, x
+    return _count, x
 
 
 def diff_info(data):
     """
     >>> diff_info([5,5,10,10,5,5,10,10])
     (0, 15)
     >>> diff_info([5,10,10,5,5,10,10,5])
@@ -728,15 +728,15 @@
         yield y
 
 
 def sinus_values_by_hz(framerate, hz, max_value):
     """
     Create sinus values with the given framerate and Hz.
     Note:
-    We skip the first zero-crossing, so the values can be used directy in a loop.
+    We skip the first zero-crossing, so the values can be used directly in a loop.
 
     >>> values = sinus_values_by_hz(22050, 1200, 255)
     >>> len(values) # 22050 / 1200Hz = 18,375
     18
     >>> values
     (87, 164, 221, 251, 251, 221, 164, 87, 0, -87, -164, -221, -251, -251, -221, -164, -87, 0)
```

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC/wave2bitstream.py` & `dragonpyemulator-0.9.2/PyDC/PyDC/wave2bitstream.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/PyDC_cli.py` & `dragonpyemulator-0.9.2/PyDC/PyDC_cli.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/README.creole` & `dragonpyemulator-0.9.2/PyDC/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/test_files/HelloWorld1 origin.wav` & `dragonpyemulator-0.9.2/PyDC/test_files/HelloWorld1 origin.wav`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/test_files/HelloWorld1 xroar.wav` & `dragonpyemulator-0.9.2/PyDC/test_files/HelloWorld1 xroar.wav`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/test_files/LineNumber Test 01.wav` & `dragonpyemulator-0.9.2/PyDC/test_files/LineNumber Test 01.wav`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/PyDC/test_files/LineNumber Test 02.wav` & `dragonpyemulator-0.9.2/PyDC/test_files/LineNumber Test 02.wav`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/README.md` & `dragonpyemulator-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,39 +102,38 @@
 ```
 Usage: ./cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
-│ download-roms              Download/Test only ROM files                                          │
-│ editor                     Run only the BASIC editor                                             │
-│ gui                        Start the DragonPy tkinter starter GUI                                │
-│ log-list                   List all exiting loggers and exit.                                    │
-│ run                        Run a machine emulation                                               │
-│ version                    Print version and exit                                                │
+│ download-roms       Download/Test only ROM files                                                 │
+│ editor              Run only the BASIC editor                                                    │
+│ gui                 <<< **start this** - Start the DragonPy tkinter starter GUI                  │
+│ log-list            List all exiting loggers and exit.                                           │
+│ run                 Run a machine emulation                                                      │
+│ version             Print version and exit                                                       │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated main help end ✂✂✂)
 
 
 The output of `./cli.py run --help` looks like:
 
 [comment]: <> (✂✂✂ auto generated run help start ✂✂✂)
 ```
 Usage: ./cli.py run [OPTIONS]
 
  Run a machine emulation
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
-│ --verbosity           [1|10|20|30|40|50|99|100]            1:hardcode DEBUG ;), 10:DEBUG,        │
-│                                                            20:INFO, 30:WARNING, 40:ERROR,        │
-│                                                            50:CRITICAL/FATAL, 99:nearly all off, │
-│                                                            100:all off                           │
-│                                                            [default: 100]                        │
+│ --verbosity           INTEGER RANGE [0<=x<=3]              Verbosity level; Accepts integer      │
+│                                                            value e.g.: "--verbose 2" or can be   │
+│                                                            count e.g.: "-vv"                     │
+│                                                            [default: 0; 0<=x<=3]                 │
 │ --trace/--no-trace                                         Create trace lines                    │
 │                                                            [default: no-trace]                   │
 │ --max-ops             INTEGER                              If given: Stop CPU after given cycles │
 │                                                            else: run forever                     │
 │ --machine             [CoCo2b|Dragon32|Dragon64|Multicomp  Used machine configuration            │
 │                       6809|Simple6809|Vectrex|sbc09]       [default: Dragon32]                   │
 │ --help                                                     Show this message and exit.           │
@@ -177,23 +176,24 @@
 Usage: ./dev-cli.py [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --help      Show this message and exit.                                                          │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────╮
 │ check-code-style            Check code style by calling darker + flake8                          │
-│ coverage                    Run and show coverage.                                               │
-│ fix-code-style              Fix code style of all dragonpy source code files via darker          │
-│ install                     Run pip-sync and install 'dragonpy' via pip as editable.             │
+│ coverage                    Run tests and show coverage report.                                  │
+│ fix-code-style              Fix code style of all cli_base source code files via darker          │
+│ install                     Run pip-sync and install 'cli_base' via pip as editable.             │
 │ mypy                        Run Mypy (configured in pyproject.toml)                              │
 │ publish                     Build and upload this project to PyPi                                │
 │ safety                      Run safety check against current requirements files                  │
 │ test                        Run unittests                                                        │
 │ tox                         Run tox                                                              │
 │ update                      Update "requirements*.txt" dependencies files                        │
+│ update-readme-history       Update project history base on git commits/tags in README.md         │
 │ update-test-snapshot-files  Update all test snapshot files (by remove and recreate all snapshot  │
 │                             files)                                                               │
 │ version                     Print version and exit                                               │
 ╰──────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 [comment]: <> (✂✂✂ auto generated dev help end ✂✂✂)
 
@@ -461,14 +461,22 @@
 * Create release
 
 
 ## History
 
 [comment]: <> (✂✂✂ auto generated history start ✂✂✂)
 
+* [v0.9.2](https://github.com/jedie/DragonPy/compare/v0.9.1...v0.9.2)
+  * 2024-04-16 - Bugfix packaging
+  * 2024-04-16 - Update requirements and apply manageproject updates
+  * 2024-02-09 - Update requirements
+  * 2024-01-16 - Update requirements + fix code style
+  * 2023-12-17 - Fix code style and typos
+  * 2023-12-17 - Don't slow down tests because of mass DEBUG log output
+  * 2023-12-17 - Apply manageprojects updates
 * [v0.9.1](https://github.com/jedie/DragonPy/compare/v0.9.0...v0.9.1)
   * 2023-11-03 - Fix CI
   * 2023-11-03 - Apply manageprojects updates
   * 2023-11-03 - fix test_tokens_in_string()
   * 2023-11-03 - Auto generate README history
   * 2023-11-03 - Use https://github.com/jedie/cli-base-utilities
   * 2023-11-02 - Bump pip from 23.2.1 to 23.3
@@ -502,14 +510,17 @@
   * 2022-01-30 - update utils.py
   * 2022-01-30 - fix format
   * 2022-01-30 - fix meta config stuff
   * 2022-01-30 - Refacotor "download_roms" from old CLI into a dev-shell command
   * 2022-01-30 - remove nose test from CLI
   * 2022-01-30 - Use dev-shell
   * 2022-01-30 - Cache pip+roms
+
+<details><summary>Expand older history entries ...</summary>
+
 * [v0.7.0](https://github.com/jedie/DragonPy/compare/v0.6.0...v0.7.0)
   * 2020-10-01 - update README
   * 2020-10-01 - Update windows tk work-a-round: https://github.com/pypa/virtualenv/issues/93
   * 2020-10-01 - update vectrex
   * 2020-10-01 - Bugfix "--max_ops" cli options
   * 2020-10-01 - Update ROM download URLs for CoCo2b, Multicomp6809 and Simple6809
   * 2020-10-01 - Update Dragon 32/64 ROM download urls
@@ -524,17 +535,14 @@
   * 2020-02-10 - Update pythonapp.yml
   * 2020-02-10 - apply pyupgrate + code style
   * 2020-02-10 - apply code style
   * 2020-02-10 - fixup! remove bootstrap files
   * 2020-02-10 - run 2to3 and make minimal updates to get the tests running and pass
   * 2020-02-10 - remove bootstrap files
   * 2020-02-10 - WIP: modernize project setup
-
-<details><summary>Expand older history entries ...</summary>
-
 * [v0.6.0](https://github.com/jedie/DragonPy/compare/v0.5.3...v0.6.0)
   * 2018-06-19 - Fix "No module named 'nose'" on normal PyPi installation
   * 2018-06-19 - +build.log
   * 2018-06-19 - https://pypi.python.org/pypi/ -> https://pypi.org/project/
   * 2018-06-19 - +python-creole
   * 2018-06-19 - +twine
   * 2018-06-19 - update setup.py publish code
```

### Comparing `DragonPyEmulator-0.9.1/basic_editor/editor.py` & `dragonpyemulator-0.9.2/basic_editor/editor.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/basic_editor/editor_base.py` & `dragonpyemulator-0.9.2/basic_editor/editor_base.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/basic_editor/highlighting.py` & `dragonpyemulator-0.9.2/basic_editor/highlighting.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/basic_editor/scrolled_text.py` & `dragonpyemulator-0.9.2/basic_editor/scrolled_text.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/basic_editor/status_bar.py` & `dragonpyemulator-0.9.2/basic_editor/status_bar.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/basic_editor/tkinter_utils.py` & `dragonpyemulator-0.9.2/basic_editor/tkinter_utils.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/basic_editor/token_window.py` & `dragonpyemulator-0.9.2/basic_editor/token_window.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/cli.py` & `dragonpyemulator-0.9.2/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     bootstrap CLI
     ~~~~~~~~~~~~~
 
     Just call this file, and the magic happens ;)
 """
 
 import hashlib
+import shlex
 import subprocess
 import sys
 import venv
 from pathlib import Path
 
 
 def print_no_pip_error():
@@ -28,15 +29,15 @@
     raise
 else:
     if not version():
         print_no_pip_error()
         sys.exit(-1)
 
 
-assert sys.version_info >= (3, 9), 'Python version is too old!'
+assert sys.version_info >= (3, 9), f'Python version {sys.version_info} is too old!'
 
 
 if sys.platform == 'win32':  # wtf
     # Files under Windows, e.g.: .../.venv/Scripts/python.exe
     BIN_NAME = 'Scripts'
     FILE_EXT = '.exe'
 else:
@@ -73,15 +74,15 @@
     """Is existing .venv is up-to-date?"""
     if DEP_HASH_PATH.is_file():
         return DEP_HASH_PATH.read_text() == get_dep_hash()
     return False
 
 
 def verbose_check_call(*popen_args):
-    print(f'\n+ {" ".join(str(arg) for arg in popen_args)}\n')
+    print(f'\n+ {shlex.join(str(arg) for arg in popen_args)}\n')
     return subprocess.check_call(popen_args)
 
 
 def main(argv):
     assert DEP_LOCK_PATH.is_file(), f'File not found: "{DEP_LOCK_PATH}" !'
 
     # Create virtual env in ".venv/":
```

### Comparing `DragonPyEmulator-0.9.1/dev-cli.py` & `dragonpyemulator-0.9.2/dev-cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     bootstrap CLI
     ~~~~~~~~~~~~~
 
     Just call this file, and the magic happens ;)
 """
 
 import hashlib
+import shlex
 import subprocess
 import sys
 import venv
 from pathlib import Path
 
 
 def print_no_pip_error():
@@ -28,15 +29,15 @@
     raise
 else:
     if not version():
         print_no_pip_error()
         sys.exit(-1)
 
 
-assert sys.version_info >= (3, 9), 'Python version is too old!'
+assert sys.version_info >= (3, 9), f'Python version {sys.version_info} is too old!'
 
 
 if sys.platform == 'win32':  # wtf
     # Files under Windows, e.g.: .../.venv/Scripts/python.exe
     BIN_NAME = 'Scripts'
     FILE_EXT = '.exe'
 else:
@@ -73,15 +74,15 @@
     """Is existing .venv is up-to-date?"""
     if DEP_HASH_PATH.is_file():
         return DEP_HASH_PATH.read_text() == get_dep_hash()
     return False
 
 
 def verbose_check_call(*popen_args):
-    print(f'\n+ {" ".join(str(arg) for arg in popen_args)}\n')
+    print(f'\n+ {shlex.join(str(arg) for arg in popen_args)}\n')
     return subprocess.check_call(popen_args)
 
 
 def main(argv):
     assert DEP_LOCK_PATH.is_file(), f'File not found: "{DEP_LOCK_PATH}" !'
 
     # Create virtual env in ".venv/":
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/CoCo/CoCo2b_rom.py` & `dragonpyemulator-0.9.2/dragonpy/CoCo/CoCo2b_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/CoCo/config.py` & `dragonpyemulator-0.9.2/dragonpy/CoCo/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/CoCo/machine.py` & `dragonpyemulator-0.9.2/dragonpy/CoCo/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/CoCo/mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/CoCo/mem_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,13 +64,13 @@
     #         if s == e:
     #             addr = nice_hex(s)
     #         else:
     #             addr = "%s-%s" % (nice_hex(s), nice_hex(e))
     #
     #         print "%-11s ; %s" % (addr, txt)
 
-    for start_addr, end_addr, comment in Dragon64MemInfo.MEM_INFO:
+    for start_addr, _end_addr, comment in Dragon64MemInfo.MEM_INFO:
         comment = comment.replace('"', '\\"')
         comment = comment.replace('$', '\\$')
         print(f'\tcomment=0x{start_addr:x},"{comment}" \\')
 
     print("\n --- END --- \n")
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/CoCo/periphery_coco.py` & `dragonpyemulator-0.9.2/dragonpy/CoCo/periphery_coco.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/Dragon32_rom.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/Dragon32_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/MC6821_PIA.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/MC6821_PIA.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/MC6847.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/MC6847.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/MC6883_SAM.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/MC6883_SAM.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/cassette.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/cassette.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/config.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/dragon_charmap.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/dragon_charmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,17 +201,17 @@
         DRAGON_CHARS_MAP.append(
             (item, item_type)
         )
 
 
 def list_chars():
     index = 0
-    for x in range(8):
+    for _x in range(8):
         line = ""
-        for y in range(32):
+        for _y in range(32):
             try:
                 line += DRAGON_CHARS_MAP[index][0]
             except KeyError:
                 break
             index += 1
         print(line.encode("utf-8"))
 
@@ -287,10 +287,9 @@
     create_dict()
 
     print()
     print("=" * 79)
     print()
 
     import doctest
-    print(doctest.testmod(
-        verbose=1
-    ))
+
+    print(doctest.testmod(verbose=True))
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/dragon_font.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/dragon_font.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/gui_config.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/gui_config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/keyboard_map.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/keyboard_map.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/machine.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/periphery_dragon.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/periphery_dragon.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon32/speaker.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon32/speaker.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/6809dasm_comments.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/6809dasm_comments.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,23 @@
             start_addr = self.eval_addr(start_addr_raw)
             if end_addr_raw:
                 end_addr = self.eval_addr(end_addr_raw)
             else:
                 end_addr = start_addr
 
             rom_info.append(
-                (start_addr, end_addr, comment.strip())
+                (start_addr, end_addr, comment.strip()),
             )
         sys.stderr.write(
-            f"ROM Info file: {rom_info_file.name!r} readed.\n"
+            f"ROM Info file: {rom_info_file.name!r} read.\n",
         )
         return rom_info
 
     def create_comments(self, outfile):
-        for start_addr, end_addr, comment in self.mem_info:
+        for start_addr, _end_addr, comment in self.mem_info:
             comment = comment.replace('"', '\\"')
             comment = comment.replace('$', '\\$')
             outfile.write(
                 f'\tcomment=0x{start_addr:x},"{comment}" \\\n'
             )
 #            outfile.write(
 #                '\tlabel="%s",0x%x \\\n' % (comment, start_addr)
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/Dragon 64 in 32 mode.txt` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/Dragon 64 in 32 mode.txt`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/Dragon64_rom.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/Dragon64_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/config.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/create_mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/create_mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/dasm_asm_d64_rom.sh` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/dasm_asm_d64_rom.sh`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/machine.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Dragon64/mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/Dragon64/mem_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,25 +745,25 @@
         (0x89c1, 0x89c1, "get varptr of variable in X"),
         (0x89c6, 0x89c6, "numeric / string flag"),
         (0x89c8, 0x89c8, "RTS (string)"),
         (0x89ca, 0x89ca, "load variable into FPA1 (X is varptr)"),
         (0x89cd, 0x8a03, "evaluate function"),
         (0x89cd, 0x89cd, "get next character from BASIC source"),
         (0x89d2, 0x89d2, "get next character from BASIC source"),
-        (0x89d8, 0x89d8, "disk function despatch"),
+        (0x89d8, 0x89d8, "disk function dispatch"),
         (0x89e0, 0x89e0, "functions with single arguments"),
         (0x89e4, 0x89e4, "functions with special or no arguments"),
         (0x89e6, 0x89e6, "skip open bracket"),
         (0x89ec, 0x89ec, "not LEFT$, RIGHT$ or MID$"),
         (0x89ee, 0x89ee, "get expression"),
         (0x89f1, 0x89f1, "skip comma"),
         (0x89f3, 0x89f3, "validate string"),
         (0x89fc, 0x89fc, "get number into B"),
         (0x8a06, 0x8a0e, "(8A04 8D99       BSR   $899F)   ;get expression inside brackets"),
-        (0x8a08, 0x8a08, "function despatch table"),
+        (0x8a08, 0x8a08, "function dispatch table"),
         (0x8a0e, 0x8a0e, "validate numeric expression"),
         (0x8a11, 0x8a11, "OR"),
         (0x8a13, 0x8a2e, "AND"),
         (0x8a13, 0x8a2e, "(8A12 4F         CLRA)"),
         (0x8a15, 0x8a15, "read signed number from FPA1 to $52 & D"),
         (0x8a1a, 0x8a1a, "copy FPA2 to FPA1"),
         (0x8a1d, 0x8a1d, "read signed number from FPA1 to $52 & D"),
@@ -1614,15 +1614,15 @@
         (0x9a85, 0x9a85, "RTS"),
         (0x9a8b, 0x9a8b, "output character to DEVN"),
         (0x9a8e, 0x9a96, "EDIT: test for search functions"),
         (0x9a8e, 0x9a8e, "(K = wipe chrs until nth occurrence of chr)"),
         (0x9a92, 0x9a92, "(S = search for nth occurrence of chr)"),
         (0x9a97, 0x9ab7, "EDIT: search functions"),
         (0x9a99, 0x9a99, "read keys (carry clear if control key)"),
-        (0x9a9f, 0x9a9f, "PULS Y,PC"),
+        (0x9a9f, 0x9a9f, "PLUS Y,PC"),
         (0x9aa3, 0x9aa3, "Kill (not Search)"),
         (0x9aa5, 0x9aa5, "output character to DEVN"),
         (0x9aab, 0x9aab, "close line up over removed character"),
         (0x9ab2, 0x9ab2, "not found"),
         (0x9ab5, 0x9ab5, "find next occurrence"),
         (0x9ab9, 0x9ad8, "read keys (carry clear if control key)"),
         (0x9ab9, 0x9ab9, "read character from DEVN & strip MSB"),
@@ -2904,15 +2904,15 @@
         (0xb415, 0xb415, "set up PLAY & graphics variables"),
         (0xb418, 0xb418, "set up USR vectors"),
         (0xb41b, 0xb41b, "address of USR table"),
         (0xb41d, 0xb41d, "?FC ERROR"),
         (0xb427, 0xb427, "PCLEAR 4"),
         (0xb42f, 0xb42f, "enable vsync irq"),
         (0xb432, 0xb432, "check for 'DK' disk"),
-        (0xb435, 0xb435, "cartridge sigature"),
+        (0xb435, 0xb435, "cartridge signature"),
         (0xb43c, 0xb43c, "enable interrupts"),
         (0xb441, 0xb441, "display copyright message"),
         (0xb444, 0xb444, "set up soft reset vector"),
         (0xb447, 0xb447, "soft reset vector"),
         (0xb44b, 0xb44b, "cold boot flag"),
         (0xb44d, 0xb44d, "(JMP $8371 - command mode)"),
         (0xb44f, 0xb466, "normal soft reset routine"),
@@ -2923,15 +2923,15 @@
         (0xb461, 0xb461, "enable interrupts"),
         (0xb463, 0xb463, "clear screen"),
         (0xb466, 0xb466, "command mode"),
         (0xb469, 0xb47d, "FIRQ service routine"),
         (0xb46c, 0xb46c, "cartridge"),
         (0xb46f, 0xb46f, "delay"),
         (0xb47b, 0xb47b, "cold boot flag"),
-        (0xb480, 0xb486, "delay before starting FIRQ cartrige"),
+        (0xb480, 0xb486, "delay before starting FIRQ cartridge"),
         (0xb480, 0xb480, "zero"),
         (0xb487, 0x7ebb, "copied to $9d - $aa on start up"),
         (0xb487, 0x7ebb, "(default EXEC & get character routine)"),
         (0xb495, 0xb4a9, "copied to $10c - $129 on start up"),
         (0xb495, 0xb4a9, "(IRQ, FIRQ, RND seeds, key delay, command addresses)"),
         (0xb4b3, 0xb503, "copyright message"),
         (0xb505, 0xb509, "read 7 bit character from device DEVN"),
@@ -3157,15 +3157,15 @@
         (0xb793, 0xb793, "text cursor address"),
         (0xb796, 0xb7a7, "INKEY$"),
         (0xb796, 0xb796, "last key pressed"),
         (0xb798, 0xb798, "key ready"),
         (0xb79a, 0xb79a, "scan keyboard"),
         (0xb79d, 0xb79d, "last key pressed"),
         (0xb7a1, 0xb7a1, "set up character & put on varptr stack"),
-        (0xb7a7, 0xb7a7, "leas 2,s & put temp string on varptr stack"),
+        (0xb7a7, 0xb7a7, "lease 2,s & put temp string on varptr stack"),
         (0xb7aa, 0xb7c9, "called by get filename routine"),
         (0xb7aa, 0xb7c9, "(reads filename from command into usual location)"),
         (0xb7b3, 0xb7b3, "IO buffer"),
         (0xb7b8, 0xb7b8, "get current character from BASIC source"),
         (0xb7ba, 0xb7ba, "RTS"),
         (0xb7bc, 0xb7bc, "get expression"),
         (0xb7bf, 0xb7bf, "validate string & point X to it (len in B)"),
@@ -3781,13 +3781,13 @@
     #         if s == e:
     #             addr = nice_hex(s)
     #         else:
     #             addr = "%s-%s" % (nice_hex(s), nice_hex(e))
     #
     #         print "%-11s ; %s" % (addr, txt)
 
-    for start_addr, end_addr, comment in Dragon64MemInfo.MEM_INFO:
+    for start_addr, _end_addr, comment in Dragon64MemInfo.MEM_INFO:
         comment = comment.replace('"', '\\"')
         comment = comment.replace('$', '\\$')
         print(f'\tcomment=0x{start_addr:x},"{comment}" \\')
 
     print("\n --- END --- \n")
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/Multicomp6809_rom.py` & `dragonpyemulator-0.9.2/dragonpy/Multicomp6809/Multicomp6809_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/README.creole` & `dragonpyemulator-0.9.2/dragonpy/Multicomp6809/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/config.py` & `dragonpyemulator-0.9.2/dragonpy/Multicomp6809/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/machine.py` & `dragonpyemulator-0.9.2/dragonpy/Multicomp6809/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Multicomp6809/periphery_Multicomp6809.py` & `dragonpyemulator-0.9.2/dragonpy/Multicomp6809/periphery_Multicomp6809.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/README.creole` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/Simple6809_rom.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/Simple6809_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/asm_lst2py_unittest.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/asm_lst2py_unittest.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/config.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/machine.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/make_mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/make_mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/periphery_simple6809.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/periphery_simple6809.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/Simple6809/reformat_rom.py` & `dragonpyemulator-0.9.2/dragonpy/Simple6809/reformat_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/__init__.py` & `dragonpyemulator-0.9.2/dragonpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from dragonpy.sbc09.machine import run_sbc09
 from dragonpy.Simple6809.config import Simple6809Cfg
 from dragonpy.Simple6809.machine import run_Simple6809
 from dragonpy.vectrex.config import VectrexCfg
 from dragonpy.vectrex.machine import run_Vectrex
 
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __author__ = 'Jens Diemer <git@jensdiemer.de>'
 
 
 machine_dict.register(constants.DRAGON32, (run_Dragon32, Dragon32Cfg), default=True)
 machine_dict.register(constants.DRAGON64, (run_Dragon64, Dragon64Cfg))
 machine_dict.register(constants.COCO2B, (run_CoCo2b, CoCo2bCfg))
 machine_dict.register(constants.SBC09, (run_sbc09, SBC09Cfg))
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/components/memory.py` & `dragonpyemulator-0.9.2/dragonpy/components/memory.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/components/periphery.py` & `dragonpyemulator-0.9.2/dragonpy/components/periphery.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/components/rom.py` & `dragonpyemulator-0.9.2/dragonpy/components/rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/core/cli.py` & `dragonpyemulator-0.9.2/dragonpy/core/cli.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/core/configs.py` & `dragonpyemulator-0.9.2/dragonpy/core/configs.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/core/gui.py` & `dragonpyemulator-0.9.2/dragonpy/core/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,16 @@
                             "https://github.com/jedie/DragonPy#readme"
                             )
 
     def exit(self):
         log.critical("DragonTkinterGUI.exit()")
         try:
             self.root.destroy()
-        except BaseException:
-            pass
+        except Exception as err:
+            log.exception(f'destroy error: {err}')
 
     # -----------------------------------------------------------------------------------------
 
     def close_config(self):
         self.config_window.root.destroy()
         self.config_window = None
 
@@ -251,18 +251,15 @@
         self.machine.cpu.max_burst_count = self.runtime_cfg.max_burst_count
 
         new_cycles = self.machine.cpu.cycles - self.last_cpu_cycles
         duration = time.time() - self.last_update
 
         cycles_per_sec = new_cycles / duration
 
-        msg = (
-            "%s cylces/sec (burst op count: outer: %s - inner: %s)\n"
-            "%i CPU interval calls"
-        ) % (
+        msg = ("%s cycles/sec (burst op count: outer: %s - inner: %s)\n" "%i CPU interval calls") % (
             locale_format_number(cycles_per_sec),
 
             locale_format_number(self.machine.cpu.outer_burst_op_count),
             locale_format_number(self.machine.cpu.inner_burst_op_count),
 
             self.cpu_interval_calls,
         )
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/core/gui_starter.py` & `dragonpyemulator-0.9.2/dragonpy/core/gui_starter.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/core/machine.py` & `dragonpyemulator-0.9.2/dragonpy/core/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/README.creole` & `dragonpyemulator-0.9.2/dragonpy/sbc09/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/config.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/create_trace.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/create_trace.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/machine.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/make_mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/make_mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/periphery.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/periphery.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/sbc09.creole` & `dragonpyemulator-0.9.2/dragonpy/sbc09/sbc09.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/sbc09_rom.py` & `dragonpyemulator-0.9.2/dragonpy/sbc09/sbc09_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/sbc09/v09.rom` & `dragonpyemulator-0.9.2/dragonpy/sbc09/v09.rom`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/project_setup.py` & `dragonpyemulator-0.9.2/dragonpy/tests/project_setup.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_BASIC_Dragon32.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_BASIC_Dragon32.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_BASIC_simple09.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_BASIC_simple09.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_base.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_config.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_readme.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from bx_py_utils.auto_doc import assert_readme_block
 from bx_py_utils.path import assert_is_file
 from manageprojects.test_utils.click_cli_utils import invoke_click
 from manageprojects.tests.base import BaseTestCase
 
 from dragonpy import constants
-from dragonpy.cli.cli_app import PACKAGE_ROOT, cli
-from dragonpy.cli.dev import cli as dev_cli
+from dragonpy.cli_app import cli
+from dragonpy.cli_dev import PACKAGE_ROOT
+from dragonpy.cli_dev import cli as dev_cli
 
 
 def assert_cli_help_in_readme(text_block: str, marker: str):
     README_PATH = PACKAGE_ROOT / 'README.md'
     assert_is_file(README_PATH)
 
     text_block = text_block.replace(constants.CLI_EPILOG, '')
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_readme_history.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_readme_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest import TestCase
 
 from bx_py_utils.auto_doc import assert_readme_block
 from cli_base.cli_tools.git_history import get_git_history
 
 import dragonpy
-from dragonpy.cli.cli_app import PACKAGE_ROOT
+from dragonpy.cli_dev import PACKAGE_ROOT
 
 
 class ReadmeHistoryTestCase(TestCase):
     def test_readme_history(self):
         git_history = get_git_history(
             current_version=dragonpy.__version__,
             add_author=False,
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_rom_download.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_rom_download.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/tests/test_sbc09.py` & `dragonpyemulator-0.9.2/dragonpy/tests/test_sbc09.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/BASIC09_floating_point.py` & `dragonpyemulator-0.9.2/dragonpy/utils/BASIC09_floating_point.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/bits.py` & `dragonpyemulator-0.9.2/dragonpy/utils/bits.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/disable_logging.py` & `dragonpyemulator-0.9.2/dragonpy/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/hex2bin.py` & `dragonpyemulator-0.9.2/dragonpy/utils/hex2bin.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/humanize.py` & `dragonpyemulator-0.9.2/dragonpy/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/pager.py` & `dragonpyemulator-0.9.2/dragonpy/utils/pager.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/simple_debugger.py` & `dragonpyemulator-0.9.2/dragonpy/utils/simple_debugger.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,9 +73,9 @@
                 value = repr(value)
 
             if len(value) > MAX_CHARS:
                 value = f"{value[:MAX_CHARS]}..."
 
             try:
                 click.echo(value)
-            except BaseException:
+            except BaseException:  # noqa: B036
                 click.echo("<ERROR WHILE PRINTING VALUE>")
```

### Comparing `DragonPyEmulator-0.9.1/dragonpy/utils/srecord_utils.py` & `dragonpyemulator-0.9.2/dragonpy/utils/srecord_utils.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/MOS6522.py` & `dragonpyemulator-0.9.2/dragonpy/vectrex/MOS6522.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/SYSTEM.IMG` & `dragonpyemulator-0.9.2/dragonpy/vectrex/SYSTEM.IMG`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/config.py` & `dragonpyemulator-0.9.2/dragonpy/vectrex/config.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/machine.py` & `dragonpyemulator-0.9.2/dragonpy/vectrex/machine.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/mem_info.py` & `dragonpyemulator-0.9.2/dragonpy/vectrex/mem_info.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/periphery.py` & `dragonpyemulator-0.9.2/dragonpy/vectrex/periphery.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/dragonpy/vectrex/vectrex_rom.py` & `dragonpyemulator-0.9.2/dragonpy/vectrex/vectrex_rom.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/misc/README.creole` & `dragonpyemulator-0.9.2/misc/README.creole`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/misc/add_info_in_trace.py` & `dragonpyemulator-0.9.2/misc/add_info_in_trace.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/misc/filter_xroar_trace.py` & `dragonpyemulator-0.9.2/misc/filter_xroar_trace.py`

 * *Files identical despite different names*

### Comparing `DragonPyEmulator-0.9.1/misc/xroar_gdb_tests.py` & `dragonpyemulator-0.9.2/misc/xroar_gdb_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,12 +83,12 @@
         xroar_gdb.send("g")
         time.sleep(1)
     finally:
         print("tear down")
         try:
             xroar_gdb.running = False
             xroar_gdb.s.close()
-        except BaseException:
+        except BaseException:  # noqa: B036
             pass
 
     time.sleep(1)
     print(" --- END --- ")
```

### Comparing `DragonPyEmulator-0.9.1/pyproject.toml` & `dragonpyemulator-0.9.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,40 +4,44 @@
 description = "Emulator for 6809 CPU based system like Dragon 32 / CoCo written in Python..."
 keywords=["Emulator","6809","Dragon","CoCo","Vectrex","tkinter","pypy"]
 license = {text = "GPL-3.0-or-later"}
 readme = "README.md"
 authors = [
     {name = 'Jens Diemer', email = 'git@jensdiemer.de'}
 ]
-requires-python = ">=3.9,<4"
+requires-python = ">=3.9"
 dependencies = [
     "MC6809",  # https://github.com/6809/MC6809
     "dragonlib",  # https://github.com/6809/dragonlib
     "cli-base-utilities",  # https://github.com/jedie/cli-base-utilities
     "manageprojects",  # https://github.com/jedie/manageprojects
     "pygments",  # https://pygments.org/
     "bx_py_utils",  # https://github.com/boxine/bx_py_utils
     "click",  # https://github.com/pallets/click/
     "rich-click",  # https://github.com/ewels/rich-click
     "rich",  # https://github.com/Textualize/rich
 ]
 [project.optional-dependencies]
 dev = [
+    "manageprojects",  # https://github.com/jedie/manageprojects
+    "urllib3", # for bx_py_utils.test_utils.deny_requests.deny_any_real_request() in tests
     "pip-tools",  # https://github.com/jazzband/pip-tools/
     "tox",  # https://github.com/tox-dev/tox
     "coverage",  # https://github.com/nedbat/coveragepy
     "autopep8",  # https://github.com/hhatto/autopep8
     "pyupgrade",  # https://github.com/asottile/pyupgrade
     "flake8",  # https://github.com/pycqa/flake8
+    "flake8-bugbear",  # https://github.com/PyCQA/flake8-bugbear
     "pyflakes",  # https://github.com/PyCQA/pyflakes
     "codespell",  # https://github.com/codespell-project/codespell
     "EditorConfig",  # https://github.com/editorconfig/editorconfig-core-py
     "safety",  # https://github.com/pyupio/safety
     "mypy",  # https://github.com/python/mypy
     "twine",  # https://github.com/pypa/twine
+    "typeguard",  # https://github.com/agronholm/typeguard/
 
     # https://github.com/akaihola/darker
     # https://github.com/ikamensh/flynt
     # https://github.com/pycqa/isort
     # https://github.com/pygments/pygments
     "darker[flynt, isort, color]",
 
@@ -50,15 +54,19 @@
 
 [project.urls]
 Documentation = "https://github.com/jedie/DragonPy"
 Source = "https://github.com/jedie/DragonPy"
 
 [project.scripts]
 dragonpy_app = "dragonpy.__main__:main"
-dragonpy_dev = "dragonpy.cli.dev:main"
+dragonpy_dev = "dragonpy.cli_dev:main"
+
+[tool.cli_base]
+version_module_name = "dragonpy"
+
 
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm>=7.1"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
@@ -68,22 +76,20 @@
 version = {attr = "dragonpy.__version__"}
 
 
 [tool.darker]
 src = ['.']
 revision = "origin/main..."
 line_length = 119
-verbose = true
 color = true
 skip_string_normalization = true
 diff = false
 check = false
 stdout = false
 isort = true
-flynt = true
 lint = [
     "flake8",
 ]
 log_level = "INFO"
 
 
 [tool.isort]
@@ -127,17 +133,14 @@
 passenv = *
 skip_install = true
 commands_pre =
     pip install -U pip-tools
     pip-sync requirements.dev.txt
 commands =
     {envpython} -m coverage run --context='{envname}'
-    {envpython} -m coverage combine --append
-    {envpython} -m coverage xml
-    {envpython} -m coverage report
 """
 
 
 [tool.mypy]
 warn_unused_configs = true
 ignore_missing_imports = true
 allow_redefinition = true  # https://github.com/python/mypy/issues/7165
@@ -147,14 +150,17 @@
 
 
 [manageprojects] # https://github.com/jedie/manageprojects
 initial_revision = "47cac0a"
 initial_date = 2023-03-06T19:46:41+01:00
 cookiecutter_template = "https://github.com/jedie/cookiecutter_templates/"
 cookiecutter_directory = "piptools-python"
+applied_migrations = [
+    "765b8fb", # 2024-03-12T09:08:01+01:00
+]
 
 [manageprojects.cookiecutter_context.cookiecutter]
 full_name = "Jens Diemer"
 github_username = "jedie"
 author_email = "git@jensdiemer.de"
 package_name = "dragonpy"
 package_version = "0.7.0"
@@ -163,8 +169,9 @@
 issues_url = "https://github.com/jedie/DragonPy/issues"
 license = "GPL-3.0-or-later"
 _template = "https://github.com/jedie/cookiecutter_templates/"
 applied_migrations = [
     "04d5a25", # 2023-03-07T16:25:36+01:00
     "da054d6", # 2023-08-04T17:39:02+02:00
     "c1a9d97", # 2023-11-01T19:59:17+01:00
+    "fd79154", # 2023-12-17T13:42:30+01:00
 ]
```

### Comparing `DragonPyEmulator-0.9.1/requirements.dev.txt` & `dragonpyemulator-0.9.2/requirements.dev.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,97 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    ./cli.py update
+#    ./dev-cli.py update
 #
+annotated-types==0.6.0 \
+    --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
+    --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
+    # via pydantic
 arrow==1.3.0 \
     --hash=sha256:c728b120ebc00eb84e01882a6f5e7927a53960aa990ce7dd2b10f39005a67f80 \
     --hash=sha256:d4540617648cb5f895730f1ad8c82a65f2dad0166f57b75f3ca54759c4d67a85
     # via cookiecutter
 astor==0.8.1 \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
     --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
     # via flynt
-autoflake==2.2.1 \
-    --hash=sha256:265cde0a43c1f44ecfb4f30d95b0437796759d07be7706a2f70e4719234c0f79 \
-    --hash=sha256:62b7b6449a692c3c9b0c916919bbc21648da7281e8506bcf8d3f8280e431ebc1
+async-timeout==4.0.3 \
+    --hash=sha256:4640d96be84d82d02ed59ea2b7105a0f7b33abe8703703cd0ab0bf87c427522f \
+    --hash=sha256:7405140ff1230c310e51dc27b3145b9092d659ce68ff733fb0cefe3ee42be028
+    # via cli-base-utilities
+attrs==23.2.0 \
+    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
+    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
+    # via flake8-bugbear
+authlib==1.3.0 \
+    --hash=sha256:959ea62a5b7b5123c5059758296122b57cd2585ae2ed1c0622c21b371ffdae06 \
+    --hash=sha256:9637e4de1fb498310a56900b3e2043a206b03cb11c05422014b0302cbc814be3
+    # via safety
+autoflake==2.3.1 \
+    --hash=sha256:3ae7495db9084b7b32818b4140e6dc4fc280b712fb414f5b8fe57b0a8e85a840 \
+    --hash=sha256:c98b75dc5b0a86459c4f01a1d32ac7eb4338ec4317a4469515ff1e687ecd909e
     # via manageprojects
-autopep8==2.0.4 \
-    --hash=sha256:067959ca4a07b24dbd5345efa8325f5f58da4298dab0dde0443d5ed765de80cb \
-    --hash=sha256:2913064abd97b3419d1cc83ea71f042cb821f87e45b9c88cad5ad3c4ea87fe0c
+autopep8==2.1.0 \
+    --hash=sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7 \
+    --hash=sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
+backports-tarfile==1.1.0 \
+    --hash=sha256:91d59138ea401ee2a95e8b839c1e2f51f3e9ca76bdba8b6a29f8d773564686a8 \
+    --hash=sha256:b2f4df351db942d094db94588bbf2c6938697a5f190f44c934acc697da56008b
+    # via jaraco-context
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-black==23.10.1 \
-    --hash=sha256:037e9b4664cafda5f025a1728c50a9e9aedb99a759c89f760bd83730e76ba884 \
-    --hash=sha256:1b917a2aa020ca600483a7b340c165970b26e9029067f019e3755b56e8dd5916 \
-    --hash=sha256:1f8ce316753428ff68749c65a5f7844631aa18c8679dfd3ca9dc1a289979c258 \
-    --hash=sha256:33d40f5b06be80c1bbce17b173cda17994fbad096ce60eb22054da021bf933d1 \
-    --hash=sha256:3f157a8945a7b2d424da3335f7ace89c14a3b0625e6593d21139c2d8214d55ce \
-    --hash=sha256:5ed45ac9a613fb52dad3b61c8dea2ec9510bf3108d4db88422bacc7d1ba1243d \
-    --hash=sha256:6d23d7822140e3fef190734216cefb262521789367fbdc0b3f22af6744058982 \
-    --hash=sha256:7670242e90dc129c539e9ca17665e39a146a761e681805c54fbd86015c7c84f7 \
-    --hash=sha256:7b4d10b0f016616a0d93d24a448100adf1699712fb7a4efd0e2c32bbb219b173 \
-    --hash=sha256:7cb5936e686e782fddb1c73f8aa6f459e1ad38a6a7b0e54b403f1f05a1507ee9 \
-    --hash=sha256:7d56124b7a61d092cb52cce34182a5280e160e6aff3137172a68c2c2c4b76bcb \
-    --hash=sha256:840015166dbdfbc47992871325799fd2dc0dcf9395e401ada6d88fe11498abad \
-    --hash=sha256:9c74de4c77b849e6359c6f01987e94873c707098322b91490d24296f66d067dc \
-    --hash=sha256:b15b75fc53a2fbcac8a87d3e20f69874d161beef13954747e053bca7a1ce53a0 \
-    --hash=sha256:cfcce6f0a384d0da692119f2d72d79ed07c7159879d0bb1bb32d2e443382bf3a \
-    --hash=sha256:d431e6739f727bb2e0495df64a6c7a5310758e87505f5f8cde9ff6c0f2d7e4fe \
-    --hash=sha256:e293e4c2f4a992b980032bbd62df07c1bcff82d6964d6c9496f2cd726e246ace \
-    --hash=sha256:ec3f8e6234c4e46ff9e16d9ae96f4ef69fa328bb4ad08198c8cee45bb1f08c69
+black==24.4.0 \
+    --hash=sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d \
+    --hash=sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd \
+    --hash=sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33 \
+    --hash=sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965 \
+    --hash=sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070 \
+    --hash=sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397 \
+    --hash=sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745 \
+    --hash=sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1 \
+    --hash=sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665 \
+    --hash=sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436 \
+    --hash=sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb \
+    --hash=sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e \
+    --hash=sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6 \
+    --hash=sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702 \
+    --hash=sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8 \
+    --hash=sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8 \
+    --hash=sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3 \
+    --hash=sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad \
+    --hash=sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf \
+    --hash=sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e \
+    --hash=sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641 \
+    --hash=sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2
     # via darker
-build==1.0.3 \
-    --hash=sha256:538aab1b64f9828977f84bc63ae570b060a8ed1be419e7870b8b4fc5e6ea553b \
-    --hash=sha256:589bf99a67df7c9cf07ec0ac0e5e2ea5d4b37ac63301c4986d1acb126aa83f8f
+build==1.2.1 \
+    --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
+    --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
     # via pip-tools
-bx-py-utils==88 \
-    --hash=sha256:32fbc7e9ff3dfb0a817c80fb1d165ec559643dab59c0be549e646acbf8223b75 \
-    --hash=sha256:3a6f4eeef6abcac834b2c1ea4c5211130fd930a064aa0baabddd7c2bd00e38ac
+bx-py-utils==92 \
+    --hash=sha256:38641b2e1a09ed0c64cd6ba0e03c97fea347302439db0234a0492c365ae32719 \
+    --hash=sha256:849c59429af6ca0bf35265569884193c60be578285a66b533146e5782a10637b
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   cli-base-utilities
     #   mc6809
-cachetools==5.3.2 \
-    --hash=sha256:086ee420196f7b2ab9ca2db2520aca326318b68fe5ba8bc4d49cca91add450f2 \
-    --hash=sha256:861f35a13a451f94e301ce2bec7cac63e881232ccce7ed67fab9b5df4d3beaa1
+cachetools==5.3.3 \
+    --hash=sha256:0abad1021d3f8325b2fc1d2e9c8b9c9d57b04c3932657a72465447332c24d945 \
+    --hash=sha256:ba29e2dfa0b8b556606f097407ed1aa62080ee108ab0dc5ec9d6a723a007d105
     # via tox
-certifi==2023.7.22 \
-    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
-    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
+certifi==2024.2.2 \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
     # via requests
 cffi==1.16.0 \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
@@ -213,421 +237,560 @@
     --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
     --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
     # via requests
-cli-base-utilities==0.4.4 \
-    --hash=sha256:110bef895fb7dfc29662f463ccedc4c985a880afbde2e6dea387d0d2f96f4985 \
-    --hash=sha256:72d4248776519a21c3448d6e348511ce6fe8c3742c154e158473236c8278fb1c
+cli-base-utilities==0.8.0 \
+    --hash=sha256:1009551eba81b33a0315c4fcfe3b6ef1633a99e303c9562dff39b824bff83ff0 \
+    --hash=sha256:79628db9fc7ca01b5ab18c97c8fa5f3d8b96af9975c608f7fee9a44256edb2ab
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
+    #   mc6809
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   black
     #   cli-base-utilities
     #   cookiecutter
     #   manageprojects
     #   mc6809
     #   pip-tools
     #   rich-click
     #   safety
+    #   typer
 codespell==2.2.6 \
     --hash=sha256:9ee9a3e5df0990604013ac2a9f22fa8e57669c827124a2e961fe8a1da4cacc07 \
     --hash=sha256:a8c65d8eb3faa03deabab6b3bbe798bea72e1799c7e9e955d57eca4096abcff9
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
-cookiecutter==2.4.0 \
-    --hash=sha256:6d1494e66a784f23324df9d593f3e43af3db4f4b926b9e49e6ff060169fc042a \
-    --hash=sha256:8344663028abc08ec09b912e663636a97e1775bffe973425ec0107431acd390e
+cookiecutter==2.6.0 \
+    --hash=sha256:a54a8e37995e4ed963b3e82831072d1ad4b005af736bb17b99c2cbd9d41b6e2d \
+    --hash=sha256:db21f8169ea4f4fdc2408d48ca44859349de2647fbe494a9d6c3edfc0542c21c
     # via manageprojects
-coverage==7.3.2 \
-    --hash=sha256:0cbf38419fb1a347aaf63481c00f0bdc86889d9fbf3f25109cf96c26b403fda1 \
-    --hash=sha256:12d15ab5833a997716d76f2ac1e4b4d536814fc213c85ca72756c19e5a6b3d63 \
-    --hash=sha256:149de1d2401ae4655c436a3dced6dd153f4c3309f599c3d4bd97ab172eaf02d9 \
-    --hash=sha256:1981f785239e4e39e6444c63a98da3a1db8e971cb9ceb50a945ba6296b43f312 \
-    --hash=sha256:2443cbda35df0d35dcfb9bf8f3c02c57c1d6111169e3c85fc1fcc05e0c9f39a3 \
-    --hash=sha256:289fe43bf45a575e3ab10b26d7b6f2ddb9ee2dba447499f5401cfb5ecb8196bb \
-    --hash=sha256:2f11cc3c967a09d3695d2a6f03fb3e6236622b93be7a4b5dc09166a861be6d25 \
-    --hash=sha256:307adb8bd3abe389a471e649038a71b4eb13bfd6b7dd9a129fa856f5c695cf92 \
-    --hash=sha256:310b3bb9c91ea66d59c53fa4989f57d2436e08f18fb2f421a1b0b6b8cc7fffda \
-    --hash=sha256:315a989e861031334d7bee1f9113c8770472db2ac484e5b8c3173428360a9148 \
-    --hash=sha256:3a4006916aa6fee7cd38db3bfc95aa9c54ebb4ffbfc47c677c8bba949ceba0a6 \
-    --hash=sha256:3c7bba973ebee5e56fe9251300c00f1579652587a9f4a5ed8404b15a0471f216 \
-    --hash=sha256:4175e10cc8dda0265653e8714b3174430b07c1dca8957f4966cbd6c2b1b8065a \
-    --hash=sha256:43668cabd5ca8258f5954f27a3aaf78757e6acf13c17604d89648ecc0cc66640 \
-    --hash=sha256:4cbae1051ab791debecc4a5dcc4a1ff45fc27b91b9aee165c8a27514dd160836 \
-    --hash=sha256:5c913b556a116b8d5f6ef834038ba983834d887d82187c8f73dec21049abd65c \
-    --hash=sha256:5f7363d3b6a1119ef05015959ca24a9afc0ea8a02c687fe7e2d557705375c01f \
-    --hash=sha256:630b13e3036e13c7adc480ca42fa7afc2a5d938081d28e20903cf7fd687872e2 \
-    --hash=sha256:72c0cfa5250f483181e677ebc97133ea1ab3eb68645e494775deb6a7f6f83901 \
-    --hash=sha256:7dbc3ed60e8659bc59b6b304b43ff9c3ed858da2839c78b804973f613d3e92ed \
-    --hash=sha256:88ed2c30a49ea81ea3b7f172e0269c182a44c236eb394718f976239892c0a27a \
-    --hash=sha256:89a937174104339e3a3ffcf9f446c00e3a806c28b1841c63edb2b369310fd074 \
-    --hash=sha256:9028a3871280110d6e1aa2df1afd5ef003bab5fb1ef421d6dc748ae1c8ef2ebc \
-    --hash=sha256:99b89d9f76070237975b315b3d5f4d6956ae354a4c92ac2388a5695516e47c84 \
-    --hash=sha256:9f805d62aec8eb92bab5b61c0f07329275b6f41c97d80e847b03eb894f38d083 \
-    --hash=sha256:a889ae02f43aa45032afe364c8ae84ad3c54828c2faa44f3bfcafecb5c96b02f \
-    --hash=sha256:aa72dbaf2c2068404b9870d93436e6d23addd8bbe9295f49cbca83f6e278179c \
-    --hash=sha256:ac8c802fa29843a72d32ec56d0ca792ad15a302b28ca6203389afe21f8fa062c \
-    --hash=sha256:ae97af89f0fbf373400970c0a21eef5aa941ffeed90aee43650b81f7d7f47637 \
-    --hash=sha256:af3d828d2c1cbae52d34bdbb22fcd94d1ce715d95f1a012354a75e5913f1bda2 \
-    --hash=sha256:b4275802d16882cf9c8b3d057a0839acb07ee9379fa2749eca54efbce1535b82 \
-    --hash=sha256:b4767da59464bb593c07afceaddea61b154136300881844768037fd5e859353f \
-    --hash=sha256:b631c92dfe601adf8f5ebc7fc13ced6bb6e9609b19d9a8cd59fa47c4186ad1ce \
-    --hash=sha256:be32ad29341b0170e795ca590e1c07e81fc061cb5b10c74ce7203491484404ef \
-    --hash=sha256:beaa5c1b4777f03fc63dfd2a6bd820f73f036bfb10e925fce067b00a340d0f3f \
-    --hash=sha256:c0ba320de3fb8c6ec16e0be17ee1d3d69adcda99406c43c0409cb5c41788a611 \
-    --hash=sha256:c9eacf273e885b02a0273bb3a2170f30e2d53a6d53b72dbe02d6701b5296101c \
-    --hash=sha256:cb536f0dcd14149425996821a168f6e269d7dcd2c273a8bff8201e79f5104e76 \
-    --hash=sha256:d1bc430677773397f64a5c88cb522ea43175ff16f8bfcc89d467d974cb2274f9 \
-    --hash=sha256:d1c88ec1a7ff4ebca0219f5b1ef863451d828cccf889c173e1253aa84b1e07ce \
-    --hash=sha256:d3d9df4051c4a7d13036524b66ecf7a7537d14c18a384043f30a303b146164e9 \
-    --hash=sha256:d51ac2a26f71da1b57f2dc81d0e108b6ab177e7d30e774db90675467c847bbdf \
-    --hash=sha256:d872145f3a3231a5f20fd48500274d7df222e291d90baa2026cc5152b7ce86bf \
-    --hash=sha256:d8f17966e861ff97305e0801134e69db33b143bbfb36436efb9cfff6ec7b2fd9 \
-    --hash=sha256:dbc1b46b92186cc8074fee9d9fbb97a9dd06c6cbbef391c2f59d80eabdf0faa6 \
-    --hash=sha256:e10c39c0452bf6e694511c901426d6b5ac005acc0f78ff265dbe36bf81f808a2 \
-    --hash=sha256:e267e9e2b574a176ddb983399dec325a80dbe161f1a32715c780b5d14b5f583a \
-    --hash=sha256:f47d39359e2c3779c5331fc740cf4bce6d9d680a7b4b4ead97056a0ae07cb49a \
-    --hash=sha256:f6e9589bd04d0461a417562649522575d8752904d35c12907d8c9dfeba588faf \
-    --hash=sha256:f94b734214ea6a36fe16e96a70d941af80ff3bfd716c141300d95ebc85339738 \
-    --hash=sha256:fa28e909776dc69efb6ed975a63691bc8172b64ff357e663a1bb06ff3c9b589a \
-    --hash=sha256:fe494faa90ce6381770746077243231e0b83ff3f17069d748f645617cefe19d4
+coverage==7.4.4 \
+    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
+    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
+    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
+    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
+    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
+    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
+    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
+    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
+    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
+    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
+    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
+    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
+    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
+    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
+    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
+    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
+    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
+    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
+    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
+    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
+    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
+    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
+    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
+    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
+    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
+    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
+    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
+    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
+    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
+    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
+    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
+    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
+    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
+    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
+    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
+    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
+    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
+    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
+    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
+    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
+    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
+    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
+    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
+    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
+    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
+    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
+    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
+    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
+    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
+    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
+    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
+    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
     # via DragonPyEmulator (pyproject.toml)
-cryptography==41.0.5 \
-    --hash=sha256:0c327cac00f082013c7c9fb6c46b7cc9fa3c288ca702c74773968173bda421bf \
-    --hash=sha256:0d2a6a598847c46e3e321a7aef8af1436f11c27f1254933746304ff014664d84 \
-    --hash=sha256:227ec057cd32a41c6651701abc0328135e472ed450f47c2766f23267b792a88e \
-    --hash=sha256:22892cc830d8b2c89ea60148227631bb96a7da0c1b722f2aac8824b1b7c0b6b8 \
-    --hash=sha256:392cb88b597247177172e02da6b7a63deeff1937fa6fec3bbf902ebd75d97ec7 \
-    --hash=sha256:3be3ca726e1572517d2bef99a818378bbcf7d7799d5372a46c79c29eb8d166c1 \
-    --hash=sha256:573eb7128cbca75f9157dcde974781209463ce56b5804983e11a1c462f0f4e88 \
-    --hash=sha256:580afc7b7216deeb87a098ef0674d6ee34ab55993140838b14c9b83312b37b86 \
-    --hash=sha256:5a70187954ba7292c7876734183e810b728b4f3965fbe571421cb2434d279179 \
-    --hash=sha256:73801ac9736741f220e20435f84ecec75ed70eda90f781a148f1bad546963d81 \
-    --hash=sha256:7d208c21e47940369accfc9e85f0de7693d9a5d843c2509b3846b2db170dfd20 \
-    --hash=sha256:8254962e6ba1f4d2090c44daf50a547cd5f0bf446dc658a8e5f8156cae0d8548 \
-    --hash=sha256:88417bff20162f635f24f849ab182b092697922088b477a7abd6664ddd82291d \
-    --hash=sha256:a48e74dad1fb349f3dc1d449ed88e0017d792997a7ad2ec9587ed17405667e6d \
-    --hash=sha256:b948e09fe5fb18517d99994184854ebd50b57248736fd4c720ad540560174ec5 \
-    --hash=sha256:c707f7afd813478e2019ae32a7c49cd932dd60ab2d2a93e796f68236b7e1fbf1 \
-    --hash=sha256:d38e6031e113b7421db1de0c1b1f7739564a88f1684c6b89234fbf6c11b75147 \
-    --hash=sha256:d3977f0e276f6f5bf245c403156673db103283266601405376f075c849a0b936 \
-    --hash=sha256:da6a0ff8f1016ccc7477e6339e1d50ce5f59b88905585f77193ebd5068f1e797 \
-    --hash=sha256:e270c04f4d9b5671ebcc792b3ba5d4488bf7c42c3c241a3748e2599776f29696 \
-    --hash=sha256:e886098619d3815e0ad5790c973afeee2c0e6e04b4da90b88e6bd06e2a0b1b72 \
-    --hash=sha256:ec3b055ff8f1dce8e6ef28f626e0972981475173d7973d63f271b29c8a2897da \
-    --hash=sha256:fba1e91467c65fe64a82c689dc6cf58151158993b13eb7a7f3f4b7f395636723
-    # via secretstorage
-darker[color,flynt,isort]==1.7.2 \
-    --hash=sha256:ec5b7c382d9537611c164f3ecca2e1b8a7923bc5a02bf22f6e7f6c8bcbdf593a \
-    --hash=sha256:ec9d130ab2a0f7fa49ab68a08fd231a5bec66147ecbbf94c92a1f33d97b5ef6f
+cryptography==42.0.5 \
+    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
+    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
+    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
+    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
+    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
+    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
+    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
+    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
+    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
+    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
+    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
+    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
+    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
+    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
+    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
+    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
+    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
+    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
+    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
+    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
+    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
+    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
+    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
+    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
+    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
+    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
+    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
+    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
+    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
+    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
+    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
+    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+    # via
+    #   authlib
+    #   secretstorage
+darker[color,flynt,isort]==2.1.1 \
+    --hash=sha256:a6e6a682c0604e76fe9aec7650e96a944f517563c69b28fcc076db9d957d98ea \
+    --hash=sha256:ead701414c45359fc0312bc285614d3285fc135476d43f3bc08d989ee19d9020
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
-distlib==0.3.7 \
-    --hash=sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057 \
-    --hash=sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8
+darkgraylib==1.2.0 \
+    --hash=sha256:1df3f35f3f7d2f944d506501c31d3fe145bad57cf4707c033b48083fba048d59 \
+    --hash=sha256:fefc821d5f88000aa36020f5fa35af64cbc7345f0a8f015edab7f37e3aec4997
+    # via
+    #   darker
+    #   graylint
+distlib==0.3.8 \
+    --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
+    --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
     # via virtualenv
-docutils==0.20.1 \
-    --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
-    --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
+docutils==0.21.1 \
+    --hash=sha256:14c8d34a55b46c88f9f714adb29cefbdd69fb82f3fef825e59c5faab935390d8 \
+    --hash=sha256:65249d8a5345bc95e0f40f280ba63c98eb24de35c6c8f5b662e3e8948adea83f
     # via readme-renderer
-dparse==0.6.3 \
-    --hash=sha256:0d8fe18714056ca632d98b24fbfc4e9791d4e47065285ab486182288813a5318 \
-    --hash=sha256:27bb8b4bcaefec3997697ba3f6e06b2447200ba273c0b085c3d012a04571b528
-    # via safety
+dparse==0.6.4b0 \
+    --hash=sha256:592ff183348b8a5ea0a18442a7965e29445d3a26063654ec2c7e8ef42cd5753c \
+    --hash=sha256:f8d49b41a527f3d16a269f854e6665245b325e50e41d2c213810cb984553e5c8
+    # via
+    #   safety
+    #   safety-schemas
 dragonlib==0.1.7 \
     --hash=sha256:1021c9bc4e62e39712f3fee7ddf454b0882168927dcee9a8dbc9fc50ff641b30 \
     --hash=sha256:89646eaa63b45185c5635387434bcf5a3bc6169502c1a19f8e47469d370ccf32
     # via DragonPyEmulator (pyproject.toml)
-editorconfig==0.12.3 \
-    --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
-    --hash=sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1
+editorconfig==0.12.4 \
+    --hash=sha256:24857fa1793917dd9ccf0c7810a07e05404ce9b823521c7dce22a4fb5d125f80
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
-filelock==3.13.1 \
-    --hash=sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e \
-    --hash=sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c
+filelock==3.13.4 \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
     # via
     #   tox
     #   virtualenv
-flake8==6.1.0 \
-    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
-    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
+flake8==7.0.0 \
+    --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
+    --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
+    # via
+    #   DragonPyEmulator (pyproject.toml)
+    #   flake8-bugbear
+    #   manageprojects
+flake8-bugbear==24.2.6 \
+    --hash=sha256:663ef5de80cd32aacd39d362212983bc4636435a6f83700b4ed35acbd0b7d1b8 \
+    --hash=sha256:f9cb5f2a9e792dd80ff68e89a14c12eed8620af8b41a49d823b7a33064ac9658
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
-flynt==0.77 \
-    --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
-    --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
+flynt==1.0.1 \
+    --hash=sha256:65d1c546434827275123222a98408e9561bcd67db832dd58f530ff17b8329ec1 \
+    --hash=sha256:988aac00672a5469726cc0a17cef7d1178c284a9fe8563458db2475d0aaed965
+    # via darker
+graylint==1.1.1 \
+    --hash=sha256:0fd8e02972ca03d0ef2bf0adea76b5343efcd492d7afb5f658f3e3a724f55a36 \
+    --hash=sha256:b7e0eab6c159684dbf5ef84e942c3340f6a6549b02a3d11b1a1763cc4f8f0593
     # via darker
-idna==3.4 \
-    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
-    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
-importlib-metadata==6.8.0 \
-    --hash=sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb \
-    --hash=sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743
+importlib-metadata==7.1.0 \
+    --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
+    --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
     # via
     #   keyring
     #   twine
-isort==5.12.0 \
-    --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
-    --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
+isort==5.13.2 \
+    --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
+    --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
     # via darker
-jaraco-classes==3.3.0 \
-    --hash=sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb \
-    --hash=sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621
+jaraco-classes==3.4.0 \
+    --hash=sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd \
+    --hash=sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790
+    # via keyring
+jaraco-context==5.3.0 \
+    --hash=sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266 \
+    --hash=sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2
+    # via keyring
+jaraco-functools==4.0.0 \
+    --hash=sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925 \
+    --hash=sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d
     # via keyring
 jeepney==0.8.0 \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.2 \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-    # via cookiecutter
-keyring==24.2.0 \
-    --hash=sha256:4901caaf597bfd3bbd78c9a0c7c4c29fcd8310dab2cffefe749e916b6527acd6 \
-    --hash=sha256:ca0746a19ec421219f4d713f848fa297a661a8a8c1504867e55bfb5e09091509
+jinja2==3.1.3 \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+    # via
+    #   cookiecutter
+    #   safety
+keyring==25.1.0 \
+    --hash=sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427 \
+    --hash=sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893
     # via twine
-manageprojects==0.15.2 \
-    --hash=sha256:44ac8973f9fede20693bd52c062d3b780268001f146100e6f3fc1bbaaa9ba720 \
-    --hash=sha256:f264f238e5f2998019e2a654103c28519110c47d509ba9652b77883148fe3c85
+manageprojects==0.17.1 \
+    --hash=sha256:355d970261f14b53b574d102e7e82462fe6769baa06c479f00f07a0bcfcb8e4d \
+    --hash=sha256:4662ff7f0e64ea9b420b67c270594c88542858a1434ebe8b5f93b7bf2ae2e706
     # via DragonPyEmulator (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
     # via rich
-markupsafe==2.1.3 \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
+markupsafe==2.1.5 \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
     # via jinja2
-mc6809==0.7.1 \
-    --hash=sha256:46b30c68dd000c82a20c57bb6e6322ac63b6414cecae7cf723fbfea29ebb2d06 \
-    --hash=sha256:d9d63dbba30a28e018906b0708df5101f9c643bb2b87f2825529d739eced9cc0
+marshmallow==3.21.1 \
+    --hash=sha256:4e65e9e0d80fc9e609574b9983cf32579f305c718afb30d7233ab818571768c3 \
+    --hash=sha256:f085493f79efb0644f270a9bf2892843142d80d7174bbbd2f3713f2a589dc633
+    # via safety
+mc6809==0.7.2 \
+    --hash=sha256:933f5405f261db30681efbc3810bdcae385349d4ff95865cf2f53f534606faa9 \
+    --hash=sha256:f7592dadaaa52a35fa2af2fa4e259e032ca89ccf86c481e55d6e63e89ca6ab38
     # via DragonPyEmulator (pyproject.toml)
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
     # via flake8
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
-more-itertools==10.1.0 \
-    --hash=sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a \
-    --hash=sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6
-    # via jaraco-classes
-mypy==1.6.1 \
-    --hash=sha256:19f905bcfd9e167159b3d63ecd8cb5e696151c3e59a1742e79bc3bcb540c42c7 \
-    --hash=sha256:21a1ad938fee7d2d96ca666c77b7c494c3c5bd88dff792220e1afbebb2925b5e \
-    --hash=sha256:40b1844d2e8b232ed92e50a4bd11c48d2daa351f9deee6c194b83bf03e418b0c \
-    --hash=sha256:41697773aa0bf53ff917aa077e2cde7aa50254f28750f9b88884acea38a16169 \
-    --hash=sha256:49ae115da099dcc0922a7a895c1eec82c1518109ea5c162ed50e3b3594c71208 \
-    --hash=sha256:4c46b51de523817a0045b150ed11b56f9fff55f12b9edd0f3ed35b15a2809de0 \
-    --hash=sha256:4cbe68ef919c28ea561165206a2dcb68591c50f3bcf777932323bc208d949cf1 \
-    --hash=sha256:4d01c00d09a0be62a4ca3f933e315455bde83f37f892ba4b08ce92f3cf44bcc1 \
-    --hash=sha256:59a0d7d24dfb26729e0a068639a6ce3500e31d6655df8557156c51c1cb874ce7 \
-    --hash=sha256:68351911e85145f582b5aa6cd9ad666c8958bcae897a1bfda8f4940472463c45 \
-    --hash=sha256:7274b0c57737bd3476d2229c6389b2ec9eefeb090bbaf77777e9d6b1b5a9d143 \
-    --hash=sha256:81af8adaa5e3099469e7623436881eff6b3b06db5ef75e6f5b6d4871263547e5 \
-    --hash=sha256:82e469518d3e9a321912955cc702d418773a2fd1e91c651280a1bda10622f02f \
-    --hash=sha256:8b27958f8c76bed8edaa63da0739d76e4e9ad4ed325c814f9b3851425582a3cd \
-    --hash=sha256:8c223fa57cb154c7eab5156856c231c3f5eace1e0bed9b32a24696b7ba3c3245 \
-    --hash=sha256:8f57e6b6927a49550da3d122f0cb983d400f843a8a82e65b3b380d3d7259468f \
-    --hash=sha256:925cd6a3b7b55dfba252b7c4561892311c5358c6b5a601847015a1ad4eb7d332 \
-    --hash=sha256:a43ef1c8ddfdb9575691720b6352761f3f53d85f1b57d7745701041053deff30 \
-    --hash=sha256:a8032e00ce71c3ceb93eeba63963b864bf635a18f6c0c12da6c13c450eedb183 \
-    --hash=sha256:b96ae2c1279d1065413965c607712006205a9ac541895004a1e0d4f281f2ff9f \
-    --hash=sha256:bb8ccb4724f7d8601938571bf3f24da0da791fe2db7be3d9e79849cb64e0ae85 \
-    --hash=sha256:bbaf4662e498c8c2e352da5f5bca5ab29d378895fa2d980630656178bd607c46 \
-    --hash=sha256:cfd13d47b29ed3bbaafaff7d8b21e90d827631afda134836962011acb5904b71 \
-    --hash=sha256:d4473c22cc296425bbbce7e9429588e76e05bc7342da359d6520b6427bf76660 \
-    --hash=sha256:d8fbb68711905f8912e5af474ca8b78d077447d8f3918997fecbf26943ff3cbb \
-    --hash=sha256:e5012e5cc2ac628177eaac0e83d622b2dd499e28253d4107a08ecc59ede3fc2c \
-    --hash=sha256:eb4f18589d196a4cbe5290b435d135dee96567e07c2b2d43b5c4621b6501531a
+more-itertools==10.2.0 \
+    --hash=sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684 \
+    --hash=sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+mypy==1.9.0 \
+    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
+    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
+    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
+    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
+    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
+    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
+    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
+    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
+    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
+    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
+    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
+    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
+    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
+    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
+    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
+    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
+    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
+    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
+    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
+    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
+    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
+    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
+    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
+    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
+    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
+    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
+    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
-nh3==0.2.14 \
-    --hash=sha256:116c9515937f94f0057ef50ebcbcc10600860065953ba56f14473ff706371873 \
-    --hash=sha256:18415df36db9b001f71a42a3a5395db79cf23d556996090d293764436e98e8ad \
-    --hash=sha256:203cac86e313cf6486704d0ec620a992c8bc164c86d3a4fd3d761dd552d839b5 \
-    --hash=sha256:2b0be5c792bd43d0abef8ca39dd8acb3c0611052ce466d0401d51ea0d9aa7525 \
-    --hash=sha256:377aaf6a9e7c63962f367158d808c6a1344e2b4f83d071c43fbd631b75c4f0b2 \
-    --hash=sha256:525846c56c2bcd376f5eaee76063ebf33cf1e620c1498b2a40107f60cfc6054e \
-    --hash=sha256:5529a3bf99402c34056576d80ae5547123f1078da76aa99e8ed79e44fa67282d \
-    --hash=sha256:7771d43222b639a4cd9e341f870cee336b9d886de1ad9bec8dddab22fe1de450 \
-    --hash=sha256:88c753efbcdfc2644a5012938c6b9753f1c64a5723a67f0301ca43e7b85dcf0e \
-    --hash=sha256:93a943cfd3e33bd03f77b97baa11990148687877b74193bf777956b67054dcc6 \
-    --hash=sha256:9be2f68fb9a40d8440cbf34cbf40758aa7f6093160bfc7fb018cce8e424f0c3a \
-    --hash=sha256:a0c509894fd4dccdff557068e5074999ae3b75f4c5a2d6fb5415e782e25679c4 \
-    --hash=sha256:ac8056e937f264995a82bf0053ca898a1cb1c9efc7cd68fa07fe0060734df7e4 \
-    --hash=sha256:aed56a86daa43966dd790ba86d4b810b219f75b4bb737461b6886ce2bde38fd6 \
-    --hash=sha256:e8986f1dd3221d1e741fda0a12eaa4a273f1d80a35e31a1ffe579e7c621d069e \
-    --hash=sha256:f99212a81c62b5f22f9e7c3e347aa00491114a5647e1f13bbebd79c3e5f08d75
+nh3==0.2.17 \
+    --hash=sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a \
+    --hash=sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911 \
+    --hash=sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb \
+    --hash=sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a \
+    --hash=sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc \
+    --hash=sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028 \
+    --hash=sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9 \
+    --hash=sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3 \
+    --hash=sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351 \
+    --hash=sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10 \
+    --hash=sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71 \
+    --hash=sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f \
+    --hash=sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b \
+    --hash=sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a \
+    --hash=sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062 \
+    --hash=sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a
     # via readme-renderer
-packaging==23.2 \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packaging==24.0 \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
     # via
     #   black
     #   build
+    #   cli-base-utilities
     #   dparse
+    #   marshmallow
     #   pyproject-api
     #   safety
+    #   safety-schemas
     #   tox
-pathspec==0.11.2 \
-    --hash=sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20 \
-    --hash=sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3
+pathspec==0.12.1 \
+    --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
+    --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
     # via black
-pip-tools==7.3.0 \
-    --hash=sha256:8717693288720a8c6ebd07149c93ab0be1fced0b5191df9e9decd3263e20d85e \
-    --hash=sha256:8e9c99127fe024c025b46a0b2d15c7bd47f18f33226cf7330d35493663fc1d1d
+pip-tools==7.4.1 \
+    --hash=sha256:4c690e5fbae2f21e87843e89c26191f0d9454f362d8acdbd695716493ec8b3a9 \
+    --hash=sha256:864826f5073864450e24dbeeb85ce3920cdfb09848a3d69ebf537b521f14bcc9
     # via DragonPyEmulator (pyproject.toml)
-pkginfo==1.9.6 \
-    --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
-    --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
+pkginfo==1.10.0 \
+    --hash=sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297 \
+    --hash=sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097
     # via twine
-platformdirs==3.11.0 \
-    --hash=sha256:cf8ee52a3afdb965072dcc652433e0c7e3e40cf5ea1477cd4b3b1d2eb75495b3 \
-    --hash=sha256:e9d171d00af68be50e9202731309c4e658fd8bc76f55c11c7dd760d023bda68e
+platformdirs==4.2.0 \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
     # via
     #   black
     #   tox
     #   virtualenv
-pluggy==1.3.0 \
-    --hash=sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12 \
-    --hash=sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7
+pluggy==1.4.0 \
+    --hash=sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981 \
+    --hash=sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be
     # via tox
 pycodestyle==2.11.1 \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
     # via
     #   autopep8
     #   flake8
-pycparser==2.21 \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
+pycparser==2.22 \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
     # via cffi
-pyflakes==3.1.0 \
-    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
-    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
+pydantic==2.7.0 \
+    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
+    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
+    # via
+    #   safety
+    #   safety-schemas
+pydantic-core==2.18.1 \
+    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
+    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
+    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
+    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
+    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
+    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
+    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
+    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
+    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
+    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
+    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
+    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
+    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
+    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
+    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
+    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
+    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
+    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
+    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
+    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
+    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
+    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
+    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
+    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
+    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
+    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
+    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
+    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
+    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
+    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
+    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
+    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
+    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
+    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
+    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
+    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
+    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
+    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
+    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
+    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
+    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
+    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
+    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
+    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
+    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
+    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
+    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
+    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
+    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
+    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
+    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
+    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
+    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
+    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
+    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
+    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
+    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
+    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
+    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
+    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
+    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
+    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
+    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
+    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
+    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
+    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
+    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
+    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
+    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
+    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
+    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
+    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
+    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
+    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
+    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
+    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
+    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
+    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
+    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
+    # via pydantic
+pyflakes==3.2.0 \
+    --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
+    --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   autoflake
     #   flake8
     #   manageprojects
-pygments==2.16.1 \
-    --hash=sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692 \
-    --hash=sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29
+pygments==2.17.2 \
+    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
+    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   darker
     #   readme-renderer
     #   rich
 pyproject-api==1.6.1 \
     --hash=sha256:1817dc018adc0d1ff9ca1ed8c60e1623d5aaca40814b953af14a9cf9a5cae538 \
     --hash=sha256:4c0116d60476b0786c88692cf4e325a9814965e2469c5998b830bba16b183675
     # via tox
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
-    # via build
-python-dateutil==2.8.2 \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
+    # via
+    #   build
+    #   pip-tools
+python-dateutil==2.9.0.post0 \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
     # via arrow
-python-slugify==8.0.1 \
-    --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
-    --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
+python-slugify==8.0.4 \
+    --hash=sha256:276540b79961052b66b7d116620b36518847f52d5fd9e3a70164fc8c50faa6b8 \
+    --hash=sha256:59202371d1d05b54a9e7720c5e038f928f45daaffe41dd10822f3907b937c856
     # via cookiecutter
-pyupgrade==3.15.0 \
-    --hash=sha256:8dc8ebfaed43566e2c65994162795017c7db11f531558a74bc8aa077907bc305 \
-    --hash=sha256:a7fde381060d7c224f55aef7a30fae5ac93bbc428367d27e70a603bc2acd4f00
+pyupgrade==3.15.2 \
+    --hash=sha256:c488d6896c546d25845712ef6402657123008d56c1063174e27aabe15bd6b4e5 \
+    --hash=sha256:ce309e0ff8ecb73f56a45f12570be84bbbde9540d13697cacb261a7f595fb1f5
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
 pyyaml==6.0.1 \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
@@ -653,14 +816,15 @@
     --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
     --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
     --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
     --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
     --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
     --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
     --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
     --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
     --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
     --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
     --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
     --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
     --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
     --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
@@ -675,17 +839,17 @@
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via cookiecutter
-readme-renderer==42.0 \
-    --hash=sha256:13d039515c1f24de668e2c93f2e877b9dbe6c6c32328b90a40a49d8b2b85f36d \
-    --hash=sha256:2d55489f83be4992fe4454939d1a051c33edbab778e82761d060c9fc6b308cd1
+readme-renderer==43.0 \
+    --hash=sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311 \
+    --hash=sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9
     # via twine
 requests==2.31.0 \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   cookiecutter
     #   requests-toolbelt
@@ -695,97 +859,109 @@
     --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
     --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
     # via twine
 rfc3986==2.0.0 \
     --hash=sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd \
     --hash=sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c
     # via twine
-rich==13.6.0 \
-    --hash=sha256:2b38e2fe9ca72c9a00170a1a2d20c63c790d0e10ef1fe35eba76e1e7b1d7d245 \
-    --hash=sha256:5c14d22737e6d5084ef4771b62d5d4363165b403455a30a1c8ca39dc7b644bef
+rich==13.7.1 \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   cli-base-utilities
     #   cookiecutter
     #   manageprojects
     #   mc6809
     #   rich-click
+    #   safety
     #   twine
-rich-click==1.7.1 \
-    --hash=sha256:660c8ea345343f47c5de88f62afa34a19d9f4c7accdd9c6e39dc17eece6affcd \
-    --hash=sha256:c37d19af85c86b9a256c18e9d23637ae89478300ec8dc5e220c6ca213675f2f9
+    #   typer
+rich-click==1.7.4 \
+    --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
+    --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   cli-base-utilities
     #   manageprojects
     #   mc6809
-ruamel-yaml==0.18.4 \
-    --hash=sha256:a2778930d2573358f7c43f26e4bd5715015dccebf53c9943ed611200c1e2adcd \
-    --hash=sha256:ca864776af7b0cbcbb223c38707a440bfabea926ba5b4163b2ef4991aae8f8c1
-    # via safety
+ruamel-yaml==0.18.6 \
+    --hash=sha256:57b53ba33def16c4f3d807c0ccbc00f8a6081827e81ba2491691b76882d0c636 \
+    --hash=sha256:8b27e6a217e786c6fbe5634d8f3f11bc63e0f80f6a5890f28863d9c45aac311b
+    # via
+    #   safety
+    #   safety-schemas
 ruamel-yaml-clib==0.2.8 \
     --hash=sha256:024cfe1fc7c7f4e1aff4a81e718109e13409767e4f871443cbff3dba3578203d \
     --hash=sha256:03d1162b6d1df1caa3a4bd27aa51ce17c9afc2046c31b0ad60a0a96ec22f8001 \
     --hash=sha256:07238db9cbdf8fc1e9de2489a4f68474e70dffcb32232db7c08fa61ca0c7c462 \
     --hash=sha256:09b055c05697b38ecacb7ac50bdab2240bfca1a0c4872b0fd309bb07dc9aa3a9 \
+    --hash=sha256:1707814f0d9791df063f8c19bb51b0d1278b8e9a2353abbb676c2f685dee6afe \
     --hash=sha256:1758ce7d8e1a29d23de54a16ae867abd370f01b5a69e1a3ba75223eaa3ca1a1b \
     --hash=sha256:184565012b60405d93838167f425713180b949e9d8dd0bbc7b49f074407c5a8b \
     --hash=sha256:1b617618914cb00bf5c34d4357c37aa15183fa229b24767259657746c9077615 \
+    --hash=sha256:1dc67314e7e1086c9fdf2680b7b6c2be1c0d8e3a8279f2e993ca2a7545fecf62 \
     --hash=sha256:25ac8c08322002b06fa1d49d1646181f0b2c72f5cbc15a85e80b4c30a544bb15 \
     --hash=sha256:25c515e350e5b739842fc3228d662413ef28f295791af5e5110b543cf0b57d9b \
+    --hash=sha256:305889baa4043a09e5b76f8e2a51d4ffba44259f6b4c72dec8ca56207d9c6fe1 \
     --hash=sha256:3213ece08ea033eb159ac52ae052a4899b56ecc124bb80020d9bbceeb50258e9 \
     --hash=sha256:3f215c5daf6a9d7bbed4a0a4f760f3113b10e82ff4c5c44bec20a68c8014f675 \
-    --hash=sha256:3fcc54cb0c8b811ff66082de1680b4b14cf8a81dce0d4fbf665c2265a81e07a1 \
     --hash=sha256:46d378daaac94f454b3a0e3d8d78cafd78a026b1d71443f4966c696b48a6d899 \
     --hash=sha256:4ecbf9c3e19f9562c7fdd462e8d18dd902a47ca046a2e64dba80699f0b6c09b7 \
     --hash=sha256:53a300ed9cea38cf5a2a9b069058137c2ca1ce658a874b79baceb8f892f915a7 \
     --hash=sha256:56f4252222c067b4ce51ae12cbac231bce32aee1d33fbfc9d17e5b8d6966c312 \
     --hash=sha256:5c365d91c88390c8d0a8545df0b5857172824b1c604e867161e6b3d59a827eaa \
-    --hash=sha256:665f58bfd29b167039f714c6998178d27ccd83984084c286110ef26b230f259f \
     --hash=sha256:700e4ebb569e59e16a976857c8798aee258dceac7c7d6b50cab63e080058df91 \
-    --hash=sha256:7048c338b6c86627afb27faecf418768acb6331fc24cfa56c93e8c9780f815fa \
     --hash=sha256:75e1ed13e1f9de23c5607fe6bd1aeaae21e523b32d83bb33918245361e9cc51b \
+    --hash=sha256:77159f5d5b5c14f7c34073862a6b7d34944075d9f93e681638f6d753606c6ce6 \
     --hash=sha256:7f67a1ee819dc4562d444bbafb135832b0b909f81cc90f7aa00260968c9ca1b3 \
     --hash=sha256:840f0c7f194986a63d2c2465ca63af8ccbbc90ab1c6001b1978f05119b5e7334 \
     --hash=sha256:84b554931e932c46f94ab306913ad7e11bba988104c5cff26d90d03f68258cd5 \
     --hash=sha256:87ea5ff66d8064301a154b3933ae406b0863402a799b16e4a1d24d9fbbcbe0d3 \
     --hash=sha256:955eae71ac26c1ab35924203fda6220f84dce57d6d7884f189743e2abe3a9fbe \
-    --hash=sha256:9eb5dee2772b0f704ca2e45b1713e4e5198c18f515b52743576d196348f374d3 \
+    --hash=sha256:a1a45e0bb052edf6a1d3a93baef85319733a888363938e1fc9924cb00c8df24c \
     --hash=sha256:a5aa27bad2bb83670b71683aae140a1f52b0857a2deff56ad3f6c13a017a26ed \
     --hash=sha256:a6a9ffd280b71ad062eae53ac1659ad86a17f59a0fdc7699fd9be40525153337 \
     --hash=sha256:a75879bacf2c987c003368cf14bed0ffe99e8e85acfa6c0bfffc21a090f16880 \
+    --hash=sha256:aa2267c6a303eb483de8d02db2871afb5c5fc15618d894300b88958f729ad74f \
     --hash=sha256:aab7fd643f71d7946f2ee58cc88c9b7bfc97debd71dcc93e03e2d174628e7e2d \
     --hash=sha256:b16420e621d26fdfa949a8b4b47ade8810c56002f5389970db4ddda51dbff248 \
     --hash=sha256:b42169467c42b692c19cf539c38d4602069d8c1505e97b86387fcf7afb766e1d \
-    --hash=sha256:b5edda50e5e9e15e54a6a8a0070302b00c518a9d32accc2346ad6c984aacd279 \
     --hash=sha256:bba64af9fa9cebe325a62fa398760f5c7206b215201b0ec825005f1b18b9bccf \
     --hash=sha256:beb2e0404003de9a4cab9753a8805a8fe9320ee6673136ed7f04255fe60bb512 \
     --hash=sha256:bef08cd86169d9eafb3ccb0a39edb11d8e25f3dae2b28f5c52fd997521133069 \
     --hash=sha256:c2a72e9109ea74e511e29032f3b670835f8a59bbdc9ce692c5b4ed91ccf1eedb \
     --hash=sha256:c58ecd827313af6864893e7af0a3bb85fd529f862b6adbefe14643947cfe2942 \
     --hash=sha256:c69212f63169ec1cfc9bb44723bf2917cbbd8f6191a00ef3410f5a7fe300722d \
     --hash=sha256:cabddb8d8ead485e255fe80429f833172b4cadf99274db39abc080e068cbcc31 \
     --hash=sha256:d176b57452ab5b7028ac47e7b3cf644bcfdc8cacfecf7e71759f7f51a59e5c92 \
-    --hash=sha256:d92f81886165cb14d7b067ef37e142256f1c6a90a65cd156b063a43da1708cfd \
     --hash=sha256:da09ad1c359a728e112d60116f626cc9f29730ff3e0e7db72b9a2dbc2e4beed5 \
     --hash=sha256:e2b4c44b60eadec492926a7270abb100ef9f72798e18743939bdbf037aab8c28 \
     --hash=sha256:e79e5db08739731b0ce4850bed599235d601701d5694c36570a99a0c5ca41a9d \
     --hash=sha256:ebc06178e8821efc9692ea7544aa5644217358490145629914d8020042c24aa1 \
     --hash=sha256:edaef1c1200c4b4cb914583150dcaa3bc30e592e907c01117c08b13a07255ec2 \
     --hash=sha256:f481f16baec5290e45aebdc2a5168ebc6d35189ae6fea7a58787613a25f6e875 \
     --hash=sha256:fff3573c2db359f091e1589c3d7c5fc2f86f5bdb6f24252c2d8e539d4e45f412
     # via ruamel-yaml
-safety==2.3.4 \
-    --hash=sha256:6224dcd9b20986a2b2c5e7acfdfba6bca42bb11b2783b24ed04f32317e5167ea \
-    --hash=sha256:b9e74e794e82f54d11f4091c5d820c4d2d81de9f953bf0b4f33ac8bc402ae72c
+safety==3.1.0 \
+    --hash=sha256:71f47b82ece153ec2f240e277f7cbfa70d5da2e0d143162c67f63b2f7459a1aa \
+    --hash=sha256:f2ba2d36f15ac1e24751547a73b854509a7d6db31efd30b57f64ffdf9d021934
     # via DragonPyEmulator (pyproject.toml)
+safety-schemas==0.0.2 \
+    --hash=sha256:277c077ce6e53221874a87c29515ffdd2f3773a6db4d035a9f67cc98db3b8c7f \
+    --hash=sha256:7d1b040ec06480f05cff6b45ea7a93e09c8942df864fb0d01ddeb67c323cfa8c
+    # via safety
 secretstorage==3.3.3 \
     --hash=sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77 \
     --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
     # via keyring
+shellingham==1.5.4 \
+    --hash=sha256:7ecfff8f2fd72616f7481040475a65b2bf8af90a56c89140852d1120324e8686 \
+    --hash=sha256:8dbca0739d487e5bd35ab3ca4b36e11c4078f3a234bfce294b0a0291363404de
+    # via typer
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via
     #   dragonlib
     #   python-dateutil
 text-unidecode==1.3 \
@@ -795,68 +971,86 @@
 tokenize-rt==5.2.0 \
     --hash=sha256:9fe80f8a5c1edad2d3ede0f37481cc0cc1538a2f442c9c2f9e4feacd2792d054 \
     --hash=sha256:b79d41a65cfec71285433511b50271b05da3584a1da144a0752e9c621a285289
     # via pyupgrade
 toml==0.10.2 \
     --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
     --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
-    # via darker
+    # via
+    #   darker
+    #   darkgraylib
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   DragonPyEmulator (pyproject.toml)
-    #   flynt
-tomlkit==0.12.2 \
-    --hash=sha256:df32fab589a81f0d7dc525a4267b6d7a64ee99619cbd1eeb0fae32c1dd426977 \
-    --hash=sha256:eeea7ac7563faeab0a1ed8fe12c2e5a51c61f933f2502f7e9db0241a65163ad0
+    #   cli-base-utilities
+tomlkit==0.12.4 \
+    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
+    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
     # via
     #   cli-base-utilities
     #   manageprojects
-tox==4.11.3 \
-    --hash=sha256:5039f68276461fae6a9452a3b2c7295798f00a0e92edcd9a3b78ba1a73577951 \
-    --hash=sha256:599af5e5bb0cad0148ac1558a0b66f8fff219ef88363483b8d92a81e4246f28f
+tox==4.14.2 \
+    --hash=sha256:0defb44f6dafd911b61788325741cc6b2e12ea71f987ac025ad4d649f1f1a104 \
+    --hash=sha256:2900c4eb7b716af4a928a7fdc2ed248ad6575294ed7cfae2ea41203937422847
     # via DragonPyEmulator (pyproject.toml)
-twine==4.0.2 \
-    --hash=sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8 \
-    --hash=sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8
+twine==5.0.0 \
+    --hash=sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4 \
+    --hash=sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0
     # via DragonPyEmulator (pyproject.toml)
-types-python-dateutil==2.8.19.14 \
-    --hash=sha256:1f4f10ac98bb8b16ade9dbee3518d9ace017821d94b057a425b069f834737f4b \
-    --hash=sha256:f977b8de27787639986b4e28963263fd0e5158942b3ecef91b9335c130cb1ce9
+typeguard==4.2.1 \
+    --hash=sha256:7da3bd46e61f03e0852f8d251dcbdc2a336aa495d7daff01e092b55327796eb8 \
+    --hash=sha256:c556a1b95948230510070ca53fa0341fb0964611bd05d598d87fb52115d65fee
+    # via DragonPyEmulator (pyproject.toml)
+typer==0.12.3 \
+    --hash=sha256:070d7ca53f785acbccba8e7d28b08dcd88f79f1fbda035ade0aecec71ca5c914 \
+    --hash=sha256:49e73131481d804288ef62598d97a1ceef3058905aa536a1134f90891ba35482
+    # via safety
+types-python-dateutil==2.9.0.20240316 \
+    --hash=sha256:5d2f2e240b86905e40944dd787db6da9263f0deabef1076ddaed797351ec0202 \
+    --hash=sha256:6b8cb66d960771ce5ff974e9dd45e38facb81718cc1e208b10b1baccbfdbee3b
     # via arrow
-typing-extensions==4.8.0 \
-    --hash=sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0 \
-    --hash=sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   mypy
+    #   pydantic
+    #   pydantic-core
     #   rich-click
-urllib3==2.0.7 \
-    --hash=sha256:c97dfde1f7bd43a71c8d2a58e369e9b2bf692d1334ea9f9cae55add7d0dd0f84 \
-    --hash=sha256:fdb6d215c776278489906c2f8916e6e7d4f5a9b602ccbcfdf7f016fc8da0596e
+    #   safety
+    #   safety-schemas
+    #   typeguard
+    #   typer
+urllib3==2.2.1 \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via
+    #   DragonPyEmulator (pyproject.toml)
     #   requests
+    #   safety
     #   twine
-virtualenv==20.24.6 \
-    --hash=sha256:02ece4f56fbf939dbbc33c0715159951d6bf14aaf5457b092e4548e1382455af \
-    --hash=sha256:520d056652454c5098a00c0f073611ccbea4c79089331f60bf9d7ba247bb7381
+virtualenv==20.25.1 \
+    --hash=sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a \
+    --hash=sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197
     # via tox
-wheel==0.41.3 \
-    --hash=sha256:488609bc63a29322326e05560731bf7bfea8e48ad646e1f5e40d366607de0942 \
-    --hash=sha256:4d4987ce51a49370ea65c0bfd2234e8ce80a12780820d9dc462597a6e60d0841
+wheel==0.43.0 \
+    --hash=sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85 \
+    --hash=sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81
     # via pip-tools
-zipp==3.17.0 \
-    --hash=sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31 \
-    --hash=sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0
+zipp==3.18.1 \
+    --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
+    --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==23.3.1 \
-    --hash=sha256:1fcaa041308d01f14575f6d0d2ea4b75a3e2871fe4f9c694976f908768e14174 \
-    --hash=sha256:55eb67bb6171d37447e82213be585b75fe2b12b359e993773aca4de9247a052b
+pip==24.0 \
+    --hash=sha256:ba0d021a166865d2265246961bec0152ff124de910c5cc39f1156ce3fa7c69dc \
+    --hash=sha256:ea9bd1a847e8c5774a5777bb398c19e80bcd4e2aa16a4b301b718fe6f593aba2
     # via pip-tools
-setuptools==68.2.2 \
-    --hash=sha256:4ac1475276d2f1c48684874089fefcd83bd7162ddaafb81fac866ba0db282a87 \
-    --hash=sha256:b454a35605876da60632df1a60f736524eb73cc47bbc9f3f1ef1b644de74fd2a
+setuptools==69.5.1 \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
     # via
     #   pip-tools
     #   safety
```

### Comparing `DragonPyEmulator-0.9.1/requirements.txt` & `dragonpyemulator-0.9.2/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,75 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    ./cli.py update
+#    ./dev-cli.py update
 #
 arrow==1.3.0 \
     --hash=sha256:c728b120ebc00eb84e01882a6f5e7927a53960aa990ce7dd2b10f39005a67f80 \
     --hash=sha256:d4540617648cb5f895730f1ad8c82a65f2dad0166f57b75f3ca54759c4d67a85
     # via cookiecutter
 astor==0.8.1 \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
     --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
     # via flynt
-autoflake==2.2.1 \
-    --hash=sha256:265cde0a43c1f44ecfb4f30d95b0437796759d07be7706a2f70e4719234c0f79 \
-    --hash=sha256:62b7b6449a692c3c9b0c916919bbc21648da7281e8506bcf8d3f8280e431ebc1
+async-timeout==4.0.3 \
+    --hash=sha256:4640d96be84d82d02ed59ea2b7105a0f7b33abe8703703cd0ab0bf87c427522f \
+    --hash=sha256:7405140ff1230c310e51dc27b3145b9092d659ce68ff733fb0cefe3ee42be028
+    # via cli-base-utilities
+attrs==23.2.0 \
+    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
+    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
+    # via flake8-bugbear
+autoflake==2.3.1 \
+    --hash=sha256:3ae7495db9084b7b32818b4140e6dc4fc280b712fb414f5b8fe57b0a8e85a840 \
+    --hash=sha256:c98b75dc5b0a86459c4f01a1d32ac7eb4338ec4317a4469515ff1e687ecd909e
     # via manageprojects
-autopep8==2.0.4 \
-    --hash=sha256:067959ca4a07b24dbd5345efa8325f5f58da4298dab0dde0443d5ed765de80cb \
-    --hash=sha256:2913064abd97b3419d1cc83ea71f042cb821f87e45b9c88cad5ad3c4ea87fe0c
+autopep8==2.1.0 \
+    --hash=sha256:1fa8964e4618929488f4ec36795c7ff12924a68b8bf01366c094fc52f770b6e7 \
+    --hash=sha256:2bb76888c5edbcafe6aabab3c47ba534f5a2c2d245c2eddced4a30c4b4946357
     # via manageprojects
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
-black==23.10.1 \
-    --hash=sha256:037e9b4664cafda5f025a1728c50a9e9aedb99a759c89f760bd83730e76ba884 \
-    --hash=sha256:1b917a2aa020ca600483a7b340c165970b26e9029067f019e3755b56e8dd5916 \
-    --hash=sha256:1f8ce316753428ff68749c65a5f7844631aa18c8679dfd3ca9dc1a289979c258 \
-    --hash=sha256:33d40f5b06be80c1bbce17b173cda17994fbad096ce60eb22054da021bf933d1 \
-    --hash=sha256:3f157a8945a7b2d424da3335f7ace89c14a3b0625e6593d21139c2d8214d55ce \
-    --hash=sha256:5ed45ac9a613fb52dad3b61c8dea2ec9510bf3108d4db88422bacc7d1ba1243d \
-    --hash=sha256:6d23d7822140e3fef190734216cefb262521789367fbdc0b3f22af6744058982 \
-    --hash=sha256:7670242e90dc129c539e9ca17665e39a146a761e681805c54fbd86015c7c84f7 \
-    --hash=sha256:7b4d10b0f016616a0d93d24a448100adf1699712fb7a4efd0e2c32bbb219b173 \
-    --hash=sha256:7cb5936e686e782fddb1c73f8aa6f459e1ad38a6a7b0e54b403f1f05a1507ee9 \
-    --hash=sha256:7d56124b7a61d092cb52cce34182a5280e160e6aff3137172a68c2c2c4b76bcb \
-    --hash=sha256:840015166dbdfbc47992871325799fd2dc0dcf9395e401ada6d88fe11498abad \
-    --hash=sha256:9c74de4c77b849e6359c6f01987e94873c707098322b91490d24296f66d067dc \
-    --hash=sha256:b15b75fc53a2fbcac8a87d3e20f69874d161beef13954747e053bca7a1ce53a0 \
-    --hash=sha256:cfcce6f0a384d0da692119f2d72d79ed07c7159879d0bb1bb32d2e443382bf3a \
-    --hash=sha256:d431e6739f727bb2e0495df64a6c7a5310758e87505f5f8cde9ff6c0f2d7e4fe \
-    --hash=sha256:e293e4c2f4a992b980032bbd62df07c1bcff82d6964d6c9496f2cd726e246ace \
-    --hash=sha256:ec3f8e6234c4e46ff9e16d9ae96f4ef69fa328bb4ad08198c8cee45bb1f08c69
+black==24.4.0 \
+    --hash=sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d \
+    --hash=sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd \
+    --hash=sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33 \
+    --hash=sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965 \
+    --hash=sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070 \
+    --hash=sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397 \
+    --hash=sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745 \
+    --hash=sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1 \
+    --hash=sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665 \
+    --hash=sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436 \
+    --hash=sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb \
+    --hash=sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e \
+    --hash=sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6 \
+    --hash=sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702 \
+    --hash=sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8 \
+    --hash=sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8 \
+    --hash=sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3 \
+    --hash=sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad \
+    --hash=sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf \
+    --hash=sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e \
+    --hash=sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641 \
+    --hash=sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2
     # via darker
-bx-py-utils==88 \
-    --hash=sha256:32fbc7e9ff3dfb0a817c80fb1d165ec559643dab59c0be549e646acbf8223b75 \
-    --hash=sha256:3a6f4eeef6abcac834b2c1ea4c5211130fd930a064aa0baabddd7c2bd00e38ac
+bx-py-utils==92 \
+    --hash=sha256:38641b2e1a09ed0c64cd6ba0e03c97fea347302439db0234a0492c365ae32719 \
+    --hash=sha256:849c59429af6ca0bf35265569884193c60be578285a66b533146e5782a10637b
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   cli-base-utilities
     #   mc6809
-certifi==2023.7.22 \
-    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
-    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
+certifi==2024.2.2 \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
     # via requests
 chardet==5.2.0 \
     --hash=sha256:1b3b6ff479a8c414bc3fa2c0852995695c4a026dcd6d0633b2dd092ca39c1cf7 \
     --hash=sha256:e1cf59446890a00105fe7b7912492ea04b6e6f06d4b742b2c788469e34c82970
     # via binaryornot
 charset-normalizer==3.3.2 \
     --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
@@ -147,20 +159,21 @@
     --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
     --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
     # via requests
-cli-base-utilities==0.4.4 \
-    --hash=sha256:110bef895fb7dfc29662f463ccedc4c985a880afbde2e6dea387d0d2f96f4985 \
-    --hash=sha256:72d4248776519a21c3448d6e348511ce6fe8c3742c154e158473236c8278fb1c
+cli-base-utilities==0.8.0 \
+    --hash=sha256:1009551eba81b33a0315c4fcfe3b6ef1633a99e303c9562dff39b824bff83ff0 \
+    --hash=sha256:79628db9fc7ca01b5ab18c97c8fa5f3d8b96af9975c608f7fee9a44256edb2ab
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   manageprojects
+    #   mc6809
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   black
     #   cli-base-utilities
@@ -168,210 +181,227 @@
     #   manageprojects
     #   mc6809
     #   rich-click
 codespell==2.2.6 \
     --hash=sha256:9ee9a3e5df0990604013ac2a9f22fa8e57669c827124a2e961fe8a1da4cacc07 \
     --hash=sha256:a8c65d8eb3faa03deabab6b3bbe798bea72e1799c7e9e955d57eca4096abcff9
     # via manageprojects
-cookiecutter==2.4.0 \
-    --hash=sha256:6d1494e66a784f23324df9d593f3e43af3db4f4b926b9e49e6ff060169fc042a \
-    --hash=sha256:8344663028abc08ec09b912e663636a97e1775bffe973425ec0107431acd390e
+cookiecutter==2.6.0 \
+    --hash=sha256:a54a8e37995e4ed963b3e82831072d1ad4b005af736bb17b99c2cbd9d41b6e2d \
+    --hash=sha256:db21f8169ea4f4fdc2408d48ca44859349de2647fbe494a9d6c3edfc0542c21c
     # via manageprojects
-darker[color,flynt,isort]==1.7.2 \
-    --hash=sha256:ec5b7c382d9537611c164f3ecca2e1b8a7923bc5a02bf22f6e7f6c8bcbdf593a \
-    --hash=sha256:ec9d130ab2a0f7fa49ab68a08fd231a5bec66147ecbbf94c92a1f33d97b5ef6f
+darker[color,flynt,isort]==2.1.1 \
+    --hash=sha256:a6e6a682c0604e76fe9aec7650e96a944f517563c69b28fcc076db9d957d98ea \
+    --hash=sha256:ead701414c45359fc0312bc285614d3285fc135476d43f3bc08d989ee19d9020
     # via manageprojects
+darkgraylib==1.2.0 \
+    --hash=sha256:1df3f35f3f7d2f944d506501c31d3fe145bad57cf4707c033b48083fba048d59 \
+    --hash=sha256:fefc821d5f88000aa36020f5fa35af64cbc7345f0a8f015edab7f37e3aec4997
+    # via
+    #   darker
+    #   graylint
 dragonlib==0.1.7 \
     --hash=sha256:1021c9bc4e62e39712f3fee7ddf454b0882168927dcee9a8dbc9fc50ff641b30 \
     --hash=sha256:89646eaa63b45185c5635387434bcf5a3bc6169502c1a19f8e47469d370ccf32
     # via DragonPyEmulator (pyproject.toml)
-editorconfig==0.12.3 \
-    --hash=sha256:57f8ce78afcba15c8b18d46b5170848c88d56fd38f05c2ec60dbbfcb8996e89e \
-    --hash=sha256:6b0851425aa875b08b16789ee0eeadbd4ab59666e9ebe728e526314c4a2e52c1
+editorconfig==0.12.4 \
+    --hash=sha256:24857fa1793917dd9ccf0c7810a07e05404ce9b823521c7dce22a4fb5d125f80
     # via manageprojects
-flake8==6.1.0 \
-    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
-    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
+flake8==7.0.0 \
+    --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
+    --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
+    # via
+    #   flake8-bugbear
+    #   manageprojects
+flake8-bugbear==24.2.6 \
+    --hash=sha256:663ef5de80cd32aacd39d362212983bc4636435a6f83700b4ed35acbd0b7d1b8 \
+    --hash=sha256:f9cb5f2a9e792dd80ff68e89a14c12eed8620af8b41a49d823b7a33064ac9658
     # via manageprojects
-flynt==0.77 \
-    --hash=sha256:2863ac8ec19d6ec8d29e760546e6ced644baf6dff3c7cdc77e03abbd29b80f14 \
-    --hash=sha256:2bd1b37043ad88a3f3c3c34a76fc0b64d24e5f03d36ea6b48cb69cc642bff17e
+flynt==1.0.1 \
+    --hash=sha256:65d1c546434827275123222a98408e9561bcd67db832dd58f530ff17b8329ec1 \
+    --hash=sha256:988aac00672a5469726cc0a17cef7d1178c284a9fe8563458db2475d0aaed965
+    # via darker
+graylint==1.1.1 \
+    --hash=sha256:0fd8e02972ca03d0ef2bf0adea76b5343efcd492d7afb5f658f3e3a724f55a36 \
+    --hash=sha256:b7e0eab6c159684dbf5ef84e942c3340f6a6549b02a3d11b1a1763cc4f8f0593
     # via darker
-idna==3.4 \
-    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
-    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
-isort==5.12.0 \
-    --hash=sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504 \
-    --hash=sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6
+isort==5.13.2 \
+    --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
+    --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
     # via darker
-jinja2==3.1.2 \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
+jinja2==3.1.3 \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
     # via cookiecutter
-manageprojects==0.15.2 \
-    --hash=sha256:44ac8973f9fede20693bd52c062d3b780268001f146100e6f3fc1bbaaa9ba720 \
-    --hash=sha256:f264f238e5f2998019e2a654103c28519110c47d509ba9652b77883148fe3c85
+manageprojects==0.17.1 \
+    --hash=sha256:355d970261f14b53b574d102e7e82462fe6769baa06c479f00f07a0bcfcb8e4d \
+    --hash=sha256:4662ff7f0e64ea9b420b67c270594c88542858a1434ebe8b5f93b7bf2ae2e706
     # via DragonPyEmulator (pyproject.toml)
 markdown-it-py==3.0.0 \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
     # via rich
-markupsafe==2.1.3 \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
+markupsafe==2.1.5 \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
     # via jinja2
-mc6809==0.7.1 \
-    --hash=sha256:46b30c68dd000c82a20c57bb6e6322ac63b6414cecae7cf723fbfea29ebb2d06 \
-    --hash=sha256:d9d63dbba30a28e018906b0708df5101f9c643bb2b87f2825529d739eced9cc0
+mc6809==0.7.2 \
+    --hash=sha256:933f5405f261db30681efbc3810bdcae385349d4ff95865cf2f53f534606faa9 \
+    --hash=sha256:f7592dadaaa52a35fa2af2fa4e259e032ca89ccf86c481e55d6e63e89ca6ab38
     # via DragonPyEmulator (pyproject.toml)
 mccabe==0.7.0 \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
     # via flake8
 mdurl==0.1.2 \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
     # via markdown-it-py
-mypy==1.6.1 \
-    --hash=sha256:19f905bcfd9e167159b3d63ecd8cb5e696151c3e59a1742e79bc3bcb540c42c7 \
-    --hash=sha256:21a1ad938fee7d2d96ca666c77b7c494c3c5bd88dff792220e1afbebb2925b5e \
-    --hash=sha256:40b1844d2e8b232ed92e50a4bd11c48d2daa351f9deee6c194b83bf03e418b0c \
-    --hash=sha256:41697773aa0bf53ff917aa077e2cde7aa50254f28750f9b88884acea38a16169 \
-    --hash=sha256:49ae115da099dcc0922a7a895c1eec82c1518109ea5c162ed50e3b3594c71208 \
-    --hash=sha256:4c46b51de523817a0045b150ed11b56f9fff55f12b9edd0f3ed35b15a2809de0 \
-    --hash=sha256:4cbe68ef919c28ea561165206a2dcb68591c50f3bcf777932323bc208d949cf1 \
-    --hash=sha256:4d01c00d09a0be62a4ca3f933e315455bde83f37f892ba4b08ce92f3cf44bcc1 \
-    --hash=sha256:59a0d7d24dfb26729e0a068639a6ce3500e31d6655df8557156c51c1cb874ce7 \
-    --hash=sha256:68351911e85145f582b5aa6cd9ad666c8958bcae897a1bfda8f4940472463c45 \
-    --hash=sha256:7274b0c57737bd3476d2229c6389b2ec9eefeb090bbaf77777e9d6b1b5a9d143 \
-    --hash=sha256:81af8adaa5e3099469e7623436881eff6b3b06db5ef75e6f5b6d4871263547e5 \
-    --hash=sha256:82e469518d3e9a321912955cc702d418773a2fd1e91c651280a1bda10622f02f \
-    --hash=sha256:8b27958f8c76bed8edaa63da0739d76e4e9ad4ed325c814f9b3851425582a3cd \
-    --hash=sha256:8c223fa57cb154c7eab5156856c231c3f5eace1e0bed9b32a24696b7ba3c3245 \
-    --hash=sha256:8f57e6b6927a49550da3d122f0cb983d400f843a8a82e65b3b380d3d7259468f \
-    --hash=sha256:925cd6a3b7b55dfba252b7c4561892311c5358c6b5a601847015a1ad4eb7d332 \
-    --hash=sha256:a43ef1c8ddfdb9575691720b6352761f3f53d85f1b57d7745701041053deff30 \
-    --hash=sha256:a8032e00ce71c3ceb93eeba63963b864bf635a18f6c0c12da6c13c450eedb183 \
-    --hash=sha256:b96ae2c1279d1065413965c607712006205a9ac541895004a1e0d4f281f2ff9f \
-    --hash=sha256:bb8ccb4724f7d8601938571bf3f24da0da791fe2db7be3d9e79849cb64e0ae85 \
-    --hash=sha256:bbaf4662e498c8c2e352da5f5bca5ab29d378895fa2d980630656178bd607c46 \
-    --hash=sha256:cfd13d47b29ed3bbaafaff7d8b21e90d827631afda134836962011acb5904b71 \
-    --hash=sha256:d4473c22cc296425bbbce7e9429588e76e05bc7342da359d6520b6427bf76660 \
-    --hash=sha256:d8fbb68711905f8912e5af474ca8b78d077447d8f3918997fecbf26943ff3cbb \
-    --hash=sha256:e5012e5cc2ac628177eaac0e83d622b2dd499e28253d4107a08ecc59ede3fc2c \
-    --hash=sha256:eb4f18589d196a4cbe5290b435d135dee96567e07c2b2d43b5c4621b6501531a
+mypy==1.9.0 \
+    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
+    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
+    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
+    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
+    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
+    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
+    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
+    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
+    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
+    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
+    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
+    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
+    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
+    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
+    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
+    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
+    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
+    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
+    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
+    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
+    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
+    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
+    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
+    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
+    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
+    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
+    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
     # via manageprojects
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via
     #   black
     #   mypy
-packaging==23.2 \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-    # via black
-pathspec==0.11.2 \
-    --hash=sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20 \
-    --hash=sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3
+packaging==24.0 \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
+    # via
+    #   black
+    #   cli-base-utilities
+pathspec==0.12.1 \
+    --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
+    --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
     # via black
-platformdirs==3.11.0 \
-    --hash=sha256:cf8ee52a3afdb965072dcc652433e0c7e3e40cf5ea1477cd4b3b1d2eb75495b3 \
-    --hash=sha256:e9d171d00af68be50e9202731309c4e658fd8bc76f55c11c7dd760d023bda68e
+platformdirs==4.2.0 \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
     # via black
 pycodestyle==2.11.1 \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
     # via
     #   autopep8
     #   flake8
-pyflakes==3.1.0 \
-    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
-    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
+pyflakes==3.2.0 \
+    --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
+    --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
     # via
     #   autoflake
     #   flake8
     #   manageprojects
-pygments==2.16.1 \
-    --hash=sha256:13fc09fa63bc8d8671a6d247e1eb303c4b343eaee81d861f3404db2935653692 \
-    --hash=sha256:1daff0494820c69bc8941e407aa20f577374ee88364ee10a98fdbe0aece96e29
+pygments==2.17.2 \
+    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
+    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   darker
     #   rich
-python-dateutil==2.8.2 \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
+python-dateutil==2.9.0.post0 \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
     # via arrow
-python-slugify==8.0.1 \
-    --hash=sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395 \
-    --hash=sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27
+python-slugify==8.0.4 \
+    --hash=sha256:276540b79961052b66b7d116620b36518847f52d5fd9e3a70164fc8c50faa6b8 \
+    --hash=sha256:59202371d1d05b54a9e7720c5e038f928f45daaffe41dd10822f3907b937c856
     # via cookiecutter
-pyupgrade==3.15.0 \
-    --hash=sha256:8dc8ebfaed43566e2c65994162795017c7db11f531558a74bc8aa077907bc305 \
-    --hash=sha256:a7fde381060d7c224f55aef7a30fae5ac93bbc428367d27e70a603bc2acd4f00
+pyupgrade==3.15.2 \
+    --hash=sha256:c488d6896c546d25845712ef6402657123008d56c1063174e27aabe15bd6b4e5 \
+    --hash=sha256:ce309e0ff8ecb73f56a45f12570be84bbbde9540d13697cacb261a7f595fb1f5
     # via manageprojects
 pyyaml==6.0.1 \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
     --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
     --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
@@ -395,14 +425,15 @@
     --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
     --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
     --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
     --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
     --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
     --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
     --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
     --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
     --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
     --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
     --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
     --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
     --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
     --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
@@ -421,27 +452,27 @@
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via cookiecutter
 requests==2.31.0 \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via cookiecutter
-rich==13.6.0 \
-    --hash=sha256:2b38e2fe9ca72c9a00170a1a2d20c63c790d0e10ef1fe35eba76e1e7b1d7d245 \
-    --hash=sha256:5c14d22737e6d5084ef4771b62d5d4363165b403455a30a1c8ca39dc7b644bef
+rich==13.7.1 \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   cli-base-utilities
     #   cookiecutter
     #   manageprojects
     #   mc6809
     #   rich-click
-rich-click==1.7.1 \
-    --hash=sha256:660c8ea345343f47c5de88f62afa34a19d9f4c7accdd9c6e39dc17eece6affcd \
-    --hash=sha256:c37d19af85c86b9a256c18e9d23637ae89478300ec8dc5e220c6ca213675f2f9
+rich-click==1.7.4 \
+    --hash=sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395 \
+    --hash=sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e
     # via
     #   DragonPyEmulator (pyproject.toml)
     #   cli-base-utilities
     #   manageprojects
     #   mc6809
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
@@ -456,32 +487,34 @@
 tokenize-rt==5.2.0 \
     --hash=sha256:9fe80f8a5c1edad2d3ede0f37481cc0cc1538a2f442c9c2f9e4feacd2792d054 \
     --hash=sha256:b79d41a65cfec71285433511b50271b05da3584a1da144a0752e9c621a285289
     # via pyupgrade
 toml==0.10.2 \
     --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
     --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
-    # via darker
+    # via
+    #   darker
+    #   darkgraylib
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-    # via flynt
-tomlkit==0.12.2 \
-    --hash=sha256:df32fab589a81f0d7dc525a4267b6d7a64ee99619cbd1eeb0fae32c1dd426977 \
-    --hash=sha256:eeea7ac7563faeab0a1ed8fe12c2e5a51c61f933f2502f7e9db0241a65163ad0
+    # via cli-base-utilities
+tomlkit==0.12.4 \
+    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
+    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
     # via
     #   cli-base-utilities
     #   manageprojects
-types-python-dateutil==2.8.19.14 \
-    --hash=sha256:1f4f10ac98bb8b16ade9dbee3518d9ace017821d94b057a425b069f834737f4b \
-    --hash=sha256:f977b8de27787639986b4e28963263fd0e5158942b3ecef91b9335c130cb1ce9
+types-python-dateutil==2.9.0.20240316 \
+    --hash=sha256:5d2f2e240b86905e40944dd787db6da9263f0deabef1076ddaed797351ec0202 \
+    --hash=sha256:6b8cb66d960771ce5ff974e9dd45e38facb81718cc1e208b10b1baccbfdbee3b
     # via arrow
-typing-extensions==4.8.0 \
-    --hash=sha256:8f92fc8806f9a6b641eaa5318da32b44d401efaac0f6678c9bc448ba3605faa0 \
-    --hash=sha256:df8e4339e9cb77357558cbdbceca33c303714cf861d1eef15e1070055ae8b7ef
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   mypy
     #   rich-click
-urllib3==2.0.7 \
-    --hash=sha256:c97dfde1f7bd43a71c8d2a58e369e9b2bf692d1334ea9f9cae55add7d0dd0f84 \
-    --hash=sha256:fdb6d215c776278489906c2f8916e6e7d4f5a9b602ccbcfdf7f016fc8da0596e
+urllib3==2.2.1 \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

