# Comparing `tmp/anedya-dev-sdk-0.1.2.tar.gz` & `tmp/anedya_dev_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anedya-dev-sdk-0.1.2.tar", last modified: Tue Apr  9 11:18:00 2024, max compression
+gzip compressed data, was "anedya_dev_sdk-0.1.3.tar", last modified: Tue Apr 16 11:14:57 2024, max compression
```

## Comparing `anedya-dev-sdk-0.1.2.tar` & `anedya_dev_sdk-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 11:18:00.644667 anedya-dev-sdk-0.1.2/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya-dev-sdk-0.1.2/LICENSE
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya-dev-sdk-0.1.2/MANIFEST.in
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2496 2024-04-09 11:18:00.644667 anedya-dev-sdk-0.1.2/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1323 2024-04-09 10:43:07.000000 anedya-dev-sdk-0.1.2/README.md
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-09 11:18:00.644667 anedya-dev-sdk-0.1.2/setup.cfg
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya-dev-sdk-0.1.2/setup.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 11:18:00.640667 anedya-dev-sdk-0.1.2/src/
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 11:18:00.640667 anedya-dev-sdk-0.1.2/src/anedya/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.2/src/anedya/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4167 2024-04-09 10:16:37.000000 anedya-dev-sdk-0.1.2/src/anedya/anedya.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 11:18:00.640667 anedya-dev-sdk-0.1.2/src/anedya/client/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya-dev-sdk-0.1.2/src/anedya/client/__init__.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1422 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.2/src/anedya/client/bindDevice.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      731 2024-04-09 10:17:45.000000 anedya-dev-sdk-0.1.2/src/anedya/client/callbacks.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya-dev-sdk-0.1.2/src/anedya/client/certs.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2127 2024-04-09 09:46:47.000000 anedya-dev-sdk-0.1.2/src/anedya/client/mqttHandlers.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2046 2024-04-09 10:24:48.000000 anedya-dev-sdk-0.1.2/src/anedya/client/submitData.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1239 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.2/src/anedya/client/timeSync.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     2578 2024-04-09 07:29:26.000000 anedya-dev-sdk-0.1.2/src/anedya/config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya-dev-sdk-0.1.2/src/anedya/errors.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1354 2024-03-05 06:37:43.000000 anedya-dev-sdk-0.1.2/src/anedya/models.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya-dev-sdk-0.1.2/src/anedya/transaction.py
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 11:18:00.644667 anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/
--rw-r--r--   0 invesun   (1000) invesun   (1000)     2496 2024-04-09 11:18:00.000000 anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      646 2024-04-09 11:18:00.000000 anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-09 11:18:00.000000 anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-09 11:18:00.000000 anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/requires.txt
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-09 11:18:00.000000 anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-09 11:18:00.644667 anedya-dev-sdk-0.1.2/tests/
--rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.2/tests/test_config.py
--rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya-dev-sdk-0.1.2/tests/test_core.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)    11357 2023-11-23 07:44:28.000000 anedya_dev_sdk-0.1.3/LICENSE
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       33 2023-12-18 11:15:14.000000 anedya_dev_sdk-0.1.3/MANIFEST.in
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1261 2024-04-09 11:23:38.000000 anedya_dev_sdk-0.1.3/README.md
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1230 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/setup.cfg
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      396 2024-02-29 09:37:09.000000 anedya_dev_sdk-0.1.3/setup.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.399822 anedya_dev_sdk-0.1.3/src/
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.399822 anedya_dev_sdk-0.1.3/src/anedya/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      321 2024-03-05 06:37:43.000000 anedya_dev_sdk-0.1.3/src/anedya/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4167 2024-04-16 11:12:11.000000 anedya_dev_sdk-0.1.3/src/anedya/anedya.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.399822 anedya_dev_sdk-0.1.3/src/anedya/client/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       25 2024-04-09 11:12:12.000000 anedya_dev_sdk-0.1.3/src/anedya/client/__init__.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2888 2024-04-16 10:38:21.000000 anedya_dev_sdk-0.1.3/src/anedya/client/bindDevice.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      731 2024-04-09 10:17:45.000000 anedya_dev_sdk-0.1.3/src/anedya/client/callbacks.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     4963 2024-02-29 09:22:48.000000 anedya_dev_sdk-0.1.3/src/anedya/client/certs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2127 2024-04-09 09:46:47.000000 anedya_dev_sdk-0.1.3/src/anedya/client/mqttHandlers.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     3237 2024-04-16 10:36:25.000000 anedya_dev_sdk-0.1.3/src/anedya/client/submitData.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2595 2024-04-16 10:48:17.000000 anedya_dev_sdk-0.1.3/src/anedya/client/submitLogs.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2796 2024-04-16 10:48:15.000000 anedya_dev_sdk-0.1.3/src/anedya/client/timeSync.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2736 2024-04-16 10:58:02.000000 anedya_dev_sdk-0.1.3/src/anedya/config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1511 2024-04-09 10:19:58.000000 anedya_dev_sdk-0.1.3/src/anedya/errors.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     2354 2024-04-16 11:09:16.000000 anedya_dev_sdk-0.1.3/src/anedya/models.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)     1622 2024-04-09 10:24:54.000000 anedya_dev_sdk-0.1.3/src/anedya/transaction.py
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/
+-rw-r--r--   0 invesun   (1000) invesun   (1000)     2434 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      678 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        1 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)       26 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/requires.txt
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        7 2024-04-16 11:14:57.000000 anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 invesun   (1000) invesun   (1000)        0 2024-04-16 11:14:57.403822 anedya_dev_sdk-0.1.3/tests/
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)      694 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.3/tests/test_config.py
+-rw-rw-r--   0 invesun   (1000) invesun   (1000)        0 2023-11-23 07:46:25.000000 anedya_dev_sdk-0.1.3/tests/test_core.py
```

### Comparing `anedya-dev-sdk-0.1.2/LICENSE` & `anedya_dev_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/PKG-INFO` & `anedya_dev_sdk-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 6564  : 2.1.Name: aned
 00000020: 7961 2d64 6576 2d73 646b 0a56 6572 7369  ya-dev-sdk.Versi
-00000030: 6f6e 3a20 302e 312e 320a 5375 6d6d 6172  on: 0.1.2.Summar
+00000030: 6f6e 3a20 302e 312e 330a 5375 6d6d 6172  on: 0.1.3.Summar
 00000040: 793a 2041 6e65 6479 6120 7079 7468 6f6e  y: Anedya python
 00000050: 2062 6173 6564 2053 444b 2066 6f72 2049   based SDK for I
 00000060: 6f54 2064 6576 6963 6573 2e20 5468 6973  oT devices. This
 00000070: 2053 444b 2073 7472 6561 6d6c 696e 6573   SDK streamlines
 00000080: 2063 6f6e 6e65 6374 6976 6974 7920 7769   connectivity wi
 00000090: 7468 2041 6e65 6479 6120 706c 6174 666f  th Anedya platfo
 000000a0: 726d 2e20 4173 2074 6869 7320 5344 4b20  rm. As this SDK 
@@ -67,90 +67,87 @@
 00000420: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
 00000430: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
 00000440: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
 00000450: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
 00000460: 6972 6573 2d44 6973 743a 2072 6571 7565  ires-Dist: reque
 00000470: 7374 730a 5265 7175 6972 6573 2d44 6973  sts.Requires-Dis
 00000480: 743a 2070 6168 6f2d 6d71 7474 3e3d 322e  t: paho-mqtt>=2.
