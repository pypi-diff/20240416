# Comparing `tmp/python3-capsolver-0.9.2.tar.gz` & `tmp/python3_capsolver-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-capsolver-0.9.2.tar", last modified: Fri Dec  8 21:50:41 2023, max compression
+gzip compressed data, was "python3_capsolver-0.9.3.tar", last modified: Tue Apr 16 14:25:55 2024, max compression
```

## Comparing `python3-capsolver-0.9.2.tar` & `python3_capsolver-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,51 @@
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2023-12-08 21:50:41.385712 python3-capsolver-0.9.2/
--rw-rw-r--   0 homea     (1000) homea     (1000)     5500 2023-12-08 21:50:41.385712 python3-capsolver-0.9.2/PKG-INFO
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2023-12-08 21:50:41.381712 python3-capsolver-0.9.2/python3_capsolver/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.9.2/python3_capsolver/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-12-08 21:50:33.000000 python3-capsolver-0.9.2/python3_capsolver/__version__.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     7988 2023-09-12 16:27:40.000000 python3-capsolver-0.9.2/python3_capsolver/akamai.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4538 2023-07-26 15:58:01.000000 python3-capsolver-0.9.2/python3_capsolver/aws_waf.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     4202 2023-09-12 20:07:38.000000 python3-capsolver-0.9.2/python3_capsolver/binance.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4468 2023-09-12 20:28:56.000000 python3-capsolver-0.9.2/python3_capsolver/cloudflare.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1958 2023-07-26 15:32:58.000000 python3-capsolver-0.9.2/python3_capsolver/control.py
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2023-12-08 21:50:41.385712 python3-capsolver-0.9.2/python3_capsolver/core/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.9.2/python3_capsolver/core/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3-capsolver-0.9.2/python3_capsolver/core/base.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1018 2023-07-27 12:52:57.000000 python3-capsolver-0.9.2/python3_capsolver/core/config.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3803 2023-09-12 19:46:32.000000 python3-capsolver-0.9.2/python3_capsolver/core/enum.py
--rw-r--r--   0 homea     (1000) homea     (1000)     5403 2023-10-30 04:43:51.000000 python3-capsolver-0.9.2/python3_capsolver/core/serializer.py
--rw-r--r--   0 homea     (1000) homea     (1000)     5247 2023-07-27 14:27:52.000000 python3-capsolver-0.9.2/python3_capsolver/cyber_si_ara.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3938 2023-07-27 19:48:25.000000 python3-capsolver-0.9.2/python3_capsolver/datadome_slider.py
--rw-r--r--   0 homea     (1000) homea     (1000)    10707 2023-07-27 19:48:09.000000 python3-capsolver-0.9.2/python3_capsolver/fun_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4310 2023-07-27 19:48:09.000000 python3-capsolver-0.9.2/python3_capsolver/gee_test.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7684 2023-07-27 19:48:09.000000 python3-capsolver-0.9.2/python3_capsolver/hcaptcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6271 2023-07-27 19:48:09.000000 python3-capsolver-0.9.2/python3_capsolver/image_to_text.py
--rw-rw-r--   0 homea     (1000) homea     (1000)     4612 2023-09-12 19:33:32.000000 python3-capsolver-0.9.2/python3_capsolver/imperva.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4948 2023-07-27 20:03:15.000000 python3-capsolver-0.9.2/python3_capsolver/mt_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6374 2023-07-27 19:48:09.000000 python3-capsolver-0.9.2/python3_capsolver/recaptcha.py
-drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2023-12-08 21:50:41.381712 python3-capsolver-0.9.2/python3_capsolver.egg-info/
--rw-rw-r--   0 homea     (1000) homea     (1000)     5500 2023-12-08 21:50:41.000000 python3-capsolver-0.9.2/python3_capsolver.egg-info/PKG-INFO
--rw-rw-r--   0 homea     (1000) homea     (1000)      920 2023-12-08 21:50:41.000000 python3-capsolver-0.9.2/python3_capsolver.egg-info/SOURCES.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)        1 2023-12-08 21:50:41.000000 python3-capsolver-0.9.2/python3_capsolver.egg-info/dependency_links.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)        1 2023-10-30 04:58:41.000000 python3-capsolver-0.9.2/python3_capsolver.egg-info/not-zip-safe
--rw-rw-r--   0 homea     (1000) homea     (1000)       62 2023-12-08 21:50:41.000000 python3-capsolver-0.9.2/python3_capsolver.egg-info/requires.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)       18 2023-12-08 21:50:41.000000 python3-capsolver-0.9.2/python3_capsolver.egg-info/top_level.txt
--rw-rw-r--   0 homea     (1000) homea     (1000)       38 2023-12-08 21:50:41.385712 python3-capsolver-0.9.2/setup.cfg
--rw-r--r--   0 homea     (1000) homea     (1000)     4202 2023-09-12 19:47:05.000000 python3-capsolver-0.9.2/setup.py
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-16 14:25:55.611544 python3_capsolver-0.9.3/
+-rw-r--r--   0 homea     (1000) homea     (1000)     1063 2023-04-28 18:48:47.000000 python3_capsolver-0.9.3/LICENSE
+-rw-r--r--   0 homea     (1000) homea     (1000)       25 2021-01-10 17:03:02.000000 python3_capsolver-0.9.3/MANIFEST.in
+-rw-r--r--   0 homea     (1000) homea     (1000)     5637 2024-04-16 14:25:55.611544 python3_capsolver-0.9.3/PKG-INFO
+-rw-r--r--   0 homea     (1000) homea     (1000)     3895 2023-12-13 19:03:43.000000 python3_capsolver-0.9.3/README.md
+-rw-r--r--   0 homea     (1000) homea     (1000)     2671 2024-04-16 14:25:51.000000 python3_capsolver-0.9.3/pyproject.toml
+-rw-rw-r--   0 homea     (1000) homea     (1000)       38 2024-04-16 14:25:55.611544 python3_capsolver-0.9.3/setup.cfg
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-16 14:25:55.605543 python3_capsolver-0.9.3/src/
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-16 14:25:55.608543 python3_capsolver-0.9.3/src/python3_capsolver/
+-rw-r--r--   0 homea     (1000) homea     (1000)       54 2024-04-16 14:20:31.000000 python3_capsolver-0.9.3/src/python3_capsolver/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)       22 2024-04-16 13:20:00.000000 python3_capsolver-0.9.3/src/python3_capsolver/__version__.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     7988 2023-09-12 16:27:40.000000 python3_capsolver-0.9.3/src/python3_capsolver/akamai.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4538 2023-07-26 15:58:01.000000 python3_capsolver-0.9.3/src/python3_capsolver/aws_waf.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4202 2023-09-12 20:07:38.000000 python3_capsolver-0.9.3/src/python3_capsolver/binance.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4468 2023-09-12 20:28:56.000000 python3_capsolver-0.9.3/src/python3_capsolver/cloudflare.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1958 2023-07-26 15:32:58.000000 python3_capsolver-0.9.3/src/python3_capsolver/control.py
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-16 14:25:55.609543 python3_capsolver-0.9.3/src/python3_capsolver/core/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3_capsolver-0.9.3/src/python3_capsolver/core/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3_capsolver-0.9.3/src/python3_capsolver/core/base.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1018 2023-07-27 12:52:57.000000 python3_capsolver-0.9.3/src/python3_capsolver/core/config.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3803 2023-09-12 19:46:32.000000 python3_capsolver-0.9.3/src/python3_capsolver/core/enum.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     5385 2024-04-16 13:18:40.000000 python3_capsolver-0.9.3/src/python3_capsolver/core/serializer.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     5247 2023-07-27 14:27:52.000000 python3_capsolver-0.9.3/src/python3_capsolver/cyber_si_ara.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3938 2023-07-27 19:48:25.000000 python3_capsolver-0.9.3/src/python3_capsolver/datadome_slider.py
+-rw-r--r--   0 homea     (1000) homea     (1000)    10707 2023-07-27 19:48:09.000000 python3_capsolver-0.9.3/src/python3_capsolver/fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4310 2023-07-27 19:48:09.000000 python3_capsolver-0.9.3/src/python3_capsolver/gee_test.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7684 2023-07-27 19:48:09.000000 python3_capsolver-0.9.3/src/python3_capsolver/hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6271 2023-07-27 19:48:09.000000 python3_capsolver-0.9.3/src/python3_capsolver/image_to_text.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4612 2023-09-12 19:33:32.000000 python3_capsolver-0.9.3/src/python3_capsolver/imperva.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4948 2023-07-27 20:03:15.000000 python3_capsolver-0.9.3/src/python3_capsolver/mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6374 2023-07-27 19:48:09.000000 python3_capsolver-0.9.3/src/python3_capsolver/recaptcha.py
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-16 14:25:55.611544 python3_capsolver-0.9.3/src/python3_capsolver.egg-info/
+-rw-r--r--   0 homea     (1000) homea     (1000)     5637 2024-04-16 14:25:55.000000 python3_capsolver-0.9.3/src/python3_capsolver.egg-info/PKG-INFO
+-rw-rw-r--   0 homea     (1000) homea     (1000)     1330 2024-04-16 14:25:55.000000 python3_capsolver-0.9.3/src/python3_capsolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)        1 2024-04-16 14:25:55.000000 python3_capsolver-0.9.3/src/python3_capsolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)       62 2024-04-16 14:25:55.000000 python3_capsolver-0.9.3/src/python3_capsolver.egg-info/requires.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)       18 2024-04-16 14:25:55.000000 python3_capsolver-0.9.3/src/python3_capsolver.egg-info/top_level.txt
+drwxrwxr-x   0 homea     (1000) homea     (1000)        0 2024-04-16 14:25:55.610543 python3_capsolver-0.9.3/tests/
+-rw-rw-r--   0 homea     (1000) homea     (1000)     4383 2023-09-12 17:32:55.000000 python3_capsolver-0.9.3/tests/test_akamai.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3121 2023-09-12 20:41:53.000000 python3_capsolver-0.9.3/tests/test_binance.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     2670 2023-09-12 20:47:40.000000 python3_capsolver-0.9.3/tests/test_cloudflare.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1544 2023-07-27 19:49:26.000000 python3_capsolver-0.9.3/tests/test_control.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3819 2023-07-27 19:49:26.000000 python3_capsolver-0.9.3/tests/test_core.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3321 2023-09-12 21:23:18.000000 python3_capsolver-0.9.3/tests/test_datadome_slider.py
+-rw-r--r--   0 homea     (1000) homea     (1000)    11922 2023-09-12 16:53:04.000000 python3_capsolver-0.9.3/tests/test_fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6779 2023-07-27 19:49:26.000000 python3_capsolver-0.9.3/tests/test_gee_test.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     9816 2023-09-12 21:19:07.000000 python3_capsolver-0.9.3/tests/test_hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3462 2023-09-12 21:27:25.000000 python3_capsolver-0.9.3/tests/test_image_to_text.py
+-rw-rw-r--   0 homea     (1000) homea     (1000)     3370 2023-09-12 20:43:41.000000 python3_capsolver-0.9.3/tests/test_imperva.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3518 2023-09-12 21:25:26.000000 python3_capsolver-0.9.3/tests/test_mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     9269 2023-09-12 21:29:51.000000 python3_capsolver-0.9.3/tests/test_recaptcha.py
```

### Comparing `python3-capsolver-0.9.2/PKG-INFO` & `python3_capsolver-0.9.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,45 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python 3.8+ Capsolver library with AIO module.
-Home-page: https://andreidrang.github.io/python3-capsolver/
-Author: AndreiDrang
-Author-email: python-captcha@pm.me
-License: MIT
+Author-email: AndreiDrang <python-captcha@pm.me>
+License: MIT License
+Project-URL: Homepage, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
-Project-URL: Source, https://github.com/AndreiDrang/python3-capsolver
-Keywords: captcha 
-                recaptcha
-                geetest
-                hcaptcha
-                capypuzzle
-                rotatecaptcha
-                funcaptcha
-                keycaptcha
-                python3
-                python-library
-                capsolver
-                datadomeslider
-                datadome
-                mtcaptcha
-				turnstile
-				cloudflare
-				amazon
-				amazon_waf
-				akamai
-				imperva
-				binance
+Project-URL: Repository, https://github.com/AndreiDrang/python3-capsolver
+Project-URL: Issues, https://github.com/AndreiDrang/python3-capsolver/issues
+Project-URL: Changelog, https://github.com/AndreiDrang/python3-capsolver/releases
+Keywords: captcha,recaptcha,geetest,hcaptcha,capypuzzle,rotatecaptcha,funcaptcha,keycaptcha,python3,python-library,capsolver,datadomeslider,datadome,mtcaptcha,turnstile,cloudflare,amazon,amazon_waf,akamai,imperva,binance
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8.0
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-
+License-File: LICENSE
+Requires-Dist: requests>=2.21.0
+Requires-Dist: aiohttp>=3.9.2
+Requires-Dist: pydantic==2.7.0
+Requires-Dist: tenacity==8.*
 
 # python3-capsolver
 
