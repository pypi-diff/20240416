# Comparing `tmp/tum_esm_lowcost_metadata-0.6.0.tar.gz` & `tmp/tum_esm_lowcost_metadata-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_lowcost_metadata-0.6.0.tar", max compression
+gzip compressed data, was "tum_esm_lowcost_metadata-0.7.0.tar", max compression
```

## Comparing `tum_esm_lowcost_metadata-0.6.0.tar` & `tum_esm_lowcost_metadata-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     3671 2023-08-29 11:55:12.691140 tum_esm_lowcost_metadata-0.6.0/README.md
--rw-r--r--   0        0        0     1158 2023-09-22 08:12:50.896539 tum_esm_lowcost_metadata-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       72 2023-08-25 08:56:09.524150 tum_esm_lowcost_metadata-0.6.0/tum_esm_lowcost_metadata/__init__.py
--rw-r--r--   0        0        0     4598 2023-09-22 08:12:22.372464 tum_esm_lowcost_metadata-0.6.0/tum_esm_lowcost_metadata/interfaces.py
--rw-r--r--   0        0        0        0 2023-06-05 12:53:28.564046 tum_esm_lowcost_metadata-0.6.0/tum_esm_lowcost_metadata/py.typed
--rw-r--r--   0        0        0     3647 2023-09-22 06:59:29.937794 tum_esm_lowcost_metadata-0.6.0/tum_esm_lowcost_metadata/types.py
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 tum_esm_lowcost_metadata-0.6.0/setup.py
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 tum_esm_lowcost_metadata-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3961 2024-04-16 07:57:54.548385 tum_esm_lowcost_metadata-0.7.0/README.md
+-rw-r--r--   0        0        0     1158 2024-04-16 07:56:27.608790 tum_esm_lowcost_metadata-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-08-25 08:56:09.524150 tum_esm_lowcost_metadata-0.7.0/tum_esm_lowcost_metadata/__init__.py
+-rw-r--r--   0        0        0     4707 2024-04-16 07:55:20.196122 tum_esm_lowcost_metadata-0.7.0/tum_esm_lowcost_metadata/interfaces.py
+-rw-r--r--   0        0        0        0 2023-06-05 12:53:28.564046 tum_esm_lowcost_metadata-0.7.0/tum_esm_lowcost_metadata/py.typed
+-rw-r--r--   0        0        0     3701 2024-04-16 07:46:23.546709 tum_esm_lowcost_metadata-0.7.0/tum_esm_lowcost_metadata/types.py
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 tum_esm_lowcost_metadata-0.7.0/PKG-INFO
```

### Comparing `tum_esm_lowcost_metadata-0.6.0/README.md` & `tum_esm_lowcost_metadata-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,41 +40,43 @@
         "site_lon": 11.5860387,
         "elevation": 514,
         "comment": "Lamp post ids:55.0"
     },
 }
 ```
 - **`SAMPLING.json`**<br/>
-This file contains basic information on which site, at which time, which sensors measured at which configuration.
+This file contains basic information on which site, at which time, which sensors measured at which configuration. A new key "radiation_shield" was added with version 0.7 as all sensors will be deployed within radiation shieling in near future.
 
 ```json
 [
     {
         "site_id": "HANV",
         "sensor_ids": [
             13171,
             13147
         ],
         "sampling_start": "2023-05-02T12:30+02:00",
         "sampling_end": null,
         "orientation": 0,
         "elevation_ag": 3,
-        "comment": ""
+        "comment": "", 
+        "radiation_shield": false
     },
 ]
 ```
 
 <br/>
 
 ## How to add new measurement days?
 
 1. Possibly add new sensor in `data/SENSORS.json`
 2. Possibly add new site in `data/SITES.json`
 2. Add a new sampling event to `data/SAMPLING.json`
 
+If necessary, use this tool to find the elevation of a certain location: <url>https://www.calcmaps.com/map-elevation/</url>
 <br/>
 
 ## How can I know whether my changes were correct?
 
 Whenever you make changes in the repository on GitHub, the integrity of the files will automatically be checked. You can check whether all tests have passed [here](https://github.com/tum-esm/lowcost-metadata/actions).
 
 A list of all integrity checks can be found in [`tests/README.md`](https://github.com/tum-esm/lowcost-metadata//tree/main/tests).
```

