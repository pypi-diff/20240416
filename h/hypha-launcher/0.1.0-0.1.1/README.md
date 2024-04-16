# Comparing `tmp/hypha-launcher-0.1.0.tar.gz` & `tmp/hypha_launcher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypha-launcher-0.1.0.tar", last modified: Sat Mar  2 15:36:05 2024, max compression
+gzip compressed data, was "hypha_launcher-0.1.1.tar", last modified: Mon Apr 15 11:04:07 2024, max compression
```

## Comparing `hypha-launcher-0.1.0.tar` & `hypha_launcher-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:36:05.289834 hypha-launcher-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-02 15:36:05.289834 hypha-launcher-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:36:05.285834 hypha-launcher-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:36:05.285834 hypha-launcher-0.1.0/hypha_launcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/hypha_startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:36:05.289834 hypha-launcher-0.1.0/hypha_launcher/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/utils/hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/hypha_launcher/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 15:36:05.289834 hypha-launcher-0.1.0/hypha_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-02 15:36:05.000000 hypha-launcher-0.1.0/hypha_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-02 15:36:05.000000 hypha-launcher-0.1.0/hypha_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 15:36:05.000000 hypha-launcher-0.1.0/hypha_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-02 15:36:05.000000 hypha-launcher-0.1.0/hypha_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-02 15:36:05.000000 hypha-launcher-0.1.0/hypha_launcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-02 15:35:53.000000 hypha-launcher-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 15:36:05.289834 hypha-launcher-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/hypha_launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/hypha_launcher/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/hypha_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/tests/test_api.py
```

### Comparing `hypha-launcher-0.1.0/CONTRIBUTING.md` & `hypha_launcher-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hypha-launcher-0.1.0/LICENSE` & `hypha_launcher-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypha-launcher-0.1.0/PKG-INFO` & `hypha_launcher-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hypha-launcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: Launcher for hypha services
 Author-email: Weize Xu <vet.xwz@gmail.com>, Wei Ouyang <oeway007@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: fire
 Requires-Dist: loguru
 Requires-Dist: executor-engine
 Requires-Dist: hypha
 Requires-Dist: uvicorn
 Requires-Dist: imjoy-rpc
 Requires-Dist: pyotritonclient
-Requires-Dist: netifaces
+Requires-Dist: psutil
 
 <div align="center">
 <h1> hypha-launcher </h1>
 
 <p> Run triton server on HPC </p>
 
 <p>
@@ -32,100 +32,78 @@
 </p>
 </div>
 
 **Work In Progress**
 
 ## Features
 
-+ CLI for downloading model from s3 and pulling docker image of triton server
++ CLI/API for:
+  - downloading model from s3 and pulling docker image of triton server
+  - launch s3 server
+  - launch triton server
+  - ...
 + Support different container engines
   - Docker
   - Apptainer
 + Support different compute environments
   - Local
   - Slurm
 
 ## Installation
 
 ```bash
 pip install hypha-launcher
 ```
 
-## Usage
+## CLI Usage
 
 ```bash
-$ hypha-launcher
-NAME
-    hypha-launcher
-
-SYNOPSIS
-    hypha-launcher - GROUP | COMMAND | VALUE
-
-GROUPS
-    GROUP is one of the following:
-
-     container_engine
-       Container engine abstraction. Provides a common interface to container engines, such as docker, apptainer, podman, etc.
-
-COMMANDS
-    COMMAND is one of the following:
-
-     download_models_from_s3
-       Download models from S3
-
-     pull_image
-
-     run_launcher_server
-       Start a launcher server, run in the login node of HPC.
-
-     run_worker
-       Run a worker server, run in the compute node of HPC.
-
-VALUES
-    VALUE is one of the following:
-
-     debug
-
-     store_dir
+$ hypha-launcher --help
 ```
 
-### Download model from s3
+### Launch the bioimage.io backend
+
+Download all models from s3 and launch triton server.
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store" - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
+$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
 ```
 
-### Pull docker image of triton server
+Launch on slurm cluster.
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store" - pull_image
+# Please replace the slurm settings with your own settings
+$ export SLURM_ACCOUNT=Your-Slurm-Account
+$ export SLURM_TIME=03:00:00
+$ export SLURM_GPUS_PER_NODE=A100:1
+$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
 ```
 
