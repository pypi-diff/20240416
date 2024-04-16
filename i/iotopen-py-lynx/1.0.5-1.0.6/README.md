# Comparing `tmp/iotopen_py_lynx-1.0.5.tar.gz` & `tmp/iotopen_py_lynx-1.0.6.tar.gz`

## Comparing `iotopen_py_lynx-1.0.5.tar` & `iotopen_py_lynx-1.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/py-lynx.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/__init__.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/api_client.py
--rw-r--r--   0        0        0    17893 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/client.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/controller.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/device_controller.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/edge_app_controller.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/file_controller.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/function_controller.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/installation_controller.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/installation_info_controller.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/log_controller.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/notification_controller.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/organization_controller.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/schedule_controller.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/trace_controller.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/controller/user_controller.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/constants.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/device.py
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/edge_app.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/file.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/function.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/installation.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/installation_info.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/log.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/notification.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/organization.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/publisher.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/responses.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/schedule.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/shared.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/trace.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/src/lynx/models/user.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/LICENSE
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/py-lynx.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/__init__.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/api_client.py
+-rw-r--r--   0        0        0    17870 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/client.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/controller.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/device_controller.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/edge_app_controller.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/file_controller.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/function_controller.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/installation_controller.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/installation_info_controller.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/log_controller.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/notification_controller.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/organization_controller.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/schedule_controller.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/trace_controller.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/controller/user_controller.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/constants.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/device.py
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/edge_app.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/file.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/function.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/installation.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/installation_info.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/log.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/notification.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/organization.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/publisher.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/responses.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/schedule.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/shared.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/trace.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/src/lynx/models/user.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/LICENSE
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 iotopen_py_lynx-1.0.6/PKG-INFO
```

### Comparing `iotopen_py_lynx-1.0.5/.idea/workspace.xml` & `iotopen_py_lynx-1.0.6/.idea/workspace.xml`

 * *Files 24% similar despite different names*

#### Comparing `iotopen_py_lynx-1.0.5/.idea/workspace.xml` & `iotopen_py_lynx-1.0.6/.idea/workspace.xml`

```diff
@@ -1,48 +1,57 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
+  <component name="AutoImportSettings">
+    <option name="autoReloadType" value="SELECTIVE"/>
+  </component>
   <component name="ChangeListManager">
     <list default="true" id="3ebfce3a-be03-4e50-b276-1512b6613de3" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/.idea/misc.xml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/misc.xml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/.idea/py-lynx.iml" beforeDir="false" afterPath="$PROJECT_DIR$/.idea/py-lynx.iml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/device.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/device.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/edge_app.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/edge_app.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/function.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/function.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/installation.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/installation.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/installation_info.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/installation_info.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/organization.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/organization.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/publisher.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/publisher.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/shared.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/shared.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/trace.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/trace.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/lynx/models/user.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/models/user.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/client.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/client.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/device_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/device_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/edge_app_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/edge_app_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/file_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/file_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/function_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/function_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/installation_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/installation_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/installation_info_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/installation_info_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/log_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/log_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/notification_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/notification_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/organization_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/organization_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/schedule_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/schedule_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/trace_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/trace_controller.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/lynx/controller/user_controller.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/lynx/controller/user_controller.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
-  <component name="ProjectColorInfo"><![CDATA[{
-  "associatedIndex": 6
-}]]></component>
+  <component name="ProjectColorInfo">{
+  &quot;associatedIndex&quot;: 6
+}</component>
   <component name="ProjectId" id="2fBlfz04SORAdZP7BD8ocfQtoXe"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "git-widget-placeholder": "master",
+    "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
@@ -55,14 +64,15 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="3ebfce3a-be03-4e50-b276-1512b6613de3" name="Changes" comment=""/>
       <created>1713282458947</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1713282458947</updated>
       <workItem from="1713282460048" duration="226000"/>
