# Comparing `tmp/jupyter_nebulagraph-0.11.1.tar.gz` & `tmp/jupyter_nebulagraph-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_nebulagraph-0.11.1.tar", last modified: Tue Apr 16 09:11:18 2024, max compression
+gzip compressed data, was "jupyter_nebulagraph-0.9.1.tar", last modified: Thu Apr  4 03:35:06 2024, max compression
```

## Comparing `jupyter_nebulagraph-0.11.1.tar` & `jupyter_nebulagraph-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:11:18.443358 jupyter_nebulagraph-0.11.1/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-16 09:11:14.000000 jupyter_nebulagraph-0.11.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-16 09:11:18.443358 jupyter_nebulagraph-0.11.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-16 09:11:14.000000 jupyter_nebulagraph-0.11.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:11:18.443358 jupyter_nebulagraph-0.11.1/jupyter_nebulagraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-16 09:11:18.000000 jupyter_nebulagraph-0.11.1/jupyter_nebulagraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 09:11:18.000000 jupyter_nebulagraph-0.11.1/jupyter_nebulagraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:11:18.000000 jupyter_nebulagraph-0.11.1/jupyter_nebulagraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 09:11:18.000000 jupyter_nebulagraph-0.11.1/jupyter_nebulagraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 09:11:18.000000 jupyter_nebulagraph-0.11.1/jupyter_nebulagraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:11:18.443358 jupyter_nebulagraph-0.11.1/ngql/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 09:11:14.000000 jupyter_nebulagraph-0.11.1/ngql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37409 2024-04-16 09:11:14.000000 jupyter_nebulagraph-0.11.1/ngql/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:11:18.443358 jupyter_nebulagraph-0.11.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-16 09:11:14.000000 jupyter_nebulagraph-0.11.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 03:35:06.000000 jupyter_nebulagraph-0.9.1/jupyter_nebulagraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/ngql/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/ngql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36253 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/ngql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:35:06.305795 jupyter_nebulagraph-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-04 03:35:02.000000 jupyter_nebulagraph-0.9.1/setup.py
```

### Comparing `jupyter_nebulagraph-0.11.1/LICENSE` & `jupyter_nebulagraph-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_nebulagraph-0.11.1/README.md` & `jupyter_nebulagraph-0.9.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/61fccff2-c9be-43a0-a26f-6f5a00b1c198)
-
 
 [![for NebulaGraph](https://img.shields.io/badge/Toolchain-NebulaGraph-blue)](https://github.com/vesoft-inc/nebula) [![Jupyter](https://img.shields.io/badge/Jupyter-Supported-brightgreen)](https://github.com/jupyterlab/jupyterlab) [![Docker Image](https://img.shields.io/docker/v/weygu/nebulagraph-jupyter?label=Image&logo=docker)](https://hub.docker.com/r/weygu/nebulagraph-jupyter) [![Docker Extension](https://img.shields.io/badge/Docker-Extension-blue?logo=docker)](https://hub.docker.com/extensions/weygu/nebulagraph-dd-ext) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/wey-gu/jupyter_nebulagraph?label=Version)](https://github.com/wey-gu/jupyter_nebulagraph/releases)
 [![pypi-version](https://img.shields.io/pypi/v/jupyter_nebulagraph)](https://pypi.org/project/jupyter_nebulagraph/)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb)
-[![Documentation](https://img.shields.io/badge/docs-Read%20The%20Docs-blue)](https://jupyter-nebulagraph.readthedocs.io/)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb)
 
 
 https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/10135264-77b5-4d3c-b68f-c5810257feeb
+`jupyter_nebulagraph` (previously known as `ipython-ngql`) is a Python package designed to facilitate connections to NebulaGraph directly from Jupyter Notebooks or iPython environments. It streamlines the process of creating, debugging, and sharing Jupyter Notebooks that interact with NebulaGraph, enhancing collaborative efforts.
 
-`jupyter_nebulagraph`, formerly `ipython-ngql`, is a Python package that simplifies the process of connecting to NebulaGraph from Jupyter Notebooks or iPython environments. It enhances the user experience by streamlining the creation, debugging, and sharing of Jupyter Notebooks. With `jupyter_nebulagraph`, users can effortlessly connect to NebulaGraph, load data, execute queries, visualize results, and fine-tune query outputs, thereby boosting collaborative efforts and productivity.
+Inspired by [ipython-sql](https://github.com/catherinedevlin/ipython-sql) by [Catherine Devlin](https://catherinedevlin.blogspot.com/).
 
-![](https://github.com/wey-gu/jupyter_nebulagraph/assets/1651790/b3d9ca07-2eb1-45ae-949b-543f58a57760)
 
-## Getting Started
+![](https://user-images.githubusercontent.com/1651790/236798634-8ccb3b5c-8a4f-4834-b602-10eeb2678bc8.png)
 
-Explore the capabilities of `jupyter_nebulagraph` by trying it on [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/docs/get_started.ipynb), and the equivalent Jupyter Notebook is available in Docs [here](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/).
+![](https://user-images.githubusercontent.com/1651790/236798238-49dd59c9-0827-4a86-b714-fb195e6be4b9.png)
 
-For a comprehensive guide, visit the [official documentation](https://jupyter-nebulagraph.readthedocs.io/).
 
-| Feature | Cheat Sheet | Example | Command Documentation |
-| ------- | ----------- | --------- | ---------------------- |
-| Connect | `%ngql --address 127.0.0.1 --port 9669 --user user --password password` | [Connect](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/#connect-to-nebulagraph) | [`%ngql`](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ngql/#connect-to-nebulagraph) |
-| Load Data from CSV | `%ng_load --source actor.csv --tag player --vid 0 --props 1:name,2:age --space basketballplayer` | [Load Data](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/#load-data-from-csv) | [`%ng_load`](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ng_load/) |
-| Query Execution | `%ngql MATCH p=(v:player{name:"Tim Duncan"})-->(v2:player) RETURN p;`| [Query Execution](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/#query) | [`%ngql` or `%%ngql`(multi-line)](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ngql/#make-queries) |
-| Result Visualization | `%ng_draw` | [Draw Graph](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ng_draw/) | [`%ng_draw`](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ng_draw/) |
-| Draw Schema | `%ng_draw_schema` | [Draw Schema](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ng_draw_schema/) | [`%ng_draw_schema`](https://jupyter-nebulagraph.readthedocs.io/en/latest/magic_words/ng_draw_schema/) |
-| Tweak Query Result | `df = _` to get last query result as `pd.dataframe` or [`ResultSet`](https://github.com/vesoft-inc/nebula-python/blob/master/nebula3/data/ResultSet.py) | [Tweak Result](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/#result-handling) | [Configure `ngql_result_style`](https://jupyter-nebulagraph.readthedocs.io/en/latest/configurations/#configure-ngql_result_style) |
+## Get Started
 
+Try it out in [Google Colab](https://colab.research.google.com/github/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
-<details>
-<summary>Click to see more!</summary>
+Or see the getting started guide [here](https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb).
 
 ### Installation
 
 `jupyter_nebulagraph` could be installed either via pip or from this git repo itself.
 
 > Install via pip
 
@@ -88,14 +77,16 @@
 
 ```python
 %%ngql
 SHOW TAGS;
 SHOW HOSTS;
 ```
 
+> There will be other options in future, i.e. from a `.ngql` file.
+
 ### Query String with Variables
 
 `jupyter_nebulagraph` supports taking variables from the local namespace, with the help of [Jinja2](https://jinja.palletsprojects.com/) template framework, it's supported to have queries like the below example.
 
 The actual query string should be `GO FROM "Sue" OVER owns_pokemon ...`, and `"{{ trainer }}"` was renderred as `"Sue"` by consuming the local variable `trainer`:
 
 ```python
@@ -161,36 +152,101 @@
 %ng_load --source https://github.com/wey-gu/jupyter_nebulagraph/raw/main/examples/actor.csv --tag player --vid 0 --props 1:name,2:age --space demo_basketballplayer
 # with rank column
 %ng_load --source follow_with_rank.csv --edge follow --src 0 --dst 1 --props 2:degree --rank 3 --space basketballplayer
 # without rank column
 %ng_load --source follow.csv --edge follow --src 0 --dst 1 --props 2:degree --space basketballplayer
 ```
 
-### Tweak Query Result
+### Configure `ngql_result_style`
 
-By default, the query result is a Pandas Dataframe, and we could access that by read from variable `_`.
+By default, `jupyter_nebulagraph` will use pandas dataframe as output style to enable more human-readable output, while it's supported to use the raw thrift data format that comes from the `nebula3-python` itself.
+
+This can be done ad-hoc with below one line:
 
 ```python
-In [1]: %ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
+%config IPythonNGQL.ngql_result_style="raw"
+```
 
-In [2]: df = _
+After the above line is executed, the output will be like this:
+
+```python
+ResultSet(ExecutionResponse(
+    error_code=0,
+    latency_in_us=2844,
+    data=DataSet(
+        column_names=[b'Trainer_Name'],
+        rows=[Row(
+            values=[Value(
+                sVal=b'Tom')]),
+...
+        Row(
+            values=[Value(
+                sVal=b'Wey')])]),
+    space_name=b'pokemon_club'))
 ```
 
-It's also configurable to have the result in raw ResultSet, to enable handy NebulaGraph Python App Development.
+The result are always stored in variable `_` in Jupyter Notebook, thus, to tweak the result, just refer a new var to it like:
+
+```python
+In [1] : %config IPythonNGQL.ngql_result_style="raw"
+
+In [2] : %%ngql USE pokemon_club;
+    ...: GO FROM "Tom" OVER owns_pokemon YIELD owns_pokemon._dst as pokemon_id
+    ...: | GO FROM $-.pokemon_id OVER owns_pokemon REVERSELY YIELD owns_pokemon._dst AS Trainer_Name;
+    ...:
+    ...:
+Out[3]:
+ResultSet(ExecutionResponse(
+    error_code=0,
+    latency_in_us=3270,
+    data=DataSet(
+        column_names=[b'Trainer_Name'],
+        rows=[Row(
+            values=[Value(
+                sVal=b'Tom')]),
+...
+        Row(
+            values=[Value(
+                sVal=b'Wey')])]),
+    space_name=b'pokemon_club'))
+
+In [4]: r = _
 
-See more via [Docs: Result Handling](https://jupyter-nebulagraph.readthedocs.io/en/latest/get_started_docs/#result-handling)
+In [5]: r.column_values(key='Trainer_Name')[0].cast()
+Out[5]: 'Tom'
+```
 
-### CheatSheet
+### Get Help
 
-If you find yourself forgetting commands or not wanting to rely solely on the cheat sheet, remember this one thing: seek help through the help command!
+Don't remember anything or even relying on the cheatsheet here, oen takeaway for you: the help!
 
 ```python
-%ngql help
+In [1]: %ngql help
 ```
 
-</details>
+### Examples
+
+#### Jupyter Notebook
+
+Please refer here:https://github.com/wey-gu/jupyter_nebulagraph/blob/main/examples/get_started.ipynb
 
-## Acknowledgments ♥️
+#### iPython
 
-- Inspiration for this project comes from [ipython-sql](https://github.com/catherinedevlin/ipython-sql), courtesy of [Catherine Devlin](https://catherinedevlin.blogspot.com/).
-- Graph visualization features are enabled by [pyvis](https://github.com/WestHealth/pyvis), a project by [WestHealth](https://github.com/WestHealth).
-- Generous sponsorship and support provided by [Vesoft Inc.](https://www.vesoft.com/) and the [NebulaGraph community](https://github.com/vesoft-inc/nebula).
+```python
+In [1]: %load_ext ngql
+
+In [2]: %ngql --address 192.168.8.128 --port 9669 --user root --password nebula
+Connection Pool Created
+Out[2]: 
+                        Name
+0           basketballplayer
+1  demo_movie_recommendation
+2                        k8s
+3                       test
+
+In [3]: %ngql USE basketballplayer;
+   ...: %ngql MATCH (v:player{name:"Tim Duncan"})-->(v2:player) RETURN v2.player.name AS Name;
+Out[3]: 
+            Name
+0    Tony Parker
+1  Manu Ginobili
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jupyter_nebulagraph-0.11.1/ngql/magic.py` & `jupyter_nebulagraph-0.9.1/ngql/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from jinja2 import Template, Environment, meta
 from traitlets.config.configurable import Configurable
 from traitlets import Bool, Int, Unicode
 
 from nebula3.data.DataObject import Node, Relationship, PathWrapper
 from nebula3.gclient.net import ConnectionPool as NebulaConnectionPool
 from nebula3.Config import Config as NebulaConfig
-from nebula3.Config import SSL_config
 
 
 rel_query_sample_edge = Template(
     """
 MATCH ()-[e:`{{ edge_type }}`]->()
 RETURN [src(e), dst(e)] AS sample_edge LIMIT 1
 """
@@ -161,27 +160,17 @@
             else:  # all connection information ready
                 connection_pool = NebulaConnectionPool()
                 config = NebulaConfig()
                 if self.max_connection_pool_size:
                     config.max_connection_pool_size = self.max_connection_pool_size
 
                 self.credential = args.user, args.password
-                try:
-                    connect_init_result = connection_pool.init(
-                        [(args.address, args.port)], config
-                    )
-                except RuntimeError:
-                    # When GraphD is over TLS
-                    print(
-                        "Got RuntimeError, trying to connect assuming GraphD is over TLS"
-                    )
-                    ssl_config = SSL_config()
-                    connect_init_result = connection_pool.init(
-                        [(args.address, args.port)], config, ssl_config
-                    )
+                connect_init_result = connection_pool.init(
+                    [(args.address, args.port)], config
+                )
                 if not connect_init_result:
                     return CONNECTION_POOL_INIT_FAILURE
                 else:
                     self.connection_pool = connection_pool
                     return CONNECTION_POOL_CREATED
 
         # else a.k.a not any(connection_info)
@@ -606,20 +595,18 @@
             else:
                 g_nx.add_node(node_id, **props)
         elif isinstance(item, Relationship):
             src_id = str(item.start_vertex_id().cast())
             dst_id = str(item.end_vertex_id().cast())
             edge_name = item.edge_name()
             props_raw = item.properties()
-            rank = item.ranking()
             props = {
                 k: str(v.cast()) if hasattr(v, "cast") else str(v)
                 for k, v in props_raw.items()
             }
-            props.update({"rank": rank})
             # ensure start and end vertex exist in graph
             if not src_id in g.node_ids:
                 g.add_node(
                     src_id,
                     label=str(src_id),
                     title=str(src_id),
                     color=get_color(src_id),
@@ -635,21 +622,15 @@
             for k in props:
                 if len(props_str_list) >= 1:
                     break
                 props_str_list.append(f"{truncate(k, 7)}: {truncate(str(props[k]), 8)}")
             props_str = "\n".join(props_str_list)
 
             label = f"{props_str}\n{edge_name}" if props else edge_name
-            g.add_edge(
-                src_id,
-                dst_id,
-                label=label,
-                title=str(props),
-                weight=props.get("rank", 0),
-            )
+            g.add_edge(src_id, dst_id, label=label, title=str(props))
             # networkx
             props["edge_type"] = edge_name
             g_nx.add_edge(src_id, dst_id, **props)
 
         elif isinstance(item, PathWrapper):
             for node in item.nodes():
                 self.render_pd_item(g, g_nx, node)
@@ -879,19 +860,15 @@
             # Now prepare INSERT query for vertices in batches
             # Example of QUERY: INSERT VERTEX t2 (name, age) VALUES "13":("n3", 12), "14":("n4", 8);
 
             for i in tqdm(
                 range(0, len(vertex_data), batch_size), desc="Loading Vertices"
             ):
                 batch = vertex_data.iloc[i : i + batch_size]
-                prop_columns = [col for col in vertex_data.columns if col != "___vid"]
-                if len(vertex_data.columns) == 1:
-                    query = f"INSERT VERTEX `{args.tag}` () VALUES "
-                else:
-                    query = f"INSERT VERTEX `{args.tag}` (`{'`, `'.join(prop_columns)}`) VALUES "
+                query = f"INSERT VERTEX {args.tag} ({', '.join([col for col in vertex_data.columns if col != '___vid'])}) VALUES "
                 for index, row in batch.iterrows():
                     vid_str = f'{QUOTE_VID}{row["___vid"]}{QUOTE_VID}'
                     prop_str = ""
                     if with_props:
                         for prop_name in props_mapping.values():
                             prop_value = row[prop_name]
                             if pd.isnull(prop_value):
@@ -925,23 +902,15 @@
             # Now prepare INSERT query for edges in batches
             # Example of QUERY:
             # with_rank INSERT EDGE e1 (name, age) VALUES "13" -> "14"@1:("n3", 12), "14" -> "15"@132:("n4", 8);
             # without_rank INSERT EDGE e1 (name, age) VALUES "13" -> "14":("n3", 12), "14" -> "15":("n4", 8);
 
             for i in tqdm(range(0, len(edge_data), batch_size), desc="Loading Edges"):
                 batch = edge_data.iloc[i : i + batch_size]
-                prop_columns = [
-                    col
-                    for col in edge_data.columns
-                    if col not in ["___src", "___dst", "___rank"]
-                ]
-                if len(prop_columns) == 0:
-                    query = f"INSERT EDGE `{args.edge}` () VALUES "
-                else:
-                    query = f"INSERT EDGE `{args.edge}` (`{'`, `'.join(prop_columns)}`) VALUES "
+                query = f"INSERT EDGE {args.edge} ({', '.join([col for col in edge_data.columns if col not in ['___src', '___dst', '___rank']])}) VALUES "
                 for index, row in batch.iterrows():
                     src_str = f'{QUOTE_VID}{row["___src"]}{QUOTE_VID}'
                     dst_str = f'{QUOTE_VID}{row["___dst"]}{QUOTE_VID}'
                     prop_str = ""
                     if with_props:
                         for prop_name in props_mapping.values():
                             prop_value = row[prop_name]
```

### Comparing `jupyter_nebulagraph-0.11.1/setup.py` & `jupyter_nebulagraph-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jupyter_nebulagraph",
-    version="0.11.1",
+    version="0.9.1",
     author="Wey Gu",
     author_email="weyl.gu@gmail.com",
     description="Jupyter extension for NebulaGraph",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wey-gu/jupyter_nebulagraph",
     project_urls={
         "Bug Tracker": "https://github.com/wey-gu/jupyter_nebulagraph/issues",
-        "Documentation": "https://jupyter-nebulagraph.readthedocs.io/",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
```

