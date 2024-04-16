# Comparing `tmp/ctf_architect-0.1.0a5.tar.gz` & `tmp/ctf_architect-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctf_architect-0.1.0a5.tar", max compression
+gzip compressed data, was "ctf_architect-0.1.0a6.tar", max compression
```

## Comparing `ctf_architect-0.1.0a5.tar` & `ctf_architect-0.1.0a6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1066 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     1134 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/README.md
--rw-r--r--   0        0        0      330 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/__init__.py
--rw-r--r--   0        0        0      153 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/__main__.py
--rw-r--r--   0        0        0      120 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/__main__.py
--rw-r--r--   0        0        0      265 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/cli.py
--rw-r--r--   0        0        0     4388 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/create.py
--rw-r--r--   0        0        0     5468 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/edit.py
--rw-r--r--   0        0        0    15972 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/terminal/create.py
--rw-r--r--   0        0        0      743 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/terminal/main.py
--rw-r--r--   0        0        0     1353 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/chall_architect/utils.py
--rw-r--r--   0        0        0     5583 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/cli/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/cli/challenge.py
--rw-r--r--   0        0        0     1272 2024-04-10 11:20:14.658512 ctf_architect-0.1.0a5/ctf_architect/cli/docker.py
--rw-r--r--   0        0        0     2135 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/cli/mapping.py
--rw-r--r--   0        0        0     4172 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/cli/stats.py
--rw-r--r--   0        0        0     8169 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/challenge.py
--rw-r--r--   0        0        0     1196 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/config.py
--rw-r--r--   0        0        0     1203 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/constants.py
--rw-r--r--   0        0        0     2234 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/docker.py
--rw-r--r--   0        0        0     1644 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/initialize.py
--rw-r--r--   0        0        0     2788 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/mapping.py
--rw-r--r--   0        0        0     6532 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/models.py
--rw-r--r--   0        0        0     6095 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/ctf_architect/core/stats.py
--rw-r--r--   0        0        0     1058 2024-04-10 11:20:14.662512 ctf_architect-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 ctf_architect-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     1123 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/README.md
+-rw-r--r--   0        0        0      330 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/__main__.py
+-rw-r--r--   0        0        0      120 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/__main__.py
+-rw-r--r--   0        0        0      265 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/cli.py
+-rw-r--r--   0        0        0     4388 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/create.py
+-rw-r--r--   0        0        0     5468 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/edit.py
+-rw-r--r--   0        0        0    15963 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/terminal/create.py
+-rw-r--r--   0        0        0      743 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/terminal/main.py
+-rw-r--r--   0        0        0     1353 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/chall_architect/utils.py
+-rw-r--r--   0        0        0     5583 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/cli/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/cli/challenge.py
+-rw-r--r--   0        0        0     1272 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/cli/docker.py
+-rw-r--r--   0        0        0     2135 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/cli/mapping.py
+-rw-r--r--   0        0        0     4172 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/cli/stats.py
+-rw-r--r--   0        0        0     8169 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/challenge.py
+-rw-r--r--   0        0        0     1196 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/config.py
+-rw-r--r--   0        0        0     1203 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/constants.py
+-rw-r--r--   0        0        0     2234 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/docker.py
+-rw-r--r--   0        0        0     1644 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/initialize.py
+-rw-r--r--   0        0        0     2788 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/mapping.py
+-rw-r--r--   0        0        0     6532 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/models.py
+-rw-r--r--   0        0        0     6095 2024-04-16 09:36:49.804860 ctf_architect-0.1.0a6/ctf_architect/core/stats.py
+-rw-r--r--   0        0        0     1058 2024-04-16 09:36:49.808860 ctf_architect-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 ctf_architect-0.1.0a6/PKG-INFO
```

### Comparing `ctf_architect-0.1.0a5/LICENSE` & `ctf_architect-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/README.md` & `ctf_architect-0.1.0a6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CTF-Architect
 
