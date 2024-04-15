# Comparing `tmp/missim_cli-1.8.0.tar.gz` & `tmp/missim_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missim_cli-1.8.0.tar", last modified: Mon Apr  8 01:46:59 2024, max compression
+gzip compressed data, was "missim_cli-1.9.0.tar", last modified: Wed Apr 10 08:34:15 2024, max compression
```

## Comparing `missim_cli-1.8.0.tar` & `missim_cli-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.711232 missim_cli-1.8.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-04-08 01:46:59.711232 missim_cli-1.8.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1072 2024-04-08 01:46:36.000000 missim_cli-1.8.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.707234 missim_cli-1.8.0/missim_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      411 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1313 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.711232 missim_cli-1.8.0/missim_cli/docker/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1894 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       84 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      241 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_editor.host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       52 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_editor.shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1307 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_editor.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       56 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_standalone.host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       64 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_standalone.shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      656 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_standalone.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      729 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/docker/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.711232 missim_cli-1.8.0/missim_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    14488 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/groups/base.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      251 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      831 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4212 2024-04-08 01:46:36.000000 missim_cli-1.8.0/missim_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-08 01:46:59.711232 missim_cli-1.8.0/missim_cli.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-04-08 01:46:59.000000 missim_cli-1.8.0/missim_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      963 2024-04-08 01:46:59.000000 missim_cli-1.8.0/missim_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-08 01:46:59.000000 missim_cli-1.8.0/missim_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-04-08 01:46:59.000000 missim_cli-1.8.0/missim_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       75 2024-04-08 01:46:59.000000 missim_cli-1.8.0/missim_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       11 2024-04-08 01:46:59.000000 missim_cli-1.8.0/missim_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-08 01:46:51.000000 missim_cli-1.8.0/missim_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)     1002 2024-04-08 01:46:59.711232 missim_cli-1.8.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-08 01:46:36.000000 missim_cli-1.8.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.441863 missim_cli-1.9.0/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-04-10 08:34:15.441863 missim_cli-1.9.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1072 2024-04-10 08:33:53.000000 missim_cli-1.9.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.441863 missim_cli-1.9.0/missim_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      411 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1313 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.441863 missim_cli-1.9.0/missim_cli/docker/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1894 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       84 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      241 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_editor.host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       52 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_editor.shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1332 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_editor.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       56 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_standalone.host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       64 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_standalone.shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      681 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_standalone.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      773 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/docker/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.441863 missim_cli-1.9.0/missim_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    14757 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/groups/base.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      251 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      831 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4212 2024-04-10 08:33:53.000000 missim_cli-1.9.0/missim_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-10 08:34:15.441863 missim_cli-1.9.0/missim_cli.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-04-10 08:34:15.000000 missim_cli-1.9.0/missim_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      963 2024-04-10 08:34:15.000000 missim_cli-1.9.0/missim_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 08:34:15.000000 missim_cli-1.9.0/missim_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-04-10 08:34:15.000000 missim_cli-1.9.0/missim_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       75 2024-04-10 08:34:15.000000 missim_cli-1.9.0/missim_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       11 2024-04-10 08:34:15.000000 missim_cli-1.9.0/missim_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-10 08:34:06.000000 missim_cli-1.9.0/missim_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1002 2024-04-10 08:34:15.441863 missim_cli-1.9.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-10 08:33:53.000000 missim_cli-1.9.0/setup.py
```

### Comparing `missim_cli-1.8.0/PKG-INFO` & `missim_cli-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: A CLI for interacting with the MISSIM platform
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_cli-1.8.0/README.md` & `missim_cli-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `missim_cli-1.8.0/missim_cli/cli.py` & `missim_cli-1.9.0/missim_cli/cli.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.8.0/missim_cli/docker/docker-compose.dev.yaml` & `missim_cli-1.9.0/missim_cli/docker/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_editor.yaml` & `missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_editor.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -32,13 +32,14 @@
       - DISPLAY
       - QT_X11_NO_MITSHM=1
       - XAUTHORITY
       - PROJECTS_HOME=/home/ue4/Unreal Projects
       - PROJECT_NAME=MissimProject
       - UNREAL_HOME=/home/ue4/UnrealEngine
       - ROS_DOMAIN_ID
+      - ROS_STATIC_PEERS
 
 secrets:
   API_TOKEN_GITHUB:
     file: ./.secrets/API_TOKEN_GITHUB
   apt_conf:
     file: ./.secrets/apt.conf
```