-00000490: 302e 300a 0a3c 703e 0a20 2020 203c 6120  0.0..<p>.    <a 
-000004a0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-000004b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f61  pi.org/project/a
-000004c0: 6e65 6479 612d 6465 762d 7364 6b2f 223e  nedya-dev-sdk/">
-000004d0: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
-000004e0: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
-000004f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000500: 732e 696f 2f70 7970 692f 762f 616e 6564  s.io/pypi/v/aned
-00000510: 7961 2d64 6576 2d73 646b 3f73 7479 6c65  ya-dev-sdk?style
-00000520: 3d66 6f72 2d74 6865 2d62 6164 6765 223e  =for-the-badge">
-00000530: 0a20 2020 203c 2f61 3e26 6e62 7370 3b0a  .    </a>&nbsp;.
-00000540: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000550: 7073 3a2f 2f64 6f63 732e 616e 6564 7961  ps://docs.anedya
-00000560: 2e69 6f3f 7574 6d5f 736f 7572 6365 3d67  .io?utm_source=g
-00000570: 6974 6875 6226 7574 6d5f 6d65 6469 756d  ithub&utm_medium
-00000580: 3d6c 696e 6b26 7574 6d5f 6361 6d70 6169  =link&utm_campai
-00000590: 676e 3d67 6974 6875 622d 7364 6b26 7574  gn=github-sdk&ut
-000005a0: 6d5f 636f 6e74 656e 743d 7079 7468 6f6e  m_content=python
-000005b0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-000005c0: 616c 743d 2241 6e65 6479 6120 446f 6375  alt="Anedya Docu
-000005d0: 6d65 6e74 6174 696f 6e22 2073 7263 3d22  mentation" src="
-000005e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005f0: 6c64 732e 696f 2f62 6164 6765 2f41 6e65  lds.io/badge/Ane
-00000600: 6479 612d 446f 6375 6d65 6e74 6174 696f  dya-Documentatio
-00000610: 6e2d 626c 7565 3f73 7479 6c65 3d66 6f72  n-blue?style=for
-00000620: 2d74 6865 2d62 6164 6765 223e 0a20 2020  -the-badge">.   
-00000630: 203c 2f61 3e0a 3c2f 703e 0a0a 0a20 3c21   </a>.</p>... <!
-00000640: 2d2d 2d3c 6469 7620 7374 796c 653d 2277  ---<div style="w
-00000650: 6964 7468 3a32 3025 3b20 6d61 7267 696e  idth:20%; margin
-00000660: 3a30 2061 7574 6f3b 6d61 7267 696e 2d62  :0 auto;margin-b
-00000670: 6f74 746f 6d3a 3530 7078 3b6d 6172 6769  ottom:50px;margi
-00000680: 6e2d 746f 703a 3530 7078 3b22 3e2d 2d3e  n-top:50px;">-->
-00000690: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000006a0: 7222 3e0a 2020 2020 3c69 6d67 2073 7263  r">.    <img src
-000006b0: 3d22 6874 7470 733a 2f2f 6364 6e2e 616e  ="https://cdn.an
-000006c0: 6564 7961 2e69 6f2f 616e 6564 7961 5f62  edya.io/anedya_b
-000006d0: 6c61 636b 5f62 616e 6e65 722e 706e 6722  lack_banner.png"
-000006e0: 2061 6c74 3d22 4c6f 676f 223e 0a3c 2f70   alt="Logo">.</p
-000006f0: 3e0a 3c21 2d2d 3c2f 6469 763e 2d2d 3e0a  >.<!--</div>-->.
-00000700: 0a23 2041 6e65 6479 6120 5344 4b0a 0a54  .# Anedya SDK..T
-00000710: 6865 202a 2a41 6e65 6479 6120 5344 4b2a  he **Anedya SDK*
-00000720: 2a20 6973 2061 2050 7974 686f 6e20 7061  * is a Python pa
-00000730: 636b 6167 6520 6465 7369 676e 6564 2074  ckage designed t
-00000740: 6f20 7072 6f76 6964 6520 616e 2065 6173  o provide an eas
-00000750: 792d 746f 2d75 7365 2069 6e74 6572 6661  y-to-use interfa
-00000760: 6365 2066 6f72 205b 416e 6564 7961 5d28  ce for [Anedya](
-00000770: 6874 7470 733a 2f2f 616e 6564 7961 2e69  https://anedya.i
-00000780: 6f2f 3f75 746d 5f73 6f75 7263 653d 6769  o/?utm_source=gi
-00000790: 7468 7562 2675 746d 5f6d 6564 6975 6d3d  thub&utm_medium=
-000007a0: 6c69 6e6b 2675 746d 5f63 616d 7061 6967  link&utm_campaig
-000007b0: 6e3d 6769 7468 7562 2d73 646b 2675 746d  n=github-sdk&utm
-000007c0: 5f63 6f6e 7465 6e74 3d70 7974 686f 6e29  _content=python)
-000007d0: 2063 6c6f 7564 2073 6572 7669 6365 732c   cloud services,
-000007e0: 2077 6869 6368 2065 6e61 626c 6573 2073   which enables s
-000007f0: 6561 6d6c 6573 7320 636f 6e6e 6563 7469  eamless connecti
-00000800: 7669 7479 2061 6e64 2064 6174 6120 7265  vity and data re
-00000810: 7472 6965 7661 6c20 6672 6f6d 2049 6f54  trieval from IoT
-00000820: 2064 6576 6963 6573 2e20 5468 6973 2053   devices. This S
-00000830: 444b 2073 7570 706f 7274 7320 626f 7468  DK supports both
-00000840: 204d 5154 5420 616e 6420 4854 5450 2063   MQTT and HTTP c
-00000850: 6f6d 6d75 6e69 6361 7469 6f6e 206d 6574  ommunication met
-00000860: 686f 6473 2e0a 0a54 6869 7320 5344 4b20  hods...This SDK 
-00000870: 7772 6170 7320 7468 6520 4465 7669 6365  wraps the Device
-00000880: 2041 5049 7320 6176 6169 6c61 626c 6520   APIs available 
-00000890: 696e 2074 6865 205b 416e 6564 7961 2044  in the [Anedya D
-000008a0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000008b0: 7470 733a 2f2f 646f 6373 2e61 6e65 6479  tps://docs.anedy
-000008c0: 612e 696f 3f75 746d 5f73 6f75 7263 653d  a.io?utm_source=
-000008d0: 6769 7468 7562 2675 746d 5f6d 6564 6975  github&utm_mediu
-000008e0: 6d3d 6c69 6e6b 2675 746d 5f63 616d 7061  m=link&utm_campa
-000008f0: 6967 6e3d 6769 7468 7562 2d73 646b 2675  ign=github-sdk&u
-00000900: 746d 5f63 6f6e 7465 6e74 3d70 7974 686f  tm_content=pytho
-00000910: 6e29 0a0a 5468 6973 2069 7320 6120 4465  n)..This is a De
-00000920: 7669 6365 2053 444b 2c20 692e 652e 2069  vice SDK, i.e. i
-00000930: 7420 6973 206d 6561 6e74 2074 6f20 6265  t is meant to be
-00000940: 2075 7365 6420 6279 2061 6e20 496f 5420   used by an IoT 
-00000950: 6465 7669 6365 2e0a 0a23 2320 496e 7374  device...## Inst
-00000960: 616c 6c61 7469 6f6e 0a0a 546f 2069 6e73  allation..To ins
-00000970: 7461 6c6c 2074 6865 2041 6e65 6479 6120  tall the Anedya 
-00000980: 5344 4b2c 2079 6f75 2063 616e 2075 7365  SDK, you can use
-00000990: 2060 7069 7060 3a0a 0a60 6060 6261 7368   `pip`:..```bash
-000009a0: 0a70 6970 2069 6e73 7461 6c6c 2061 6e65  .pip install ane
-000009b0: 6479 612d 6465 762d 7364 6b0a 6060 600a  dya-dev-sdk.```.
+00000490: 302e 300a 0a5b 3c69 6d67 2061 6c74 3d22  0.0..[<img alt="
+000004a0: 5079 5049 2220 7372 633d 2268 7474 7073  PyPI" src="https
+000004b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004c0: 6f2f 7079 7069 2f76 2f61 6e65 6479 612d  o/pypi/v/anedya-
+000004d0: 6465 762d 7364 6b3f 7374 796c 653d 666f  dev-sdk?style=fo
+000004e0: 722d 7468 652d 6261 6467 6522 3e5d 2868  r-the-badge">](h
+000004f0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000500: 7072 6f6a 6563 742f 616e 6564 7961 2d64  project/anedya-d
+00000510: 6576 2d73 646b 2f29 266e 6273 703b 266e  ev-sdk/)&nbsp;&n
+00000520: 6273 703b 5b3c 696d 6720 616c 743d 2241  bsp;[<img alt="A
+00000530: 6e65 6479 6120 446f 6375 6d65 6e74 6174  nedya Documentat
+00000540: 696f 6e22 2073 7263 3d22 6874 7470 733a  ion" src="https:
+00000550: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000560: 2f62 6164 6765 2f41 6e65 6479 612d 446f  /badge/Anedya-Do
+00000570: 6375 6d65 6e74 6174 696f 6e2d 626c 7565  cumentation-blue
+00000580: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+00000590: 6164 6765 223e 5d28 6874 7470 733a 2f2f  adge">](https://
+000005a0: 646f 6373 2e61 6e65 6479 612e 696f 3f75  docs.anedya.io?u
+000005b0: 746d 5f73 6f75 7263 653d 6769 7468 7562  tm_source=github
+000005c0: 2675 746d 5f6d 6564 6975 6d3d 6c69 6e6b  &utm_medium=link
+000005d0: 2675 746d 5f63 616d 7061 6967 6e3d 6769  &utm_campaign=gi
+000005e0: 7468 7562 2d73 646b 2675 746d 5f63 6f6e  thub-sdk&utm_con
+000005f0: 7465 6e74 3d70 7974 686f 6e29 0a0a 0a20  tent=python)... 
+00000600: 3c21 2d2d 2d3c 6469 7620 7374 796c 653d  <!---<div style=
+00000610: 2277 6964 7468 3a32 3025 3b20 6d61 7267  "width:20%; marg
+00000620: 696e 3a30 2061 7574 6f3b 6d61 7267 696e  in:0 auto;margin
+00000630: 2d62 6f74 746f 6d3a 3530 7078 3b6d 6172  -bottom:50px;mar
+00000640: 6769 6e2d 746f 703a 3530 7078 3b22 3e2d  gin-top:50px;">-
+00000650: 2d3e 0a3c 7020 616c 6967 6e3d 2263 656e  ->.<p align="cen
+00000660: 7465 7222 3e0a 2020 2020 3c69 6d67 2073  ter">.    <img s
+00000670: 7263 3d22 6874 7470 733a 2f2f 6364 6e2e  rc="https://cdn.
+00000680: 616e 6564 7961 2e69 6f2f 616e 6564 7961  anedya.io/anedya
+00000690: 5f62 6c61 636b 5f62 616e 6e65 722e 706e  _black_banner.pn
+000006a0: 6722 2061 6c74 3d22 4c6f 676f 223e 0a3c  g" alt="Logo">.<
+000006b0: 2f70 3e0a 3c21 2d2d 3c2f 6469 763e 2d2d  /p>.<!--</div>--
+000006c0: 3e0a 0a23 2041 6e65 6479 6120 5344 4b0a  >..# Anedya SDK.
+000006d0: 0a54 6865 202a 2a41 6e65 6479 6120 5344  .The **Anedya SD
+000006e0: 4b2a 2a20 6973 2061 2050 7974 686f 6e20  K** is a Python 
+000006f0: 7061 636b 6167 6520 6465 7369 676e 6564  package designed
+00000700: 2074 6f20 7072 6f76 6964 6520 616e 2065   to provide an e
+00000710: 6173 792d 746f 2d75 7365 2069 6e74 6572  asy-to-use inter
+00000720: 6661 6365 2066 6f72 205b 416e 6564 7961  face for [Anedya
+00000730: 5d28 6874 7470 733a 2f2f 616e 6564 7961  ](https://anedya
+00000740: 2e69 6f2f 3f75 746d 5f73 6f75 7263 653d  .io/?utm_source=
+00000750: 6769 7468 7562 2675 746d 5f6d 6564 6975  github&utm_mediu
+00000760: 6d3d 6c69 6e6b 2675 746d 5f63 616d 7061  m=link&utm_campa
+00000770: 6967 6e3d 6769 7468 7562 2d73 646b 2675  ign=github-sdk&u
+00000780: 746d 5f63 6f6e 7465 6e74 3d70 7974 686f  tm_content=pytho
+00000790: 6e29 2063 6c6f 7564 2073 6572 7669 6365  n) cloud service
+000007a0: 732c 2077 6869 6368 2065 6e61 626c 6573  s, which enables
+000007b0: 2073 6561 6d6c 6573 7320 636f 6e6e 6563   seamless connec
+000007c0: 7469 7669 7479 2061 6e64 2064 6174 6120  tivity and data 
+000007d0: 7265 7472 6965 7661 6c20 6672 6f6d 2049  retrieval from I
+000007e0: 6f54 2064 6576 6963 6573 2e20 5468 6973  oT devices. This
+000007f0: 2053 444b 2073 7570 706f 7274 7320 626f   SDK supports bo
+00000800: 7468 204d 5154 5420 616e 6420 4854 5450  th MQTT and HTTP
+00000810: 2063 6f6d 6d75 6e69 6361 7469 6f6e 206d   communication m
+00000820: 6574 686f 6473 2e0a 0a54 6869 7320 5344  ethods...This SD
+00000830: 4b20 7772 6170 7320 7468 6520 4465 7669  K wraps the Devi
+00000840: 6365 2041 5049 7320 6176 6169 6c61 626c  ce APIs availabl
+00000850: 6520 696e 2074 6865 205b 416e 6564 7961  e in the [Anedya
+00000860: 2044 6f63 756d 656e 7461 7469 6f6e 5d28   Documentation](
+00000870: 6874 7470 733a 2f2f 646f 6373 2e61 6e65  https://docs.ane
+00000880: 6479 612e 696f 3f75 746d 5f73 6f75 7263  dya.io?utm_sourc
+00000890: 653d 6769 7468 7562 2675 746d 5f6d 6564  e=github&utm_med
+000008a0: 6975 6d3d 6c69 6e6b 2675 746d 5f63 616d  ium=link&utm_cam
+000008b0: 7061 6967 6e3d 6769 7468 7562 2d73 646b  paign=github-sdk
+000008c0: 2675 746d 5f63 6f6e 7465 6e74 3d70 7974  &utm_content=pyt
+000008d0: 686f 6e29 0a0a 5468 6973 2069 7320 6120  hon)..This is a 
+000008e0: 4465 7669 6365 2053 444b 2c20 692e 652e  Device SDK, i.e.
+000008f0: 2069 7420 6973 206d 6561 6e74 2074 6f20   it is meant to 
+00000900: 6265 2075 7365 6420 6279 2061 6e20 496f  be used by an Io
+00000910: 5420 6465 7669 6365 2e0a 0a23 2320 496e  T device...## In
+00000920: 7374 616c 6c61 7469 6f6e 0a0a 546f 2069  stallation..To i
+00000930: 6e73 7461 6c6c 2074 6865 2041 6e65 6479  nstall the Anedy
+00000940: 6120 5344 4b2c 2079 6f75 2063 616e 2075  a SDK, you can u
+00000950: 7365 2060 7069 7060 3a0a 0a60 6060 6261  se `pip`:..```ba
+00000960: 7368 0a70 6970 2069 6e73 7461 6c6c 2061  sh.pip install a
+00000970: 6e65 6479 612d 6465 762d 7364 6b0a 6060  nedya-dev-sdk.``
+00000980: 600a                                     `.
```

### Comparing `anedya-dev-sdk-0.1.2/README.md` & `anedya_dev_sdk-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,79 @@
-00000000: 3c70 3e0a 2020 2020 3c61 2068 7265 663d  <p>.    <a href=
-00000010: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-00000020: 672f 7072 6f6a 6563 742f 616e 6564 7961  g/project/anedya
-00000030: 2d64 6576 2d73 646b 2f22 3e0a 2020 2020  -dev-sdk/">.    
-00000040: 2020 2020 3c69 6d67 2061 6c74 3d22 5079      <img alt="Py
-00000050: 5049 2220 7372 633d 2268 7474 7073 3a2f  PI" src="https:/
-00000060: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000070: 7079 7069 2f76 2f61 6e65 6479 612d 6465  pypi/v/anedya-de
-00000080: 762d 7364 6b3f 7374 796c 653d 666f 722d  v-sdk?style=for-
-00000090: 7468 652d 6261 6467 6522 3e0a 2020 2020  the-badge">.    
-000000a0: 3c2f 613e 266e 6273 703b 0a20 2020 203c  </a>&nbsp;.    <
-000000b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000000c0: 646f 6373 2e61 6e65 6479 612e 696f 3f75  docs.anedya.io?u
-000000d0: 746d 5f73 6f75 7263 653d 6769 7468 7562  tm_source=github
-000000e0: 2675 746d 5f6d 6564 6975 6d3d 6c69 6e6b  &utm_medium=link
-000000f0: 2675 746d 5f63 616d 7061 6967 6e3d 6769  &utm_campaign=gi
-00000100: 7468 7562 2d73 646b 2675 746d 5f63 6f6e  thub-sdk&utm_con
-00000110: 7465 6e74 3d70 7974 686f 6e22 3e0a 2020  tent=python">.  
-00000120: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
-00000130: 416e 6564 7961 2044 6f63 756d 656e 7461  Anedya Documenta
-00000140: 7469 6f6e 2220 7372 633d 2268 7474 7073  tion" src="https
-00000150: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000160: 6f2f 6261 6467 652f 416e 6564 7961 2d44  o/badge/Anedya-D
-00000170: 6f63 756d 656e 7461 7469 6f6e 2d62 6c75  ocumentation-blu
-00000180: 653f 7374 796c 653d 666f 722d 7468 652d  e?style=for-the-
-00000190: 6261 6467 6522 3e0a 2020 2020 3c2f 613e  badge">.    </a>
-000001a0: 0a3c 2f70 3e0a 0a0a 203c 212d 2d2d 3c64  .</p>... <!---<d
-000001b0: 6976 2073 7479 6c65 3d22 7769 6474 683a  iv style="width:
-000001c0: 3230 253b 206d 6172 6769 6e3a 3020 6175  20%; margin:0 au
-000001d0: 746f 3b6d 6172 6769 6e2d 626f 7474 6f6d  to;margin-bottom
-000001e0: 3a35 3070 783b 6d61 7267 696e 2d74 6f70  :50px;margin-top
-000001f0: 3a35 3070 783b 223e 2d2d 3e0a 3c70 2061  :50px;">-->.<p a
-00000200: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00000210: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000220: 7073 3a2f 2f63 646e 2e61 6e65 6479 612e  ps://cdn.anedya.
-00000230: 696f 2f61 6e65 6479 615f 626c 6163 6b5f  io/anedya_black_
-00000240: 6261 6e6e 6572 2e70 6e67 2220 616c 743d  banner.png" alt=
-00000250: 224c 6f67 6f22 3e0a 3c2f 703e 0a3c 212d  "Logo">.</p>.<!-
-00000260: 2d3c 2f64 6976 3e2d 2d3e 0a0a 2320 416e  -</div>-->..# An
-00000270: 6564 7961 2053 444b 0a0a 5468 6520 2a2a  edya SDK..The **
-00000280: 416e 6564 7961 2053 444b 2a2a 2069 7320  Anedya SDK** is 
-00000290: 6120 5079 7468 6f6e 2070 6163 6b61 6765  a Python package
-000002a0: 2064 6573 6967 6e65 6420 746f 2070 726f   designed to pro
-000002b0: 7669 6465 2061 6e20 6561 7379 2d74 6f2d  vide an easy-to-
-000002c0: 7573 6520 696e 7465 7266 6163 6520 666f  use interface fo
-000002d0: 7220 5b41 6e65 6479 615d 2868 7474 7073  r [Anedya](https
-000002e0: 3a2f 2f61 6e65 6479 612e 696f 2f3f 7574  ://anedya.io/?ut
-000002f0: 6d5f 736f 7572 6365 3d67 6974 6875 6226  m_source=github&
-00000300: 7574 6d5f 6d65 6469 756d 3d6c 696e 6b26  utm_medium=link&
-00000310: 7574 6d5f 6361 6d70 6169 676e 3d67 6974  utm_campaign=git
-00000320: 6875 622d 7364 6b26 7574 6d5f 636f 6e74  hub-sdk&utm_cont
-00000330: 656e 743d 7079 7468 6f6e 2920 636c 6f75  ent=python) clou
-00000340: 6420 7365 7276 6963 6573 2c20 7768 6963  d services, whic
-00000350: 6820 656e 6162 6c65 7320 7365 616d 6c65  h enables seamle
-00000360: 7373 2063 6f6e 6e65 6374 6976 6974 7920  ss connectivity 
-00000370: 616e 6420 6461 7461 2072 6574 7269 6576  and data retriev
-00000380: 616c 2066 726f 6d20 496f 5420 6465 7669  al from IoT devi
-00000390: 6365 732e 2054 6869 7320 5344 4b20 7375  ces. This SDK su
-000003a0: 7070 6f72 7473 2062 6f74 6820 4d51 5454  pports both MQTT
-000003b0: 2061 6e64 2048 5454 5020 636f 6d6d 756e   and HTTP commun
-000003c0: 6963 6174 696f 6e20 6d65 7468 6f64 732e  ication methods.
-000003d0: 0a0a 5468 6973 2053 444b 2077 7261 7073  ..This SDK wraps
-000003e0: 2074 6865 2044 6576 6963 6520 4150 4973   the Device APIs
-000003f0: 2061 7661 696c 6162 6c65 2069 6e20 7468   available in th
-00000400: 6520 5b41 6e65 6479 6120 446f 6375 6d65  e [Anedya Docume
-00000410: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-00000420: 2f64 6f63 732e 616e 6564 7961 2e69 6f3f  /docs.anedya.io?
-00000430: 7574 6d5f 736f 7572 6365 3d67 6974 6875  utm_source=githu
-00000440: 6226 7574 6d5f 6d65 6469 756d 3d6c 696e  b&utm_medium=lin
-00000450: 6b26 7574 6d5f 6361 6d70 6169 676e 3d67  k&utm_campaign=g
-00000460: 6974 6875 622d 7364 6b26 7574 6d5f 636f  ithub-sdk&utm_co
-00000470: 6e74 656e 743d 7079 7468 6f6e 290a 0a54  ntent=python)..T
-00000480: 6869 7320 6973 2061 2044 6576 6963 6520  his is a Device 
-00000490: 5344 4b2c 2069 2e65 2e20 6974 2069 7320  SDK, i.e. it is 
-000004a0: 6d65 616e 7420 746f 2062 6520 7573 6564  meant to be used
-000004b0: 2062 7920 616e 2049 6f54 2064 6576 6963   by an IoT devic
-000004c0: 652e 0a0a 2323 2049 6e73 7461 6c6c 6174  e...## Installat
-000004d0: 696f 6e0a 0a54 6f20 696e 7374 616c 6c20  ion..To install 
-000004e0: 7468 6520 416e 6564 7961 2053 444b 2c20  the Anedya SDK, 
-000004f0: 796f 7520 6361 6e20 7573 6520 6070 6970  you can use `pip
-00000500: 603a 0a0a 6060 6062 6173 680a 7069 7020  `:..```bash.pip 
-00000510: 696e 7374 616c 6c20 616e 6564 7961 2d64  install anedya-d
-00000520: 6576 2d73 646b 0a60 6060 0a              ev-sdk.```.
+00000000: 5b3c 696d 6720 616c 743d 2250 7950 4922  [<img alt="PyPI"
+00000010: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000020: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000030: 692f 762f 616e 6564 7961 2d64 6576 2d73  i/v/anedya-dev-s
+00000040: 646b 3f73 7479 6c65 3d66 6f72 2d74 6865  dk?style=for-the
+00000050: 2d62 6164 6765 223e 5d28 6874 7470 733a  -badge">](https:
+00000060: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000070: 6374 2f61 6e65 6479 612d 6465 762d 7364  ct/anedya-dev-sd
+00000080: 6b2f 2926 6e62 7370 3b26 6e62 7370 3b5b  k/)&nbsp;&nbsp;[
+00000090: 3c69 6d67 2061 6c74 3d22 416e 6564 7961  <img alt="Anedya
+000000a0: 2044 6f63 756d 656e 7461 7469 6f6e 2220   Documentation" 
+000000b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000000c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000000d0: 652f 416e 6564 7961 2d44 6f63 756d 656e  e/Anedya-Documen
+000000e0: 7461 7469 6f6e 2d62 6c75 653f 7374 796c  tation-blue?styl
+000000f0: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
+00000100: 3e5d 2868 7474 7073 3a2f 2f64 6f63 732e  >](https://docs.
+00000110: 616e 6564 7961 2e69 6f3f 7574 6d5f 736f  anedya.io?utm_so
+00000120: 7572 6365 3d67 6974 6875 6226 7574 6d5f  urce=github&utm_
+00000130: 6d65 6469 756d 3d6c 696e 6b26 7574 6d5f  medium=link&utm_
+00000140: 6361 6d70 6169 676e 3d67 6974 6875 622d  campaign=github-
+00000150: 7364 6b26 7574 6d5f 636f 6e74 656e 743d  sdk&utm_content=
+00000160: 7079 7468 6f6e 290a 0a0a 203c 212d 2d2d  python)... <!---
+00000170: 3c64 6976 2073 7479 6c65 3d22 7769 6474  <div style="widt
+00000180: 683a 3230 253b 206d 6172 6769 6e3a 3020  h:20%; margin:0 
+00000190: 6175 746f 3b6d 6172 6769 6e2d 626f 7474  auto;margin-bott
+000001a0: 6f6d 3a35 3070 783b 6d61 7267 696e 2d74  om:50px;margin-t
+000001b0: 6f70 3a35 3070 783b 223e 2d2d 3e0a 3c70  op:50px;">-->.<p
+000001c0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000001d0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+000001e0: 7474 7073 3a2f 2f63 646e 2e61 6e65 6479  ttps://cdn.anedy
+000001f0: 612e 696f 2f61 6e65 6479 615f 626c 6163  a.io/anedya_blac
+00000200: 6b5f 6261 6e6e 6572 2e70 6e67 2220 616c  k_banner.png" al
+00000210: 743d 224c 6f67 6f22 3e0a 3c2f 703e 0a3c  t="Logo">.</p>.<
+00000220: 212d 2d3c 2f64 6976 3e2d 2d3e 0a0a 2320  !--</div>-->..# 
+00000230: 416e 6564 7961 2053 444b 0a0a 5468 6520  Anedya SDK..The 
+00000240: 2a2a 416e 6564 7961 2053 444b 2a2a 2069  **Anedya SDK** i
+00000250: 7320 6120 5079 7468 6f6e 2070 6163 6b61  s a Python packa
+00000260: 6765 2064 6573 6967 6e65 6420 746f 2070  ge designed to p
+00000270: 726f 7669 6465 2061 6e20 6561 7379 2d74  rovide an easy-t
+00000280: 6f2d 7573 6520 696e 7465 7266 6163 6520  o-use interface 
+00000290: 666f 7220 5b41 6e65 6479 615d 2868 7474  for [Anedya](htt
+000002a0: 7073 3a2f 2f61 6e65 6479 612e 696f 2f3f  ps://anedya.io/?
+000002b0: 7574 6d5f 736f 7572 6365 3d67 6974 6875  utm_source=githu
+000002c0: 6226 7574 6d5f 6d65 6469 756d 3d6c 696e  b&utm_medium=lin
+000002d0: 6b26 7574 6d5f 6361 6d70 6169 676e 3d67  k&utm_campaign=g
+000002e0: 6974 6875 622d 7364 6b26 7574 6d5f 636f  ithub-sdk&utm_co
+000002f0: 6e74 656e 743d 7079 7468 6f6e 2920 636c  ntent=python) cl
+00000300: 6f75 6420 7365 7276 6963 6573 2c20 7768  oud services, wh
+00000310: 6963 6820 656e 6162 6c65 7320 7365 616d  ich enables seam
+00000320: 6c65 7373 2063 6f6e 6e65 6374 6976 6974  less connectivit
+00000330: 7920 616e 6420 6461 7461 2072 6574 7269  y and data retri
+00000340: 6576 616c 2066 726f 6d20 496f 5420 6465  eval from IoT de
+00000350: 7669 6365 732e 2054 6869 7320 5344 4b20  vices. This SDK 
+00000360: 7375 7070 6f72 7473 2062 6f74 6820 4d51  supports both MQ
+00000370: 5454 2061 6e64 2048 5454 5020 636f 6d6d  TT and HTTP comm
+00000380: 756e 6963 6174 696f 6e20 6d65 7468 6f64  unication method
+00000390: 732e 0a0a 5468 6973 2053 444b 2077 7261  s...This SDK wra
+000003a0: 7073 2074 6865 2044 6576 6963 6520 4150  ps the Device AP
+000003b0: 4973 2061 7661 696c 6162 6c65 2069 6e20  Is available in 
+000003c0: 7468 6520 5b41 6e65 6479 6120 446f 6375  the [Anedya Docu
+000003d0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
+000003e0: 3a2f 2f64 6f63 732e 616e 6564 7961 2e69  ://docs.anedya.i
+000003f0: 6f3f 7574 6d5f 736f 7572 6365 3d67 6974  o?utm_source=git
+00000400: 6875 6226 7574 6d5f 6d65 6469 756d 3d6c  hub&utm_medium=l
+00000410: 696e 6b26 7574 6d5f 6361 6d70 6169 676e  ink&utm_campaign
+00000420: 3d67 6974 6875 622d 7364 6b26 7574 6d5f  =github-sdk&utm_
+00000430: 636f 6e74 656e 743d 7079 7468 6f6e 290a  content=python).
+00000440: 0a54 6869 7320 6973 2061 2044 6576 6963  .This is a Devic
+00000450: 6520 5344 4b2c 2069 2e65 2e20 6974 2069  e SDK, i.e. it i
+00000460: 7320 6d65 616e 7420 746f 2062 6520 7573  s meant to be us
+00000470: 6564 2062 7920 616e 2049 6f54 2064 6576  ed by an IoT dev
+00000480: 6963 652e 0a0a 2323 2049 6e73 7461 6c6c  ice...## Install
+00000490: 6174 696f 6e0a 0a54 6f20 696e 7374 616c  ation..To instal
+000004a0: 6c20 7468 6520 416e 6564 7961 2053 444b  l the Anedya SDK
+000004b0: 2c20 796f 7520 6361 6e20 7573 6520 6070  , you can use `p
+000004c0: 6970 603a 0a0a 6060 6062 6173 680a 7069  ip`:..```bash.pi
+000004d0: 7020 696e 7374 616c 6c20 616e 6564 7961  p install anedya
+000004e0: 2d64 6576 2d73 646b 0a60 6060 0a         -dev-sdk.```.
```

### Comparing `anedya-dev-sdk-0.1.2/setup.cfg` & `anedya_dev_sdk-0.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = anedya-dev-sdk
-version = 0.1.2
+version = 0.1.3
 url = https://github.com/anedyaio/anedya-dev-sdk-pyhton
 author = Anedya Systems
 author_email = support@anedya.io
 description = Anedya python based SDK for IoT devices. This SDK streamlines connectivity with Anedya platform. As this SDK is in Beta release, future versions may have breaking changes.
 long_description = file: README.md
 requires_python = ">=3.7"
 dependencies = ["requests","paho-mqtt>=2.0.0"]
