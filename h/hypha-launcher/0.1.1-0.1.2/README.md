# Comparing `tmp/hypha_launcher-0.1.1.tar.gz` & `tmp/hypha_launcher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypha_launcher-0.1.1.tar", last modified: Mon Apr 15 11:04:07 2024, max compression
+gzip compressed data, was "hypha_launcher-0.1.2.tar", last modified: Tue Apr 16 07:18:57 2024, max compression
```

## Comparing `hypha_launcher-0.1.1.tar` & `hypha_launcher-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/hypha_launcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/hypha_launcher/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/hypha_launcher/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/hypha_launcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 11:04:07.000000 hypha_launcher-0.1.1/hypha_launcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:04:07.668236 hypha_launcher-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-15 11:03:57.000000 hypha_launcher-0.1.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:57.096613 hypha_launcher-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-16 07:18:57.096613 hypha_launcher-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:57.092613 hypha_launcher-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:57.092613 hypha_launcher-0.1.2/hypha_launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15624 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:57.092613 hypha_launcher-0.1.2/hypha_launcher/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/utils/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/hypha_launcher/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:57.096613 hypha_launcher-0.1.2/hypha_launcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-16 07:18:57.000000 hypha_launcher-0.1.2/hypha_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-16 07:18:57.000000 hypha_launcher-0.1.2/hypha_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:18:57.000000 hypha_launcher-0.1.2/hypha_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 07:18:57.000000 hypha_launcher-0.1.2/hypha_launcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 07:18:57.000000 hypha_launcher-0.1.2/hypha_launcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:18:57.096613 hypha_launcher-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:18:57.092613 hypha_launcher-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 07:18:47.000000 hypha_launcher-0.1.2/tests/test_api.py
```

### Comparing `hypha_launcher-0.1.1/CONTRIBUTING.md` & `hypha_launcher-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hypha_launcher-0.1.1/LICENSE` & `hypha_launcher-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hypha_launcher-0.1.1/README.md` & `hypha_launcher-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -34,45 +34,51 @@
 ```bash
 pip install hypha-launcher
 ```
 
 ## CLI Usage
 
 ```bash
-$ hypha-launcher --help
+hypha-launcher --help
 ```
 
-### Launch the bioimage.io backend
+### Launch the BioEngine Worker on HPC
+
+BioEngine consists of a set of services that are used to serve AI models from bioimage.io. We provide the model test run feature accessible from https://bioimage.io and a dedicated bioengine web client: https://bioimage-io.github.io/bioengine-web-client/. While our public instance is openly accessible for testing and evaluation, you can run your own instance of the BioEngine worker to serve the models, e.g. with your own HPC computing resources.
 
 Download all models from s3 and launch triton server.
 
+Launch on HPC cluster. You need to set the job command template via the `HYPHA_HPC_JOB_TEMPLATE` environment variable for your own HPC cluster.
+
+For example, here is an example for launching the BioEngine on a Slurm cluster:
+
 ```bash
-$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
+# Please replace the job command with your own settings
+export HYPHA_HPC_JOB_TEMPLATE="srun -A Your-Slurm-Account -t 03:00:00 --gpus-per-node A100:1 {cmd}"
+python -m hypha_launcher launch_bioengine_worker --hypha-server-url https://ai.imjoy.io --triton-service-id my-triton
 ```
 
-Launch on slurm cluster.
+In the above example, the job command template is set to use the Slurm scheduler with the specified account and time limit. The `{cmd}` placeholder will be replaced with the actual command to launch jobs.
+
+Optionally, you can also set the store path for storing the models and the triton server configuration via the `HYPHA_LAUNCHER_STORE_DIR` environment variable. By default, the store path is set to `.hypha-launcher`.
 
 ```bash
-# Please replace the slurm settings with your own settings
-$ export SLURM_ACCOUNT=Your-Slurm-Account
-$ export SLURM_TIME=03:00:00
-$ export SLURM_GPUS_PER_NODE=A100:1
-$ python -m hypha_launcher launch_bioimageio_backend --service-id my-triton
+export HYPHA_LAUNCHER_STORE_DIR=".hypha-launcher"
 ```
 
 ### Download model from s3
 
 ```bash
-$ python -m hypha-launcher - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
+python -m hypha-launcher - download_models_from_s3 bioengine-model-runner.* --n_parallel=5
 ```
 
 ### Pull docker image of triton server
 
 ```bash
-$ python -m hypha-launcher - pull_image
+python -m hypha-launcher - pull_image
 ```
 
 ## TODO
 
 * [x] Download model from s3
 * [x] Pull docker image of triton server
 * [x] Run triton server