-### Start launcher
-
-On local machine:
+### Download model from s3
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store/" - run_launcher_server 
+$ python -m hypha-launcher - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
 ```
 
-On HPC(Slurm):
+### Pull docker image of triton server
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store/" - run_launcher_server --slurm-settings='{"account": "your-account", "gpus_per_node": "V100:1", "time": "01:00:00"}'
+$ python -m hypha-launcher - pull_image
 ```
 
 ## TODO
 
 * [x] Download model from s3
 * [x] Pull docker image of triton server
 * [x] Run triton server
 * [x] Register service on hypha
 * [x] Conmmunicate with triton server
 * [x] Test on HPC
+* [ ] Support run on local machine without GPU
+* [ ] Support launch containers inside a container (For support run inside the podman-desktop)
 * [ ] Job management(Auto stop and restart)
 * [ ] Load balancing
 * [ ] Documentation
 
 
 ## Development
 Install the package in editable mode with the following command:
```

#### html2text {}

```diff
@@ -1,36 +1,33 @@
-Metadata-Version: 2.1 Name: hypha-launcher Version: 0.1.0 Summary: Launcher for
+Metadata-Version: 2.1 Name: hypha-launcher Version: 0.1.1 Summary: Launcher for
 hypha services Author-email: Weize Xu
 gmail.com>, Wei Ouyang
 gmail.com> Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: aiohttp Requires-Dist: requests Requires-Dist: tqdm Requires-
 Dist: fire Requires-Dist: loguru Requires-Dist: executor-engine Requires-Dist:
 hypha Requires-Dist: uvicorn Requires-Dist: imjoy-rpc Requires-Dist:
-pyotritonclient Requires-Dist: netifaces
+pyotritonclient Requires-Dist: psutil
                          ************ hhyypphhaa--llaauunncchheerr ************
                            Run triton server on HPC
                        _[_I_n_s_t_a_l_l_ _w_i_t_h_ _P_y_P_i_]_[_M_I_T_ _l_i_c_e_n_s_e_]
-**Work In Progress** ## Features + CLI for downloading model from s3 and
-pulling docker image of triton server + Support different container engines -
-Docker - Apptainer + Support different compute environments - Local - Slurm ##
-Installation ```bash pip install hypha-launcher ``` ## Usage ```bash $ hypha-
-launcher NAME hypha-launcher SYNOPSIS hypha-launcher - GROUP | COMMAND | VALUE
-GROUPS GROUP is one of the following: container_engine Container engine
-abstraction. Provides a common interface to container engines, such as docker,
-apptainer, podman, etc. COMMANDS COMMAND is one of the following:
-download_models_from_s3 Download models from S3 pull_image run_launcher_server
-Start a launcher server, run in the login node of HPC. run_worker Run a worker
-server, run in the compute node of HPC. VALUES VALUE is one of the following:
-debug store_dir ``` ### Download model from s3 ```bash $ hypha-launcher --
-store-dir="./triton_store" - download_models_from_s3 bioengine-model-runner.* -
--n_parallel=5 ``` ### Pull docker image of triton server ```bash $ hypha-
-launcher --store-dir="./triton_store" - pull_image ``` ### Start launcher On
-local machine: ```bash $ hypha-launcher --store-dir="./triton_store/" -
-run_launcher_server ``` On HPC(Slurm): ```bash $ hypha-launcher --store-dir="./
-triton_store/" - run_launcher_server --slurm-settings='{"account": "your-
-account", "gpus_per_node": "V100:1", "time": "01:00:00"}' ``` ## TODO * [x]
-Download model from s3 * [x] Pull docker image of triton server * [x] Run
-triton server * [x] Register service on hypha * [x] Conmmunicate with triton
-server * [x] Test on HPC * [ ] Job management(Auto stop and restart) * [ ] Load
-balancing * [ ] Documentation ## Development Install the package in editable
-mode with the following command: ```bash pip install -e . pip install -
-r requirements-dev.txt ```
+**Work In Progress** ## Features + CLI/API for: - downloading model from s3 and
+pulling docker image of triton server - launch s3 server - launch triton server
+- ... + Support different container engines - Docker - Apptainer + Support
+different compute environments - Local - Slurm ## Installation ```bash pip
+install hypha-launcher ``` ## CLI Usage ```bash $ hypha-launcher --help ``` ###
+Launch the bioimage.io backend Download all models from s3 and launch triton
+server. ```bash $ python -m hypha_launcher launch_bioimageio_backend --service-
+id my-triton ``` Launch on slurm cluster. ```bash # Please replace the slurm
+settings with your own settings $ export SLURM_ACCOUNT=Your-Slurm-Account $
+export SLURM_TIME=03:00:00 $ export SLURM_GPUS_PER_NODE=A100:1 $ python -
+m hypha_launcher launch_bioimageio_backend --service-id my-triton ``` ###
+Download model from s3 ```bash $ python -m hypha-launcher -
+download_models_from_s3 bioengine-model-runner.* --n_parallel=5 ``` ### Pull
+docker image of triton server ```bash $ python -m hypha-launcher - pull_image
+``` ## TODO * [x] Download model from s3 * [x] Pull docker image of triton
+server * [x] Run triton server * [x] Register service on hypha * [x]
+Conmmunicate with triton server * [x] Test on HPC * [ ] Support run on local
+machine without GPU * [ ] Support launch containers inside a container (For
+support run inside the podman-desktop) * [ ] Job management(Auto stop and
+restart) * [ ] Load balancing * [ ] Documentation ## Development Install the
+package in editable mode with the following command: ```bash pip install -e .
+pip install -r requirements-dev.txt ```
```