```

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/anedya.py` & `anedya_dev_sdk-0.1.3/src/anedya/anedya.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/client/callbacks.py` & `anedya_dev_sdk-0.1.3/src/anedya/client/callbacks.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/client/certs.py` & `anedya_dev_sdk-0.1.3/src/anedya/client/certs.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/client/mqttHandlers.py` & `anedya_dev_sdk-0.1.3/src/anedya/client/mqttHandlers.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/config.py` & `anedya_dev_sdk-0.1.3/src/anedya/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 import uuid
+from .errors import AnedyaInvalidConfig
 
 
 class ConnectionMode(Enum):
     HTTP = "HTTP"
     MQTT = "MQTT"
 
 
@@ -57,15 +58,18 @@
         """
         self.connection_key = key
 
     def set_deviceid(self, id: str):
         """
         Set DeviceID
         """
-        self._deviceID = uuid.UUID(id)
+        try:
+            self._deviceID = uuid.UUID(id)
+        except ValueError:
+            raise AnedyaInvalidConfig("Device ID needs to be valid UUID")
         self._deviceid_set = True
 
     def set_timeout(self, timeout):
         """
         Set timeout for automatic flush of the data
         """
         self.timeout = timeout
```

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/errors.py` & `anedya_dev_sdk-0.1.3/src/anedya/errors.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/src/anedya/transaction.py` & `anedya_dev_sdk-0.1.3/src/anedya/transaction.py`

 * *Files identical despite different names*

### Comparing `anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/PKG-INFO` & `anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 616e 6564  : 2.1.Name: aned
 00000020: 7961 2d64 6576 2d73 646b 0a56 6572 7369  ya-dev-sdk.Versi