-![Logo](https://red-panda-dev.xyz/media/images/Capsolver.max-800x600.png)
+![Logo](https://red-panda-dev.xyz/media/images/Capsolver_ugBYrN0.original.png)
 
 <a href="https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1">
     <img src="https://cdn.discordapp.com/attachments/1105172394655625306/1105180101802471575/20221207-160749.gif" alt="Capsolver's Banner">
 </a>
 <br>
 At the lowest price on the market, you may receive a variety of solutions, including reCAPTCHA V2, reCAPTCHA V3, hCaptcha, hCaptcha Click, FunCaptcha, picture-to-text, and more. With this service, 0.1s is the slowest speed ever measured.
 <hr>
```

#### html2text {}

```diff
@@ -1,27 +1,31 @@
-Metadata-Version: 2.1 Name: python3-capsolver Version: 0.9.2 Summary: Python
-3.8+ Capsolver library with AIO module. Home-page: https://
-andreidrang.github.io/python3-capsolver/ Author: AndreiDrang Author-email:
-python-captcha@pm.me License: MIT Project-URL: Documentation, https://
-andreidrang.github.io/python3-capsolver/ Project-URL: Source, https://
-github.com/AndreiDrang/python3-capsolver Keywords: captcha recaptcha geetest
-hcaptcha capypuzzle rotatecaptcha funcaptcha keycaptcha python3 python-library
-capsolver datadomeslider datadome mtcaptcha turnstile cloudflare amazon
-amazon_waf akamai imperva binance Classifier: License :: OSI Approved :: MIT
-License Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
-2.0) Classifier: Development Status :: 5 - Production/Stable Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Framework :: AsyncIO Classifier:
-Operating System :: Unix Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS Requires-Python: >=3.8.0 Description-
-Content-Type: text/markdown # python3-capsolver ![Logo](https://red-panda-
-dev.xyz/media/images/Capsolver.max-800x600.png) _[_C_a_p_s_o_l_v_e_r_'_s_ _B_a_n_n_e_r_]
+Metadata-Version: 2.1 Name: python3-capsolver Version: 0.9.3 Summary: Python
+3.8+ Capsolver library with AIO module. Author-email: AndreiDrang
+pm.me> License: MIT License Project-URL: Homepage, https://
+andreidrang.github.io/python3-capsolver/ Project-URL: Documentation, https://
+andreidrang.github.io/python3-capsolver/ Project-URL: Repository, https://
+github.com/AndreiDrang/python3-capsolver Project-URL: Issues, https://
+github.com/AndreiDrang/python3-capsolver/issues Project-URL: Changelog, https:/
+/github.com/AndreiDrang/python3-capsolver/releases Keywords:
+captcha,recaptcha,geetest,hcaptcha,capypuzzle,rotatecaptcha,funcaptcha,keycaptcha,python3,python-
+library,capsolver,datadomeslider,datadome,mtcaptcha,turnstile,cloudflare,amazon,amazon_waf,akamai,imperva,binance
+Classifier: License :: OSI Approved :: MIT License Classifier: License :: OSI
+Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Development Status
+:: 5 - Production/Stable Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Framework :: AsyncIO
+Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
+:: Windows Classifier: Operating System :: MacOS Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests>=2.21.0 Requires-Dist: aiohttp>=3.9.2 Requires-Dist: pydantic==2.7.0
+Requires-Dist: tenacity==8.* # python3-capsolver ![Logo](https://red-panda-
+dev.xyz/media/images/Capsolver_ugBYrN0.original.png) _[_C_a_p_s_o_l_v_e_r_'_s_ _B_a_n_n_e_r_]
 At the lowest price on the market, you may receive a variety of solutions,
 including reCAPTCHA V2, reCAPTCHA V3, hCaptcha, hCaptcha Click, FunCaptcha,
 picture-to-text, and more. With this service, 0.1s is the slowest speed ever
 measured.
 ===============================================================================
 [![PyPI version](https://badge.fury.io/py/python3-capsolver.svg)](https://
 badge.fury.io/py/python3-capsolver) [![Python versions](https://img.shields.io/
```

### Comparing `python3-capsolver-0.9.2/python3_capsolver/akamai.py` & `python3_capsolver-0.9.3/src/python3_capsolver/akamai.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/aws_waf.py` & `python3_capsolver-0.9.3/src/python3_capsolver/aws_waf.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/binance.py` & `python3_capsolver-0.9.3/src/python3_capsolver/binance.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/cloudflare.py` & `python3_capsolver-0.9.3/src/python3_capsolver/cloudflare.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/control.py` & `python3_capsolver-0.9.3/src/python3_capsolver/control.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/core/base.py` & `python3_capsolver-0.9.3/src/python3_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/core/config.py` & `python3_capsolver-0.9.3/src/python3_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/core/enum.py` & `python3_capsolver-0.9.3/src/python3_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/core/serializer.py` & `python3_capsolver-0.9.3/src/python3_capsolver/core/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 class CaptchaResponseSer(ResponseSer):
     taskId: Optional[str] = Field(None, description="Task ID for future use in getTaskResult method.")
     status: ResponseStatusEnm = Field(ResponseStatusEnm.Processing, description="Task current status")
     solution: Dict[str, Any] = Field(None, description="Task result data. Different for each type of task.")
 
     class Config:
-        allow_population_by_field_name = True
+        populate_by_name = True
 
 
 class ControlResponseSer(ResponseSer):
     balance: Optional[float] = Field(0, description="Account balance value in USD")
 
 
 """
@@ -116,16 +116,15 @@
 
 class DatadomeSliderSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with DatadomeSlider")
     captchaUrl: str = Field(..., description="Captcha Url where is the captcha")
     userAgent: str = Field(..., description="Browser's User-Agent which is used in emulation")
 
 
-class CloudflareTurnstileSer(WebsiteDataOptionsSer):
-    ...
+class CloudflareTurnstileSer(WebsiteDataOptionsSer): ...
 
 
 class CyberSiAraSer(WebsiteDataOptionsSer):
     SlideMasterUrlId: str = Field(
         ..., description="You can get MasterUrlId param form `api/CyberSiara/GetCyberSiara` endpoint request"
     )
     UserAgent: str = Field(..., description="Browser userAgent, you need submit your userAgent")
```

### Comparing `python3-capsolver-0.9.2/python3_capsolver/cyber_si_ara.py` & `python3_capsolver-0.9.3/src/python3_capsolver/cyber_si_ara.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/datadome_slider.py` & `python3_capsolver-0.9.3/src/python3_capsolver/datadome_slider.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/fun_captcha.py` & `python3_capsolver-0.9.3/src/python3_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/gee_test.py` & `python3_capsolver-0.9.3/src/python3_capsolver/gee_test.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/hcaptcha.py` & `python3_capsolver-0.9.3/src/python3_capsolver/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/image_to_text.py` & `python3_capsolver-0.9.3/src/python3_capsolver/image_to_text.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/imperva.py` & `python3_capsolver-0.9.3/src/python3_capsolver/imperva.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/mt_captcha.py` & `python3_capsolver-0.9.3/src/python3_capsolver/mt_captcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver/recaptcha.py` & `python3_capsolver-0.9.3/src/python3_capsolver/recaptcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.9.2/python3_capsolver.egg-info/PKG-INFO` & `python3_capsolver-0.9.3/src/python3_capsolver.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,45 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python 3.8+ Capsolver library with AIO module.
-Home-page: https://andreidrang.github.io/python3-capsolver/
-Author: AndreiDrang
-Author-email: python-captcha@pm.me
-License: MIT
+Author-email: AndreiDrang <python-captcha@pm.me>
+License: MIT License
+Project-URL: Homepage, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
-Project-URL: Source, https://github.com/AndreiDrang/python3-capsolver
-Keywords: captcha 
-                recaptcha
-                geetest
-                hcaptcha
-                capypuzzle
-                rotatecaptcha
-                funcaptcha
-                keycaptcha
-                python3
-                python-library
-                capsolver
-                datadomeslider
-                datadome
-                mtcaptcha
-				turnstile
-				cloudflare
-				amazon
-				amazon_waf
-				akamai
-				imperva
-				binance
+Project-URL: Repository, https://github.com/AndreiDrang/python3-capsolver
+Project-URL: Issues, https://github.com/AndreiDrang/python3-capsolver/issues
+Project-URL: Changelog, https://github.com/AndreiDrang/python3-capsolver/releases
+Keywords: captcha,recaptcha,geetest,hcaptcha,capypuzzle,rotatecaptcha,funcaptcha,keycaptcha,python3,python-library,capsolver,datadomeslider,datadome,mtcaptcha,turnstile,cloudflare,amazon,amazon_waf,akamai,imperva,binance
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8.0
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-
+License-File: LICENSE
+Requires-Dist: requests>=2.21.0
+Requires-Dist: aiohttp>=3.9.2
+Requires-Dist: pydantic==2.7.0
+Requires-Dist: tenacity==8.*
 
 # python3-capsolver
 
-![Logo](https://red-panda-dev.xyz/media/images/Capsolver.max-800x600.png)
+![Logo](https://red-panda-dev.xyz/media/images/Capsolver_ugBYrN0.original.png)
 
 <a href="https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1">
     <img src="https://cdn.discordapp.com/attachments/1105172394655625306/1105180101802471575/20221207-160749.gif" alt="Capsolver's Banner">
 </a>
 <br>
 At the lowest price on the market, you may receive a variety of solutions, including reCAPTCHA V2, reCAPTCHA V3, hCaptcha, hCaptcha Click, FunCaptcha, picture-to-text, and more. With this service, 0.1s is the slowest speed ever measured.
 <hr>
```

#### html2text {}

```diff
@@ -1,27 +1,31 @@
-Metadata-Version: 2.1 Name: python3-capsolver Version: 0.9.2 Summary: Python
-3.8+ Capsolver library with AIO module. Home-page: https://
-andreidrang.github.io/python3-capsolver/ Author: AndreiDrang Author-email:
-python-captcha@pm.me License: MIT Project-URL: Documentation, https://
-andreidrang.github.io/python3-capsolver/ Project-URL: Source, https://
-github.com/AndreiDrang/python3-capsolver Keywords: captcha recaptcha geetest
-hcaptcha capypuzzle rotatecaptcha funcaptcha keycaptcha python3 python-library
-capsolver datadomeslider datadome mtcaptcha turnstile cloudflare amazon
-amazon_waf akamai imperva binance Classifier: License :: OSI Approved :: MIT
-License Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL
-2.0) Classifier: Development Status :: 5 - Production/Stable Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Framework :: AsyncIO Classifier:
-Operating System :: Unix Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS Requires-Python: >=3.8.0 Description-
-Content-Type: text/markdown # python3-capsolver ![Logo](https://red-panda-
-dev.xyz/media/images/Capsolver.max-800x600.png) _[_C_a_p_s_o_l_v_e_r_'_s_ _B_a_n_n_e_r_]
+Metadata-Version: 2.1 Name: python3-capsolver Version: 0.9.3 Summary: Python
+3.8+ Capsolver library with AIO module. Author-email: AndreiDrang
+pm.me> License: MIT License Project-URL: Homepage, https://
+andreidrang.github.io/python3-capsolver/ Project-URL: Documentation, https://
+andreidrang.github.io/python3-capsolver/ Project-URL: Repository, https://
+github.com/AndreiDrang/python3-capsolver Project-URL: Issues, https://
+github.com/AndreiDrang/python3-capsolver/issues Project-URL: Changelog, https:/
+/github.com/AndreiDrang/python3-capsolver/releases Keywords:
+captcha,recaptcha,geetest,hcaptcha,capypuzzle,rotatecaptcha,funcaptcha,keycaptcha,python3,python-
+library,capsolver,datadomeslider,datadome,mtcaptcha,turnstile,cloudflare,amazon,amazon_waf,akamai,imperva,binance
+Classifier: License :: OSI Approved :: MIT License Classifier: License :: OSI
+Approved :: Mozilla Public License 2.0 (MPL 2.0) Classifier: Development Status
+:: 5 - Production/Stable Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Framework :: AsyncIO
+Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
+:: Windows Classifier: Operating System :: MacOS Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests>=2.21.0 Requires-Dist: aiohttp>=3.9.2 Requires-Dist: pydantic==2.7.0
+Requires-Dist: tenacity==8.* # python3-capsolver ![Logo](https://red-panda-
+dev.xyz/media/images/Capsolver_ugBYrN0.original.png) _[_C_a_p_s_o_l_v_e_r_'_s_ _B_a_n_n_e_r_]
 At the lowest price on the market, you may receive a variety of solutions,
 including reCAPTCHA V2, reCAPTCHA V3, hCaptcha, hCaptcha Click, FunCaptcha,
 picture-to-text, and more. With this service, 0.1s is the slowest speed ever
 measured.
 ===============================================================================
 [![PyPI version](https://badge.fury.io/py/python3-capsolver.svg)](https://
 badge.fury.io/py/python3-capsolver) [![Python versions](https://img.shields.io/
```