### Comparing `hypha-launcher-0.1.0/README.md` & `hypha_launcher-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,100 +13,78 @@
 </p>
 </div>
 
 **Work In Progress**
 
 ## Features
 
-+ CLI for downloading model from s3 and pulling docker image of triton server
++ CLI/API for:
+  - downloading model from s3 and pulling docker image of triton server
+  - launch s3 server
+  - launch triton server
+  - ...
 + Support different container engines
   - Docker
   - Apptainer
 + Support different compute environments
   - Local
   - Slurm
 
 ## Installation
 
 ```bash
 pip install hypha-launcher
 ```
 
-## Usage
+## CLI Usage
 
 ```bash
-$ hypha-launcher
-NAME
-    hypha-launcher
-
-SYNOPSIS
-    hypha-launcher - GROUP | COMMAND | VALUE
-
-GROUPS
-    GROUP is one of the following:
-
-     container_engine
-       Container engine abstraction. Provides a common interface to container engines, such as docker, apptainer, podman, etc.
-
-COMMANDS
-    COMMAND is one of the following:
-
-     download_models_from_s3
-       Download models from S3
-
-     pull_image
-
-     run_launcher_server
-       Start a launcher server, run in the login node of HPC.
-
-     run_worker
-       Run a worker server, run in the compute node of HPC.
-
-VALUES
-    VALUE is one of the following:
-
-     debug
-
-     store_dir
+$ hypha-launcher --help
 ```
 
-### Download model from s3
+### Launch the bioimage.io backend
+
+Download all models from s3 and launch triton server.
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store" - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
+$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
 ```
 
-### Pull docker image of triton server
+Launch on slurm cluster.
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store" - pull_image
+# Please replace the slurm settings with your own settings
+$ export SLURM_ACCOUNT=Your-Slurm-Account
+$ export SLURM_TIME=03:00:00
+$ export SLURM_GPUS_PER_NODE=A100:1
+$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
 ```
 
-### Start launcher
-
-On local machine:
+### Download model from s3
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store/" - run_launcher_server 
+$ python -m hypha-launcher - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
 ```
 
-On HPC(Slurm):
+### Pull docker image of triton server
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store/" - run_launcher_server --slurm-settings='{"account": "your-account", "gpus_per_node": "V100:1", "time": "01:00:00"}'
+$ python -m hypha-launcher - pull_image
 ```
 
 ## TODO
 
 * [x] Download model from s3
 * [x] Pull docker image of triton server
 * [x] Run triton server
 * [x] Register service on hypha
 * [x] Conmmunicate with triton server
 * [x] Test on HPC