-00000030: 6f6e 3a20 302e 312e 320a 5375 6d6d 6172  on: 0.1.2.Summar
+00000030: 6f6e 3a20 302e 312e 330a 5375 6d6d 6172  on: 0.1.3.Summar
 00000040: 793a 2041 6e65 6479 6120 7079 7468 6f6e  y: Anedya python
 00000050: 2062 6173 6564 2053 444b 2066 6f72 2049   based SDK for I
 00000060: 6f54 2064 6576 6963 6573 2e20 5468 6973  oT devices. This
 00000070: 2053 444b 2073 7472 6561 6d6c 696e 6573   SDK streamlines
 00000080: 2063 6f6e 6e65 6374 6976 6974 7920 7769   connectivity wi
 00000090: 7468 2041 6e65 6479 6120 706c 6174 666f  th Anedya platfo
 000000a0: 726d 2e20 4173 2074 6869 7320 5344 4b20  rm. As this SDK 
@@ -67,90 +67,87 @@
 00000420: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
 00000430: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
 00000440: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
 00000450: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
 00000460: 6972 6573 2d44 6973 743a 2072 6571 7565  ires-Dist: reque
 00000470: 7374 730a 5265 7175 6972 6573 2d44 6973  sts.Requires-Dis
 00000480: 743a 2070 6168 6f2d 6d71 7474 3e3d 322e  t: paho-mqtt>=2.
