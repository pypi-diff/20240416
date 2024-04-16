# Comparing `tmp/cumo-0.33.1.tar.gz` & `tmp/cumo-0.33.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumo-0.33.1.tar", max compression
+gzip compressed data, was "cumo-0.33.2.tar", max compression
```

## Comparing `cumo-0.33.1.tar` & `cumo-0.33.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1275 2024-04-12 06:09:25.380276 cumo-0.33.1/README.md
--rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/.gitignore
--rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/__init__.py
--rw-r--r--   0        0        0     3683 2024-04-12 05:59:32.220796 cumo-0.33.1/cumo/__main__.py
--rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/.gitignore
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/__init__.py
--rw-r--r--   0        0        0     1675 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/_internal/down_sample.py
--rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/members/__init__.py
--rw-r--r--   0        0        0     8722 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/_internal/members/camera.py
--rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/members/capture_screen.py
--rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/members/custom_control.py
--rw-r--r--   0        0        0     5927 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/_internal/members/event_handler.py
--rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/members/internal_utils.py
--rw-r--r--   0        0        0     6396 2023-09-11 09:15:41.832883 cumo-0.33.1/cumo/_internal/members/keyboard_event_handler.py
--rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_internal/members/remove_object.py
--rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.33.1/cumo/_internal/members/send_object.py
--rw-r--r--   0        0        0    10336 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/_internal/members/set_custom_control.py
--rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.33.1/cumo/_internal/members/set_enable.py
--rw-r--r--   0        0        0     1256 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/_internal/members/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 06:09:01.228811 cumo-0.33.1/cumo/_internal/protobuf/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-12 06:09:01.208810 cumo-0.33.1/cumo/_internal/protobuf/client_pb2.py
--rw-r--r--   0        0        0    10387 2024-04-12 06:09:01.208810 cumo-0.33.1/cumo/_internal/protobuf/client_pb2.pyi
--rw-r--r--   0        0        0    12303 2024-04-12 06:09:00.658791 cumo-0.33.1/cumo/_internal/protobuf/server_pb2.py
--rw-r--r--   0        0        0    40121 2024-04-12 06:09:00.658791 cumo-0.33.1/cumo/_internal/protobuf/server_pb2.pyi
--rw-r--r--   0        0        0     4200 2024-03-21 11:15:04.876331 cumo-0.33.1/cumo/_internal/server.py
--rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_vendor/pypcd/LICENSE
--rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/_vendor/pypcd/pypcd.py
--rw-r--r--   0        0        0     1119 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/camera_state.py
--rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.33.1/cumo/keyboard_event.py
--rw-r--r--   0        0        0     3554 2023-09-13 10:26:38.801824 cumo-0.33.1/cumo/pointcloudviewer.py
--rw-r--r--   0        0        0  5077306 2024-04-12 06:09:25.380276 cumo-0.33.1/cumo/public/bundle-daa57634.js
--rw-r--r--   0        0        0   243028 2024-04-12 06:09:25.380276 cumo-0.33.1/cumo/public/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      515 2024-04-12 06:09:25.370275 cumo-0.33.1/cumo/public/index-31f52342.css
--rw-r--r--   0        0        0      281 2024-04-12 06:09:25.380276 cumo-0.33.1/cumo/public/index.html
--rw-r--r--   0        0        0     1219 2024-04-12 06:07:57.972332 cumo-0.33.1/pyproject.toml
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.33.1/PKG-INFO
+-rw-r--r--   0        0        0     1275 2024-04-16 06:10:32.298157 cumo-0.33.2/README.md
+-rw-r--r--   0        0        0        7 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/.gitignore
+-rw-r--r--   0        0        0      117 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/__init__.py
+-rw-r--r--   0        0        0     3683 2024-04-12 05:59:32.220796 cumo-0.33.2/cumo/__main__.py
+-rw-r--r--   0        0        0        9 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/.gitignore
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/__init__.py
+-rw-r--r--   0        0        0     1675 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/_internal/down_sample.py
+-rw-r--r--   0        0        0        0 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/members/__init__.py
+-rw-r--r--   0        0        0     8722 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/_internal/members/camera.py
+-rw-r--r--   0        0        0     1177 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/members/capture_screen.py
+-rw-r--r--   0        0        0    12413 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/members/custom_control.py
+-rw-r--r--   0        0        0     5927 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/_internal/members/event_handler.py
+-rw-r--r--   0        0        0      974 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/members/internal_utils.py
+-rw-r--r--   0        0        0     6396 2023-09-11 09:15:41.832883 cumo-0.33.2/cumo/_internal/members/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1360 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_internal/members/remove_object.py
+-rw-r--r--   0        0        0    20526 2023-07-27 11:30:24.682816 cumo-0.33.2/cumo/_internal/members/send_object.py
+-rw-r--r--   0        0        0    10336 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/_internal/members/set_custom_control.py
+-rw-r--r--   0        0        0     1045 2022-12-22 06:09:32.016687 cumo-0.33.2/cumo/_internal/members/set_enable.py
+-rw-r--r--   0        0        0     1256 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/_internal/members/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 06:08:49.259643 cumo-0.33.2/cumo/_internal/protobuf/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-16 06:08:49.239642 cumo-0.33.2/cumo/_internal/protobuf/client_pb2.py
+-rw-r--r--   0        0        0    10387 2024-04-16 06:08:49.239642 cumo-0.33.2/cumo/_internal/protobuf/client_pb2.pyi
+-rw-r--r--   0        0        0    12303 2024-04-16 06:08:45.989436 cumo-0.33.2/cumo/_internal/protobuf/server_pb2.py
+-rw-r--r--   0        0        0    40121 2024-04-16 06:08:45.989436 cumo-0.33.2/cumo/_internal/protobuf/server_pb2.pyi
+-rw-r--r--   0        0        0     4200 2024-03-21 11:15:04.876331 cumo-0.33.2/cumo/_internal/server.py
+-rw-r--r--   0        0        0     1509 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_vendor/pypcd/LICENSE
+-rw-r--r--   0        0        0    28920 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/_vendor/pypcd/pypcd.py
+-rw-r--r--   0        0        0     1119 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/camera_state.py
+-rw-r--r--   0        0        0      924 2022-05-27 04:27:01.699189 cumo-0.33.2/cumo/keyboard_event.py
+-rw-r--r--   0        0        0     3554 2023-09-13 10:26:38.801824 cumo-0.33.2/cumo/pointcloudviewer.py
+-rw-r--r--   0        0        0  5077283 2024-04-16 06:10:32.278154 cumo-0.33.2/cumo/public/bundle-b281c36a.js
+-rw-r--r--   0        0        0   243028 2024-04-16 06:10:32.278154 cumo-0.33.2/cumo/public/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      515 2024-04-16 06:10:32.268153 cumo-0.33.2/cumo/public/index-31f52342.css
+-rw-r--r--   0        0        0      281 2024-04-16 06:10:32.278154 cumo-0.33.2/cumo/public/index.html
+-rw-r--r--   0        0        0     1219 2024-04-16 06:06:05.532667 cumo-0.33.2/pyproject.toml
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.33.2/PKG-INFO
```

### Comparing `cumo-0.33.1/README.md` & `cumo-0.33.2/README.md`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/__main__.py` & `cumo-0.33.2/cumo/__main__.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/down_sample.py` & `cumo-0.33.2/cumo/_internal/down_sample.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/camera.py` & `cumo-0.33.2/cumo/_internal/members/camera.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/capture_screen.py` & `cumo-0.33.2/cumo/_internal/members/capture_screen.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/custom_control.py` & `cumo-0.33.2/cumo/_internal/members/custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/event_handler.py` & `cumo-0.33.2/cumo/_internal/members/event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/internal_utils.py` & `cumo-0.33.2/cumo/_internal/members/internal_utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/keyboard_event_handler.py` & `cumo-0.33.2/cumo/_internal/members/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/remove_object.py` & `cumo-0.33.2/cumo/_internal/members/remove_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/send_object.py` & `cumo-0.33.2/cumo/_internal/members/send_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/set_custom_control.py` & `cumo-0.33.2/cumo/_internal/members/set_custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/set_enable.py` & `cumo-0.33.2/cumo/_internal/members/set_enable.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/members/utils.py` & `cumo-0.33.2/cumo/_internal/members/utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/protobuf/client_pb2.py` & `cumo-0.33.2/cumo/_internal/protobuf/client_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/protobuf/client_pb2.pyi` & `cumo-0.33.2/cumo/_internal/protobuf/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/protobuf/server_pb2.py` & `cumo-0.33.2/cumo/_internal/protobuf/server_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/protobuf/server_pb2.pyi` & `cumo-0.33.2/cumo/_internal/protobuf/server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_internal/server.py` & `cumo-0.33.2/cumo/_internal/server.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_vendor/pypcd/LICENSE` & `cumo-0.33.2/cumo/_vendor/pypcd/LICENSE`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/_vendor/pypcd/pypcd.py` & `cumo-0.33.2/cumo/_vendor/pypcd/pypcd.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/camera_state.py` & `cumo-0.33.2/cumo/camera_state.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/keyboard_event.py` & `cumo-0.33.2/cumo/keyboard_event.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/pointcloudviewer.py` & `cumo-0.33.2/cumo/pointcloudviewer.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/public/bundle-daa57634.js` & `cumo-0.33.2/cumo/public/bundle-b281c36a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -116325,15 +116325,15 @@
             for (let b = 0; b < C; b++) S[b * 4 + 0] = m[b * 3 + 2], S[b * 4 + 1] = m[b * 3 + 1], S[b * 4 + 2] = m[b * 3 + 0], S[b * 4 + 3] = 1;
             h.set(S, VertexBuffer.ColorKind)
         } else sendFailure(l, t, `unsupported element size: ${g.BYTES_PER_ELEMENT}`)
     }
     const d = new StandardMaterial(t, r.scene);
     d.emissiveColor = new Color3(1, 1, 1), d.disableLighting = !0, d.pointsCloud = !0, d.pointSize = s.pointSize;
     const p = new Mesh(t, r.scene);