+A tool for managing challenges for CTFs.
+
+> [!WARNING]
+> This tool is still a work in progress, bugs are to be expected. If you find any, please open an [issue](https://github.com/Jus-Codin/CTF-Architect/issues)
+
+
 ---
 
 <p align="center">
     <a href="https://pypi.org/project/ctf-architect/" target="_blank">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ctf-architect">
     </a>
     <a href="https://pypi.org/project/ctf-architect/" target="_blank">
@@ -15,18 +21,13 @@
 
 Github: <a href="https://github.com/Jus-Codin/CTF-Architect" target="_blank">https://github.com/Jus-Codin/CTF-Architect</a>
 
 Documentation: <a href="https://jus-codin.github.io/CTF-Architect/" target="_blank">https://jus-codin.github.io/CTF-Architect/</a>
 
 ---
 
-CTF Architect is a tool for managing challenges for CTFs.
-
-Warning: This tool is still a work in progress, bugs are to be expected. If you find any, please open an [issue](https://github.com/Jus-Codin/CTF-Architect/issues)
-
-
 ## Installation
 Refer to the [installation guide](./guides/installation.md) for instructions on how to install CTF-Architect.
 
 ## Usage
 - [For Challenge Creators](./guides/packaging-challenges.md)
 - [For CTF Organizers](./guides/repository-setup.md)
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-# CTF-Architect ---
+# CTF-Architect A tool for managing challenges for CTFs. > [!WARNING] > This
+tool is still a work in progress, bugs are to be expected. If you find any,
+please open an [issue](https://github.com/Jus-Codin/CTF-Architect/issues) ---
                     _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
 --- Github: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_J_u_s_-_C_o_d_i_n_/_C_T_F_-_A_r_c_h_i_t_e_c_t Documentation: _h_t_t_p_s_:_/_/
-_j_u_s_-_c_o_d_i_n_._g_i_t_h_u_b_._i_o_/_C_T_F_-_A_r_c_h_i_t_e_c_t_/ --- CTF Architect is a tool for managing
-challenges for CTFs. Warning: This tool is still a work in progress, bugs are
-to be expected. If you find any, please open an [issue](https://github.com/Jus-
-Codin/CTF-Architect/issues) ## Installation Refer to the [installation guide]
-(./guides/installation.md) for instructions on how to install CTF-Architect. ##
-Usage - [For Challenge Creators](./guides/packaging-challenges.md) - [For CTF
-Organizers](./guides/repository-setup.md)
+_j_u_s_-_c_o_d_i_n_._g_i_t_h_u_b_._i_o_/_C_T_F_-_A_r_c_h_i_t_e_c_t_/ --- ## Installation Refer to the
+[installation guide](./guides/installation.md) for instructions on how to
+install CTF-Architect. ## Usage - [For Challenge Creators](./guides/packaging-
+challenges.md) - [For CTF Organizers](./guides/repository-setup.md)
```

### Comparing `ctf_architect-0.1.0a5/ctf_architect/chall_architect/create.py` & `ctf_architect-0.1.0a6/ctf_architect/chall_architect/create.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/chall_architect/edit.py` & `ctf_architect-0.1.0a6/ctf_architect/chall_architect/edit.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/chall_architect/terminal/create.py` & `ctf_architect-0.1.0a6/ctf_architect/chall_architect/terminal/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
   elif files is not None:
     console.print("[green]Files selected: [/green]")
     for file in files:
       console.print(f"[light_green]- {file}[/]")
 
   services = get_services()
 
-  if len(services) > 0 and Confirm.ask(":rocket: [cyan]Does the service(s) need a Docker Compose file?[/]"):
+  if services and Confirm.ask(":rocket: [cyan]Does the service(s) need a Docker Compose file?[/]"):
     # Ask for a docker-compose file
     console.print("[bright_cyan]Please select the Docker Compose file for the services[/bright_cyan]")
     docker_compose = askopenfilename(
       title="Select the Docker Compose file for the services",
       filetypes=[("Docker Compose files", "*.yml")]
     )
     if docker_compose == "":
```

### Comparing `ctf_architect-0.1.0a5/ctf_architect/chall_architect/terminal/main.py` & `ctf_architect-0.1.0a6/ctf_architect/chall_architect/terminal/main.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/chall_architect/utils.py` & `ctf_architect-0.1.0a6/ctf_architect/chall_architect/utils.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/cli/__init__.py` & `ctf_architect-0.1.0a6/ctf_architect/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/cli/challenge.py` & `ctf_architect-0.1.0a6/ctf_architect/cli/challenge.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/cli/docker.py` & `ctf_architect-0.1.0a6/ctf_architect/cli/docker.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/cli/mapping.py` & `ctf_architect-0.1.0a6/ctf_architect/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/cli/stats.py` & `ctf_architect-0.1.0a6/ctf_architect/cli/stats.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/challenge.py` & `ctf_architect-0.1.0a6/ctf_architect/core/challenge.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/config.py` & `ctf_architect-0.1.0a6/ctf_architect/core/config.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/constants.py` & `ctf_architect-0.1.0a6/ctf_architect/core/constants.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/docker.py` & `ctf_architect-0.1.0a6/ctf_architect/core/docker.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/initialize.py` & `ctf_architect-0.1.0a6/ctf_architect/core/initialize.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/mapping.py` & `ctf_architect-0.1.0a6/ctf_architect/core/mapping.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/models.py` & `ctf_architect-0.1.0a6/ctf_architect/core/models.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/ctf_architect/core/stats.py` & `ctf_architect-0.1.0a6/ctf_architect/core/stats.py`

 * *Files identical despite different names*

### Comparing `ctf_architect-0.1.0a5/pyproject.toml` & `ctf_architect-0.1.0a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctf-architect"
-version = "0.1.0a5"
+version = "0.1.0a6"
 description = "A tool for managing challenges for CTFs."
 authors = ["Jus-Codin <70018166+Jus-Codin@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `ctf_architect-0.1.0a5/PKG-INFO` & `ctf_architect-0.1.0a6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctf-architect
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: A tool for managing challenges for CTFs.
 License: MIT
 Author: Jus-Codin
 Author-email: 70018166+Jus-Codin@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -22,14 +22,20 @@
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: tomlkit (>=0.12.3,<0.13.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # CTF-Architect
 
+A tool for managing challenges for CTFs.
+
+> [!WARNING]
+> This tool is still a work in progress, bugs are to be expected. If you find any, please open an [issue](https://github.com/Jus-Codin/CTF-Architect/issues)
+
+
 ---
 
 <p align="center">
     <a href="https://pypi.org/project/ctf-architect/" target="_blank">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/ctf-architect">
     </a>
     <a href="https://pypi.org/project/ctf-architect/" target="_blank">
@@ -41,18 +47,13 @@
 
 Github: <a href="https://github.com/Jus-Codin/CTF-Architect" target="_blank">https://github.com/Jus-Codin/CTF-Architect</a>
 
 Documentation: <a href="https://jus-codin.github.io/CTF-Architect/" target="_blank">https://jus-codin.github.io/CTF-Architect/</a>
 
 ---
 
-CTF Architect is a tool for managing challenges for CTFs.
-
-Warning: This tool is still a work in progress, bugs are to be expected. If you find any, please open an [issue](https://github.com/Jus-Codin/CTF-Architect/issues)
-
-
 ## Installation
 Refer to the [installation guide](./guides/installation.md) for instructions on how to install CTF-Architect.
 
 ## Usage
 - [For Challenge Creators](./guides/packaging-challenges.md)
 - [For CTF Organizers](./guides/repository-setup.md)
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: ctf-architect Version: 0.1.0a5 Summary: A tool for
+Metadata-Version: 2.1 Name: ctf-architect Version: 0.1.0a6 Summary: A tool for
 managing challenges for CTFs. License: MIT Author: Jus-Codin Author-email:
 70018166+Jus-Codin@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: MacOS Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: pydantic
 (>=2.6.1,<3.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rich
 (>=13.7.1,<14.0.0) Requires-Dist: tomlkit (>=0.12.3,<0.13.0) Requires-Dist:
 typer[all] (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown # CTF-
-Architect ---
+Architect A tool for managing challenges for CTFs. > [!WARNING] > This tool is
+still a work in progress, bugs are to be expected. If you find any, please open
+an [issue](https://github.com/Jus-Codin/CTF-Architect/issues) ---
                     _[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]
 --- Github: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_J_u_s_-_C_o_d_i_n_/_C_T_F_-_A_r_c_h_i_t_e_c_t Documentation: _h_t_t_p_s_:_/_/
-_j_u_s_-_c_o_d_i_n_._g_i_t_h_u_b_._i_o_/_C_T_F_-_A_r_c_h_i_t_e_c_t_/ --- CTF Architect is a tool for managing
-challenges for CTFs. Warning: This tool is still a work in progress, bugs are
-to be expected. If you find any, please open an [issue](https://github.com/Jus-
-Codin/CTF-Architect/issues) ## Installation Refer to the [installation guide]
-(./guides/installation.md) for instructions on how to install CTF-Architect. ##
-Usage - [For Challenge Creators](./guides/packaging-challenges.md) - [For CTF
-Organizers](./guides/repository-setup.md)
+_j_u_s_-_c_o_d_i_n_._g_i_t_h_u_b_._i_o_/_C_T_F_-_A_r_c_h_i_t_e_c_t_/ --- ## Installation Refer to the
+[installation guide](./guides/installation.md) for instructions on how to
+install CTF-Architect. ## Usage - [For Challenge Creators](./guides/packaging-
+challenges.md) - [For CTF Organizers](./guides/repository-setup.md)
```