### Comparing `tum_esm_lowcost_metadata-0.6.0/pyproject.toml` & `tum_esm_lowcost_metadata-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_lowcost_metadata"
-version = "0.6.0"
+version = "0.7.0"
 description = "Single source of truth for ESM's lowcost measurement logistics"
 readme = "README.md"
 authors = [
     "Moritz Makowski <moritz.makowski@tum.de>",
     "Daniel Kühbacher <daniel.kuehbacher@tum.de>",
     "Felix Böhm <felix.boehm@tum.de>",
 ]
```

### Comparing `tum_esm_lowcost_metadata-0.6.0/tum_esm_lowcost_metadata/interfaces.py` & `tum_esm_lowcost_metadata-0.7.0/tum_esm_lowcost_metadata/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             start_up_date=sensor.start_up_date,
             shut_down_date=sensor.shut_down_date,
             sensor_comment=sensor.comment,
             sampling_since = sample.sampling_start,
             sampling_until= sample.sampling_end,
             orientation=sample.orientation,
             elevation_ag=sample.elevation_ag,
+            radiation_shield=sample.radiation_shield,
             sampling_comment=sample.comment,
         )
         
         
 def print_beautiful(metadata:types.MetaData) -> None:
     """Prints metadata in a more accessible way."""
     
@@ -80,14 +81,15 @@
     print(f"\nMetadata for Sensor {m.sensor_id}, located at {m.site_id}.")
     print(f"---")
     print(f"Sensor type: \t\t{m.sensor_make} {m.sensor_model}")
     print(f"Site coordinates: \t{m.site_lat} lat")
     print(f"\t\t\t{m.site_lon} lon")
     print(f"\t\t\t{m.elevation} m a.s.l.")
     print(f"Site type: \t\t{m.site_type}")
+    print(f"Radiation shield: \t{m.radiation_shield}")
     print(f"Sampling since: \t{m.sampling_since}")
     if m.sampling_until is not None: print(f"Sampling until: \t{m.sampling_until}")
     print(f"Orientation \t\t{m.orientation}°")
     print(f"Elevation above ground:\t{m.elevation_ag} m")
 
     comment_str = ''.join(map(lambda comm: (comm+"\n\t\t\t"), 
                               filter(lambda i: len(i)>1, [m.sensor_comment, m.site_comment, m.sampling_comment])))
```

### Comparing `tum_esm_lowcost_metadata-0.6.0/tum_esm_lowcost_metadata/types.py` & `tum_esm_lowcost_metadata-0.7.0/tum_esm_lowcost_metadata/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         typing.Literal["all"],
     ]
     sampling_start: pendulum.DateTime
     sampling_end: typing.Optional[pendulum.DateTime] = ...  # Can be None, but must be set
     orientation: pydantic.confloat(ge=0, le=360)
     elevation_ag: pydantic.confloat(ge = 0, le = 300)
     comment: pydantic.constr(max_length=256)