+      <workItem from="1713282795038" duration="364000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
 </project>
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/api_client.py` & `iotopen_py_lynx-1.0.6/src/lynx/api_client.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/client.py` & `iotopen_py_lynx-1.0.6/src/lynx/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import *
-from src.lynx.api_client import APIClient
-from src.lynx.controller import *
+from . import *
+from .api_client import APIClient
+from .controller import *
 
 
 class Client:
 
     def __init__(self, base_url: str, api_key: str):
         self.api_client = APIClient(base_url, api_key)
         self.__load_controllers()
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/__init__.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/device_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/device_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import Filter, Device, MetaObject, OKResponse
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import Filter, Device, MetaObject, OKResponse
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class DeviceController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/edge_app_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/edge_app_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import EdgeApp, EdgeAppVersion, EdgeAppConfig, OKResponse
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import EdgeApp, EdgeAppVersion, EdgeAppConfig, OKResponse
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class EdgeAppController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_edge_apps(self):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/file_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/file_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from src.lynx import File, OKResponse
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import File, OKResponse
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class FileController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_files_installation(self, installation_id: int):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/function_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/function_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import Function, Filter, MetaObject, OKResponse
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import Function, Filter, MetaObject, OKResponse
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class FunctionController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_functions(self, installation_id: int, filter: Optional[Filter] = None):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/installation_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/installation_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import Installation, MetaObject, OKResponse, Filter
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import Installation, MetaObject, OKResponse, Filter
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class InstallationController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_installations(self, filter: Optional[Filter] = None):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/installation_info_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/installation_info_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import InstallationInfo
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import InstallationInfo
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class InstallationInfoController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_installation_info(self, assigned_only: Optional[bool] = False):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/log_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/log_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 from typing import Optional
 
-from src.lynx import LogEntry, LogPage
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import LogEntry, LogPage
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class LogController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_logs(self, installation_id: int, fromm: Optional[float] = None, to: Optional[float] = None,
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/notification_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/notification_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import NotificationMessage, NotificationOutput, OKResponse, NotificationOutputExecutor
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import NotificationMessage, NotificationOutput, OKResponse, NotificationOutputExecutor
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class NotificationController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_notification_messages(self, installation_id: int):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/organization_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/organization_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import Filter, Organization, MetaObject, OKResponse
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import Filter, Organization, MetaObject, OKResponse
+from .. api_client import APIClient
+from .. controller import Controller
 
 
 class OrganizationController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_organizations(self, minimal: Optional[bool] = False, filter: Optional[Filter] = None):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/schedule_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/schedule_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import Device, OKResponse, Schedule
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import OKResponse, Schedule
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class ScheduleController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_schedules(self, installation_id: int, executor: Optional[str] = None):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/trace_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/trace_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime, timedelta
 from typing import Optional
 
-from src.lynx import TracePage, TraceEntry
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import TracePage, TraceEntry
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class TraceController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_traces(self, fromm: Optional[float] = None, to: Optional[float] = None, limit: Optional[int] = 1000,
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/controller/user_controller.py` & `iotopen_py_lynx-1.0.6/src/lynx/controller/user_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from src.lynx import Filter, User, OKResponse, MetaObject
-from src.lynx.api_client import APIClient
-from src.lynx.controller import Controller
+from .. import Filter, User, OKResponse, MetaObject
+from ..api_client import APIClient
+from ..controller import Controller
 
 
 class UserController(Controller):
     def __init__(self, api_client: APIClient):
         super().__init__(api_client)
 
     def get_users(self, filter: Optional[Filter] = None):
```

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/__init__.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/constants.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/constants.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/device.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/device.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/edge_app.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/edge_app.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/file.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/file.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/function.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/function.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/installation.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/installation.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/installation_info.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/installation_info.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/log.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/log.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/notification.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/notification.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/organization.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/organization.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/publisher.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/publisher.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/schedule.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/schedule.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/shared.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/shared.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/trace.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/trace.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/src/lynx/models/user.py` & `iotopen_py_lynx-1.0.6/src/lynx/models/user.py`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/LICENSE` & `iotopen_py_lynx-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/README.md` & `iotopen_py_lynx-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `iotopen_py_lynx-1.0.5/pyproject.toml` & `iotopen_py_lynx-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/lynx"]
 
 [project]
 name = "iotopen-py-lynx"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name = "Jesper Falk", email = "jesper.falk@iotopen.se" },
 ]
 description = "A wrapper library for the IoT Open Lynx API"
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `iotopen_py_lynx-1.0.5/PKG-INFO` & `iotopen_py_lynx-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: iotopen-py-lynx
-Version: 1.0.5
+Version: 1.0.6
 Summary: A wrapper library for the IoT Open Lynx API
 Project-URL: Homepage, https://github.com/IoTOpen/py-lynx
 Project-URL: Issues, https://github.com/IoTOpen/py-lynx/issues
 Author-email: Jesper Falk <jesper.falk@iotopen.se>
 License-File: LICENSE
 Keywords: api,iot,iot-open
 Classifier: Intended Audience :: Developers
```

