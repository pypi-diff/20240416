# Comparing `tmp/pycityagent-1.1.8.tar.gz` & `tmp/pycityagent-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.1.8.tar", last modified: Sat Apr 13 15:44:00 2024, max compression
+gzip compressed data, was "pycityagent-1.1.9.tar", last modified: Tue Apr 16 13:57:51 2024, max compression
```

## Comparing `pycityagent-1.1.8.tar` & `pycityagent-1.1.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-13 15:43:55.000000 pycityagent-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 15:44:00.028281 pycityagent-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-13 15:43:55.000000 pycityagent-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.020281 pycityagent-1.1.8/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.020281 pycityagent-1.1.8/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/action_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.024281 pycityagent-1.1.8/pycityagent/ac/citizen_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/citizen_actions/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/citizen_actions/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/citizen_actions/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/citizen_actions/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/citizen_actions/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/hub_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/ac/sim_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/agent_citizen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/agent_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.024281 pycityagent-1.1.8/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.024281 pycityagent-1.1.8/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.024281 pycityagent-1.1.8/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.024281 pycityagent-1.1.8/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28861 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:44:00.028281 pycityagent-1.1.8/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 15:44:00.000000 pycityagent-1.1.8/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 15:44:00.000000 pycityagent-1.1.8/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:44:00.000000 pycityagent-1.1.8/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-13 15:44:00.000000 pycityagent-1.1.8/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 15:44:00.000000 pycityagent-1.1.8/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-13 15:43:55.000000 pycityagent-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:44:00.028281 pycityagent-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 13:57:42.000000 pycityagent-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-16 13:57:51.072736 pycityagent-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-16 13:57:42.000000 pycityagent-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.064736 pycityagent-1.1.9/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.068736 pycityagent-1.1.9/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.068736 pycityagent-1.1.9/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.068736 pycityagent-1.1.9/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.068736 pycityagent-1.1.9/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28858 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:51.072736 pycityagent-1.1.9/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-16 13:57:51.000000 pycityagent-1.1.9/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-16 13:57:51.000000 pycityagent-1.1.9/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:57:51.000000 pycityagent-1.1.9/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-16 13:57:51.000000 pycityagent-1.1.9/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 13:57:51.000000 pycityagent-1.1.9/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 13:57:42.000000 pycityagent-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:57:51.072736 pycityagent-1.1.9/setup.cfg
```

### Comparing `pycityagent-1.1.8/LICENSE` & `pycityagent-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/PKG-INFO` & `pycityagent-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.8
+Version: 1.1.9
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,17 +75,18 @@
 llm_request:
   text_request:
     request_type: openai / qwen
     api_key: xxx
     model: xxx
     (api_base): xxx (this is an optional config, if you use opanai and want to use your own backend LLM model, default to "https://api.openai.com/v1")
   img_understand_request:
-    request_type: qwen
+    request_type: openai / qwen
     api_key: xxx
-    model: xxx
+    model: xxx ('gpt-4-turbo' if you use openai)
+    (api_base): same as text_request
   img_generate_request:
     request_type: qwen
     api_key: xxx
     model: xxx
 
 citysim_request:
   simulator: 
@@ -106,19 +107,27 @@
   app_secret: your APP Secret
   profile_image: the profile image of your agent
 ```
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
 - As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
-- By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
-    - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
-- Get your **api_key** and chooce your **model**
-- If you want to use your backend models, set the **api_base** (only available when using **openai**)
-  - default value: "https://api.openai.com/v1"
+- **text_request**
+  - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
+      - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
+  - Get your **api_key** and chooce your **model**
+  - If you want to use your backend models, set the **api_base** (only available when using **openai**)
+    - default value: "https://api.openai.com/v1"
+- **img_understand_request**
+  - By now, we support **qwen** and **openai**
+  - If choose **openai**, then the **model** has to be '**gpt-4-turbo**'
+  - If you want to use your backend models, set the **api_base** (only available when using **openai**)
+      - default value: "https://api.openai.com/v1"
+- **img_generate_request**
+  - By now, only [**qwen**] is supported
 
 #### CITYSIM_REQUEST
 - Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
 - **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
 - **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
   - if you choose baidumap engine, you need to get a baidumap api-key
     ``` yaml
```

### Comparing `pycityagent-1.1.8/README.md` & `pycityagent-1.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 llm_request:
   text_request:
     request_type: openai / qwen
     api_key: xxx
     model: xxx
     (api_base): xxx (this is an optional config, if you use opanai and want to use your own backend LLM model, default to "https://api.openai.com/v1")
   img_understand_request:
-    request_type: qwen
+    request_type: openai / qwen
     api_key: xxx
-    model: xxx
+    model: xxx ('gpt-4-turbo' if you use openai)
+    (api_base): same as text_request
   img_generate_request:
     request_type: qwen
     api_key: xxx
     model: xxx
 
 citysim_request:
   simulator: 