+* [ ] Support run on local machine without GPU
+* [ ] Support launch containers inside a container (For support run inside the podman-desktop)
 * [ ] Job management(Auto stop and restart)
 * [ ] Load balancing
 * [ ] Documentation
 
 
 ## Development
 Install the package in editable mode with the following command:
```

#### html2text {}

```diff
@@ -1,28 +1,25 @@
                          ************ hhyypphhaa--llaauunncchheerr ************
                            Run triton server on HPC
                        _[_I_n_s_t_a_l_l_ _w_i_t_h_ _P_y_P_i_]_[_M_I_T_ _l_i_c_e_n_s_e_]
-**Work In Progress** ## Features + CLI for downloading model from s3 and
-pulling docker image of triton server + Support different container engines -
-Docker - Apptainer + Support different compute environments - Local - Slurm ##
-Installation ```bash pip install hypha-launcher ``` ## Usage ```bash $ hypha-
-launcher NAME hypha-launcher SYNOPSIS hypha-launcher - GROUP | COMMAND | VALUE
-GROUPS GROUP is one of the following: container_engine Container engine
-abstraction. Provides a common interface to container engines, such as docker,
-apptainer, podman, etc. COMMANDS COMMAND is one of the following:
-download_models_from_s3 Download models from S3 pull_image run_launcher_server
-Start a launcher server, run in the login node of HPC. run_worker Run a worker
-server, run in the compute node of HPC. VALUES VALUE is one of the following:
-debug store_dir ``` ### Download model from s3 ```bash $ hypha-launcher --
-store-dir="./triton_store" - download_models_from_s3 bioengine-model-runner.* -
--n_parallel=5 ``` ### Pull docker image of triton server ```bash $ hypha-
-launcher --store-dir="./triton_store" - pull_image ``` ### Start launcher On
-local machine: ```bash $ hypha-launcher --store-dir="./triton_store/" -
-run_launcher_server ``` On HPC(Slurm): ```bash $ hypha-launcher --store-dir="./
-triton_store/" - run_launcher_server --slurm-settings='{"account": "your-
-account", "gpus_per_node": "V100:1", "time": "01:00:00"}' ``` ## TODO * [x]
-Download model from s3 * [x] Pull docker image of triton server * [x] Run
-triton server * [x] Register service on hypha * [x] Conmmunicate with triton
-server * [x] Test on HPC * [ ] Job management(Auto stop and restart) * [ ] Load
-balancing * [ ] Documentation ## Development Install the package in editable
-mode with the following command: ```bash pip install -e . pip install -
-r requirements-dev.txt ```
+**Work In Progress** ## Features + CLI/API for: - downloading model from s3 and
+pulling docker image of triton server - launch s3 server - launch triton server
+- ... + Support different container engines - Docker - Apptainer + Support
+different compute environments - Local - Slurm ## Installation ```bash pip
+install hypha-launcher ``` ## CLI Usage ```bash $ hypha-launcher --help ``` ###
+Launch the bioimage.io backend Download all models from s3 and launch triton
+server. ```bash $ python -m hypha_launcher launch_bioimageio_backend --service-
+id my-triton ``` Launch on slurm cluster. ```bash # Please replace the slurm
+settings with your own settings $ export SLURM_ACCOUNT=Your-Slurm-Account $
+export SLURM_TIME=03:00:00 $ export SLURM_GPUS_PER_NODE=A100:1 $ python -
+m hypha_launcher launch_bioimageio_backend --service-id my-triton ``` ###
+Download model from s3 ```bash $ python -m hypha-launcher -
+download_models_from_s3 bioengine-model-runner.* --n_parallel=5 ``` ### Pull
+docker image of triton server ```bash $ python -m hypha-launcher - pull_image
+``` ## TODO * [x] Download model from s3 * [x] Pull docker image of triton
+server * [x] Run triton server * [x] Register service on hypha * [x]
+Conmmunicate with triton server * [x] Test on HPC * [ ] Support run on local
+machine without GPU * [ ] Support launch containers inside a container (For
+support run inside the podman-desktop) * [ ] Job management(Auto stop and
+restart) * [ ] Load balancing * [ ] Documentation ## Development Install the
+package in editable mode with the following command: ```bash pip install -e .
+pip install -r requirements-dev.txt ```
```