+    radiation_shield: bool
 
 
 class Site(_BaseModel):
     #site_id: SiteIdentifier
     site_type: typing.Literal[
         "individual",
         "lfu_colocation",
@@ -88,14 +89,15 @@
     start_up_date: pendulum.DateTime
     shut_down_date: typing.Optional[pendulum.DateTime] = ...
     sensor_comment: pydantic.constr(max_length=256)
     sampling_since: pendulum.DateTime
     sampling_until: typing.Optional[pendulum.DateTime] = ...
     orientation: pydantic.confloat(ge=0, le=360)
     elevation_ag: pydantic.confloat(ge = 0, le = 300)
+    radiation_shield: bool
     sampling_comment: pydantic.constr(max_length=256)
 
 ####################################################################################################
 # Document models
 ####################################################################################################
```

### Comparing `tum_esm_lowcost_metadata-0.6.0/setup.py` & `tum_esm_lowcost_metadata-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,161 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tum_esm_lowcost_metadata
+Version: 0.7.0
+Summary: Single source of truth for ESM's lowcost measurement logistics
+Home-page: https://github.com/tum-esm/lowcost-metadata
+Author: Moritz Makowski
+Author-email: moritz.makowski@tum.de
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deepdiff (>=6.3.0,<7.0.0)
+Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: poetry-dotenv-plugin (>=0.2.0,<0.3.0)
+Requires-Dist: poetry-plugin-dotenv (>=0.5.3,<0.6.0)
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: tum-esm-utils (>=1.2.1,<2.0.0)
+Project-URL: Repository, https://github.com/tum-esm/lowcost-metadata
+Description-Content-Type: text/markdown
+
+# Lowcost Metadata
+
+This repository handles the metadata around the lowcost sensor network in Munich.<br/>
+We selected this format over putting it in a database due to various reasons:
+
+-   Easy to read, modify and extend by selective group members using GitHub permissions
+-   Changes to this are more obvious here than in database logs
+-   Versioning (easy to revert mistakes)
+-   Automatic testing of the files integrities
+-   Easy import as a statically typed Python library
+
+<br/>
+
+## What does this data look like?
+
+There is a set of **`JSON`** files in the data folder holding the follwing information:
+
+- **`SENSORS.json`**<br/>
+This files contains basic information about the sensors in use in the monitoring network.
+```json
+{
+    "13077": {
+        "sensor_type": "LP8",
+        "sensor_make": "Decentlab",
+        "sensor_model": "DL-LP8",
+        "start_up_date": "2022-08-01T08:00:00+00:00",
+        "shut_down_date": null,
+        "comment": ""
+    },
+}
+```
+- **`SITES.json`**<br/>
+This file contains basic information about the sites/locations where sensors have been installed.
+
+```json
+{
+    "FREV": {
+        "site_type": "individual",
+        "site_lat": 48.1615591,
+        "site_lon": 11.5860387,
+        "elevation": 514,
+        "comment": "Lamp post ids:55.0"
+    },
+}
+```
+- **`SAMPLING.json`**<br/>
+This file contains basic information on which site, at which time, which sensors measured at which configuration. A new key "radiation_shield" was added with version 0.7 as all sensors will be deployed within radiation shieling in near future.
 
-packages = \
-['tum_esm_lowcost_metadata']
+```json
+[
+    {
+        "site_id": "HANV",
+        "sensor_ids": [
+            13171,
+            13147
+        ],
+        "sampling_start": "2023-05-02T12:30+02:00",
+        "sampling_end": null,
+        "orientation": 0,
+        "elevation_ag": 3,
+        "comment": "", 
+        "radiation_shield": false
+    },
+]
+```
 
-package_data = \
-{'': ['*']}
+<br/>
 
-modules = \
-['py']
-install_requires = \
-['deepdiff>=6.3.0,<7.0.0',
- 'pendulum>=2.1.2,<3.0.0',
- 'poetry-dotenv-plugin>=0.2.0,<0.3.0',
- 'poetry-plugin-dotenv>=0.5.3,<0.6.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'tum-esm-utils>=1.2.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'tum-esm-lowcost-metadata',
-    'version': '0.6.0',
-    'description': "Single source of truth for ESM's lowcost measurement logistics",
-    'long_description': '# Lowcost Metadata\n\nThis repository handles the metadata around the lowcost sensor network in Munich.<br/>\nWe selected this format over putting it in a database due to various reasons:\n\n-   Easy to read, modify and extend by selective group members using GitHub permissions\n-   Changes to this are more obvious here than in database logs\n-   Versioning (easy to revert mistakes)\n-   Automatic testing of the files integrities\n-   Easy import as a statically typed Python library\n\n<br/>\n\n## What does this data look like?\n\nThere is a set of **`JSON`** files in the data folder holding the follwing information:\n\n- **`SENSORS.json`**<br/>\nThis files contains basic information about the sensors in use in the monitoring network.\n```json\n{\n    "13077": {\n        "sensor_type": "LP8",\n        "sensor_make": "Decentlab",\n        "sensor_model": "DL-LP8",\n        "start_up_date": "2022-08-01T08:00:00+00:00",\n        "shut_down_date": null,\n        "comment": ""\n    },\n}\n```\n- **`SITES.json`**<br/>\nThis file contains basic information about the sites/locations where sensors have been installed.\n\n```json\n{\n    "FREV": {\n        "site_type": "individual",\n        "site_lat": 48.1615591,\n        "site_lon": 11.5860387,\n        "elevation": 514,\n        "comment": "Lamp post ids:55.0"\n    },\n}\n```\n- **`SAMPLING.json`**<br/>\nThis file contains basic information on which site, at which time, which sensors measured at which configuration.\n\n```json\n[\n    {\n        "site_id": "HANV",\n        "sensor_ids": [\n            13171,\n            13147\n        ],\n        "sampling_start": "2023-05-02T12:30+02:00",\n        "sampling_end": null,\n        "orientation": 0,\n        "elevation_ag": 3,\n        "comment": ""\n    },\n]\n```\n\n<br/>\n\n## How to add new measurement days?\n\n1. Possibly add new sensor in `data/SENSORS.json`\n2. Possibly add new site in `data/SITES.json`\n2. Add a new sampling event to `data/SAMPLING.json`\n\n<br/>\n\n## How can I know whether my changes were correct?\n\nWhenever you make changes in the repository on GitHub, the integrity of the files will automatically be checked. You can check whether all tests have passed [here](https://github.com/tum-esm/lowcost-metadata/actions).\n\nA list of all integrity checks can be found in [`tests/README.md`](https://github.com/tum-esm/lowcost-metadata//tree/main/tests).\n\n<br/>\n\n## How to use it in your codebase?\n\n1. Install python library\n\n```bash\npoetry add tum_esm_lowcost_metadata\n# or\npip install tum_esm_lowcost_metadata\n```\n\n2. Create a personal access token for a GitHub account that has read access to the metadata repository: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token\n\n3. Use the metadata anywhere\n\n```python\nimport tum_esm_lowcost_metadata\n\nlowcost_metadata_interface = tum_esm_lowcost_metadata.load_from_github(\n    github_repository = "org-name/repo-name",\n    access_token = "ghp_..."\n)\n\nmetadata = lowcost_metadata_interface.get(\n    sensor_id = "13077", date = pendulum.datetime(2023, 6, 6)\n)  # is of type list[tum_esm_lowcost_metadata.types.SensorDataContext]\n\nmetadata = interface.get(sensor_id = \'13155\', timestamp=pendulum.datetime(2023, 6, 6))\ninterfaces.print_beautiful(metadata))\n```\n\n... prints out:\n\n```\nMetadata for Sensor 13155, located at MOSV.\n---\nSensor type:            Decentlab DL-LP8\nSite coordinates:       48.1870436 lat\n                        11.5622708 lon\n                        508.0 m a.s.l.\nOrientation             0.0°\nElevation above ground: 3.0 m\nComment:                Lamp post ids:32.0\n\n---\n```\n\n<br/>\n\n## For Developers: Publish the Package to PyPI\n\n```bash\npoetry build\npoetry publish\n```\n',
-    'author': 'Moritz Makowski',
-    'author_email': 'moritz.makowski@tum.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tum-esm/lowcost-metadata',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+## How to add new measurement days?
+
+1. Possibly add new sensor in `data/SENSORS.json`
+2. Possibly add new site in `data/SITES.json`
+2. Add a new sampling event to `data/SAMPLING.json`
+
+If necessary, use this tool to find the elevation of a certain location: <url>https://www.calcmaps.com/map-elevation/</url>
+<br/>
+
+## How can I know whether my changes were correct?
+
+Whenever you make changes in the repository on GitHub, the integrity of the files will automatically be checked. You can check whether all tests have passed [here](https://github.com/tum-esm/lowcost-metadata/actions).
+
+A list of all integrity checks can be found in [`tests/README.md`](https://github.com/tum-esm/lowcost-metadata//tree/main/tests).
+
+<br/>
+
+## How to use it in your codebase?
+
+1. Install python library
+
+```bash
+poetry add tum_esm_lowcost_metadata
+# or
+pip install tum_esm_lowcost_metadata
+```
+
+2. Create a personal access token for a GitHub account that has read access to the metadata repository: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
+
+3. Use the metadata anywhere
+
+```python
+import tum_esm_lowcost_metadata
+
+lowcost_metadata_interface = tum_esm_lowcost_metadata.load_from_github(
+    github_repository = "org-name/repo-name",
+    access_token = "ghp_..."
+)
+
+metadata = lowcost_metadata_interface.get(
+    sensor_id = "13077", date = pendulum.datetime(2023, 6, 6)
+)  # is of type list[tum_esm_lowcost_metadata.types.SensorDataContext]
+
+metadata = interface.get(sensor_id = '13155', timestamp=pendulum.datetime(2023, 6, 6))
+interfaces.print_beautiful(metadata))
+```
+
+... prints out:
+
+```
+Metadata for Sensor 13155, located at MOSV.
+---
+Sensor type:            Decentlab DL-LP8
+Site coordinates:       48.1870436 lat
+                        11.5622708 lon
+                        508.0 m a.s.l.
+Orientation             0.0°
+Elevation above ground: 3.0 m
+Comment:                Lamp post ids:32.0
+
+---
+```
+
+<br/>
+
+## For Developers: Publish the Package to PyPI
 
+```bash
+poetry build
+poetry publish
+```
 
-setup(**setup_kwargs)
```