@@ -59,19 +60,27 @@
   app_secret: your APP Secret
   profile_image: the profile image of your agent
 ```
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
 - As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
-- By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
-    - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
-- Get your **api_key** and chooce your **model**
-- If you want to use your backend models, set the **api_base** (only available when using **openai**)
-  - default value: "https://api.openai.com/v1"
+- **text_request**
+  - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
+      - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
+  - Get your **api_key** and chooce your **model**
+  - If you want to use your backend models, set the **api_base** (only available when using **openai**)
+    - default value: "https://api.openai.com/v1"
+- **img_understand_request**
+  - By now, we support **qwen** and **openai**
+  - If choose **openai**, then the **model** has to be '**gpt-4-turbo**'
+  - If you want to use your backend models, set the **api_base** (only available when using **openai**)
+      - default value: "https://api.openai.com/v1"
+- **img_generate_request**
+  - By now, only [**qwen**] is supported
 
 #### CITYSIM_REQUEST
 - Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
 - **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
 - **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
   - if you choose baidumap engine, you need to get a baidumap api-key
     ``` yaml
```

### Comparing `pycityagent-1.1.8/pycityagent/ac/ac.py` & `pycityagent-1.1.9/pycityagent/ac/ac.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/action.py` & `pycityagent-1.1.9/pycityagent/ac/action.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/action_stream.py` & `pycityagent-1.1.9/pycityagent/ac/action_stream.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/citizen_actions/controled.py` & `pycityagent-1.1.9/pycityagent/ac/citizen_actions/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/citizen_actions/converse.py` & `pycityagent-1.1.9/pycityagent/ac/citizen_actions/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/citizen_actions/idle.py` & `pycityagent-1.1.9/pycityagent/ac/citizen_actions/idle.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/citizen_actions/shop.py` & `pycityagent-1.1.9/pycityagent/ac/citizen_actions/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/citizen_actions/trip.py` & `pycityagent-1.1.9/pycityagent/ac/citizen_actions/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/hub_actions.py` & `pycityagent-1.1.9/pycityagent/ac/hub_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/ac/sim_actions.py` & `pycityagent-1.1.9/pycityagent/ac/sim_actions.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/agent.py` & `pycityagent-1.1.9/pycityagent/agent.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/agent_citizen.py` & `pycityagent-1.1.9/pycityagent/agent_citizen.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/agent_func.py` & `pycityagent-1.1.9/pycityagent/agent_func.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/brain.py` & `pycityagent-1.1.9/pycityagent/brain/brain.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/memory.py` & `pycityagent-1.1.9/pycityagent/brain/memory.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.9/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.9/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/reason/social.py` & `pycityagent-1.1.9/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.9/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/reason/user.py` & `pycityagent-1.1.9/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/scheduler.py` & `pycityagent-1.1.9/pycityagent/brain/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/brain/sence.py` & `pycityagent-1.1.9/pycityagent/brain/sence.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,18 +142,18 @@
 
         self.plug_buffer = {}
         """
         感知插件结果Buffer: 用于存储感知插件的输出结果
         SencePlug Buffer: used to store those sence plug content
         """
 
-        self.enable_streeview = False
+        self.enable_streeview = True
         """
-        街景感知功能接口, 默认为False
-        Interface of streetview function, defualt: False
+        街景感知功能接口, 默认为True
+        Interface of streetview function, defualt: True
         """
 
         self._lane_type_mapping = {1: 'driving', 2: 'walking'}
 
     def set_sence(self, content: list):
         """
         感知配置接口
```

### Comparing `pycityagent-1.1.8/pycityagent/brain/static.py` & `pycityagent-1.1.9/pycityagent/brain/static.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/cc/cc.py` & `pycityagent-1.1.9/pycityagent/cc/cc.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.9/pycityagent/hubconnector/hubconnector.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/image/image.py` & `pycityagent-1.1.9/pycityagent/image/image.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/simulator.py` & `pycityagent-1.1.9/pycityagent/simulator.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/st/st.py` & `pycityagent-1.1.9/pycityagent/st/st.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.9/pycityagent/urbanllm/urbanllm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """UrbanLLM: 智能能力类及其定义"""
 
 from openai import OpenAI
 from http import HTTPStatus
 import dashscope
-from urllib.parse import urlparse, unquote
-from pathlib import PurePosixPath
 import requests
 from dashscope import ImageSynthesis
 from PIL import Image
 from io import BytesIO
+from typing import Union
+import base64
+
+def encode_image(image_path):
+  with open(image_path, "rb") as image_file:
+    return base64.b64encode(image_file.read()).decode('utf-8')
 
 class LLMConfig:
     """
     大语言模型相关配置
     The config of LLM
     """
     def __init__(
@@ -80,45 +84,93 @@
                 return response.output.choices[0]['message']['content']
             else:
                 return "Error: {}".format(response.status_code)
         else:
             print("ERROR: Wrong Config")
             return "wrong config"
 
-    def img_understand(self, img_path:str, prompt:str=None) -> str:
+    def img_understand(self, img_path:Union[str, list[str]], prompt:str=None) -> str:
         """
         图像理解
         Image understanding
 
         Args:
-        - img_path: 目标图像的路径. The path of selected Image
-        - prompt: 理解提示词 - 例如理解方向. The understanding prompts
+        - img_path (Union[str, list[str]]): 目标图像的路径, 既可以是一个路径也可以是包含多张图片路径的list. The path of selected Image
+        - prompt (str): 理解提示词 - 例如理解方向. The understanding prompts
 
         Returns:
         - (str): the understanding content
         """
         ppt = "如何理解这幅图像？"
         if prompt != None:
             ppt = prompt
-        dialog = [{
-            'role': 'user',
-            'content': [
-                {'image': 'file://' + img_path},
-                {'text': ppt}
-            ]
-        }]
-        response = dashscope.MultiModalConversation.call(
-                    model=self.config.image_u['model'],
-                    api_key=self.config.image_u['api_key'],
-                    messages=dialog
-                )
-        if response.status_code == HTTPStatus.OK:
-            return response.output.choices[0]['message']['content']
+        if self.config.image_u['request_type'] == 'openai':
+            if 'api_base' in self.config.image_u.keys():
+                api_base = self.config.image_u['api_base']
+            else:
+                api_base = None
+            client = OpenAI(
+                api_key=self.config.text['api_key'], 
+                base_url=api_base,
+            )
+            content = []
+            content.append({'type': 'text', 'text': ppt})
+            if isinstance(img_path, str):
+                base64_image = encode_image(img_path)
+                content.append({
+                    'type': 'image_url', 
+                    'image_url': {
+                            'url': f"data:image/jpeg;base64,{base64_image}"
+                        }
+                })
+            elif isinstance(img_path, list) and all(isinstance(item, str) for item in img_path):
+                for item in img_path:
+                    base64_image = encode_image(item)
+                    content.append({
+                        'type': 'image_url',
+                        'image_url': {
+                            'url': f"data:image/jpeg;base64,{base64_image}"
+                        }
+                    })
+            response = client.chat.completions.create(
+                model=self.config.image_u['model'],
+                messages=[{
+                    'role': 'user',
+                    'content': content
+                }]
+            )
+            return response.choices[0].message.content
+        elif self.config.image_u['request_type'] == 'qwen':
+            content = []
+            if isinstance(img_path, str):
+                content.append({'image': 'file://' + img_path})
+                content.append({'text': ppt})
+            elif isinstance(img_path, list) and all(isinstance(item, str) for item in img_path):
+                for item in img_path:
+                    content.append({
+                        'image': 'file://' + item
+                    })
+                content.append({'text': ppt})
+
+            dialog = [{
+                'role': 'user',
+                'content': content
+            }]
+            response = dashscope.MultiModalConversation.call(
+                        model=self.config.image_u['model'],
+                        api_key=self.config.image_u['api_key'],
+                        messages=dialog
+                    )
+            if response.status_code == HTTPStatus.OK:
+                return response.output.choices[0]['message']['content']
+            else:
+                print(response.code)  # The error code.
+                return "Error"
         else:
-            print(response.code)  # The error code.
+            print("ERROR: wrong image understanding type, only 'openai' and 'openai' is available")
             return "Error"
 
     def img_generate(self, prompt:str, size:str='512*512', quantity:int = 1):
         """
         图像生成
         Image generation
```

### Comparing `pycityagent-1.1.8/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.9/pycityagent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.8
+Version: 1.1.9
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,17 +75,18 @@
 llm_request:
   text_request:
     request_type: openai / qwen
     api_key: xxx
     model: xxx
     (api_base): xxx (this is an optional config, if you use opanai and want to use your own backend LLM model, default to "https://api.openai.com/v1")
   img_understand_request:
-    request_type: qwen
+    request_type: openai / qwen
     api_key: xxx
-    model: xxx
+    model: xxx ('gpt-4-turbo' if you use openai)
+    (api_base): same as text_request
   img_generate_request:
     request_type: qwen
     api_key: xxx
     model: xxx
 
 citysim_request:
   simulator: 
@@ -106,19 +107,27 @@
   app_secret: your APP Secret
   profile_image: the profile image of your agent
 ```
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
 - As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
-- By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
-    - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
-- Get your **api_key** and chooce your **model**
-- If you want to use your backend models, set the **api_base** (only available when using **openai**)
-  - default value: "https://api.openai.com/v1"
+- **text_request**
+  - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
+      - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
+  - Get your **api_key** and chooce your **model**
+  - If you want to use your backend models, set the **api_base** (only available when using **openai**)
+    - default value: "https://api.openai.com/v1"
+- **img_understand_request**
+  - By now, we support **qwen** and **openai**
+  - If choose **openai**, then the **model** has to be '**gpt-4-turbo**'
+  - If you want to use your backend models, set the **api_base** (only available when using **openai**)
+      - default value: "https://api.openai.com/v1"
+- **img_generate_request**
+  - By now, only [**qwen**] is supported
 
 #### CITYSIM_REQUEST
 - Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
 - **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
 - **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
   - if you choose baidumap engine, you need to get a baidumap api-key
     ``` yaml
```

### Comparing `pycityagent-1.1.8/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.9/pycityagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.8/pyproject.toml` & `pycityagent-1.1.9/pyproject.toml`

 * *Files identical despite different names*