### Comparing `hypha-launcher-0.1.0/hypha_launcher/utils/container.py` & `hypha_launcher-0.1.1/hypha_launcher/utils/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             raise RuntimeError(
                 "Cannot find supported container engine: " f"{self.supported_engines}"
             )
 
     @staticmethod
     def process_image_name_for_docker(image_name: str):
         if image_name.startswith("docker://"):
-            return image_name[len("docker://") :]
+            return image_name[len("docker://"):]
         return image_name
 
     @staticmethod
     def process_image_name_for_podman(image_name: str):
         return f"{ContainerEngine.process_image_name_for_docker(image_name)}"
 
     def pull_image(self, image_name: str):
@@ -69,71 +69,73 @@
             self.sif_files[image_name] = sif_path
         elif self.engine_type == "podman":
             image_name = self.process_image_name_for_podman(image_name)
             run_cmd(["podman", "pull", image_name], check=True)
         else:
             raise NotImplementedError
 
-    def run_command(
+    def get_command(
         self,
         cmd: str,
         image_name: str,
         volumes: T.Optional[dict] = None,
         ports: T.Optional[dict] = None,
-    ):
-        """Start container with a command,
-        supporting volume and port mapping.
+        envs: T.Optional[dict] = None,
+    ) -> str:
+        """Get the command for run process in the container
 
         Args:
             cmd (str): command to run in the container
             image_name (str): image name
             volumes (dict, optional): volume mapping
                 The key is the host path and the value is the container path
             ports (dict, optional): port mapping
                 The key is the host port and the value is the container port
+            envs (dict, optional): environment variables
+                The key is the environment variable name and the value is the value
         """
         # Initialize volume and port mappings as empty strings
         volume_mapping = ""
         port_mapping = ""
+        env_options = ""
+        if volumes is None:
+            volumes = {}
         # If volumes are provided, construct volume mapping options
-        if volumes:
-            for host_path, container_path in volumes.items():
-                volume_mapping += f"-v {host_path}:{container_path} "
+        for host_path, container_path in volumes.items():
+            volume_mapping += f"-v {host_path}:{container_path} "
         # If ports are provided, construct port mapping options
         if ports:
             for host_port, container_port in ports.items():
                 port_mapping += f"-p {host_port}:{container_port} "
+        # If environment variables are provided, construct environment variable options
+        if envs:
+            for env_name, env_value in envs.items():
+                env_options += f"-e {env_name}={env_value} "
         # Construct the command based on the engine type
         if self.engine_type == "docker":
             image_name = self.process_image_name_for_docker(image_name)
-            run_cmd(
-                f"docker run {volume_mapping} {port_mapping} {image_name} {cmd}",
-                check=True,
-            )  # noqa
+            return f"docker run --rm {env_options} {volume_mapping} {port_mapping} {image_name} {cmd}"
         elif self.engine_type == "apptainer":
             # add tmp dir mapping when using apptainer
             host_tmp_dir = self.store_dir / "apptainer_tmp"
             host_tmp_dir.mkdir(exist_ok=True)
             volumes[host_tmp_dir.as_posix()] = "/tmp"
             # Note: Apptainer (formerly Singularity) has different options
             sif_path = self.sif_files[image_name]
             # For Apptainer, bind options are used for volume mapping
             bind_option = ""
             if volumes:
                 binds = [f"{host}:{container}" for host, container in volumes.items()]
                 bind_option = f"--bind {','.join(binds)} "
-            run_cmd(
-                f"apptainer run --contain {bind_option} {sif_path} {cmd}", check=True
-            )  # noqa
+            if envs:
+                env_options = " ".join([f"--env {k}={v}" for k, v in envs.items()])
+            return f"apptainer run --contain {env_options} {bind_option} {sif_path} {cmd}"
         elif self.engine_type == "podman":
             image_name = self.process_image_name_for_docker(image_name)
-            run_cmd(
-                f"podman run {volume_mapping} {port_mapping} {image_name} {cmd}",
-                check=True,
-            )  # noqa
+            return f"podman run {env_options} {volume_mapping} {port_mapping} {image_name} {cmd}"
         else:
             raise NotImplementedError
 
 
 if __name__ == "__main__":
     import fire
```

### Comparing `hypha-launcher-0.1.0/hypha_launcher/utils/download.py` & `hypha_launcher-0.1.1/hypha_launcher/utils/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,34 +78,43 @@
     :return: The content of the URL as a string.
     """
     response = requests.get(url)
     response.raise_for_status()
     return response.text
 
 
-def parse_s3_xml(content: str, key_pattern: str) -> list[str]:
+def parse_s3_xml(content: str, key_pattern: str) -> list[dict]:
     # Parse the XML content
     root = ET.fromstring(content)
 
     # Define the namespace mapping
     ns = {"ns": "http://s3.amazonaws.com/doc/2006-03-01/"}
 
     # Compile the regex pattern for matching keys
     pattern = re.compile(key_pattern)
 
     # Find all 'Contents' elements considering the namespace
     contents_elements = root.findall("ns:Contents", ns)
 
     # Extract the 'Key' element text if it matches the pattern
-    matching_keys = [
-        elem.find("ns:Key", ns).text
-        for elem in contents_elements
-        if pattern.match(elem.find("ns:Key", ns).text)
-    ]
-
-    return matching_keys
+    items = []
+    for elem in contents_elements:
+        key = elem.find("ns:Key", ns)
+        if key is None:
+            continue
+        key_text = key.text
+        if key_text and pattern.match(key_text):
+            size_field = elem.find("ns:Size", ns)
+            if (size_field is None) or (size_field.text is None):
+                continue
+            size = int(size_field.text)
+            items.append({
+                "key": key_text,
+                "size": size,
+            })
+    return items
 
 
 if __name__ == "__main__":
     import fire
 
     fire.Fire(download_files)
```

### Comparing `hypha-launcher-0.1.0/hypha_launcher.egg-info/PKG-INFO` & `hypha_launcher-0.1.1/hypha_launcher.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hypha-launcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: Launcher for hypha services
 Author-email: Weize Xu <vet.xwz@gmail.com>, Wei Ouyang <oeway007@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: fire
 Requires-Dist: loguru
 Requires-Dist: executor-engine
 Requires-Dist: hypha
 Requires-Dist: uvicorn
 Requires-Dist: imjoy-rpc
 Requires-Dist: pyotritonclient
-Requires-Dist: netifaces
+Requires-Dist: psutil
 
 <div align="center">
 <h1> hypha-launcher </h1>
 
 <p> Run triton server on HPC </p>
 
 <p>
@@ -32,100 +32,78 @@
 </p>
 </div>
 
 **Work In Progress**
 
 ## Features
 
-+ CLI for downloading model from s3 and pulling docker image of triton server
++ CLI/API for:
+  - downloading model from s3 and pulling docker image of triton server
+  - launch s3 server
+  - launch triton server
+  - ...
 + Support different container engines
   - Docker
   - Apptainer
 + Support different compute environments
   - Local
   - Slurm
 
 ## Installation
 
 ```bash
 pip install hypha-launcher
 ```
 
-## Usage
+## CLI Usage
 
 ```bash
-$ hypha-launcher
-NAME
-    hypha-launcher
-
-SYNOPSIS
-    hypha-launcher - GROUP | COMMAND | VALUE
-
-GROUPS
-    GROUP is one of the following:
-
-     container_engine
-       Container engine abstraction. Provides a common interface to container engines, such as docker, apptainer, podman, etc.
-
-COMMANDS
-    COMMAND is one of the following:
-
-     download_models_from_s3
-       Download models from S3
-
-     pull_image
-
-     run_launcher_server
-       Start a launcher server, run in the login node of HPC.
-
-     run_worker
-       Run a worker server, run in the compute node of HPC.
-
-VALUES
-    VALUE is one of the following:
-
-     debug
-
-     store_dir
+$ hypha-launcher --help
 ```
 
-### Download model from s3
+### Launch the bioimage.io backend
+
+Download all models from s3 and launch triton server.
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store" - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
+$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
 ```
 
-### Pull docker image of triton server
+Launch on slurm cluster.
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store" - pull_image
+# Please replace the slurm settings with your own settings
+$ export SLURM_ACCOUNT=Your-Slurm-Account
+$ export SLURM_TIME=03:00:00
+$ export SLURM_GPUS_PER_NODE=A100:1
+$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
 ```
 
-### Start launcher
-
-On local machine:
+### Download model from s3
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store/" - run_launcher_server 
+$ python -m hypha-launcher - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
 ```
 
-On HPC(Slurm):
+### Pull docker image of triton server
 
 ```bash
-$ hypha-launcher --store-dir="./triton_store/" - run_launcher_server --slurm-settings='{"account": "your-account", "gpus_per_node": "V100:1", "time": "01:00:00"}'
+$ python -m hypha-launcher - pull_image
 ```
 
 ## TODO
 
 * [x] Download model from s3
 * [x] Pull docker image of triton server
 * [x] Run triton server
 * [x] Register service on hypha
 * [x] Conmmunicate with triton server
 * [x] Test on HPC
+* [ ] Support run on local machine without GPU
+* [ ] Support launch containers inside a container (For support run inside the podman-desktop)
 * [ ] Job management(Auto stop and restart)
 * [ ] Load balancing
 * [ ] Documentation
 
 
 ## Development
 Install the package in editable mode with the following command:
```

#### html2text {}

```diff
@@ -1,36 +1,33 @@
-Metadata-Version: 2.1 Name: hypha-launcher Version: 0.1.0 Summary: Launcher for
+Metadata-Version: 2.1 Name: hypha-launcher Version: 0.1.1 Summary: Launcher for
 hypha services Author-email: Weize Xu
 gmail.com>, Wei Ouyang
 gmail.com> Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: aiohttp Requires-Dist: requests Requires-Dist: tqdm Requires-
 Dist: fire Requires-Dist: loguru Requires-Dist: executor-engine Requires-Dist:
 hypha Requires-Dist: uvicorn Requires-Dist: imjoy-rpc Requires-Dist:
-pyotritonclient Requires-Dist: netifaces
+pyotritonclient Requires-Dist: psutil
                          ************ hhyypphhaa--llaauunncchheerr ************
                            Run triton server on HPC
                        _[_I_n_s_t_a_l_l_ _w_i_t_h_ _P_y_P_i_]_[_M_I_T_ _l_i_c_e_n_s_e_]
-**Work In Progress** ## Features + CLI for downloading model from s3 and
-pulling docker image of triton server + Support different container engines -
-Docker - Apptainer + Support different compute environments - Local - Slurm ##
-Installation ```bash pip install hypha-launcher ``` ## Usage ```bash $ hypha-
-launcher NAME hypha-launcher SYNOPSIS hypha-launcher - GROUP | COMMAND | VALUE
-GROUPS GROUP is one of the following: container_engine Container engine
-abstraction. Provides a common interface to container engines, such as docker,
-apptainer, podman, etc. COMMANDS COMMAND is one of the following:
-download_models_from_s3 Download models from S3 pull_image run_launcher_server
-Start a launcher server, run in the login node of HPC. run_worker Run a worker
-server, run in the compute node of HPC. VALUES VALUE is one of the following:
-debug store_dir ``` ### Download model from s3 ```bash $ hypha-launcher --
-store-dir="./triton_store" - download_models_from_s3 bioengine-model-runner.* -
--n_parallel=5 ``` ### Pull docker image of triton server ```bash $ hypha-
-launcher --store-dir="./triton_store" - pull_image ``` ### Start launcher On
-local machine: ```bash $ hypha-launcher --store-dir="./triton_store/" -
-run_launcher_server ``` On HPC(Slurm): ```bash $ hypha-launcher --store-dir="./
-triton_store/" - run_launcher_server --slurm-settings='{"account": "your-
-account", "gpus_per_node": "V100:1", "time": "01:00:00"}' ``` ## TODO * [x]
-Download model from s3 * [x] Pull docker image of triton server * [x] Run
-triton server * [x] Register service on hypha * [x] Conmmunicate with triton
-server * [x] Test on HPC * [ ] Job management(Auto stop and restart) * [ ] Load
-balancing * [ ] Documentation ## Development Install the package in editable
-mode with the following command: ```bash pip install -e . pip install -
-r requirements-dev.txt ```
+**Work In Progress** ## Features + CLI/API for: - downloading model from s3 and
+pulling docker image of triton server - launch s3 server - launch triton server
+- ... + Support different container engines - Docker - Apptainer + Support
+different compute environments - Local - Slurm ## Installation ```bash pip
+install hypha-launcher ``` ## CLI Usage ```bash $ hypha-launcher --help ``` ###
+Launch the bioimage.io backend Download all models from s3 and launch triton
+server. ```bash $ python -m hypha_launcher launch_bioimageio_backend --service-
+id my-triton ``` Launch on slurm cluster. ```bash # Please replace the slurm
+settings with your own settings $ export SLURM_ACCOUNT=Your-Slurm-Account $
+export SLURM_TIME=03:00:00 $ export SLURM_GPUS_PER_NODE=A100:1 $ python -
+m hypha_launcher launch_bioimageio_backend --service-id my-triton ``` ###
+Download model from s3 ```bash $ python -m hypha-launcher -
+download_models_from_s3 bioengine-model-runner.* --n_parallel=5 ``` ### Pull
+docker image of triton server ```bash $ python -m hypha-launcher - pull_image
+``` ## TODO * [x] Download model from s3 * [x] Pull docker image of triton
+server * [x] Run triton server * [x] Register service on hypha * [x]
+Conmmunicate with triton server * [x] Test on HPC * [ ] Support run on local
+machine without GPU * [ ] Support launch containers inside a container (For
+support run inside the podman-desktop) * [ ] Job management(Auto stop and
+restart) * [ ] Load balancing * [ ] Documentation ## Development Install the
+package in editable mode with the following command: ```bash pip install -e .
+pip install -r requirements-dev.txt ```
```

### Comparing `hypha-launcher-0.1.0/hypha_launcher.egg-info/SOURCES.txt` & `hypha_launcher-0.1.1/hypha_launcher.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 MANIFEST.in
 README.md
 pyproject.toml
 docs/index.md
 docs/mkdocs.yml
 hypha_launcher/__init__.py
 hypha_launcher/__main__.py
-hypha_launcher/app.py
+hypha_launcher/api.py
 hypha_launcher/constants.py
-hypha_launcher/hypha_startup.py
 hypha_launcher.egg-info/PKG-INFO
 hypha_launcher.egg-info/SOURCES.txt
 hypha_launcher.egg-info/dependency_links.txt
 hypha_launcher.egg-info/requires.txt
 hypha_launcher.egg-info/top_level.txt
 hypha_launcher/utils/__init__.py
 hypha_launcher/utils/container.py
 hypha_launcher/utils/download.py
 hypha_launcher/utils/hpc.py
 hypha_launcher/utils/log.py
-hypha_launcher/utils/misc.py
+hypha_launcher/utils/misc.py
+tests/test_api.py
```

### Comparing `hypha-launcher-0.1.0/pyproject.toml` & `hypha_launcher-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "hypha-launcher"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 description = "Launcher for hypha services"
 authors = [
     {name = "Weize Xu", email = "vet.xwz@gmail.com" },
     {name = "Wei Ouyang", email = "oeway007@gmail.com" }
 ]
 dependencies = [
@@ -17,15 +17,15 @@
     "fire",
     "loguru",
     "executor-engine",
     "hypha",
     "uvicorn",
     "imjoy-rpc",
     "pyotritonclient",
-    "netifaces",
+    "psutil",
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["hypha_launcher*"]
```