### Comparing `missim_cli-1.8.0/missim_cli/docker/docker-compose.ue_standalone.yaml` & `missim_cli-1.9.0/missim_cli/docker/docker-compose.ue_standalone.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -19,7 +19,8 @@
     environment:
       - DISPLAY
       - XDG_RUNTIME_DIR
       - QT_X11_NO_MITSHM=1
       - XAUTHORITY
       - SIM_ARGS=-ResX=1280 -ResY=720 -WINDOWED
       - ROS_DOMAIN_ID
+      - ROS_STATIC_PEERS
```

### Comparing `missim_cli-1.8.0/missim_cli/groups/base.py` & `missim_cli-1.9.0/missim_cli/groups/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,20 +101,21 @@
 )
 def build(mode: Mode, clean: bool, services: List[str]):
     """Builds the sim"""
     # If building standalone, we first build the dev sim
 
     config = missim_config.read()
     os.environ["ROS_DOMAIN_ID"] = str(config.ros_domain_id)
+    os.environ["ROS_STATIC_PEERS"] = str(config.static_peers)
     log_config(config)
 
     services_list = list(services) if services else None
     if config.mode == Mode.LOW_FIDELITY:
         docker = DockerClient(
-            compose_files=_get_compose_files(config.mode, config.network),
+            compose_files=_get_compose_files(mode=config.mode, network=config.network),
             compose_project_directory=get_project_root(),
         )
         docker.compose.build(services=services_list)
         return
 
     # If we are not low-fidelity, we must do Unreal things....
 
@@ -181,14 +182,15 @@
 )
 def up(spin: bool, build: bool, services: List[str]):
     """Starts the simulator"""
     config = missim_config.read()
     mode = config.mode
     dev_mode = is_dev_version()
     os.environ["ROS_DOMAIN_ID"] = str(config.ros_domain_id)
+    os.environ["ROS_STATIC_PEERS"] = str(config.static_peers)
     os.environ["USE_HTTPS"] = "true" if config.use_https else "false"
     os.environ["MISSIM_VERSION"] = get_missim_version()
     os.environ["MISSIM_CONFIG"] = missim_config.serialise(config)
     log_config(config)
 
     docker = DockerClient(
         compose_files=_get_compose_files(mode, dev_mode=dev_mode, network=config.network),
@@ -354,14 +356,17 @@
         except Exception:
             config_current = MissimConfig()
 
         config = MissimConfig(
             ros_domain_id=click.prompt(
                 "ROS domain ID", default=config_current.ros_domain_id, type=int
             ),
+            static_peers=click.prompt(
+                "Static peers", default=config_current.static_peers, type=str
+            ),
             network=click.prompt(
                 "Network",
                 default=config_current.network,
                 type=click.Choice([item.value for item in Network]),
             ),
             log_level=click.prompt(
                 "Log level",
```

### Comparing `missim_cli-1.8.0/missim_cli/groups/setup.py` & `missim_cli-1.9.0/missim_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.8.0/missim_cli/helpers.py` & `missim_cli-1.9.0/missim_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.8.0/missim_cli.egg-info/PKG-INFO` & `missim_cli-1.9.0/missim_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: A CLI for interacting with the MISSIM platform
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_cli-1.8.0/missim_cli.egg-info/SOURCES.txt` & `missim_cli-1.9.0/missim_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `missim_cli-1.8.0/setup.cfg` & `missim_cli-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = missim_cli
-version = 1.8.0
+version = 1.9.0
 url = https://github.com/Greenroom-Robotics/missim
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