```

#### html2text {}

```diff
@@ -1,25 +1,39 @@
                          ************ hhyypphhaa--llaauunncchheerr ************
                            Run triton server on HPC
                        _[_I_n_s_t_a_l_l_ _w_i_t_h_ _P_y_P_i_]_[_M_I_T_ _l_i_c_e_n_s_e_]
 **Work In Progress** ## Features + CLI/API for: - downloading model from s3 and
 pulling docker image of triton server - launch s3 server - launch triton server
 - ... + Support different container engines - Docker - Apptainer + Support
 different compute environments - Local - Slurm ## Installation ```bash pip
-install hypha-launcher ``` ## CLI Usage ```bash $ hypha-launcher --help ``` ###
-Launch the bioimage.io backend Download all models from s3 and launch triton
-server. ```bash $ python -m hypha_launcher launch_bioimageio_backend --service-
-id my-triton ``` Launch on slurm cluster. ```bash # Please replace the slurm
-settings with your own settings $ export SLURM_ACCOUNT=Your-Slurm-Account $
-export SLURM_TIME=03:00:00 $ export SLURM_GPUS_PER_NODE=A100:1 $ python -
-m hypha_launcher launch_bioimageio_backend --service-id my-triton ``` ###
-Download model from s3 ```bash $ python -m hypha-launcher -
+install hypha-launcher ``` ## CLI Usage ```bash hypha-launcher --help ``` ###
+Launch the BioEngine Worker on HPC BioEngine consists of a set of services that
+are used to serve AI models from bioimage.io. We provide the model test run
+feature accessible from https://bioimage.io and a dedicated bioengine web
+client: https://bioimage-io.github.io/bioengine-web-client/. While our public
+instance is openly accessible for testing and evaluation, you can run your own
+instance of the BioEngine worker to serve the models, e.g. with your own HPC
+computing resources. Download all models from s3 and launch triton server.
+Launch on HPC cluster. You need to set the job command template via the
+`HYPHA_HPC_JOB_TEMPLATE` environment variable for your own HPC cluster. For
+example, here is an example for launching the BioEngine on a Slurm cluster:
+```bash # Please replace the job command with your own settings export
+HYPHA_HPC_JOB_TEMPLATE="srun -A Your-Slurm-Account -t 03:00:00 --gpus-per-node
+A100:1 {cmd}" python -m hypha_launcher launch_bioengine_worker --hypha-server-
+url https://ai.imjoy.io --triton-service-id my-triton ``` In the above example,
+the job command template is set to use the Slurm scheduler with the specified
+account and time limit. The `{cmd}` placeholder will be replaced with the
+actual command to launch jobs. Optionally, you can also set the store path for
+storing the models and the triton server configuration via the
+`HYPHA_LAUNCHER_STORE_DIR` environment variable. By default, the store path is
+set to `.hypha-launcher`. ```bash export HYPHA_LAUNCHER_STORE_DIR=".hypha-
+launcher" ``` ### Download model from s3 ```bash python -m hypha-launcher -
 download_models_from_s3 bioengine-model-runner.* --n_parallel=5 ``` ### Pull
-docker image of triton server ```bash $ python -m hypha-launcher - pull_image
-``` ## TODO * [x] Download model from s3 * [x] Pull docker image of triton
-server * [x] Run triton server * [x] Register service on hypha * [x]
-Conmmunicate with triton server * [x] Test on HPC * [ ] Support run on local
-machine without GPU * [ ] Support launch containers inside a container (For
-support run inside the podman-desktop) * [ ] Job management(Auto stop and
-restart) * [ ] Load balancing * [ ] Documentation ## Development Install the
-package in editable mode with the following command: ```bash pip install -e .
-pip install -r requirements-dev.txt ```
+docker image of triton server ```bash python -m hypha-launcher - pull_image ```
+## TODO * [x] Download model from s3 * [x] Pull docker image of triton server *
+[x] Run triton server * [x] Register service on hypha * [x] Conmmunicate with
+triton server * [x] Test on HPC * [ ] Support run on local machine without GPU
+* [ ] Support launch containers inside a container (For support run inside the
+podman-desktop) * [ ] Job management(Auto stop and restart) * [ ] Load
+balancing * [ ] Documentation ## Development Install the package in editable
+mode with the following command: ```bash pip install -e . pip install -
+r requirements-dev.txt ```
```

### Comparing `hypha_launcher-0.1.1/hypha_launcher/api.py` & `hypha_launcher-0.1.2/hypha_launcher/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,21 +25,23 @@
 
 logger = get_logger()
 
 
 class HyphaLauncher:
     def __init__(
             self,
-            store_dir: str = ".hypha_launcher",
+            store_dir: T.Optional[str] = None,
             debug: bool = False,
             container_engine_kwargs: T.Optional[T.Dict[str, T.Any]] = None,
             hpc_manager_kwargs: T.Optional[T.Dict[str, T.Any]] = None,
             executor_engine_kwargs: T.Optional[T.Dict[str, T.Any]] = None,
             ):
