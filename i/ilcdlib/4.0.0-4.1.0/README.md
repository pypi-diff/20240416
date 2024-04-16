# Comparing `tmp/ilcdlib-4.0.0.tar.gz` & `tmp/ilcdlib-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.0.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.1.0.tar", max compression
```

## Comparing `ilcdlib-4.0.0.tar` & `ilcdlib-4.1.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0    11357 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/LICENSE
--rw-r--r--   0        0        0     5311 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/README.md
--rw-r--r--   0        0        0     3525 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17587 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1796 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4703 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6946 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4160 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4226 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-04-15 14:41:50.180519 ilcdlib-4.0.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3797 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10086 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     1329 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2217 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3440 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    32351 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2067 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     2588 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1735 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    10655 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2513 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3682 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-04-15 14:41:50.184519 ilcdlib-4.0.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6444 1970-01-01 00:00:00.000000 ilcdlib-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 15:22:15.327666 ilcdlib-4.1.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-04-16 15:22:15.327666 ilcdlib-4.1.0/README.md
+-rw-r--r--   0        0        0     3525 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17587 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1796 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4407 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6946 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4160 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4230 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3797 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     1329 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2217 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3440 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    32351 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2067 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     2588 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-04-16 15:22:15.331667 ilcdlib-4.1.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1735 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    10655 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2513 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3682 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-04-16 15:22:15.335667 ilcdlib-4.1.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.1.0/PKG-INFO
```

### Comparing `ilcdlib-4.0.0/LICENSE` & `ilcdlib-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/README.md` & `ilcdlib-4.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,14 @@
 If you don't need CLI tool, you can omit `cli` extra. The following extras are available:
 
 * `lxml` - install lxml library for faster XML parsing
 * `cli` - install CLI tool so it could be used from command line via `ilcdtool` command.
 
 ## Usage
 
-**❗ ATTENTION**: Pick the right version. There are 2 versions of the library available:
-
-* Use version **below** `2.0.0` if your project uses Pydantic version below `2.0.0`
-* Use version `2.x.x` or higher if your project uses Pydantic version `2.0.0` or above
-
-Branch 1.x.x is not maintained anymore, so if you don't use pydantic 2.x.x should be your choice.
-
 ### CLI
 
 At the moment the primary function of the CLI tool is to convert ILCD XML files to openEPD (json) format. 
 
 Here is a simple example of how to use it to convert ILCD archive to openEPD format:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -11,23 +11,18 @@
            _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_c_c_h_a_n_g_e_l_a_b_s_/_i_l_c_d_l_i_b_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 Python library providing parsing capabilities for ILCD XML files. ##
 Installation Install the library from PyPi. The following command will install
 the library with all optional dependencies: ```bash pip install "ilcdlib
 [lxml,cli]" ``` If you don't need CLI tool, you can omit `cli` extra. The
 following extras are available: * `lxml` - install lxml library for faster XML
 parsing * `cli` - install CLI tool so it could be used from command line via
-`ilcdtool` command. ## Usage **â ATTENTION**: Pick the right version. There
-are 2 versions of the library available: * Use version **below** `2.0.0` if
-your project uses Pydantic version below `2.0.0` * Use version `2.x.x` or
-higher if your project uses Pydantic version `2.0.0` or above Branch 1.x.x is
-not maintained anymore, so if you don't use pydantic 2.x.x should be your
-choice. ### CLI At the moment the primary function of the CLI tool is to
-convert ILCD XML files to openEPD (json) format. Here is a simple example of
-how to use it to convert ILCD archive to openEPD format: ```bash ilcdtool --
-debug convert-epd -i ilcd+epd -o openEPD "
+`ilcdtool` command. ## Usage ### CLI At the moment the primary function of the
+CLI tool is to convert ILCD XML files to openEPD (json) format. Here is a
+simple example of how to use it to convert ILCD archive to openEPD format:
+```bash ilcdtool --debug convert-epd -i ilcd+epd -o openEPD "
 o/archive.zip>" ``` It is also possible to point the tool to the http endpoint
 instead. At the moment Soda4Lca web UI and api endpoints are supported. ```bash
 ilcdtool convert-epd -i ilcd+epd -o openEPD "https://oekobaudat.de/OEKOBAU.DAT/
 datasetdetail/process.xhtml?uuid=ee8863aa-7276-4896-b07a-
 713937a3134d&version=00.00.018&stock=OBD_2021_II〈=en" ``` Another important
 feature is the ability to specify a **dialect**. Dialect is a set of rules that
 define how the handle provider specific data. It is useful for the cases when