-00000490: 302e 300a 0a3c 703e 0a20 2020 203c 6120  0.0..<p>.    <a 
-000004a0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-000004b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f61  pi.org/project/a
-000004c0: 6e65 6479 612d 6465 762d 7364 6b2f 223e  nedya-dev-sdk/">
-000004d0: 0a20 2020 2020 2020 203c 696d 6720 616c  .        <img al
-000004e0: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
-000004f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000500: 732e 696f 2f70 7970 692f 762f 616e 6564  s.io/pypi/v/aned
-00000510: 7961 2d64 6576 2d73 646b 3f73 7479 6c65  ya-dev-sdk?style
-00000520: 3d66 6f72 2d74 6865 2d62 6164 6765 223e  =for-the-badge">
-00000530: 0a20 2020 203c 2f61 3e26 6e62 7370 3b0a  .    </a>&nbsp;.
-00000540: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
-00000550: 7073 3a2f 2f64 6f63 732e 616e 6564 7961  ps://docs.anedya
-00000560: 2e69 6f3f 7574 6d5f 736f 7572 6365 3d67  .io?utm_source=g
-00000570: 6974 6875 6226 7574 6d5f 6d65 6469 756d  ithub&utm_medium
-00000580: 3d6c 696e 6b26 7574 6d5f 6361 6d70 6169  =link&utm_campai
-00000590: 676e 3d67 6974 6875 622d 7364 6b26 7574  gn=github-sdk&ut
-000005a0: 6d5f 636f 6e74 656e 743d 7079 7468 6f6e  m_content=python
-000005b0: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
-000005c0: 616c 743d 2241 6e65 6479 6120 446f 6375  alt="Anedya Docu
-000005d0: 6d65 6e74 6174 696f 6e22 2073 7263 3d22  mentation" src="
-000005e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000005f0: 6c64 732e 696f 2f62 6164 6765 2f41 6e65  lds.io/badge/Ane
-00000600: 6479 612d 446f 6375 6d65 6e74 6174 696f  dya-Documentatio
-00000610: 6e2d 626c 7565 3f73 7479 6c65 3d66 6f72  n-blue?style=for
-00000620: 2d74 6865 2d62 6164 6765 223e 0a20 2020  -the-badge">.   
-00000630: 203c 2f61 3e0a 3c2f 703e 0a0a 0a20 3c21   </a>.</p>... <!
-00000640: 2d2d 2d3c 6469 7620 7374 796c 653d 2277  ---<div style="w
-00000650: 6964 7468 3a32 3025 3b20 6d61 7267 696e  idth:20%; margin
-00000660: 3a30 2061 7574 6f3b 6d61 7267 696e 2d62  :0 auto;margin-b
-00000670: 6f74 746f 6d3a 3530 7078 3b6d 6172 6769  ottom:50px;margi
-00000680: 6e2d 746f 703a 3530 7078 3b22 3e2d 2d3e  n-top:50px;">-->
-00000690: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-000006a0: 7222 3e0a 2020 2020 3c69 6d67 2073 7263  r">.    <img src
-000006b0: 3d22 6874 7470 733a 2f2f 6364 6e2e 616e  ="https://cdn.an
-000006c0: 6564 7961 2e69 6f2f 616e 6564 7961 5f62  edya.io/anedya_b
-000006d0: 6c61 636b 5f62 616e 6e65 722e 706e 6722  lack_banner.png"
-000006e0: 2061 6c74 3d22 4c6f 676f 223e 0a3c 2f70   alt="Logo">.</p
-000006f0: 3e0a 3c21 2d2d 3c2f 6469 763e 2d2d 3e0a  >.<!--</div>-->.
-00000700: 0a23 2041 6e65 6479 6120 5344 4b0a 0a54  .# Anedya SDK..T
-00000710: 6865 202a 2a41 6e65 6479 6120 5344 4b2a  he **Anedya SDK*
-00000720: 2a20 6973 2061 2050 7974 686f 6e20 7061  * is a Python pa
-00000730: 636b 6167 6520 6465 7369 676e 6564 2074  ckage designed t
-00000740: 6f20 7072 6f76 6964 6520 616e 2065 6173  o provide an eas
-00000750: 792d 746f 2d75 7365 2069 6e74 6572 6661  y-to-use interfa
-00000760: 6365 2066 6f72 205b 416e 6564 7961 5d28  ce for [Anedya](
-00000770: 6874 7470 733a 2f2f 616e 6564 7961 2e69  https://anedya.i
-00000780: 6f2f 3f75 746d 5f73 6f75 7263 653d 6769  o/?utm_source=gi
-00000790: 7468 7562 2675 746d 5f6d 6564 6975 6d3d  thub&utm_medium=
-000007a0: 6c69 6e6b 2675 746d 5f63 616d 7061 6967  link&utm_campaig
-000007b0: 6e3d 6769 7468 7562 2d73 646b 2675 746d  n=github-sdk&utm
-000007c0: 5f63 6f6e 7465 6e74 3d70 7974 686f 6e29  _content=python)
-000007d0: 2063 6c6f 7564 2073 6572 7669 6365 732c   cloud services,
-000007e0: 2077 6869 6368 2065 6e61 626c 6573 2073   which enables s
-000007f0: 6561 6d6c 6573 7320 636f 6e6e 6563 7469  eamless connecti
-00000800: 7669 7479 2061 6e64 2064 6174 6120 7265  vity and data re
-00000810: 7472 6965 7661 6c20 6672 6f6d 2049 6f54  trieval from IoT
-00000820: 2064 6576 6963 6573 2e20 5468 6973 2053   devices. This S
-00000830: 444b 2073 7570 706f 7274 7320 626f 7468  DK supports both
-00000840: 204d 5154 5420 616e 6420 4854 5450 2063   MQTT and HTTP c
-00000850: 6f6d 6d75 6e69 6361 7469 6f6e 206d 6574  ommunication met
-00000860: 686f 6473 2e0a 0a54 6869 7320 5344 4b20  hods...This SDK 
-00000870: 7772 6170 7320 7468 6520 4465 7669 6365  wraps the Device
-00000880: 2041 5049 7320 6176 6169 6c61 626c 6520   APIs available 
-00000890: 696e 2074 6865 205b 416e 6564 7961 2044  in the [Anedya D
-000008a0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000008b0: 7470 733a 2f2f 646f 6373 2e61 6e65 6479  tps://docs.anedy
-000008c0: 612e 696f 3f75 746d 5f73 6f75 7263 653d  a.io?utm_source=
-000008d0: 6769 7468 7562 2675 746d 5f6d 6564 6975  github&utm_mediu
-000008e0: 6d3d 6c69 6e6b 2675 746d 5f63 616d 7061  m=link&utm_campa
-000008f0: 6967 6e3d 6769 7468 7562 2d73 646b 2675  ign=github-sdk&u
-00000900: 746d 5f63 6f6e 7465 6e74 3d70 7974 686f  tm_content=pytho
-00000910: 6e29 0a0a 5468 6973 2069 7320 6120 4465  n)..This is a De
-00000920: 7669 6365 2053 444b 2c20 692e 652e 2069  vice SDK, i.e. i
-00000930: 7420 6973 206d 6561 6e74 2074 6f20 6265  t is meant to be
-00000940: 2075 7365 6420 6279 2061 6e20 496f 5420   used by an IoT 
-00000950: 6465 7669 6365 2e0a 0a23 2320 496e 7374  device...## Inst
-00000960: 616c 6c61 7469 6f6e 0a0a 546f 2069 6e73  allation..To ins
-00000970: 7461 6c6c 2074 6865 2041 6e65 6479 6120  tall the Anedya 
-00000980: 5344 4b2c 2079 6f75 2063 616e 2075 7365  SDK, you can use
-00000990: 2060 7069 7060 3a0a 0a60 6060 6261 7368   `pip`:..```bash
-000009a0: 0a70 6970 2069 6e73 7461 6c6c 2061 6e65  .pip install ane
-000009b0: 6479 612d 6465 762d 7364 6b0a 6060 600a  dya-dev-sdk.```.
+00000490: 302e 300a 0a5b 3c69 6d67 2061 6c74 3d22  0.0..[<img alt="
+000004a0: 5079 5049 2220 7372 633d 2268 7474 7073  PyPI" src="https
+000004b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004c0: 6f2f 7079 7069 2f76 2f61 6e65 6479 612d  o/pypi/v/anedya-
+000004d0: 6465 762d 7364 6b3f 7374 796c 653d 666f  dev-sdk?style=fo
+000004e0: 722d 7468 652d 6261 6467 6522 3e5d 2868  r-the-badge">](h
+000004f0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000500: 7072 6f6a 6563 742f 616e 6564 7961 2d64  project/anedya-d
+00000510: 6576 2d73 646b 2f29 266e 6273 703b 266e  ev-sdk/)&nbsp;&n
+00000520: 6273 703b 5b3c 696d 6720 616c 743d 2241  bsp;[<img alt="A
+00000530: 6e65 6479 6120 446f 6375 6d65 6e74 6174  nedya Documentat
+00000540: 696f 6e22 2073 7263 3d22 6874 7470 733a  ion" src="https:
+00000550: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000560: 2f62 6164 6765 2f41 6e65 6479 612d 446f  /badge/Anedya-Do
+00000570: 6375 6d65 6e74 6174 696f 6e2d 626c 7565  cumentation-blue
+00000580: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+00000590: 6164 6765 223e 5d28 6874 7470 733a 2f2f  adge">](https://
+000005a0: 646f 6373 2e61 6e65 6479 612e 696f 3f75  docs.anedya.io?u
+000005b0: 746d 5f73 6f75 7263 653d 6769 7468 7562  tm_source=github
+000005c0: 2675 746d 5f6d 6564 6975 6d3d 6c69 6e6b  &utm_medium=link
+000005d0: 2675 746d 5f63 616d 7061 6967 6e3d 6769  &utm_campaign=gi
+000005e0: 7468 7562 2d73 646b 2675 746d 5f63 6f6e  thub-sdk&utm_con
+000005f0: 7465 6e74 3d70 7974 686f 6e29 0a0a 0a20  tent=python)... 
+00000600: 3c21 2d2d 2d3c 6469 7620 7374 796c 653d  <!---<div style=
+00000610: 2277 6964 7468 3a32 3025 3b20 6d61 7267  "width:20%; marg
+00000620: 696e 3a30 2061 7574 6f3b 6d61 7267 696e  in:0 auto;margin
+00000630: 2d62 6f74 746f 6d3a 3530 7078 3b6d 6172  -bottom:50px;mar
+00000640: 6769 6e2d 746f 703a 3530 7078 3b22 3e2d  gin-top:50px;">-
+00000650: 2d3e 0a3c 7020 616c 6967 6e3d 2263 656e  ->.<p align="cen
+00000660: 7465 7222 3e0a 2020 2020 3c69 6d67 2073  ter">.    <img s
+00000670: 7263 3d22 6874 7470 733a 2f2f 6364 6e2e  rc="https://cdn.
+00000680: 616e 6564 7961 2e69 6f2f 616e 6564 7961  anedya.io/anedya
+00000690: 5f62 6c61 636b 5f62 616e 6e65 722e 706e  _black_banner.pn
+000006a0: 6722 2061 6c74 3d22 4c6f 676f 223e 0a3c  g" alt="Logo">.<
+000006b0: 2f70 3e0a 3c21 2d2d 3c2f 6469 763e 2d2d  /p>.<!--</div>--
+000006c0: 3e0a 0a23 2041 6e65 6479 6120 5344 4b0a  >..# Anedya SDK.
+000006d0: 0a54 6865 202a 2a41 6e65 6479 6120 5344  .The **Anedya SD
+000006e0: 4b2a 2a20 6973 2061 2050 7974 686f 6e20  K** is a Python 
+000006f0: 7061 636b 6167 6520 6465 7369 676e 6564  package designed
+00000700: 2074 6f20 7072 6f76 6964 6520 616e 2065   to provide an e
+00000710: 6173 792d 746f 2d75 7365 2069 6e74 6572  asy-to-use inter
+00000720: 6661 6365 2066 6f72 205b 416e 6564 7961  face for [Anedya
+00000730: 5d28 6874 7470 733a 2f2f 616e 6564 7961  ](https://anedya
+00000740: 2e69 6f2f 3f75 746d 5f73 6f75 7263 653d  .io/?utm_source=
+00000750: 6769 7468 7562 2675 746d 5f6d 6564 6975  github&utm_mediu
+00000760: 6d3d 6c69 6e6b 2675 746d 5f63 616d 7061  m=link&utm_campa
+00000770: 6967 6e3d 6769 7468 7562 2d73 646b 2675  ign=github-sdk&u
+00000780: 746d 5f63 6f6e 7465 6e74 3d70 7974 686f  tm_content=pytho
+00000790: 6e29 2063 6c6f 7564 2073 6572 7669 6365  n) cloud service
+000007a0: 732c 2077 6869 6368 2065 6e61 626c 6573  s, which enables
+000007b0: 2073 6561 6d6c 6573 7320 636f 6e6e 6563   seamless connec
+000007c0: 7469 7669 7479 2061 6e64 2064 6174 6120  tivity and data 
+000007d0: 7265 7472 6965 7661 6c20 6672 6f6d 2049  retrieval from I
+000007e0: 6f54 2064 6576 6963 6573 2e20 5468 6973  oT devices. This
+000007f0: 2053 444b 2073 7570 706f 7274 7320 626f   SDK supports bo
+00000800: 7468 204d 5154 5420 616e 6420 4854 5450  th MQTT and HTTP
+00000810: 2063 6f6d 6d75 6e69 6361 7469 6f6e 206d   communication m
+00000820: 6574 686f 6473 2e0a 0a54 6869 7320 5344  ethods...This SD
+00000830: 4b20 7772 6170 7320 7468 6520 4465 7669  K wraps the Devi
+00000840: 6365 2041 5049 7320 6176 6169 6c61 626c  ce APIs availabl
+00000850: 6520 696e 2074 6865 205b 416e 6564 7961  e in the [Anedya
+00000860: 2044 6f63 756d 656e 7461 7469 6f6e 5d28   Documentation](
+00000870: 6874 7470 733a 2f2f 646f 6373 2e61 6e65  https://docs.ane
+00000880: 6479 612e 696f 3f75 746d 5f73 6f75 7263  dya.io?utm_sourc
+00000890: 653d 6769 7468 7562 2675 746d 5f6d 6564  e=github&utm_med
+000008a0: 6975 6d3d 6c69 6e6b 2675 746d 5f63 616d  ium=link&utm_cam
+000008b0: 7061 6967 6e3d 6769 7468 7562 2d73 646b  paign=github-sdk
+000008c0: 2675 746d 5f63 6f6e 7465 6e74 3d70 7974  &utm_content=pyt
+000008d0: 686f 6e29 0a0a 5468 6973 2069 7320 6120  hon)..This is a 
+000008e0: 4465 7669 6365 2053 444b 2c20 692e 652e  Device SDK, i.e.
+000008f0: 2069 7420 6973 206d 6561 6e74 2074 6f20   it is meant to 
+00000900: 6265 2075 7365 6420 6279 2061 6e20 496f  be used by an Io
+00000910: 5420 6465 7669 6365 2e0a 0a23 2320 496e  T device...## In
+00000920: 7374 616c 6c61 7469 6f6e 0a0a 546f 2069  stallation..To i
+00000930: 6e73 7461 6c6c 2074 6865 2041 6e65 6479  nstall the Anedy
+00000940: 6120 5344 4b2c 2079 6f75 2063 616e 2075  a SDK, you can u
+00000950: 7365 2060 7069 7060 3a0a 0a60 6060 6261  se `pip`:..```ba
+00000960: 7368 0a70 6970 2069 6e73 7461 6c6c 2061  sh.pip install a
+00000970: 6e65 6479 612d 6465 762d 7364 6b0a 6060  nedya-dev-sdk.``
+00000980: 600a                                     `.
```

### Comparing `anedya-dev-sdk-0.1.2/src/anedya_dev_sdk.egg-info/SOURCES.txt` & `anedya_dev_sdk-0.1.3/src/anedya_dev_sdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/anedya/transaction.py
 src/anedya/client/__init__.py
 src/anedya/client/bindDevice.py
 src/anedya/client/callbacks.py
 src/anedya/client/certs.py
 src/anedya/client/mqttHandlers.py
 src/anedya/client/submitData.py
+src/anedya/client/submitLogs.py
 src/anedya/client/timeSync.py
 src/anedya_dev_sdk.egg-info/PKG-INFO
 src/anedya_dev_sdk.egg-info/SOURCES.txt
 src/anedya_dev_sdk.egg-info/dependency_links.txt
 src/anedya_dev_sdk.egg-info/requires.txt
 src/anedya_dev_sdk.egg-info/top_level.txt
 tests/test_config.py
```

### Comparing `anedya-dev-sdk-0.1.2/tests/test_config.py` & `anedya_dev_sdk-0.1.3/tests/test_config.py`

 * *Files identical despite different names*