-        store_dir = os.environ.get("HYPHA_LAUNCHER_STORE_DIR", store_dir)
+        store_dir = store_dir or os.environ.get("HYPHA_LAUNCHER_STORE_DIR")
+        if store_dir is None:
+            store_dir = ".hypha_launcher"
         self.store_dir = Path(store_dir).expanduser().absolute()
         if not self.store_dir.exists():
             self.store_dir.mkdir(parents=True)
         logger.info(f"Store dir: {self.store_dir}")
         self.debug = debug
         if container_engine_kwargs is None:
             container_engine_kwargs = {
@@ -313,21 +315,21 @@
                             break
             await asyncio.sleep(1)
         if job.status == "failed":
             raise ValueError("Failed to launch Triton server")
         self._task_uuid_to_job[task_uuid] = job
         return job_dict
 
-    async def launch_bioimageio_backend(
+    async def launch_bioengine_worker(
             self,
             models_dir: T.Optional[str] = None,
             hypha_server_url: str = "https://ai.imjoy.io/",
-            service_name: str = "triton",
-            service_id: T.Optional[str] = None,
-            service_config: T.Optional[dict] = None,
+            triton_service_name: str = "triton",
+            triton_service_id: T.Optional[str] = None,
+            triton_service_config: T.Optional[dict] = None,
             ):
         if models_dir is None:
             models_dir = (self.store_dir / "models").as_posix()
         await self.download_models_from_s3(".*", models_dir)
         await self.launch_ip_record_server()
         triton_job = await self.launch_triton_server(models_dir)
         triton_address = triton_job['address']
@@ -359,30 +361,32 @@
                 )
                 return res
             except Exception as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
 
         server = await self._get_hypha_server(hypha_server_url)
-        if service_id is None:
-            service_id = f"{service_name}-{secrets.token_urlsafe(8)}"
-        logger.info(f"Registering service: {service_name} with id: {service_id}")
-        if service_config is None:
-            service_config = {"visibility": "public"}
+        if triton_service_id is None:
+            triton_service_id = f"{triton_service_name}-{secrets.token_urlsafe(8)}"
+        logger.info(f"Registering service: {triton_service_name} with id: {triton_service_id}")
+        if triton_service_config is None:
+            triton_service_config = {"visibility": "public"}
         await server.register_service(
             {
-                "name": service_name,
-                "id": service_id,
-                "config": service_config,
+                "name": triton_service_name,
+                "id": triton_service_id,
+                "type": "triton-client",
+                "config": triton_service_config,
                 "get_config": get_triton_config,
                 "execute": execute_triton,
             }
         )
 
         await self.engine.wait_async()
+        print(f"Bioengine worker is ready, you can try the BioEngine worker with the web client: https://bioimage-io.github.io/bioengine-web-client/?server-url={hypha_server_url}&triton-service-id={triton_service_id}")
 
     async def launch_hello_world(self):
         """Detect in which environment, docker/k8s/apptainer"""
         # detect env
         # print env name
         # launch a ubuntu, echo hello world from {ENV_NAME}
         pass
```

### Comparing `hypha_launcher-0.1.1/hypha_launcher/constants.py` & `hypha_launcher-0.1.2/hypha_launcher/constants.py`

 * *Files identical despite different names*

### Comparing `hypha_launcher-0.1.1/hypha_launcher/utils/container.py` & `hypha_launcher-0.1.2/hypha_launcher/utils/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     such as docker, apptainer, podman, etc.
     """
 
     supported_engines = ["docker", "apptainer", "podman"]
 
     def __init__(
         self,
-        store_dir: str = "~/.hypha_launcher/containers",
+        store_dir: str = ".hypha_launcher/containers",
         engine_type: T.Optional[str] = None,
     ):
 
         self.store_dir = Path(store_dir).expanduser()
         if not self.store_dir.exists():
             self.store_dir.mkdir(parents=True)
         if engine_type is not None:
```

### Comparing `hypha_launcher-0.1.1/hypha_launcher/utils/download.py` & `hypha_launcher-0.1.2/hypha_launcher/utils/download.py`

 * *Files identical despite different names*

### Comparing `hypha_launcher-0.1.1/hypha_launcher/utils/misc.py` & `hypha_launcher-0.1.2/hypha_launcher/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hypha_launcher-0.1.1/hypha_launcher.egg-info/SOURCES.txt` & `hypha_launcher-0.1.2/hypha_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypha_launcher-0.1.1/pyproject.toml` & `hypha_launcher-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "hypha-launcher"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 description = "Launcher for hypha services"
 authors = [
     {name = "Weize Xu", email = "vet.xwz@gmail.com" },
     {name = "Wei Ouyang", email = "oeway007@gmail.com" }
 ]
 dependencies = [
```

### Comparing `hypha_launcher-0.1.1/tests/test_api.py` & `hypha_launcher-0.1.2/tests/test_api.py`

 * *Files identical despite different names*