-    p.renderingGroupId = 1, h.applyToMesh(p, !0), p.material = d, sendSuccess(l, t, t)
+    h.applyToMesh(p, !0), p.material = d, sendSuccess(l, t, t)
 }
 
 function handleImage(l, t, r, s) {
     if (s === void 0) {
         sendFailure(l, t, "failed to get image");
         return
     }
@@ -123915,16 +123915,16 @@
                         })
                     }
                 });
                 he(this, "custom", {})
             }
         });
         this.container = t;
-        const r = 1e-5,
-            s = 1e5;
+        const r = .1,
+            s = 1e4;
         this.canvas = document.createElement("canvas"), t.appendChild(this.canvas), this.engine = new Engine(this.canvas, !0, {
             adaptToDeviceRatio: !0
         }), this.scene = new Scene(this.engine), this.scene.clearColor = new Color4(0, 0, 0), this.scene.lightsEnabled = !1, this.camera = new FreeCamera("camera", new Vector3(-1, -1, -1), this.scene), this.camera.fov = this.config.camera.perspective.fov / 180 * Math.PI, this.camera.fovMode = Camera.FOVMODE_HORIZONTAL_FIXED, this.camera.maxZ = s, this.camera.minZ = r, this.cameraInput = new CustomCameraInput, this.camera.inputs.clear(), this.camera.inputs.add(this.cameraInput), this.camera.attachControl(), this.canvas2d = new Canvas2D, this.canvas.style.position = "absolute", this.canvas.style.width = "100vw", this.canvas.style.height = "100vh", this.canvas.width = window.innerWidth * window.devicePixelRatio, this.canvas.height = window.innerHeight * window.devicePixelRatio, this.canvas2d.domElement.style.pointerEvents = "none", t.appendChild(this.canvas2d.domElement);
         const n = () => {
             this.canvas.width = window.innerWidth * window.devicePixelRatio, this.canvas.height = window.innerHeight * window.devicePixelRatio, this.engine.setHardwareScalingLevel(1 / window.devicePixelRatio), this.engine.resize(!0)
         };
         window.addEventListener("resize", n);
```

### Comparing `cumo-0.33.1/cumo/public/bundle.js.LICENSE.txt` & `cumo-0.33.2/cumo/public/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/cumo/public/index-31f52342.css` & `cumo-0.33.2/cumo/public/index-31f52342.css`

 * *Files identical despite different names*

### Comparing `cumo-0.33.1/pyproject.toml` & `cumo-0.33.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 readme = "README.md"
 name = "cumo"
-version = "0.33.1"
+version = "0.33.2"
 description = "Webブラウザ上に点群を描画する python ライブラリ"
 authors = ["Kurusugawa Computer"]
 license = "BSD"
 keywords = ["point-cloud", "pcd"]
 repository = "https://github.com/kurusugawa-computer/cumo"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

### Comparing `cumo-0.33.1/PKG-INFO` & `cumo-0.33.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumo
-Version: 0.33.1
+Version: 0.33.2
 Summary: Webブラウザ上に点群を描画する python ライブラリ
 Home-page: https://github.com/kurusugawa-computer/cumo
 License: BSD
 Keywords: point-cloud,pcd
 Author: Kurusugawa Computer
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