```

### Comparing `ilcdlib-4.0.0/pyproject.toml` & `ilcdlib-4.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.0.0"
+version = "4.1.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.0.0/src/ilcdlib/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/__main__.py` & `ilcdlib-4.1.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/__version__.py` & `ilcdlib-4.1.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/cli.py` & `ilcdlib-4.1.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/common.py` & `ilcdlib-4.1.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.1.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/const.py` & `ilcdlib-4.1.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.1.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/dto.py` & `ilcdlib-4.1.0/src/ilcdlib/dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,39 +99,21 @@
 
     pass
 
 
 class IlcdContactInfo(BaseOpenEpdSchema):
     """Contact information extracted from ILCD contact."""
 
-    contact_person: str | None = pyd.Field(
-        default=None,
-        description="Name of the contact person",
-        json_schema_extra=dict(example="John Doe"),
-    )
-    email: pyd.EmailStr | None = pyd.Field(
-        default=None,
-        description="Email",
-        json_schema_extra=dict(example="contact@c-change-labs.com"),
-    )
-    phone: str | None = pyd.Field(
-        default=None,
-        description="Phone number",
-        json_schema_extra=dict(example="+15263327352"),
-    )
+    contact_person: str | None = pyd.Field(description="Name of the contact person", example="John Doe", default=None)
+    email: pyd.EmailStr | None = pyd.Field(description="Email", example="contact@c-change-labs.com", default=None)
+    phone: str | None = pyd.Field(description="Phone number", example="+15263327352", default=None)
     website: pyd.AnyUrl | None = pyd.Field(
-        default=None,
-        description="Url of the website",
-        json_schema_extra=dict(example="http://buildingtransparency.org"),
-    )
-    address: str | None = pyd.Field(
-        default=None,
-        description="Address",
-        json_schema_extra=dict(example="123 Main St, San Francisco, CA 94105"),
+        description="Url of the website", example="http://buildingtransparency.org", default=None
     )
+    address: str | None = pyd.Field(description="Address", example="123 Main St, San Francisco, CA 94105", default=None)
 
 
 class OpenEpdIlcdOrg(Org):
     """Org object with ILCD specific extension."""
 
     def get_contact(self) -> IlcdContactInfo | None:
         """Return ILCD contact information from extension field if any."""
@@ -141,18 +123,18 @@
         return ext.contact if ext else None
 
 
 class ComplianceDto(pyd.BaseModel):
     """Basic information about a Compliance."""
 
     uuid: str
-    short_name: str | None = None
-    name: str | None = None
-    link: str | None = None
-    issuer: OpenEpdIlcdOrg | None = None
+    short_name: str | None
+    name: str | None
+    link: str | None
+    issuer: OpenEpdIlcdOrg | None
 
 
 class ValidationDto(pyd.BaseModel):
     """Basic information about a Compliance."""
 
-    validation_type: IlcdTypeOfReview | None = None
+    validation_type: IlcdTypeOfReview | None
     org: OpenEpdIlcdOrg
```

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/lcia.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,10 +98,10 @@
         scenario_names: dict[str, str],
         lcia_method: str | None = None,
         base_url: str | None = None,
         provider_domain: str | None = None,
     ) -> Impacts:
         """Read as openEPD ImpactSet object."""
         impact_set = self.get_impact_set(scenario_names)
-        impacts = Impacts(root={})
+        impacts = Impacts(__root__={})
         impacts.set_impact_set(lcia_method, impact_set)
         return impacts
```

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.1.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,27 +196,27 @@
             )
         lang_list = [lang, None]
         if prioritize_english:
             lang_list.insert(0, "en")
         CLI.print_info("Language priority: " + ",".join([x if x is not None else "any other" for x in lang_list]))
         base_url = self.__extract_base_url(doc_ref)
         open_epd = epd_reader.to_openepd_epd(lang_list, base_url=base_url, provider_domain=provider_domain)
-        CLI.print_data(open_epd.model_dump_json(indent=2, exclude_none=True, exclude_unset=True))
+        CLI.print_data(open_epd.json(indent=2, exclude_none=True, exclude_unset=True))
         if save:
             self.save_results(epd_reader, open_epd, extract_pdf=extract_pdf, base_dir=target_dir)
 
     def save_results(
         self, epd_reader: IlcdEpdReader, result: Epd, *, extract_pdf: bool = False, base_dir: Path | None = None
     ):
         if base_dir is None:
             base_dir = Path.cwd()
         output_dir = base_dir / Path(epd_reader.get_uuid())
         ensure_dir(output_dir)
         with open(output_dir / "openEPD.json", "w") as f:
-            f.write(result.model_dump_json(indent=2, exclude_none=True, exclude_unset=True))
+            f.write(result.json(indent=2, exclude_none=True, exclude_unset=True))
         if isinstance(epd_reader.data_provider, ZipIlcdReader):
             epd_reader.data_provider.save_to(output_dir / "ilcd_epd.zip")
         if extract_pdf:
             # EPD Pdf
             pdf_stream = epd_reader.get_epd_document_stream()
             if pdf_stream is None and isinstance(epd_reader.data_provider, Soda4LcaZipReader):
                 try:
```

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.1.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/extension.py` & `ilcdlib-4.1.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/http_common.py` & `ilcdlib-4.1.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/common.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/mapping/units.py` & `ilcdlib-4.1.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.1.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.1.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.1.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.1.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.1.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.1.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.1.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.1.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/type.py` & `ilcdlib-4.1.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/utils.py` & `ilcdlib-4.1.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.1.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.0.0/PKG-INFO` & `ilcdlib-4.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.0.0
+Version: 4.1.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
@@ -55,21 +55,14 @@
 If you don't need CLI tool, you can omit `cli` extra. The following extras are available:
 
 * `lxml` - install lxml library for faster XML parsing
 * `cli` - install CLI tool so it could be used from command line via `ilcdtool` command.
 
 ## Usage
 
-**❗ ATTENTION**: Pick the right version. There are 2 versions of the library available:
-
-* Use version **below** `2.0.0` if your project uses Pydantic version below `2.0.0`
-* Use version `2.x.x` or higher if your project uses Pydantic version `2.0.0` or above
-
-Branch 1.x.x is not maintained anymore, so if you don't use pydantic 2.x.x should be your choice.
-
 ### CLI
 
 At the moment the primary function of the CLI tool is to convert ILCD XML files to openEPD (json) format. 
 
 Here is a simple example of how to use it to convert ILCD archive to openEPD format:
 
 ```bash
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.0.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.1.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
@@ -26,23 +26,18 @@
            _g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_c_c_h_a_n_g_e_l_a_b_s_/_i_l_c_d_l_i_b_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 Python library providing parsing capabilities for ILCD XML files. ##
 Installation Install the library from PyPi. The following command will install
 the library with all optional dependencies: ```bash pip install "ilcdlib
 [lxml,cli]" ``` If you don't need CLI tool, you can omit `cli` extra. The
 following extras are available: * `lxml` - install lxml library for faster XML
 parsing * `cli` - install CLI tool so it could be used from command line via
-`ilcdtool` command. ## Usage **â ATTENTION**: Pick the right version. There
-are 2 versions of the library available: * Use version **below** `2.0.0` if
-your project uses Pydantic version below `2.0.0` * Use version `2.x.x` or
-higher if your project uses Pydantic version `2.0.0` or above Branch 1.x.x is
-not maintained anymore, so if you don't use pydantic 2.x.x should be your
-choice. ### CLI At the moment the primary function of the CLI tool is to
-convert ILCD XML files to openEPD (json) format. Here is a simple example of
-how to use it to convert ILCD archive to openEPD format: ```bash ilcdtool --
-debug convert-epd -i ilcd+epd -o openEPD "
+`ilcdtool` command. ## Usage ### CLI At the moment the primary function of the
+CLI tool is to convert ILCD XML files to openEPD (json) format. Here is a
+simple example of how to use it to convert ILCD archive to openEPD format:
+```bash ilcdtool --debug convert-epd -i ilcd+epd -o openEPD "
 o/archive.zip>" ``` It is also possible to point the tool to the http endpoint
 instead. At the moment Soda4Lca web UI and api endpoints are supported. ```bash
 ilcdtool convert-epd -i ilcd+epd -o openEPD "https://oekobaudat.de/OEKOBAU.DAT/
 datasetdetail/process.xhtml?uuid=ee8863aa-7276-4896-b07a-
 713937a3134d&version=00.00.018&stock=OBD_2021_II〈=en" ``` Another important
 feature is the ability to specify a **dialect**. Dialect is a set of rules that
 define how the handle provider specific data. It is useful for the cases when
```

